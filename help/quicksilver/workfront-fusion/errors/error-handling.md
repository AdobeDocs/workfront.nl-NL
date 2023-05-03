---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Foutafhandeling in [!DNL Adobe Workfront Fusion]
description: Wanneer de fouten tijdens de uitvoering van een scenario voorkomen, is het gewoonlijk omdat de dienst wegens een mislukking niet beschikbaar is, antwoordt de dienst met onverwachte gegevens, of de bevestiging van inputgegevens ontbreekt.
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: e936bbd2837e4aec67d4136b8efcccb6f8454a89
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# Foutafhandeling in [!DNL Adobe Workfront Fusion]

Wanneer de fouten tijdens de uitvoering van een scenario voorkomen, is het gewoonlijk omdat de dienst wegens een mislukking niet beschikbaar is, antwoordt de dienst met onverwachte gegevens, of de bevestiging van inputgegevens ontbreekt.

Als een module een fout tijdens de scenariouitvoering werpt en er geen fout behandelende route aan de module verbonden is, voert de standaardfout behandelende logica uit, zoals die in wordt beschreven [Fout bij verwerken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

Door een route van de foutenmanager aan een module toe te voegen, kunt u de standaardfout behandelende logica met uw vervangen. [!DNL Adobe Workfront Fusion] biedt vijf verschillende richtlijnen aan die aan het eind van uw foutenmanager routes kunnen worden opgenomen.

Zie voor meer informatie [Richtlijnen voor foutafhandeling in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p><p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Fouthandlerroute

Om een route van de foutenmanager aan een module toe te voegen:

1. Klik met de rechtermuisknop op de module en selecteer **[!UICONTROL Add error handler]**:

   ![](assets/error-handler-route.png)

   De module bevat een lijst met richtlijnen en de toepassingen die in uw scenario worden gebruikt.

1. Als de module die u een foutenmanager aan toevoegde de de laatste module in uw route is, selecteer één van de instructies.

   of

   Voeg één of meerdere modules aan de route van de foutenmanager toe.

   Als u meer modules aan de route toevoegt, [!UICONTROL Ignore] de richtlijn wordt standaard toegepast en in geval van een fout worden de daaropvolgende modules op die route verwerkt .


>[!INFO]
>
>In dit voorbeeld, als een fout voorkomt terwijl het uitvoeren van [!UICONTROL Create a folder] de [!UICONTROL Ignore] de richtlijn zal automatisch worden toegepast en het scenario zal zich aan de volgende module op de route van de foutenmanager bewegen.
>
>Als er echter geen fout optreedt, wordt het scenario verplaatst naar de [!UICONTROL List all files in a folder module] op de gewone route.
>
>![](assets/if-there-is-no-error-350x234.png)

Merk op dat een route van de foutenmanager uit transparante cirkels bestaat, terwijl een regelmatige route uit stevige cirkels bestaat.

## Instructies voor foutafhandeling

De richtlijnen worden hieronder kort toegelicht. Zie voor meer informatie [Richtlijnen voor foutafhandeling in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

Er zijn in totaal vijf richtlijnen die in de volgende categorieën kunnen worden ondergebracht, afhankelijk van de vraag of de uitvoering van een scenario al dan niet moet worden voortgezet.

De volgende richtlijnen zorgen ervoor dat de uitvoering van een scenario wordt voortgezet:

* **[!UICONTROL Resume]**: Hiermee kunt u een vervangende uitvoer voor de module opgeven met de fout. De status van de uitvoering van het scenario is gemarkeerd als geslaagd
* **[!UICONTROL Ignore]**: negeert de fout. De status van de uitvoering van het scenario is gemarkeerd als geslaagd
* **[!UICONTROL Break]**: Hiermee wordt de invoer in de wachtrij van onvolledige uitvoeringen opgeslagen. De status van de uitvoering van het scenario wordt gemarkeerd als waarschuwing. Zie voor meer informatie [Onvolledige uitvoeringen weergeven en oplossen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Als de uitvoering van een scenario moet stoppen wanneer een fout optreedt, gebruikt u een van de volgende instructies:

* **[!UICONTROL Rollback]**: Stopt onmiddellijk de uitvoering van het scenario en markeert zijn status als fout
* **[!UICONTROL Commit]**: Stopt onmiddellijk de uitvoering van het scenario en markeert zijn status als succes

Zie voor meer informatie over foutafhandeling:

* [Richtlijnen voor foutafhandeling in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [Geavanceerde foutafhandeling in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)