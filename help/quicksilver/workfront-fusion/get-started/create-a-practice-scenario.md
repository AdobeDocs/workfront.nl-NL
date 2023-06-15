---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Een praktijkintegratiescenario maken in Adobe Workfront Fusion
description: In dit artikel wordt beschreven hoe u een integratiescenario kunt maken met Adobe Workfront Fusion. Met integratiescenario's worden afzonderlijke apps met elkaar verbonden, zodat uw gegevens door verschillende toepassingen kunnen worden geleid.
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: 99a8ad82c5fb2fb3f6adce9ff037086523be9b02
workflow-type: tm+mt
source-wordcount: '1974'
ht-degree: 0%

---

# Een praktijkintegratiescenario maken in Adobe Workfront Fusion

In dit artikel wordt beschreven hoe u een integratiescenario kunt maken met Adobe Workfront Fusion. Met integratiescenario&#39;s worden afzonderlijke apps met elkaar verbonden, zodat uw gegevens door verschillende toepassingen kunnen worden geleid.

Als u een integratiescenario wilt maken, moet uw organisatie een [!DNL Workfront Fusion for Work Automation and Integration] licentie.

Voor instructies over het bouwen van een Workfront-enige automatiseringsscenario, zie [Een praktijkautomatiseringsscenario maken in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

Voor meer informatie over Workfront Fusion-licenties raadpleegt u [Adobe Workfront Fusion-licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Een praktijkscenario maken

De rol van [!DNL Adobe Workfront Fusion] is om uw processen te automatiseren zodat u zich op nieuwe taken kunt concentreren eerder dan het herhalen van de zelfde taken opnieuw en opnieuw. Het werkt door acties binnen en tussen apps en de diensten te verbinden om een scenario tot stand te brengen dat uw gegevens automatisch overbrengt en transformeert. Het scenario dat u voor gegevens in een app of service maakt, verwerkt die gegevens om het gewenste resultaat te verkrijgen.

Een scenario bestaat uit een reeks modules die aangeven hoe gegevens binnen een app moeten worden getransformeerd of moeten worden overgebracht tussen apps en webservices.

Om te verklaren hoe te om een scenario tot stand te brengen en beste praktijken te versterken aangezien u leert te gebruiken [!DNL Workfront Fusion]Dit artikel doorloopt u stap voor stap het proces. We maken een scenario waarin een nieuwe record wordt gemaakt in [!DNL Workfront] voor elke rij in een [!DNL Google Sheets] spreadsheet.

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>Een scenario als dit zou nuttig zijn als u een spreadsheet het maken van een lijst van projecten had die aan het gebruiken van projecten in moeten worden gewerkt [!DNL Workfront]. Het scenario kon &quot;op&quot;spreadsheet voor nieuwe rijen letten en een nieuw project toevoegen binnen [!DNL Workfront] voor elk.

Het creëren van een scenario bestaat uit verscheidene hoofdtaken:

## Kies de apps en geef een naam op voor het scenario

1. Deze downloaden [spreadsheet](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx)uploadt u het vervolgens naar uw [!DNL Google Drive] gedurende deze oefening te gebruiken.

   of

   Uw eigen eenvoudige model maken of vinden [!DNL Google Sheets] Werkblad vergelijkbaar met dit:

   ![](assets/spreadsheet-headers-350x55.png)

1. Aanmelden bij uw [!DNL Workfront Fusion] account.
1. Klikken **[!UICONTROL Scenarios]** ![](assets/scenarios-icon.png) in het linkerdeelvenster.

   >[!NOTE]
   >
   >Als u het linkernavigatievenster of de bijbehorende pictogrammen niet ziet, klikt u op Menu ![Menu](assets/main-menu-icon-left-nav.png) pictogram.

   In grijs [!UICONTROL Folders] in het deelvenster dat wordt weergegeven, kunt u uw scenario&#39;s in mappen ordenen.

   Boven aan het hoofdgebied rechts kunt u de **[!UICONTROL All]** scenario&#39;s die u hebt gemaakt, uw **[!UICONTROL Active Scenarios]** en **[!UICONTROL Inactive Scenarios]**, en **[!UICONTROL Concepts]**, die scenario&#39;s zijn die nog wat meer werk behoeven [!DNL Workfront Fusion] U kunt ze indelen als actief of inactief.

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. In de [!UICONTROL Folders] klikt u op de knop **[!UICONTROL Add folder]** pictogram ![](assets/add-folder-icon.png)Typ vervolgens een naam als &quot;Praktische scenario&#39;s&quot; voor de eerste map.

1. Open de map en klik op **[!UICONTROL Create a new scenario]** in de rechterbovenhoek van de pagina.

   Op de openingspagina die wordt weergegeven, kunt u alle toepassingen die u wilt gebruiken, vooraf laden in het scenario dat u gaat maken.

1. Voor deze oefening zoekt en selecteert u **[!UICONTROL Google Sheets]** app.
1. Klikken **[!UICONTROL Continue]** in de rechterbovenhoek.

   De vertoningen van de scenario redacteur, die een lege module in het centrum bevatten, [!DNL Google Sheets] een vooraf geladen toepassing en enkele opties in de werkbalk onderaan.

<!--
   ![](assets/scenario-editor-350x235.png)
-->

Wanneer u begint creërend een nieuw scenario, is het een goed idee om te beginnen door een naam voor het te creëren.

1. Selecteer **[!UICONTROL New scenario]** naam van plaatsaanduiding in de linkerbovenhoek, typ een naam zoals &quot;Praktisch scenario 1&quot;.
1. Doorgaan met [De eerste module toevoegen en configureren](#add-and-configure-the-first-module) hieronder.

## De eerste module toevoegen en configureren

De lege module met een vraagteken vertegenwoordigt de trekkermodule u moet toevoegen. Deze module zal het scenario beginnen telkens als het loopt. Het klokpictogram op de lege module wijst erop dat een geplande module is.

![](assets/empty-module.png)

Deze module zal de gegevens bevatten die u het scenario wilt letten op.

1. Klik op de lege module om de app te kiezen waaruit u een module wilt selecteren.

   De toepassing die u eerder hebt geladen, wordt naast de lege module weergegeven. U kunt alle andere toepassingen die modules bevatten toevoegen met de opdracht [!UICONTROL Search] doos.

   ![](assets/pre-loaded-apps-350x139.png)

1. Klik op **[!DNL Google Sheets]**.

   De lijst verandert in een weergave van alle [!DNL Google Sheets] modules die u als trekkermodule kunt gebruiken.

1. Klik op de triggermodule **[!UICONTROL Watch for Records]**.

   Nu moet u een geverifieerde verbinding tot stand brengen met uw Google-account. Elke module die u aan een scenario toevoegt, moet een verbinding met de bijbehorende app hebben.

1. In de **[!DNL Google Sheets]** vak, onder **[!UICONTROL Connection]**, klikt u op **[!UICONTROL Add]**, typt u vervolgens een naam voor de verbinding, zoals &quot;Olivia&#39;s Google account&quot;, en klikt u op **[!UICONTROL Continue]**.
1. Verifieer de verbinding in het venster dat toont.

   Het proces voor het verifiëren van een verbinding kan een beetje tussen apps variëren. Mogelijk moet u zich aanmelden bij de app. Meestal moet u op een **[!UICONTROL Allow]** knop. Voor hulp zie [Verbinding maken [!DNL Adobe Workfront Fusion] naar een app of service](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## De eerste module configureren

Nadat u verbinding hebt gemaakt [!DNL Workfront Fusion] aan uw [!DNL Google Sheets] -account, kunt u een [!DNL Google Sheets] spreadsheet dat u toegang tot en de gegevens hebt daar die u de eerste module wilt verwerken.

1. Klik op de knop **[!UICONTROL Spreadsheet]** en selecteert u vervolgens de **[!UICONTROL Workfront Fusion practice scenario]#1** spreadsheet in de lijst die verschijnt.

   Dit spreadsheet bevat 2 bladen (lusjes), zodat moeten wij specificeren welk blad de gegevens bevat wij willen:

1. Selecteer in de vervolgkeuzelijst **[!UICONTROL Sheet]** de optie **[!UICONTROL Projects]**.

   Ons spreadsheet bevat kopballen en wij willen dat de module hen gebruikt om de gegevens te identificeren wij willen verwerken:

   ![](assets/spreadsheet-headers-350x55.png)

1. Verlaten **[!UICONTROL Yes]** geselecteerd voor **[!UICONTROL Table contains headers]**.

1. In de **[!UICONTROL Row with headers]** doos, kon u een waaier van rijen specificeren die u wilt omvatten, maar laten het gebrek A1:Z1 daar voor deze oefening verlaten.
1. In de **[!UICONTROL Limit]** vak, type 1.

   Deze manier, telkens als u het scenario in werking stelt, zal de module slechts 1 rij in spreadsheet verwerken. Dit is nuttig om uw testlooppas te vereenvoudigen terwijl u het scenario bouwt.

1. Klik op **[!UICONTROL OK]**.

   De **[!UICONTROL Choose where to start]** wordt u gevraagd op te geven waar in het spreadsheet de module moet beginnen met de verwerking.

1. Klikken **[!UICONTROL Choose manually]** selecteert u de bovenste optie in de lijst die wordt weergegeven en klikt u vervolgens op **[!UICONTROL OK]**.
1. Klik met de rechtermuisknop op de module en klik op **[!UICONTROL Rename]**, dan typ een naam beschrijft wat u de module wilt doen (zoals &quot;bekijk de projectlijst),&quot;dan klik **[!UICONTROL OK]**.

   De naam wordt net onder de module weergegeven. Hieronder: [!DNL Workfront Fusion] bevat een korte beschrijving van het type actie dat door de module wordt uitgevoerd.

   ![](assets/module-renamed-350x388.png)

1. Doorgaan met [De tweede module toevoegen en configureren](#add-and-configure-the-second-module).

## De tweede module toevoegen en configureren

1. Klik op de gedeeltelijke cirkel rechts van de sectie van de module om **[!UICONTROL Add another module]**.

   Deze tweede module moet een [!DNL Workfront] , maar we hebben de [!DNL Workfront] app.

1. Als u de [!DNL Workfront] app, begint met typen &quot;[!DNL Workfront]&quot; en klik op de toepassing wanneer deze wordt weergegeven.
1. In de lijst van [!DNL Workfront] modules die worden weergegeven, klikt u op **[!UICONTROL Create Record]**.

1. Zoals u eerder met de Google Sheets-app hebt gedaan, klikt u op **[!UICONTROL Add]** in de [!DNL Workfront] om een verbinding tussen Workfront Fusion en Workfront toe te voegen.

   Nu zullen wij beginnen te specificeren wat wij met de gegevens van spreadsheet willen doen.

1. Klikken **[!UICONTROL Record type]** selecteert u vervolgens **[!UICONTROL Project]** omdat we een project willen maken in [!DNL Workfront] een rij uit het werkblad gebruiken.

   >[!TIP]
   >
   >U kunt zoeken **[!UICONTROL Project]** in de lijst als u begint met het typen van het woord &quot;[!UICONTROL project].&quot;

   Het vak wordt uitgevouwen om alle beschikbare [!DNL Workfront] projectgebieden waar u de informatie kunt zetten die door de eerste module wordt gevonden.

   We gaan de **[!UICONTROL Name]** veld: wij willen deze module elk project in noemen [!DNL Workfront] de tekst gebruiken in het corresponderende [!UICONTROL Google Sheets] rij.

1. Zoeken en klikken op de knop **[!UICONTROL Name]** veld.

   >[!TIP]
   >
   >U kunt **Cmd+F** ([!DNL Mac] of **Ctrl-F**([!DNL Windows] OS) om snel een veld te vinden.

   Hiermee opent u de lijst met variabelen die u kunt gebruiken in het dialoogvenster **[!UICONTROL Name]** veld om de naam te definiëren voor elk project dat in Workfront is gemaakt.

   ![](assets/list-of-available-variables-350x261.png)

   De variabelen bij de bovenkant van de lijst komen overeen met de kolomkoppen in het werkblad.

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. Klik op de variabele **[!UICONTROL My Project Name (A)]** om het aan **[!UICONTROL Name]** veld.

   U hebt net uw eerste stuk gegevens voor dit scenario in kaart gebracht.

   Laten we nog een stukje gegevens uit het spreadsheet toewijzen aan [!DNL Workfront]: de begindatum voor elk project.

1. Zoeken en klikken op de knop **[!UICONTROL Planned Start Date]** en klik vervolgens op de knop **[!UICONTROL Planned Begin Date (E)]** variabele, om gegevens uit die kolom in het spreadsheet te trekken.

1. Klik op **[!UICONTROL OK]**.

   Nu hebt u een werkend scenario.

1. Geef de tweede module een naam, bijvoorbeeld &quot;Workfront-project maken&quot;, en ga vervolgens verder met [Het scenario testen](#test-the-scenario).

## Het scenario testen

Alvorens u uw scenario activeert, is het belangrijk om het te testen door het minstens eens in werking te stellen en de resultaten te bekijken. Dit helpt u begrijpen hoe de gegevens door het scenario stromen en om het even welke fouten vinden.

We hebben ervoor gekozen om 1 rij uit de spreadsheet te laten verwerken om een project te maken in Workfront. Als u het scenario in werking stelt, is dat wat zou moeten gebeuren.

1. Klikken **[!UICONTROL Run once]** in de linkerbenedenhoek van de scenario-editor.
1. Wanneer het scenario is voltooid, klikt u op de bel boven de [!DNL Google Sheets] module.

   ![](assets/click-bubble.png)

   In het vak dat wordt weergegeven, kunt u informatie weergeven over de bundel gegevens die de module heeft verwerkt, inclusief de feitelijke gegevens die uit het werkblad zijn gehaald voor de rij waarmee u bent begonnen.

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. Klik op de bel met de uitvoeringcontrole boven de knop [!DNL Workfront] module om de input van informatie en de output te zien, die identiteitskaart van het project is dat nu in wordt gecreeerd [!DNL Workfront]

   ![](assets/execution-inspector-wf-350x384.png)

   U kunt meer over leren hoe te om de informatie van de scenariouitvoering in de volgende artikelen te lezen:

   * Zie voor algemene informatie [Uitvoeringsstroom van scenario&#39;s in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Voor informatie over verwerkte bundels, zie [Uitvoering van scenario&#39;s, cycli en fasen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Ga naar [!DNL Workfront] en zoek naar &quot;soho downtown loft&quot; om het project te zien dat het scenario creëerde. Dit was de laatste rij in het spreadsheet.
1. In [!DNL Workfront Fusion], klikt u op **[!UICONTROL Save]** ![](assets/save-icon.png) in de linkerbenedenhoek om de voortgang van het scenario op te slaan.

   >[!IMPORTANT]
   >
   >Sla de bestanden vaak op terwijl u ze gebruikt en test een scenario.

## Voltooi het scenario en test het opnieuw

Wij moeten nog het scenario vormen om projecten voor alle andere rijen in spreadsheet tot stand te brengen.

1. Klik op de knop **[!UICONTROL Watch Rows]** die u voor Google Sheets hebt gemaakt.
1. Wijzig de **[!UICONTROL Limit]** tot en met 100.

   Het specificeren van een aantal hoger dan het aantal rijen u weet is in spreadsheet verzekert dat het scenario elk van hen zal vangen.

1. Klik met de rechtermuisknop op de knop **[!UICONTROL Watch Rows]** module, klikt u op **[!UICONTROL Choose where to start]**, klikt u op **[!UICONTROL All]** en klik vervolgens op **[!UICONTROL OK]**.

1. Klikken **[!UICONTROL Run once]** en bekijk wat er gebeurt in de bellen van de uitvoeringscontrole.

   De [!DNL Google] Bladen **[!UICONTROL Watch Rows]** de modulelooppas eens om alle rijen te lezen. Dan de Workfront **[!UICONTROL Create Record]** de modulelooppas 20 keer om een project voor elk van de resterende 20 rijen in spreadsheet tot stand te brengen.

1. Klik op de ballon van de uitvoeringcontrole voor de knop [!DNL Workfront] om alle 20 verrichtingen te bekijken, dan klik één van de verrichtingen om de informatie over het gemaakte project te bekijken.
1. Klikken **[!UICONTROL Save]** ![](assets/save-icon.png) in de linkerbenedenhoek.
1. Ga naar [!DNL Workfront] om de projecten te zien die het scenario creeerde.

>[!TIP]
>
>Wij adviseren de facultatieve maar nuttige praktijk om nota&#39;s over elke module toe te voegen.
>
>1. Klik met de rechtermuisknop op de knop [!DNL Workfront] en klik vervolgens op **[!UICONTROL Add a note]**.
>1. Typ een overzicht voor de module in de notitie die wordt weergegeven.
>
>    Dit is handig omdat u de module niet voortdurend hoeft te openen om te zien wat deze doet. U zou iets als &quot;kunnen typen creeert een project met Naam, Geplande Datum van het Begin, en Prioriteit die van spreadsheet wordt toegewezen.&quot;
>
>    Voor de [!UICONTROL Google Sheets] zou u iets als &quot;Lijst van het Project van het Controle voor nieuwe toegevoegde rijen/projecten kunnen typen.&quot;
>
>    U kunt meerdere notities toevoegen voor een module.
>
>1. Sluit de **[!UICONTROL Notes]** gebied.
>
>    Nadat u een notitie aan een scenario hebt toegevoegd, wordt een oranje stip weergegeven op het tabblad **[!UICONTROL Notes]** pictogram ![](assets/notes-icon-w-dot.png) onder aan de scenario-editor.
>
>1. Klik op de knop **[!UICONTROL Notes]** pictogram ![](assets/notes-icon-w-dot.png) om uw notities weer te geven.
>



## Het scenario activeren

Als dit een scenario zou zijn zou u voor echte gegevens gebruiken, het laatste ding u zou doen is het activeren. Nadat u een scenario activeert, door gebrek, loopt het om de 15 minuten. U kunt dit veranderen door te bepalen wanneer en hoe vaak u het wilt lopen.

Voor meer informatie over het activeren van scenario&#39;s, zie [Een scenario activeren of deactiveren in Adobe Workfront Fusion](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Voor informatie over programma&#39;s, zie [Een scenario plannen in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).
