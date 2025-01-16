---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Creeer een scenario van de praktijkautomatisering in  [!DNL Adobe Workfront Fusion]
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1482'
ht-degree: 0%

---

# Een praktijkautomatiseringsscenario maken in [!DNL Adobe Workfront Fusion]

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

Automatiseringsscenario&#39;s automatiseren Workfront-processen, waaronder gegevensmanipulatie en -transformatie. Dit artikel neemt u door het proces om een scenario te creëren dat naar een project zoekt en dan alle taken verbonden aan dat project terugkeert.

<!-- not sure why these are here?
For instructions on building an integration scenario that connects separate apps, see [Create a practice integration scenario in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

For more information on functionality available with each Workfront Fusion license, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

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

## Creeer een scenario van de automatiseringspraktijk

Met [!DNL Adobe Workfront Fusion] kunt u zich richten op belangrijke taken door herhalende taken te automatiseren. Er worden scenario&#39;s gemaakt voor het automatisch beheren van uw gegevens in verschillende apps en services.

Elk scenario bestaat uit modules die bepalen hoe gegevens binnen een app worden verwerkt of tussen verschillende apps en services worden overgedragen. U kunt bijvoorbeeld een scenario maken in Fusion om automatisch een [!DNL Workfront] -project te zoeken en de taken ervan weer te geven. Op deze manier bespaart Fusion u tijd en moeite door routinetaken uit te voeren.

Dit praktijkscenario neemt u door het proces om een scenario tot stand te brengen dat naar een [!DNL Workfront] project zoekt en de taken in het project terugkeert.

![](assets/create-practice-scenario-wf-only-350x157.png)

### Voordat u begint

Creeer een project met taken in werkfront u voor deze oefening kunt gebruiken. U hoeft geen aanvullende configuratie buiten het toevoegen van taken aan het project uit te voeren.

Zie xxx voor informatie over het maken van een project in Workfornt.

### 1. Maak en noem het scenario

1. Meld u aan bij uw [!DNL Workfront Fusion] -account.
1. Klik op **[!UICONTROL Scenarios]** ![](assets/scenarios-icon.png) in het linkerdeelvenster.

   >[!NOTE]
   >
   >Als u niet het linkernavigatievenster of zijn pictogrammen ziet, klik het pictogram van het Menu ![ Menu ](assets/main-menu-icon-left-nav.png).

1. In het [!UICONTROL **paneel van Omslagen**], klik het **[!UICONTROL Add folder]** pictogram ![](assets/add-folder-icon.png), dan typ een naam als &quot;scenario&#39;s van de Praktijk&quot;voor uw eerste omslag.

1. Open de map en klik vervolgens op **[!UICONTROL Create a new scenario]** rechtsboven op de pagina.

1. Voor deze oefening, selecteer **[!DNL Adobe Workfront]** app, dan klik **Onderzoek** dichtbij de bodem.


1. Selecteer de naam van de tijdelijke aanduiding **[!UICONTROL New scenario]** in de linkerbovenhoek en typ een naam zoals &quot;Praktisch scenario 1&quot;.

   ![](assets/name-the-scenario.png)

1. Ga met [ verder verbind de eerste module ](#2-connect-the-first-module) hieronder.

### 2. Sluit de eerste module aan

Nu moet u een geverifieerde verbinding tot stand brengen met uw [!DNL Workfront] -account. Elke module die u aan een scenario toevoegt, moet een verbinding met de bijbehorende app hebben.

1. Klik in het vak **[!DNL Workfront]** onder **[!UICONTROL Connection]** op **[!UICONTROL Add]** en typ een naam voor de verbinding, bijvoorbeeld &quot;Workfront-account van Olivia&quot;, en klik vervolgens op **[!UICONTROL Continue]** .
1. Verifieer de verbinding in het venster dat toont.

   Het proces voor het verifiëren van een verbinding kan een beetje tussen apps variëren. Het volgende proces is specifiek voor [!DNL Workfront] , maar het proces is vergelijkbaar met veel apps:

   1. Voer uw [!DNL Workfront] -domein in en klik op **[!UICONTROL Continue]** .
   1. Meld u aan bij [!DNL Workfront] .
   1. Controleer de toegang die [!DNL Workfront Fusion] aanvraagt en klik op **[!UICONTROL Allow Access]** .

   Als u hulp nodig hebt, zie [ Overzicht van Verbindingen ](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

### 3. Vorm de eerste module

Nadat u [!DNL Workfront Fusion] met uw [!DNL Workfront] rekening verbindt, kunt u een [!DNL Workfront] project specificeren dat u toegang tot en de gegevens hebt die u de eerste module wilt verwerken.

1. Selecteer **[!UICONTROL Project]** in het vak [!UICONTROL Record Type] . Dit plaatst de module aan onderzoek slechts projecten.

   >[!TIP]
   >
   >U kunt **[!UICONTROL Project]** in de lijst vinden als u begint het woord &quot;[!UICONTROL project]&quot; te typen.

1. Selecteer **[!UICONTROL First Matching Record]** in het vak **[!UICONTROL Result Set]** . Dit plaatst de module om slechts het eerste verslag terug te keren het vindt dat aan de criteria voldoet. Voor dit voorbeeld hebben we slechts één record nodig die wordt geretourneerd.
1. In het gebied **[!UICONTROL Search criteria]** wordt een filter ingesteld om het specifieke project te retourneren:

   | Veld | Handeling |
   |--------|-------------|
   | Zoekcriteria in velden | Selecteer het veld waarvan u de waarden wilt doorzoeken. Selecteer **[!UICONTROL Name]** voor dit voorbeeld. |
   | Zoekcriteria | Selecteer **[!UICONTROL Name]** in de eerste vervolgkeuzelijst. |
   | Basisoperatoren | Selecteer [!UICONTROL Contains (case insensitive)] in de tweede vervolgkeuzelijst. Hierdoor kan de module projecten zoeken met de door u gekozen woorden in de naam, zelfs als u niet de volledige naam invoert of de naam met het onjuiste geval invoert (zoals alle hoofdletters). |
   | Tekstvak | Voer een woord of woordgroep in waarvan u weet dat deze de naam is van het project waarnaar u zoekt. |

+++ Vouw uit om een voorbeeld op het scherm weer te geven.
   ![](assets/search-name.png)
+++

1. Selecteer in de lijst **[!UICONTROL Outputs]** de velden die de module moet uitvoeren. Selecteer in dit voorbeeld de velden **[!UICONTROL ID]** en **[!UICONTROL Name]** .

   >[!TIP]
   >
   >U kunt **Cmd+F** gebruiken ([!DNL Mac] OS) of **CTRL-F** ([!DNL Windows] OS) om een gebied snel te vinden.

1. Klik op **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >Aangezien dit geen triggermodule is, kunt u niet kiezen waar u deze wilt starten. Als u een triggermodule gebruikt, selecteert u nu waar u deze wilt starten.
   >
   >
   >Voor meer informatie, zie [ kiezen waar een trekkermodule in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md) begint.

1. Klik met de rechtermuisknop op de module, klik op **[!UICONTROL Rename]** en typ een naam om aan te geven wat u wilt doen met de module (bijvoorbeeld &quot;Zoeken naar project)&quot;. Klik vervolgens op **[!UICONTROL OK]** .

   De naam wordt net onder de module weergegeven. Hieronder bevat [!DNL Workfront Fusion] een korte beschrijving van het type actie dat door de module wordt uitgevoerd.

   ![](assets/module-renamed-wf.png)

1. Ga met [ verder toevoegen en vormen de tweede module ](#add-and-configure-the-second-module).

### 4. Voeg en vorm de tweede module toe

1. Klik op de gedeeltelijke cirkel rechts van de sectie van de module naar **[!UICONTROL Add another module]** .
1. Selecteer [!DNL Workfront] in de lijst met toepassingen en kies vervolgens de zoekmodule **[!UICONTROL Read Related Records]** .
1. Selecteer in het vak **[!UICONTROL Connection]** de verbinding die u voor de vorige module hebt gemaakt. U moet ervoor zorgen dat deze module dezelfde verbinding gebruikt als de vorige module.
1. Klik op **[!UICONTROL Record type]** en selecteer vervolgens **[!UICONTROL Project]** omdat we records willen lezen die betrekking hebben op een project.

   >[!TIP]
   >
   >U vindt **[!UICONTROL Project]** in de lijst als u het woord &quot;project&quot; begint te typen.

1. Klik op het veld **[!UICONTROL Parent Record ID]** . Voor dit veld is de Workfront-id vereist van het project waaruit u taken wilt retourneren.

   Als u op het veld klikt, wordt de lijst geopend met variabelen die u in het veld **[!UICONTROL Parent Record ID]** kunt gebruiken om het project in Workfront te identificeren.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Klik op de variabele **[!UICONTROL ID]** om deze aan het veld **[!UICONTROL Parent Record ID]** toe te voegen. Dit staat identiteitskaart toe die van de eerste module is teruggekeerd om als herkenningsteken voor het project worden gebruikt dat u met in de tweede module wilt werken, die ervoor zorgt dat de teruggekeerde taken tot dat project zullen behoren.
1. Selecteer **[!UICONTROL Tasks]** in het veld **[!UICONTROL Collections]** . Dit wijst erop dat de module taken verbonden aan het gekozen project moet terugkeren.
1. Selecteer **[!UICONTROL Id]** en **[!UICONTROL Name]** in het veld **[!UICONTROL Outputs]** .
1. Klikken **[!UICONTROL OK]**

   Nu hebt u een werkend scenario.

1. Geef de tweede module een naam zoals &quot;de taken van de Terugkeer verbonden aan project,&quot;dan met [ Test het scenario ](#test-the-scenario) verder.

## Het scenario testen

Alvorens u uw scenario activeert, is het belangrijk om het te testen door het minstens eens in werking te stellen en de resultaten te bekijken. Dit helpt u begrijpen hoe de gegevens door het scenario stromen en om het even welke fouten vinden.

Wij kozen ervoor om 1 project te hebben teruggekeerd, evenals de taken verbonden aan dat project. Als u het scenario in werking stelt, is dat wat zou moeten gebeuren.

1. Klik op **[!UICONTROL Run once]** in de linkerbenedenhoek van de scenarioeditor.
1. Nadat het scenario eindigt lopend, klik de bel boven de eerste module.

   ![](assets/click-bubble.png)

   In het vakje dat verschijnt, kunt u informatie over de bundel gegevens bekijken die de module verwerkte, met inbegrip van de daadwerkelijke gegevens die van het project werden getrokken dat de module terugkeerde.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Klik de uitvoercontrole bel boven de Tweede module om de input van informatie en de output te zien, die een inzameling van taken bevat in het project is.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   U kunt meer over leren hoe te om de informatie van de scenariouitvoering in de volgende artikelen te lezen:

   * Voor algemene informatie, zie [ de uitvoeringsstroom van het Scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Voor informatie over verwerkte bundels, zie [ uitvoering Scenario, cycli, en fasen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Klik in [!DNL Workfront Fusion] in de linkerbenedenhoek op **[!UICONTROL Save]** ![](assets/save-icon.png) om de voortgang van het scenario op te slaan.

   >[!IMPORTANT]
   >
   >Sla de bestanden vaak op terwijl u ze gebruikt en test een scenario.

>[!TIP]
>
>Wij adviseren de facultatieve maar nuttige praktijk om nota&#39;s over elke module toe te voegen.
>
>1. Klik met de rechtermuisknop op een module [!DNL Workfront] en klik vervolgens op **[!UICONTROL Add a note]** .
>1. Typ een overzicht voor de module in de notitie die wordt weergegeven.
>
>    U kunt meerdere notities toevoegen voor een module.
>
>1. Sluit het **[!UICONTROL Notes]** -gebied.
>
>     Nadat u een notitie aan een scenario hebt toegevoegd, wordt een oranje stip weergegeven op het **[!UICONTROL Notes]** pictogram ![](assets/notes-icon-w-dot.png) onder aan de scenario-editor.
>
>1. Klik op het pictogram **[!UICONTROL Notes]** ![](assets/notes-icon-w-dot.png) om uw notities weer te geven.
>

## Het scenario activeren

Dit voorbeeldscenario heeft geen triggermodule. Als dit een scenario zou zijn zou u voor echte gegevens gebruiken het met een trekkermodule beginnen, en het laatste ding u zou doen is het activeren. Nadat u een scenario activeert, door gebrek, loopt het om de 15 minuten. U kunt dit veranderen door te bepalen wanneer en hoe vaak u het wilt lopen.

Voor meer informatie over het activeren van scenario&#39;s, zie [ een scenario in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md) activeren of deactiveren.

Voor informatie over programma&#39;s, zie [ Plan een scenario in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
