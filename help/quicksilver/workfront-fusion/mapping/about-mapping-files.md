---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Over het toewijzen van bestanden in  [!DNL Adobe Workfront Fusion]
description: Sommige modules kunnen bestanden verwerken. Deze modules kunnen een uitvoerbestand retourneren dat voor verdere verwerking moet worden verzonden of een bestand vereisen dat voor verwerking aan hen wordt doorgegeven. Voordat deze modules kunnen samenwerken om bestanden te verwerken, moeten ze aan elkaar worden toegewezen.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# Over het toewijzen van bestanden in [!DNL Adobe Workfront Fusion]

Sommige modules kunnen bestanden verwerken. Deze modules kunnen een uitvoerbestand retourneren dat voor verdere verwerking moet worden verzonden of een bestand vereisen dat voor verwerking aan hen wordt doorgegeven. Voordat deze modules kunnen samenwerken om bestanden te verwerken, moeten ze aan elkaar worden toegewezen.

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
  </tr>  </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Toewijzingsbestanden

Modules die bestanden kunnen bewerken, vereisen twee informatie:

* Bestandsnaam
* Bestandsinhoud (gegevens)

Wanneer u een dossier in kaart brengt, kiest u de modules in uw scenario waarvan u de gegevens wilt verkrijgen. De bestandsnaam en de bestandsinhoud worden vervolgens automatisch toegewezen zoals ze zijn.

>[!NOTE]
>
>Als u een bestand vanaf een URL moet verwerken, raden we u aan het bestand met de module `HTTP > Get a File` te downloaden van de URL en het bestand vervolgens van de module `HTTP > Get a File` toe te wijzen aan het veld van de gewenste module in uw scenario.

>[!INFO]
>
>**Voorbeeld:** Dit voorbeeld toont hoe te om documenten van [!DNL Adobe Workfront] aan [!DNL Google Drive] te downloaden. De [!DNL Workfront] trigger [!UICONTROL Watch Record] retourneert gedetailleerde informatie over elk document, inclusief de naam en id.
>
>In de volgende module, [!UICONTROL Download Document] , worden de feitelijke gegevens gedownload zodat deze naar Google Drive kunnen worden geüpload.
>
>Als u deze gegevens wilt toewijzen aan [!DNL Google Drive] zodat deze kunnen worden geüpload, moet u het bronbestand opgeven van waaruit de gegevens worden toegewezen. Als u de optie [!DNL Workfront] > [!UICONTROL Download Document] onder het bronbestand selecteert, wijst [!DNL Workfront Fusion] de bestandsnaam en de bestandsinhoud toe, zodat het document van [!DNL Workfront] wordt geüpload naar de opgegeven Google-map.
>
>![](assets/wf-download-document-350x605.png)
>
>Als u echter de naam van het bestand wilt wijzigen, maar de gegevens ongewijzigd wilt laten, kunt u de optie [!UICONTROL Map] gebruiken om de bestandsnaam en de bestandsinhoud afzonderlijk toe te wijzen. U voert de volledige bestandsnaam in, inclusief de extensie. Tekstopmaak en binaire indelingen, zoals foto&#39;s, video&#39;s en PDF, worden ondersteund.
>
>![](assets/use-the-map-option-350x358.png)
