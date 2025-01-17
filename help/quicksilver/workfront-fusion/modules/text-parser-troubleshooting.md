---
content-type: tips-tricks-troubleshooting
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Problemen met tekstparser oplossen in  [!DNL Adobe Workfront Fusion]
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 8a3821cf-d0c6-4917-86e7-90a4872a5795
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Problemen met tekstparser oplossen in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ parser van de Tekst ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/text-parser.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

Gebruik deze informatie als u geen tekstparser kunt krijgen om output te veroorzaken.

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] of hoger</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u het [!UICONTROL Select] - of [!UICONTROL Prime] [!DNL Adobe Workfront] -abonnement hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Problemen oplossen

In het casescenario-voorbeeld wilt u het bestandstype &#39;filename.docx&#39; parseren en de bestandsextensie varieert altijd van DOCX tot PDF tot CSV.

De expressie die u in dit geval kunt gebruiken, is [!DNL \..+]

Als u dit op regex uitdrukking op regex101.com zou gebruiken zult u een volledige gelijke krijgen.

![](assets/regex-expression-350x130.png)

In de bovenstaande afbeelding komt de bestandsextensie op de juiste wijze overeen. Als u dit neemt en probeert om het in uw tekstparser uit te voeren:

![](assets/text-parser-350x602.png)

je krijgt geen overeenkomst:

![](assets/text-parser-you-dont-get-a-match-350x365.png)

De reden hiervoor is dat &quot;i&quot;slechts het aantal gelijken per gelijke toont zodat in dit geval, hebben wij 2 gelijken, daarom nadat &quot;i&quot;er een numerieke waarde 1 en 2 is. Het gebruik hiervan is dat als u ooit gegevens via een filter moet aanpassen of doorgeven, alleen de tweede overeenkomende waarde kan worden opgegeven welke waarde wordt vertegenwoordigd door de numerieke waarde.

![](assets/text-parser-matches-350x355.png)

Als u de overeenkomende waarden wilt ophalen die u nodig hebt om haakjes toe te voegen aan het onderdeel dat u wilt parseren (bijvoorbeeld als u wilt extraheren uit &quot;filename.docx&quot; - alleen &quot;docx&quot;), moeten de haakjes volgens de regex-expressie die we in dit casescenario gebruiken, worden toegepast op \.(.+)

Hierdoor wordt de DOCX vastgelegd, in een groep geplaatst en de &quot;.&quot; van het.

![](assets/text-parser-get-matches-350x592.png)

In de uitvoer die in de onderstaande afbeelding wordt weergegeven, komt de vastgelegde groep overeen met elk willekeurig teken (behalve regeleinde).

![](assets/text-parser-output-350x389.png)

Een andere oplossing die ook regex opneemt, gebruikt de vervangingsfunctie

`{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.\./"; ".")}}`

Vervang `abcdefghijklmno pqr stuvw xyz.docx` vervolgens door de werkelijke bestandsnaamvariabele.
