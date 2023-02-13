---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]
description: Toewijzing is het proces om de output van een module, gestructureerd in punten, aan de inputgebieden van een andere module toe te wijzen.
author: Becky
feature: Workfront Fusion
exl-id: e8d619e9-6425-4136-ac71-47d979d68a2d
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '1463'
ht-degree: 0%

---

# De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]

Toewijzing is het proces om de output van een module, gestructureerd in punten, aan de inputgebieden van een andere module toe te wijzen.

Het deelvenster Toewijzing wordt weergegeven wanneer u in een scenario op een veld klikt waarin u een waarde wilt invoegen die is uitgevoerd vanuit een voorgaande module. Binnen een module, op om het even welk gebied dat voor afbeelding beschikbaar is, kunt u een formule tot stand brengen gebruikend om het even welke combinatie functies en in kaart gebrachte punten van het toewijzingspaneel met statische teksten die u typt. Deze elementen kunnen in elkaar worden genest.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Bundels en artikelen

De verrichting van een module veroorzaakt nul, één, of meer bundels als zijn output. Een bundel bestaat uit een of meer items.

De uitvoer van een module verkennen:

1. Klikken **[!UICONTROL Run once]** om de module uit te voeren.
1. Klik op de ballon boven de module.

   Een logboek dat alle de fasenvertoningen van de module bevat. U kunt de bundel of de bundels vinden die door de verrichtingsfase van een module onder wordt uitgevoerd **[!UICONTROL Output]** kop. Elke bundel bevat zijn punten en de waarden van elk punt.

>[!INFO]
>
>**Voorbeeld:** In dit voorbeeld wordt de module getoond [!UICONTROL Email] > [!UICONTROL Watch emails]. U kunt zien dat het 1 verrichting uitvoerde die één enkele bundel produceerde die diverse punten zoals bevat `Date`, `Email ID (UID)`, `size`, enzovoort.
>
>![](assets/watch-emails-350x298.png)

>[!NOTE]
>
>De output van modules tussen verpakt [!UICONTROL Iterator] en [!UICONTROL Aggregator] niet toegankelijk zijn buiten de [!UICONTROL Aggregator] module.

## Een item toewijzen

Nadat u een opeenvolging van modules door twee of meer van hen te verbinden hebt gecreeerd, kan elke module waarden van punten verwerken die door de modules worden uitgevoerd die het voorafgaan.

De items toewijzen aan de invoervelden van een module:

1. Klik op de module die de output van de voorafgaande module of modules zou moeten verwerken.
1. Klik in het deelvenster Moduleinstellingen dat wordt weergegeven op een veld waar u de waarde wilt gebruiken van een item dat is uitgevoerd vanuit een of meer voorgaande modules.

   Het deelvenster Toewijzing wordt geopend.

1. Klik op een item in het deelvenster Toewijzing om het in te voegen in het veld.
1. (Optioneel) Als u naar een bepaald veld in het deelvenster Toewijzing wilt zoeken, klikt u op de zoekbalk van het deelvenster Toewijzing en typt u de term die u wilt zoeken. Klik op het veld wanneer dit in de lijst wordt weergegeven.

   Zoekresultaten bevatten de zoekterm en zijn niet hoofdlettergevoelig.

Zie voor meer informatie [De instellingen van een module configureren in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

## Formulas

U kunt veelvoudige punten in een gebied in kaart brengen, hen combineren met literals (vaste waarden), en exploitanten en Functies in dienst nemen om complexe formules te bouwen:

![](assets/operators-and-functions-350x187.png)

U vindt de functies en operatoren in het deelvenster Toewijzing onder een van de tabbladen.

![](assets/functions-toolbar-350x189.png)

De eerste tab ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (weergegeven bij het openen van het deelvenster) geeft de items weer die u vanuit andere modules kunt toewijzen.

De andere tabbladen bevatten de volgende typen functies:

* **Algemene functies** ![](assets/toolbar-icon-general-function.png) - Zie [Algemene functies in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) voor meer informatie .

* **Math-functies** ![](assets/toolbar-icon-math-functions.png) - Zie [Wiskundige functies in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) voor meer informatie .

* **Tekst- en binaire functies** ![](assets/toolbar-icon-text&binary-functions.png) - Zie [Tekenreeksfuncties in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) voor meer informatie .

* **Datum en tijd** ![](assets/toolbar-icon-date&time-functions.png) - Zie [Datum- en tijdfuncties in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) en de artikelen hieronder voor meer informatie .

   * [Tokens voor datum- en tijdnotaties in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Tokens voor datum- en tijdparsering in Adobe Workfront Fusion](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Functies voor het werken met arrays** ![](assets/toolbar-icon-functions-for-arrays.png) - Zie [Arrayfuncties in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) voor meer informatie .

>[!TIP]
>
>Wanneer u een complexe formule maakt die u opnieuw wilt gebruiken in een ander veld, kunt u klikken op het veld dat de combinatie bevat, Command-A of Ctrl-A gebruiken om de combinatie te selecteren en vervolgens kopiëren en in het andere veld plakken.

Zie voor meer informatie over het toewijzen van items met behulp van functies [Items toewijzen met behulp van functies in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md).

## Verzamelingen

Sommige items kunnen meerdere waarden van verschillende typen bevatten. Dit zijn verzamelingstypepunten.

U kunt een [!UICONTROL collection] Typ item door de kleine zwarte rechthoek rechts van het label van het item en de automatisch uitgevouwen lijst met subitems:

![](assets/collection.png)

>[!NOTE]
>
>In de meeste gevallen wijst u de subitems van de verzameling toe in plaats van het item dat de gehele verzameling vertegenwoordigt.

Voor meer informatie over verzamelingen raadpleegt u [Gegevenstypen item in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)

## Arrays

Sommige items kunnen meerdere elementen van hetzelfde type bevatten. Dit zijn arraytype-items.

U kunt een arraytype-item herkennen aan de vierkante haakjes aan het einde van het label van het item. Klik op de kleine zwarte rechthoek rechts van het label van het item om de items van het element weer te geven:

![](assets/array.png)

Zie voor meer informatie over arrays [Gegevenstypen item in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)

### Het eerste element van een array toewijzen

Als u een array toewijst `Recipient name` item, wordt het als volgt in het veld weergegeven:

![](assets/map-array-1st-element.png)

Het getal tussen de vierkante haakjes is een index die bepaalt welk element van de array wordt gebruikt. Deze is standaard ingesteld op 1.

### Het n-de element van een array toewijzen

Als u toegang wilt krijgen tot een ander element, klikt u op de vierkante haakjes en bewerkt u de indexwaarde:

![](assets/access-another-element.png)

### Het element van een array toewijzen met een bepaalde sleutel

Sommige arrays bevatten verschillende verzamelingen met sleutel- en waardeitems. Dit zijn doorgaans verschillende metagegevens, kenmerken, enzovoort.

In het volgende voorbeeld wordt de uitvoer van de [!DNL Jira] App.

![](assets/output-of-jira-app-350x100.png)

In dit voorbeeld krijgen we een bestandsnaam van een array met bijlagen voor de specifieke bijlage met een id van 10108.

De uitvoer van [!DNL Jira] ziet er als volgt uit:

![](assets/output-from-jira-350x261.png)

De typische eis moet een element door zijn bepaalde zeer belangrijke waarde opzoeken en de overeenkomstige waarde van het waardepunt verkrijgen. Dit kan worden bereikt met een formule die een combinatie van de `map()` en `get()` functies.

Hieronder volgt een gedetailleerde uitsplitsing van de formule:

1. De eerste parameter van de `map()` function is the entire array item.
1. De tweede parameter is de onbewerkte naam van het waardeitem. Als u de onbewerkte naam wilt verkrijgen, plaatst u de muisaanwijzer boven het item in het dialoogvenster [!UICONTROL mapping] paneel:

   ![](assets/obtain-raw-name-350x124.png)

   >[!NOTE]
   >
   >Alle parameters zijn hoofdlettergevoelig. Hoewel het label van het item in dit voorbeeld alleen in hoofdletters verschilt van de onbewerkte naam, moet u de naam Raw gebruiken. Dit is een kleine waarde in tegenstelling tot de labelwaarde.

1. De derde parameter is de onbewerkte naam van het sleutelitem:

   ![](assets/3rd-parameter-350x166.png)

1. De vierde parameter is de opgegeven sleutelwaarde.

Omdat `map()` functie retourneert een array (aangezien er meer elementen met de opgegeven sleutelwaarde kunnen zijn), is het nodig om de `get()` functie om het eerste element op te halen:

* De eerste parameter van de `get()` is het resultaat van de `map()` functie.

* De tweede parameter is de index van het element - één.

Voor meer informatie over de `map()` functie, zie [Arrayfuncties in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md).

Voor meer informatie over de `get()` functie, zie [Algemene functies in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md).

## Elementen omzetten in een reeks bundels

Arrays kunnen in een reeks bundels worden omgezet met behulp van de [!UICONTROL Iterator] module. Zie voor meer informatie [[!UICONTROL Iterator] module in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

![](assets/series-of-bundles-350x169.png)

## Problemen oplossen

### Ontbrekende items in het deelvenster Toewijzing

In het deelvenster Toewijzing worden voor elke module alle uitvoeritems weergegeven die door de auteur van de module worden vermeld. In sommige gevallen is deze lijst om verschillende redenen mogelijk onvolledig en ontbreken sommige items. [!DNL Workfront Fusion] kan de ontbrekende outputpunten automatisch ontdekken wanneer u de module in de scenarioredacteur in werking stelt. De nauwkeurige procedure verschilt lichtjes afhankelijk van het type van de module:

#### Instant trigger

1. Klik met de rechtermuisknop op de module en klik vervolgens op **[!UICONTROL Run this module only]** in het menu dat wordt weergegeven.

   Als er geen webhooks in de wachtrij zijn, wacht de module tot een nieuwe webhaak wordt verwerkt.

1. Genereer een webhaak.

   De module Webhaak **[!DNL Slack]>[!UICONTROL Listen for new events]** (die voor nieuwe kanaalberichten in een kanaal) kijkt verzendt een bericht naar het kanaal.

1. Wanneer de module eindigt lopend, klik de bel boven de module om zijn volledige output te onderzoeken.

   Het deelvenster Toewijzing bevat alle items die in de uitvoer van de module zijn aangetroffen.

#### Opiniepeilingtrigger

1. Klik met de rechtermuisknop op de module en klik vervolgens op **[!UICONTROL Run this module only]** in het menu dat wordt weergegeven.
1. Als er geen uitvoer is, klikt u op **[!UICONTROL Choose where to start]** en pas de instellingen aan.
1. Als er geen gebeurtenis moet worden verwerkt, maakt u er een en gaat u terug naar stap 2.

   De module Webhaak **[!UICONTROL Gmail]>[!UICONTROL Watch emails]** verzendt een e-mail naar de map die de module volgt.

1. Wanneer de module eindigt lopend, klik de bel boven de module om zijn volledige output te onderzoeken.

   Het deelvenster Toewijzing bevat nu alle items die zijn aangetroffen in de uitvoer van de module.

#### Overige modules

U kunt kiezen om uit te voeren:

* Het hele scenario (of alleen het onderdeel dat de module bevat)

   Als uw scenario met een trekker begint, verwijs naar [Instant trigger](#instant-trigger) of [Opiniepeilingtrigger](#polling-trigger) hierboven.

* Alleen de enkele module

Als u ervoor kiest alleen de enkele module uit te voeren:

1. Klik met de rechtermuisknop op de module en klik vervolgens op **[!UICONTROL Run this module only]** in het menu dat wordt weergegeven..
1. Geef voorbeeldwaarden op voor de invoeritems en klik vervolgens op **[!UICONTROL OK]** .
1. Wanneer de module eindigt lopend, klik de bel boven de module om zijn volledige output te onderzoeken.

   Het deelvenster Toewijzing bevat nu alle items die zijn aangetroffen in de uitvoer van de module.
