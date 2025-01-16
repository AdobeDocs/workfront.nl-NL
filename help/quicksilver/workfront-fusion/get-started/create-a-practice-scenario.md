---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Een praktijkintegratiescenario maken in Adobe Workfront Fusion
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '2062'
ht-degree: 0%

---

# Een praktijkintegratiescenario maken in Adobe Workfront Fusion

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ Werkschema voor het creëren van een scenario ](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/plan-a-scenario/create-a-scenario-workflow.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

In dit artikel wordt beschreven hoe u een integratiescenario kunt maken met Adobe Workfront Fusion. Met integratiescenario&#39;s worden afzonderlijke apps met elkaar verbonden, zodat uw gegevens door verschillende toepassingen kunnen worden geleid.

Als u een integratiescenario wilt maken, moet uw organisatie een [!DNL Workfront Fusion for Work Automation and Integration] -licentie hebben.

Voor instructies bij het bouwen van een Workfront-Enige automatiseringsscenario, zie [ een scenario van de praktijkautomatisering in de Fusie van Adobe Workfront ](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md) creëren

Voor meer informatie over de vergunningen van de Fusie van Workfront, zie [ de Fusie van Adobe Workfront vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

>[!NOTE]
>
>Uw organisatie staat mogelijk geen toegang toe tot Google Sheets. Als dat het geval is, zult u niet deze integratie kunnen opzetten, maar de hier gepresenteerde informatie kan als algemeen voorbeeld van hoe de integratiescenario&#39;s functioneren worden gebruikt.

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

## Een praktijkscenario maken

De rol van [!DNL Adobe Workfront Fusion] is om uw processen te automatiseren zodat u zich op nieuwe taken kunt concentreren eerder dan het herhalen van de zelfde taken opnieuw en opnieuw. Het werkt door acties binnen en tussen apps en de diensten te verbinden om een scenario tot stand te brengen dat uw gegevens automatisch overbrengt en transformeert. Het scenario dat u voor gegevens in een app of service maakt, verwerkt die gegevens om het gewenste resultaat te verkrijgen.

Een scenario bestaat uit een reeks modules die aangeven hoe gegevens binnen een app moeten worden getransformeerd of moeten worden overgebracht tussen apps en webservices.

In dit artikel wordt stapsgewijs uitgelegd hoe u een scenario kunt maken en de beste werkwijzen kunt versterken terwijl u [!DNL Workfront Fusion] leert gebruiken. Er wordt een scenario gemaakt dat voor elke rij in een [!DNL Google Sheets] -spreadsheet een nieuwe record maakt in [!DNL Workfront] .

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>Een dergelijk scenario zou nuttig zijn als u een spreadsheet met projecten had die aan het gebruiken van projecten in [!DNL Workfront] moeten worden gewerkt. Het scenario kan de spreadsheet voor nieuwe rijen &#39;bekijken&#39; en voor elke rij een nieuw project toevoegen in [!DNL Workfront] .

Het creëren van een scenario bestaat uit verscheidene hoofdtaken:

## Kies de apps en geef een naam op voor het scenario

1. Download dit [ spreadsheet ](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx), dan upload het aan uw [!DNL Google Drive] voor gebruik door deze oefening.

   of

   Maak of zoek een eenvoudige [!DNL Google Sheets] -spreadsheet die vergelijkbaar is met deze:

   ![](assets/spreadsheet-headers-350x55.png)

1. Meld u aan bij uw [!DNL Workfront Fusion] -account.
1. Klik op **[!UICONTROL Scenarios]** ![](assets/scenarios-icon.png) in het linkerdeelvenster.

   >[!NOTE]
   >
   >Als u niet het linkernavigatievenster of zijn pictogrammen ziet, klik het pictogram van het Menu ![ Menu ](assets/main-menu-icon-left-nav.png).

   In het grijze [!UICONTROL Folders] deelvenster dat wordt weergegeven, kunt u uw scenario&#39;s ordenen in mappen.

   Boven aan het hoofdgebied rechts kunt u **[!UICONTROL All]** gemaakte scenario&#39;s, uw **[!UICONTROL Active Scenarios]** en **[!UICONTROL Inactive Scenarios]** en **[!UICONTROL Concepts]** weergeven. Dit zijn scenario&#39;s die meer werk vereisen voordat [!DNL Workfront Fusion] ze als actief of inactief kan classificeren.

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. Klik in het deelvenster [!UICONTROL Folders] op **[!UICONTROL Add folder]** icon ![](assets/add-folder-icon.png) en typ een naam als ‘Praktische scenario&#39;s’ voor de eerste map.

1. Open de map en klik vervolgens op **[!UICONTROL Create a new scenario]** rechtsboven op de pagina.

   Op de openingspagina die wordt weergegeven, kunt u alle toepassingen die u wilt gebruiken, vooraf laden in het scenario dat u gaat maken.

1. Zoek en selecteer hiervoor de app **[!UICONTROL Google Sheets]** .
1. Klik op **[!UICONTROL Continue]** in de rechterbovenhoek.

   De scenario-editor wordt weergegeven, met daarin een lege module in het midden, de [!DNL Google Sheets] -app die u vooraf hebt geladen en enkele opties op de werkbalk onderaan.

<!--
   ![](assets/scenario-editor.png)
-->

Wanneer u begint creërend een nieuw scenario, is het een goed idee om te beginnen door een naam voor het te creëren.

1. Selecteer de naam van de tijdelijke aanduiding **[!UICONTROL New scenario]** in de linkerbovenhoek en typ een naam zoals &quot;Praktisch scenario 1&quot;.
1. Ga met [ verder voeg en vorm de eerste hieronder module ](#add-and-configure-the-first-module) toe.

## De eerste module toevoegen en configureren

De lege module met een vraagteken vertegenwoordigt de trekkermodule u moet toevoegen. Deze module zal het scenario beginnen telkens als het loopt. Het klokpictogram op de lege module wijst erop dat een geplande module is.

![](assets/empty-module.png)

Deze module zal de gegevens bevatten die u het scenario wilt letten op.

1. Klik op de lege module om de app te kiezen waaruit u een module wilt selecteren.

   De toepassing die u eerder hebt geladen, wordt naast de lege module weergegeven. Met het vak [!UICONTROL Search] kunt u andere toepassingen toevoegen die modules bevatten.

   ![](assets/pre-loaded-apps-350x139.png)

1. Klik op **[!DNL Google Sheets]**.

   De lijst verandert om alle [!DNL Google Sheets] modules te tonen die u als trekkermodule kunt gebruiken.

1. Klik op de triggermodule **[!UICONTROL Watch for Records]** .

   Nu moet u een geverifieerde verbinding tot stand brengen met uw Google-account. Elke module die u aan een scenario toevoegt, moet een verbinding met de bijbehorende app hebben.

1. Klik in het vak **[!DNL Google Sheets]** onder **[!UICONTROL Connection]** op **[!UICONTROL Add]** en typ een naam voor de verbinding, bijvoorbeeld &quot;Google-account van Olivia&quot;, en klik vervolgens op **[!UICONTROL Continue]** .
1. Verifieer de verbinding in het venster dat toont.

   Het proces voor het verifiëren van een verbinding kan een beetje tussen apps variëren. Mogelijk moet u zich aanmelden bij de app. Meestal moet u op een knop **[!UICONTROL Allow]** klikken. Als u hulp nodig hebt, zie [ Overzicht van Verbindingen ](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## De eerste module configureren

Nadat u [!DNL Workfront Fusion] hebt verbonden met uw [!DNL Google Sheets] -account, kunt u een [!DNL Google Sheets] -spreadsheet opgeven waartoe u toegang hebt en de gegevens daar die de eerste module moet verwerken.

1. Klik op het vak **[!UICONTROL Spreadsheet]** en selecteer vervolgens het werkblad **[!UICONTROL Workfront Fusion practice scenario]#1** in de lijst die wordt weergegeven.

   Dit spreadsheet bevat 2 bladen (lusjes), zodat moeten wij specificeren welk blad de gegevens bevat wij willen:

1. Selecteer in de vervolgkeuzelijst **[!UICONTROL Sheet]** de optie **[!UICONTROL Projects]**.

   Ons spreadsheet bevat kopballen en wij willen dat de module hen gebruikt om de gegevens te identificeren wij willen verwerken:

   ![](assets/spreadsheet-headers-350x55.png)

1. Laat **[!UICONTROL Yes]** geselecteerd voor **[!UICONTROL Table contains headers]** .

1. In de doos **[!UICONTROL Row with headers]**, kon u een waaier van rijen specificeren die u wilt omvatten, maar laten het gebrek A1:Z1 daar voor deze oefening verlaten.
1. Typ 1 in het vak **[!UICONTROL Limit]** .

   Deze manier, telkens als u het scenario in werking stelt, zal de module slechts 1 rij in spreadsheet verwerken. Dit is nuttig om uw testlooppas te vereenvoudigen terwijl u het scenario bouwt.

1. Klik op **[!UICONTROL OK]**.

   In het vak **[!UICONTROL Choose where to start]** wordt u gevraagd op te geven waar in het werkblad de module moet beginnen met de verwerking.

1. Klik op **[!UICONTROL Choose manually]**, selecteer de bovenste optie in de lijst die wordt weergegeven en klik op **[!UICONTROL OK]** .
1. Klik met de rechtermuisknop op de module, klik op **[!UICONTROL Rename]** en typ een naam om te beschrijven wat de module moet doen (zoals &quot;De projectlijst bekijken&quot;). Klik vervolgens op **[!UICONTROL OK]** .

   De naam wordt net onder de module weergegeven. Hieronder bevat [!DNL Workfront Fusion] een korte beschrijving van het type actie dat door de module wordt uitgevoerd.

   ![](assets/module-renamed-350x388.png)

1. Ga met [ verder toevoegen en vormen de tweede module ](#add-and-configure-the-second-module).

## De tweede module toevoegen en configureren

1. Klik op de gedeeltelijke cirkel rechts van de sectie van de module naar **[!UICONTROL Add another module]** .

   Deze tweede module moet een [!DNL Workfront] -module zijn, maar we hebben de [!DNL Workfront] -app niet vooraf geladen.

1. Als u de app [!DNL Workfront] wilt zoeken, typt u &quot; [!DNL Workfront]&quot; en klikt u op de app wanneer deze wordt weergegeven.
1. Klik in de lijst met [!DNL Workfront] -modules die wordt weergegeven op **[!UICONTROL Create Record]** .

1. Zoals u eerder met de Google Sheets-app hebt gedaan, klikt u op **[!UICONTROL Add]** in het vak [!DNL Workfront] om een verbinding tussen Workfront Fusion en Workfront toe te voegen.

   Nu zullen wij beginnen te specificeren wat wij met de gegevens van spreadsheet willen doen.

1. Klik op **[!UICONTROL Record type]** en selecteer vervolgens **[!UICONTROL Project]** omdat we een project in [!DNL Workfront] willen maken met behulp van een rij in het werkblad.

   >[!TIP]
   >
   >U kunt **[!UICONTROL Project]** in de lijst vinden als u begint het woord &quot;[!UICONTROL project]&quot; te typen.

   Het vakje breidt zich uit om alle beschikbare [!DNL Workfront] projectgebieden te tonen waar u de informatie kunt plaatsen die door de eerste module wordt gevonden.

   We gebruiken het veld **[!UICONTROL Name]** : we willen dat deze module elk project in [!DNL Workfront] een naam geeft met de tekst in de bijbehorende [!UICONTROL Google Sheets] rij.

1. Zoek en klik op het veld **[!UICONTROL Name]** .

   >[!TIP]
   >
   >U kunt **Cmd+F** gebruiken ([!DNL Mac] OS) of **CTRL-F** ([!DNL Windows] OS) om een gebied snel te vinden.

   Hierdoor wordt de lijst geopend met variabelen die u in het veld **[!UICONTROL Name]** kunt gebruiken om de naam te definiëren voor elk project dat in Workfront is gemaakt.

   ![](assets/list-of-available-variables-350x261.png)

   De variabelen bij de bovenkant van de lijst komen overeen met de kolomkoppen in het werkblad.

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. Klik op de variabele **[!UICONTROL My Project Name (A)]** om deze aan het veld **[!UICONTROL Name]** toe te voegen.

   U hebt net uw eerste stuk gegevens voor dit scenario in kaart gebracht.

   Laten we nog een stukje gegevens uit het werkblad toewijzen aan [!DNL Workfront]: de begindatum voor elk project.

1. Zoek en klik op het veld **[!UICONTROL Planned Start Date]** en klik vervolgens op de variabele **[!UICONTROL Planned Begin Date (E)]** om gegevens uit die kolom in het werkblad te trekken.

1. Klik op **[!UICONTROL OK]**.

   Nu hebt u een werkend scenario.

1. Geef de tweede module een naam zoals &quot;creeer het project van Workfront,&quot;dan met [ test het scenario ](#test-the-scenario) verder.

## Het scenario testen

Alvorens u uw scenario activeert, is het belangrijk om het te testen door het minstens eens in werking te stellen en de resultaten te bekijken. Dit helpt u begrijpen hoe de gegevens door het scenario stromen en om het even welke fouten vinden.

We hebben ervoor gekozen om 1 rij uit de spreadsheet te laten verwerken om een project te maken in Workfront. Als u het scenario in werking stelt, is dat wat zou moeten gebeuren.

1. Klik op **[!UICONTROL Run once]** in de linkerbenedenhoek van de scenarioeditor.
1. Nadat het scenario is voltooid, klikt u op de bel boven de module [!DNL Google Sheets] .

   ![](assets/click-bubble.png)

   In het vak dat wordt weergegeven, kunt u informatie weergeven over de bundel gegevens die de module heeft verwerkt, inclusief de feitelijke gegevens die uit het werkblad zijn gehaald voor de rij waarmee u bent begonnen.

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. Klik op de ballon met de uitvoeringscontrole boven de module [!DNL Workfront] om de invoer van informatie en de uitvoer te zien. Dit is de id van het project dat nu is gemaakt in [!DNL Workfront]

   ![](assets/execution-inspector-wf-350x384.png)

   U kunt meer over leren hoe te om de informatie van de scenariouitvoering in de volgende artikelen te lezen:

   * Voor algemene informatie, zie [ de uitvoeringsstroom van het Scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Voor informatie over verwerkte bundels, zie [ uitvoering Scenario, cycli, en fasen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Ga naar [!DNL Workfront] en zoek naar &quot;soho downtown loft&quot; om het project te zien dat het scenario heeft gemaakt. Dit was de laatste rij in het spreadsheet.
1. Klik in [!DNL Workfront Fusion] in de linkerbenedenhoek op **[!UICONTROL Save]** ![](assets/save-icon.png) om de voortgang van het scenario op te slaan.

   >[!IMPORTANT]
   >
   >Sla de bestanden vaak op terwijl u ze gebruikt en test een scenario.

## Voltooi het scenario en test het opnieuw

Wij moeten nog het scenario vormen om projecten voor alle andere rijen in spreadsheet tot stand te brengen.

1. Klik op de module **[!UICONTROL Watch Rows]** die u voor Google Sheets hebt gemaakt.
1. Wijzig de **[!UICONTROL Limit]** in 100.

   Het specificeren van een aantal hoger dan het aantal rijen u weet is in spreadsheet verzekert dat het scenario elk van hen zal vangen.

1. Klik met de rechtermuisknop op de module **[!UICONTROL Watch Rows]** , klik op **[!UICONTROL Choose where to start]** , klik op **[!UICONTROL All]** en klik vervolgens op **[!UICONTROL OK]** .

1. Klik op **[!UICONTROL Run once]** en bekijk wat er gebeurt in de bellen van de uitvoercontrole.

   De module [!DNL Google] Bladen **[!UICONTROL Watch Rows]** wordt één keer uitgevoerd om alle rijen te lezen. Vervolgens wordt de Workfront **[!UICONTROL Create Record]** -module 20 keer uitgevoerd om een project te maken voor elk van de resterende 20 rijen in het werkblad.

1. Klik op de bel met de uitvoeringscontrole voor de module [!DNL Workfront] om alle 20 bewerkingen weer te geven en klik vervolgens op een van de bewerkingen om de informatie over het gemaakte project weer te geven.
1. Klik op **[!UICONTROL Save]** ![](assets/save-icon.png) in de linkerbenedenhoek.
1. Ga naar [!DNL Workfront] om de projecten te zien die het scenario creeerde.

>[!TIP]
>
>Wij adviseren de facultatieve maar nuttige praktijk om nota&#39;s over elke module toe te voegen.
>
>1. Klik met de rechtermuisknop op de module [!DNL Workfront] en klik vervolgens op **[!UICONTROL Add a note]** .
>1. Typ een overzicht voor de module in de notitie die wordt weergegeven.
>
>    Dit is handig omdat u de module niet voortdurend hoeft te openen om te zien wat deze doet. U zou iets als &quot;kunnen typen creeert een project met Naam, Geplande Datum van het Begin, en Prioriteit die van spreadsheet wordt toegewezen.&quot;
>
>    Voor de module [!UICONTROL Google Sheets] zou u iets als &quot;de Lijst van het Project van het Controle voor nieuwe toegevoegde rijen/projecten kunnen typen.&quot;
>
>    U kunt meerdere notities toevoegen voor een module.
>
>1. Sluit het **[!UICONTROL Notes]** -gebied.
>
>    Nadat u een notitie aan een scenario hebt toegevoegd, wordt een oranje stip weergegeven op het **[!UICONTROL Notes]** pictogram ![](assets/notes-icon-w-dot.png) onder aan de scenario-editor.
>
>1. Klik op het pictogram **[!UICONTROL Notes]** ![](assets/notes-icon-w-dot.png) om uw notities weer te geven.
>



## Het scenario activeren

Als dit een scenario zou zijn zou u voor echte gegevens gebruiken, het laatste ding u zou doen is het activeren. Nadat u een scenario activeert, door gebrek, loopt het om de 15 minuten. U kunt dit veranderen door te bepalen wanneer en hoe vaak u het wilt lopen.

Voor meer informatie over het activeren van scenario&#39;s, zie [ een scenario in de Fusie van Adobe Workfront activeren of deactiveren ](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Voor informatie over programma&#39;s, zie [ Plan een scenario in de Fusie van Adobe Workfront ](../../workfront-fusion/scenarios/schedule-a-scenario.md).
