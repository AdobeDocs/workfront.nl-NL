---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Een scenario maken in Adobe Workfront Fusion
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1398'
ht-degree: 0%

---

# Een scenario maken in [!DNL Adobe Workfront Fusion]

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

De volgende taken verklaren hoe te om een [!DNL Adobe Workfront Fusion] scenario tot stand te brengen.

Voor een oefening die u door het creëren van een automatiseringsscenario loopt, zie [ een scenario van de praktijkautomatisering in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md) creëren.

Voor een praktijkoefening die u door het creëren van een integratiescenario gebruikend gegevens loopt die wij verstrekken, zie [ een scenario van de praktijkintegratie in de Fusie van Adobe Workfront ](../../workfront-fusion/get-started/create-a-practice-scenario.md) creëren.

>[!NOTE]
>
>Om een scenario van een malplaatje tot stand te brengen, zie [ scenario&#39;s met  [!DNL Adobe Workfront Fusion]  malplaatjes ](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md) creëren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Adobe Workfront-plan</td>  
      <td>Alle</td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront-licentie</td>  
      <td>
        Nieuw: Standaard <br>
        Of<br>
        Huidig: Werk of hoger
      </td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront Fusion-licentie</td>  
      <td> 
        Huidig: Geen Workfront Fusion-licentievereisten.<br>
        Of<br>
        Verouderd: alle
      </td>  
    </tr>  
    <tr>  
      <td>Product</td>  
      <td> 
        Nieuw: Select- of Prime Workfront-abonnement: uw organisatie moet Adobe Workfront Fusion aanschaffen.<br>
        Ultimate Workfront Plan: Workfront Fusion is inbegrepen.<br>
        Of<br>
        Huidig: Uw organisatie moet Adobe Workfront Fusion aanschaffen.
      </td>  
    </tr> 
  </tbody>  
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Beginnen met het maken van een scenario

1. Klik op **[!UICONTROL Scenarios]** ![](assets/scenarios-icon.png) in het linkerdeelvenster.

1. Klik op **[!UICONTROL Create a new scenario]** rechtsboven op de pagina.
1. Als u een nieuw scenario maakt in het scherm dat wordt weergegeven (de scenario-editor), klikt u op **[!UICONTROL New scenario]** in de linkerbovenhoek en typt u een naam voor het scenario.
1. Ga op [ verder toevoegen een module in een scenario ](#add-a-module-in-a-scenario).

## Voeg een module in een scenario toe

1. Als u de eerste module aan het scenario wilt toevoegen, klikt u op het pictogram met het vraagteken. ![](assets/question-mark-icon.gif)

   of

   Om extra modules aan het scenario toe te voegen, klik de handvat op de rechterkant van de module u het wilt volgen.

1. Zoek en klik in het vak dat wordt weergegeven op de app of service waarmee u wilt beginnen.

   Eerder geselecteerde apps worden weergegeven in het vak, zodat u ze gemakkelijk kunt openen, en in de sectie **[!UICONTROL Favorites]** onder aan het scherm.

   Als u op **[!UICONTROL Add another module]** klikt, zijn de modules die worden weergegeven afhankelijk van waar in het scenario u de module toevoegt. Sommige modules kunnen slechts binnen tussen andere modules, en anderen slechts aan het begin van het scenario worden geplaatst.

   >[!TIP]
   >
   >De twee gemeenschappelijkste types van modules zijn acties en trekkers. Voor meer informatie, zie [ Types van modules ](../../workfront-fusion/modules/module-types.md).

1. In de lijst van modules die toont, klik de eerste module u aan het scenario wilt toevoegen.

   De modules die tonen hangen van af waar u een module in uw scenario wilt toevoegen. Sommige modules kunnen slechts binnen tussen andere modules, en anderen slechts aan het begin van het scenario worden geplaatst.

   De twee gemeenschappelijkste types van modules zijn acties en trekkers. Voor meer informatie, zie [ Types van modules ](../../workfront-fusion/modules/module-types.md).

1. Ga verder [ verbinden app of Webdienst van de module met  [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion).

## De app of webservice van de module verbinden met [!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

Workfront Fusion-modules die verbinding maken met een toepassing (zoals [!DNL Workfront] , [!DNL Salesforce] of [!DNL Jira)] ), hebben het veld [!UICONTROL Connection] . Hier kunt u opgeven welke verbinding deze module moet gebruiken om verbinding te maken met de app. U kunt een bestaande verbinding selecteren in het vervolgkeuzemenu of een nieuwe verbinding maken.

Wanneer u in een scenario een verbinding voor een app selecteert of maakt, gebruiken andere modules voor die app automatisch dezelfde verbinding, tenzij u een andere verbinding selecteert bij het instellen van de latere modules.

Voor meer informatie, zie [ Overzicht van Verbindingen ](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

Een verbinding maken binnen een module [!DNL Workfront Fusion] :

1. Klik op **[!UICONTROL Add]** om het vak **[!UICONTROL Create a connection]** te openen.
1. (Optioneel) Wijzig de standaardinstelling **[!UICONTROL Connection name]** .
1. (Voorwaardelijk) Als de toepassing geavanceerde verbindingsinstellingen nodig heeft, zoals een id, sleutel of [!UICONTROL secret] , voert u die gegevens in.

   Mogelijk moet u op **[!UICONTROL Show advanced settings]** klikken om de velden weer te geven waarin u dit soort informatie kunt invoeren.

1. Klik op **[!UICONTROL Continue]**.
1. Voer in het aanmeldingsvenster dat wordt weergegeven uw aanmeldingsgegevens in om u aan te melden bij de app als u dat nog niet hebt gedaan.
1. (Voorwaardelijk) Als een knop **[!UICONTROL Allow]** wordt weergegeven, controleert u de handelingen die de aansluiting kan uitvoeren en klikt u op de knop om de app aan te sluiten op [!DNL Workfront Fusion] .
1. Ga op [ verder vormen de module ](#configure-the-module).


## De module configureren

1. In de gebieden onder het gebied van de Verbinding, vorm de montages voor de module, dan klik **[!UICONTROL OK]**.

   ![](assets/conf-settigs-mod-350x547.png)

   Deze instellingen verschillen voor elke module. Een bolde titel wijst op een vereiste het plaatsen.

   >[!TIP]
   >
   >Terwijl u aan uw scenario werkt, kunt u op de module klikken om dit vak met instellingen op elk gewenst moment weer te geven.
   >
   >
   >Als u een zwarte cirkel op een module ziet, hebt u niet klaar met het vormen van zijn montages. Klik op de module om deze te openen en verder te configureren.
   >
   >
   >![](assets/black-error-circle-on-module.png)

1. Als u de eerste module in uw scenario toevoegt, selecteer een optie om erop te wijzen waar u het scenario wilt beginnen telkens als het loopt.

   ![](assets/choose-where-start-350x194.png)

1. Herhaal de stappen in de secties [ toevoegen een module in een scenario ](#add-a-module-in-a-scenario) en [ vormen de module ](#configure-the-module) om andere modules aan het scenario toe te voegen.

1. (Optioneel) Kopieer en plak een module of groep modules.

   Voor meer informatie, zie [ modules of scenario&#39;s van het Exemplaar in de Fusie van Adobe Workfront ](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

1. Ga op [ verder vormen en met uw scenario ](#configure-and-work-with-your-scenario) werken.

## Vorm en werk met uw scenario

1. Voer een van de volgende handelingen uit om uw scenario te configureren:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Opgeven wanneer en hoe vaak het scenario wordt uitgevoerd</td> 
      <td> <p>Klik op het klokpictogram. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Voor meer informatie, zie <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref"> Plan een scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een route instellen</td> 
      <td> <p>Klik op het moersleutelpictogram <img src="assets/wrench-icon.gif"> tussen de twee modules en gebruik een van de volgende opties. Voor meer informatie, zie <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref"> een filter aan een scenario in [!DNL Adobe Workfront Fusion]</a> toevoegen.</p> 
       <ul> 
        <li><strong>[!UICONTROL Set up a filter]</strong>: Hiermee bepaalt u welke bundels op bepaalde punten in het scenario worden gebruikt.</li> 
        <li><strong>[!UICONTROL Unlink]</strong>: Verwijdert een route.</li> 
        <li><strong>[!UICONTROL Add a router]</strong>: Voegt een router tussen modules toe. </li> 
        <li><strong>[!UICONTROL Add a module]</strong>: Voegt een nieuwe module tussen modules toe.</li> 
        <li><strong>[!UICONTROL Add a note]</strong>: Voegt een nota aan de route toe.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">De scenario-instellingen configureren</td> 
      <td>Klik op het pictogram [!UICONTROL Scenario settings] . <img src="assets/gear-icon-settings.png"> Deze instellingen zijn vooral bedoeld voor geavanceerde gebruikers. Zie <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref"> Het deelvenster met scenario-instellingen in [!DNL Adobe Workfront Fusion]</a> voor meer informatie.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stroomregelinstellingen configureren</td> 
      <td> <p>Klik op het pictogram [!UICONTROL Flow Control] . <img src="assets/flow-control-icon.gif"> U kunt een taak instellen om een bepaald aantal keren te herhalen, een array om te zetten in een reeks bundels en verschillende bundels samen te voegen tot één bundel. Voor meer informatie, zie <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref"> controle van de Stroom in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Het scenario verbeteren met geavanceerde gereedschappen</td> 
      <td>Klik op het pictogram [!DNL Tools] . <img src="assets/tools-icon.gif"> U kunt triggers, handelingen, aggregators en transformatoren maken. Voor meer informatie, zie <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref"> Hulpmiddelen </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gereedschappen voor het parseren van tekst door gebruikers</td> 
      <td>Klik op het pictogram [!DNL Text parser] <img src="assets/text-parser-icon.gif"> . U kunt HTML-elementen ophalen, tekenreekselementen zoeken en uitpakken die overeenkomen met een zoekpatroon, tekst zoeken en vervangen en gegevens van een website verwijderen. Voor meer informatie, zie <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref"> Hulpmiddelen </a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Voer een van de volgende handelingen uit om met uw scenario te werken:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Bekijk een logboek van de gebeurtenissen die voorkomen wanneer het scenario loopt</td> 
      <td> <p>Klik op de [!UICONTROL Exit editing] pijl <img src="assets/exit-editing-arrow.png"> in de scenarioeditor om de vervolgkeuzepagina Scenario-detail weer te geven. Het logbestand wordt onder in het venster of in de rechterbenedenhoek weergegeven. Het bevat informatie over elke fase en om het even welke fouten die tijdens de uitvoering van het scenario worden ontmoet.</p> <p>Als u wilt terugkeren naar het werken met uw scenario in de [!DNL scenario editor] , klikt u ergens op de detailpagina Scenario.</p> <p>Voor meer informatie over de de detailpagina van het Scenario, zie <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref"> details van het Scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Toegang tot veelgebruikte apps en services</td> 
      <td> Klik op een pictogram in de sectie <strong>[!UICONTROL Favorites]</strong> onder aan het scherm. Pictogrammen worden automatisch in deze sectie weergegeven wanneer u apps en services toevoegt aan uw scenario. U kunt ook handmatig op het pictogram [!UICONTROL Add] <img src="assets/add-icon.gif"> klikken om apps en services aan dit gebied toe te voegen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een animatie weergeven die aangeeft hoe gegevens door het scenario lopen</td> 
      <td>Klik op het pictogram [!UICONTROL Explain flow] <img src="assets/explain-flow-airplane-icon.gif"> .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">De lay-out van de modules automatisch uitlijnen </td> 
      <td>Klik op het pictogram [!UICONTROL Auto-align] <img src="assets/auto-align-icon.gif"> .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Opmerkingen over het scenario typen of weergeven</td> 
      <td>Klik op het pictogram [!UICONTROL Notes] <img src="assets/notes-icon.gif"> .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een module verwijderen</td> 
      <td>Klik met de rechtermuisknop op de module en klik vervolgens op <strong>[!UICONTROL Delete module]</strong> .</td> 
     </tr> 
    </tbody> 
   </table>

1. Klik op **[!UICONTROL Run once]** als u het scenario wilt testen.

   Het is belangrijk om te verifiëren dat het scenario zoals u verwacht loopt alvorens u het activeert. Nadat het scenario is geactiveerd, wordt het volgens het schema uitgevoerd. Als alles niet zoals verwacht loopt, zie [ Fout behandeling in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).

1. Wanneer u klaar bent met het bewerken van het scenario (of op elk gewenst moment terwijl u aan het bewerken bent), klikt u op het pictogram [!UICONTROL Save] onder aan het venster ![](assets/save-icon.gif) .

Voor informatie over het activeren van een scenario, zie [ een scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md) activeren of deactiveren.

## Sneltoetsen voor Workfront Fusion-scenario

U kunt de volgende sneltoetsen gebruiken bij het maken of bewerken van een scenario:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p>Handeling</p> </th> 
   <th>[!DNL Windows]</th> 
   <th> <p>[!DNL MacOS]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Save] </td> 
   <td>Ctrl+Shift+S</td> 
   <td><span style="font-weight: normal;"> Cmd+Shift+S </span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Run Once]</td> 
   <td>Ctrl+Shift+Enter</td> 
   <td><span style="font-weight: normal;"> Cmd+Shift+Enter </span> </td> 
  </tr> 
 </tbody> 
</table>
