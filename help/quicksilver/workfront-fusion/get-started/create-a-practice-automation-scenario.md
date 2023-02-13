---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Creeer een scenario van de praktijkautomatisering in [!DNL Adobe Workfront Fusion]
description: In dit artikel wordt beschreven hoe u een automatiseringsscenario kunt maken met Adobe Workfront Fusion. Automatiseringsscenario's automatiseren Workfront-processen, waaronder gegevensmanipulatie en -transformatie. Dit voorbeeld neemt u door het proces om een scenario tot stand te brengen dat naar een project zoekt en dan alle taken verbonden aan dat project terugkeert.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '1683'
ht-degree: 0%

---

# Creeer een scenario van de praktijkautomatisering in [!DNL Adobe Workfront Fusion]

In dit artikel wordt beschreven hoe u een automatiseringsscenario kunt maken met Adobe Workfront Fusion. Automatiseringsscenario&#39;s automatiseren Workfront-processen, waaronder gegevensmanipulatie en -transformatie. Dit voorbeeld neemt u door het proces om een scenario tot stand te brengen dat naar een project zoekt en dan alle taken verbonden aan dat project terugkeert.

Voor instructies over het ontwikkelen van een integratiescenario dat afzonderlijke apps verbindt, zie [Een praktijkintegratiescenario maken in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

Ga voor meer informatie over de functionaliteit die beschikbaar is bij elke Workfront Fusion-licentie naar [Adobe Workfront Fusion-licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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

## Een praktijkscenario maken

De rol van [!DNL Adobe Workfront Fusion] is om uw processen te automatiseren zodat u zich op nieuwe taken kunt concentreren eerder dan het herhalen van de zelfde taken opnieuw en opnieuw. Het werkt door acties binnen en tussen apps en de diensten te verbinden om een scenario tot stand te brengen dat uw gegevens automatisch overbrengt en transformeert. Het scenario dat u voor gegevens in een app of service maakt, verwerkt die gegevens om het gewenste resultaat te verkrijgen.

Een scenario bestaat uit een reeks modules die aangeven hoe gegevens binnen een app moeten worden getransformeerd of moeten worden overgebracht tussen apps en webservices.
In dit voorbeeld wordt u door het proces geleid voor het maken van een scenario waarin wordt gezocht naar een [!DNL Workfront] en retourneert de taken in het project.

![](assets/create-practice-scenario-wf-only-350x157.png)

Het creëren van een scenario bestaat uit verscheidene hoofdtaken:

## Kies de apps en geef een naam op voor het scenario

1. Aanmelden bij uw [!DNL Workfront Fusion] account.
1. Klikken **[!UICONTROL Scenarios]** ![](assets/scenarios-icon.png) in het linkerdeelvenster.

   In het linkerpaneel dat toont, kunt u uw scenario&#39;s in omslagen organiseren.

   Boven aan het hoofdgebied rechts kunt u de **[!UICONTROL All]** scenario&#39;s die u hebt gemaakt, uw **[!UICONTROL Active Scenarios]**, **[!UICONTROL Inactive Scenarios]**, en **[!UICONTROL Concepts]**. Concepten zijn scenario&#39;s die nog wat werk nodig hebben [!DNL Workfront Fusion] U kunt ze indelen als actief of inactief.

   ![](assets/scenarios-left-panel-350x215.png)

1. Klik in het linkerdeelvenster op de knop **[!UICONTROL Add folder]** pictogram ![](assets/add-folder-icon.png)Typ vervolgens een naam als &quot;Praktische scenario&#39;s&quot; voor de eerste map.

1. Open de map en klik op **[!UICONTROL Create a new scenario]** in de rechterbovenhoek van de pagina.

   Op de openingspagina die wordt weergegeven, kunt u alle toepassingen die u wilt gebruiken, vooraf laden in het scenario dat u gaat maken.

1. Voor deze oefening zoekt en selecteert u **[!DNL Workfront]** app.
1. Klikken **[!UICONTROL Continue]** in de rechterbovenhoek.

   De vertoningen van de scenario redacteur, die een lege module in het centrum bevatten, [!DNL Workfront] een vooraf geladen toepassing en enkele opties in de werkbalk onderaan.

   ![](assets/scenario-editor-350x235.png)

   Wanneer u begint creërend een nieuw scenario, is het een goed idee om te beginnen door een naam voor het te creëren.

1. Selecteer **[!UICONTROL New scenario]** naam van plaatsaanduiding in de linkerbovenhoek, typ een naam zoals &quot;Praktisch scenario 1&quot;.
1. Doorgaan met [De eerste module toevoegen en configureren](#add-and-configure-the-first-module) hieronder.

## De eerste module toevoegen en configureren

De lege module met een vraagteken vertegenwoordigt de trekkermodule u moet toevoegen. Deze module zal het scenario beginnen telkens als het loopt. Het klokpictogram op de lege module wijst erop dat een geplande module is.

![](assets/empty-module.png)

Deze module zal de gegevens bevatten die u het scenario wilt letten op.

Voor dit voorbeeld gebruiken we geen triggermodule. In plaats daarvan begint dit scenario met een zoekopdracht.

1. Klik op de lege module om de app te kiezen waaruit u een module wilt selecteren.

   De toepassing die u eerder hebt geladen, wordt naast de lege module weergegeven. U kunt alle andere toepassingen die modules bevatten toevoegen met de opdracht [!UICONTROL Search] doos.

   ![](assets/pre-loaded-app-wf-350x172.png)

1. Klik op **[!DNL Workfront]**.

   De lijst verandert in een weergave van alle [!DNL Workfront] modules die u als trekkermodule kunt gebruiken.

1. Klik op de module Zoeken **[!UICONTROL Search]**.

   Nu moet u een geverifieerde verbinding tot stand brengen met uw [!DNL Workfront] account. Elke module die u aan een scenario toevoegt, moet een verbinding met de bijbehorende app hebben.

1. In de **[!DNL Workfront]** vak, onder **[!UICONTROL Connection]**, klikt u op **[!UICONTROL Add]**, typt u vervolgens een naam voor de verbinding, zoals &quot;Olivia&#39;s Workfront account&quot;, en klikt u op **[!UICONTROL Continue]**.
1. Verifieer de verbinding in het venster dat toont.

   Het proces voor het verifiëren van een verbinding kan een beetje tussen apps variëren. Het volgende proces is specifiek voor [!DNL Workfront], maar het proces is vergelijkbaar met veel apps.

   1. Voer uw [!DNL Workfront] domein, klik dan **[!UICONTROL Continue]**.
   1. Aanmelden [!DNL Workfront].
   1. Onderzoek de toegang die [!DNL Workfront Fusion] heeft een aanvraag ingediend en klikt u vervolgens op **[!UICONTROL Allow Access]**.

   Voor hulp zie [Verbinding maken [!DNL Adobe Workfront Fusion] naar een app of service](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## De eerste module configureren

Nadat u verbinding hebt gemaakt [!DNL Workfront Fusion] aan uw [!DNL Workfront] -account, kunt u een [!DNL Workfront] verzoekrij die u toegang tot en de gegevens hebt daar die u de eerste module wilt verwerken.

1. In de [!UICONTROL Record Type] selecteert u **[!UICONTROL Project]**. Dit plaatst de module aan onderzoek slechts projecten.

   >[!TIP]
   >
   >U kunt zoeken **[!UICONTROL Project]** in de lijst als u begint met het typen van het woord &quot;[!UICONTROL project].&quot;

1. In de **[!UICONTROL Result Set]** selecteert u **[!UICONTROL First Matching Record]**. Dit plaatst de module om slechts het eerste verslag terug te keren het vindt dat aan de criteria voldoet. Voor dit voorbeeld hebben we slechts één record nodig.
1. In de **[!UICONTROL Search criteria]** in dat gebied, zetten we een filter op om het specifieke project te retourneren.

   1. In het eerste vak onder [!UICONTROL Search Criteria]selecteert u het veld waarvan u de waarden wilt doorzoeken. In dit voorbeeld selecteert u **[!UICONTROL Name]**.
   1. Selecteer voor de operator [!UICONTROL Contains (case insensitive)]. Hierdoor kan de module projecten zoeken met de door u gekozen woorden in de naam, zelfs als u niet de volledige naam invoert of de naam met het onjuiste geval invoert (zoals alle hoofdletters).
   1. In het laatste veld onder [!UICONTROL Search Criteria], voert u een woord of woordgroep in waarvan u weet dat deze voorkomt in de naam van het project waarnaar u zoekt.

1. In de **[!UICONTROL Outputs]** selecteert u de velden die u wilt laten uitvoeren door de uitgave. Selecteer in dit voorbeeld de optie **[!UICONTROL ID]** en **[!UICONTROL Name]** velden.

   >[!TIP]
   >
   >U kunt **Cmd+F** ([!DNL Mac] of **Ctrl-F** ([!DNL Windows] OS) om snel een veld te vinden.

1. Klik op **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >(Alleen informatie) Aangezien dit geen triggermodule is, kunt u niet kiezen waar u de module wilt starten. Als u een triggermodule gebruikt, selecteert u nu waar u deze wilt starten.
   >
   >
   >Zie voor meer informatie [Kiezen waar een triggermodule begint in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. Klik met de rechtermuisknop op de module en klik op **[!UICONTROL Rename]**, dan typ een naam beschrijft wat u de module wilt doen (zoals &quot;Onderzoek naar project),&quot;dan klik **[!UICONTROL OK]**.

   De naam wordt net onder de module weergegeven. Hieronder: [!DNL Workfront Fusion] bevat een korte beschrijving van het type actie dat door de module wordt uitgevoerd.

   ![](assets/module-renamed-wf.png)

1. Doorgaan met [De tweede module toevoegen en configureren](#add-and-configure-the-second-module).

## De tweede module toevoegen en configureren

1. Klik op de gedeeltelijke cirkel rechts van de sectie van de module om **[!UICONTROL Add another module]**.
1. Selecteren [!DNL Workfront] Kies vervolgens de zoekmodule in de lijst met toepassingen **[!UICONTROL Read Related Records]**.
1. U hebt al een verbinding gemaakt met [!DNL Workfront] voor de vorige module. U te hoeven om het hier niet opnieuw tot stand te brengen, maar u moet ervoor zorgen deze module de zelfde verbinding zoals de vorige module gebruikt.\
   In de **[!UICONTROL Connection]** selecteert u de verbinding die u voor de vorige module hebt gemaakt.
1. Klikken **[!UICONTROL Record type]** selecteert u vervolgens **[!UICONTROL Project]**, omdat we records met betrekking tot een project willen lezen.

   >[!TIP]
   >
   >U kunt zoeken **[!UICONTROL Project]** in de lijst als u begint het woord &quot;project&quot; te typen.

1. Klik op de knop **[!UICONTROL Parent Record ID]** veld. Voor dit veld is de Workfront-id vereist van het project waaruit u taken wilt retourneren.

   Als u op het veld klikt, wordt de lijst met variabelen geopend die u kunt gebruiken in het dialoogvenster **[!UICONTROL Parent Record ID]** ter identificatie van het project in Workfront.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Klik op de variabele **[!UICONTROL ID]** om het aan **[!UICONTROL Parent Record ID]** veld. Dit staat identiteitskaart toe die van de eerste module is teruggekeerd om als herkenningsteken voor het project worden gebruikt dat u met in de tweede module wilt werken, die ervoor zorgt dat de teruggekeerde taken tot dat project zullen behoren.
1. In de **[!UICONTROL Collections]** veld, selecteren **[!UICONTROL Tasks]**. Dit wijst erop dat de module taken verbonden aan het gekozen project moet terugkeren.
1. Klik op **[!UICONTROL OK]**

   Nu hebt u een werkend scenario.

1. Geef de tweede module een naam zoals &quot;de taken van de Terugkeer verbonden aan project,&quot;dan verdergaan met [Het scenario testen](#test-the-scenario).

## Het scenario testen

Alvorens u uw scenario activeert, is het belangrijk om het te testen door het minstens eens in werking te stellen en de resultaten te bekijken. Dit helpt u begrijpen hoe de gegevens door het scenario stromen en om het even welke fouten vinden.

Wij kozen ervoor om 1 project te hebben teruggekeerd, evenals de taken verbonden aan dat project. Als u het scenario in werking stelt, is dat wat zou moeten gebeuren.

1. Klikken **[!UICONTROL Run once]** in de linkerbenedenhoek van de scenario-editor.
1. Nadat het scenario eindigt lopend, klik de bel boven de eerste module.

   ![](assets/click-bubble.png)

   In het vakje dat verschijnt, kunt u informatie over de bundel gegevens bekijken die de module verwerkte, met inbegrip van de daadwerkelijke gegevens die van het project werden getrokken dat de module terugkeerde.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Klik de uitvoercontrole bel boven de Tweede module om de input van informatie en de output te zien, die een inzameling van taken bevat in het project is.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   U kunt meer over leren hoe te om de informatie van de scenariouitvoering in de volgende artikelen te lezen:

   * Zie voor algemene informatie [Uitvoeringsstroom van scenario&#39;s in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Voor informatie over verwerkte bundels, zie [Uitvoering van scenario&#39;s, cycli en fasen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. In [!DNL Workfront Fusion], klikt u op **[!UICONTROL Save]** ![](assets/save-icon.png) in de linkerbenedenhoek om de voortgang van het scenario op te slaan.

   >[!IMPORTANT]
   >
   >Sla de bestanden vaak op terwijl u ze gebruikt en test een scenario.

>[!TIP]
>
>Wij adviseren de facultatieve maar nuttige praktijk om nota&#39;s over elke module toe te voegen.
>
>1. Klik met de rechtermuisknop op een [!DNL Workfront] en klik vervolgens op **[!UICONTROL Add a note]**.
>1. Typ een overzicht voor de module in de notitie die wordt weergegeven.

>
>   U kunt meerdere notities toevoegen voor een module.
>
>1. Sluit de **[!UICONTROL Notes]** gebied.
>
>   Nadat u een notitie aan een scenario hebt toegevoegd, wordt een oranje stip weergegeven op het tabblad **[!UICONTROL Notes]** pictogram ![](assets/notes-icon-w-dot.png) onder aan de scenario-editor.
>
>1. Klik op de knop **[!UICONTROL Notes]** pictogram ![](assets/notes-icon-w-dot.png) om uw notities weer te geven.

>




## Het scenario activeren

Dit voorbeeldscenario heeft geen triggermodule. Als dit een scenario zou zijn zou u voor echte gegevens gebruiken het met een trekkermodule beginnen, en het laatste ding u zou doen is het activeren. Nadat u een scenario activeert, door gebrek, loopt het om de 15 minuten. U kunt dit veranderen door te bepalen wanneer en hoe vaak u het wilt lopen.

Voor meer informatie over het activeren van scenario&#39;s, zie [Een scenario activeren of deactiveren in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Voor informatie over programma&#39;s, zie [Een scenario plannen in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
