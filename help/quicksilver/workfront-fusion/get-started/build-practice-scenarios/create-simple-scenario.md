---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Een basisscenario maken in [!DNL Adobe Workfront Fusion]
description: Leer hoe u een eenvoudig automatiseringsscenario maakt met Adobe Workfront Fusion. Automatiseringsscenario's automatiseren Workfront-processen, waaronder gegevensmanipulatie en -transformatie. In dit voorbeeld wordt u door het proces geleid voor het maken van een scenario waarin wordt gezocht naar een [!DNL Workfront] in Workfront en converteert het naar een project.
author: Becky
feature: Workfront Fusion
source-git-commit: 91d3dcde8eda416286c6781f6eef85404fd382c2
workflow-type: tm+mt
source-wordcount: '1240'
ht-degree: 0%

---

# Een basisscenario maken in [!DNL Adobe Workfront Fusion]

De rol van [!DNL Adobe Workfront Fusion] is om uw processen te automatiseren zodat u zich op nieuwe taken kunt concentreren eerder dan het herhalen van de zelfde taken opnieuw en opnieuw. Het werkt door acties binnen en tussen apps en de diensten te verbinden om een scenario tot stand te brengen dat uw gegevens automatisch overbrengt en transformeert. Het scenario dat u voor gegevens in een app of service maakt, verwerkt die gegevens om het gewenste resultaat te verkrijgen.

In dit voorbeeld wordt u door het proces geleid voor het maken van een scenario waarin wordt gezocht naar een [!DNL Workfront] in Workfront en converteert het naar een project.

<!--# Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>
To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## Een praktijkscenario maken

### Beginnen met het maken van het scenario

1. In de **Scenarios** gebied, klikken **Een nieuw scenario maken**.

   <!--To locate the Scenarios area, see navigation article-->

   De vertoningen van de scenario redacteur, die een lege module in het centrum bevatten.

   <!--picture?-->

1. Selecteer de **[!UICONTROL New scenario]** Geef een naam op voor de tijdelijke aanduiding in de linkerbovenhoek.
1. Doorgaan met [De eerste module toevoegen en configureren](#add-and-configure-the-first-module) hieronder.

### De eerste module toevoegen en configureren

1. Klik op de lege module om de app te kiezen waaruit u een module wilt selecteren.

   Rechts van de module wordt een lijst met apps weergegeven.

1. Selecteren **[!DNL Adobe Workfront]**. Als deze niet zichtbaar is, klikt u op de zoekbalk onder aan de lijst, typt u &quot;Workfront&quot; en selecteert u deze wanneer deze wordt weergegeven in de lijst.

   De lijst verandert in een weergave van alle [!DNL Workfront] modules die u kunt gebruiken.

1. Klik op de knop **[!UICONTROL Search]** -module.

   Het venster van de moduleconfiguratie opent.

1. In de [!UICONTROL Connection] selecteert u de Workfront-verbinding.

   Als u geen Workfront-verbinding hebt, raadpleegt u [Verbinding maken met [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. In de [!UICONTROL Record Type] vak, selecteren **[!UICONTROL Task]**. Hiermee stelt u de module in om alleen taken te zoeken.

   U kunt zoeken **[!UICONTROL Task]** in de lijst als u begint met het typen van het woord &quot;[!UICONTROL task].&quot;

1. In de **[!UICONTROL Result Set]** vak, selecteren **[!UICONTROL First Matching Record]**.

   Dit plaatst de module om slechts het eerste verslag terug te keren het vindt dat aan de criteria voldoet.
1. In de **[!UICONTROL Search criteria]** op, configureert u de criteria om de specifieke taak te retourneren.

   1. In het eerste vak onder [!UICONTROL Search Criteria]selecteert u het veld dat u in de zoekopdracht wilt opnemen. In dit voorbeeld selecteert u **[!UICONTROL Name]**.

      U kunt zoeken **[!UICONTROL Name]** in de lijst als u begint met het typen van het woord &quot;[!UICONTROL name].&quot;
   1. Voor de operator klikt u op de vervolgkeuzepijl naast **Exist** en wijzig deze in [!UICONTROL **Bevat (hoofdlettergevoelig)**].

      Hierdoor kan de module projecten zoeken met de door u gekozen woorden in de naam, zelfs als u niet de volledige naam invoert of de naam met het onjuiste geval invoert (zoals alle hoofdletters).
   1. In het laatste veld onder [!UICONTROL Search Criteria], voert u een woord of woordgroep in waarvan u weet dat deze zich in de naam van de taak bevindt waarnaar u zoekt.

1. In de **[!UICONTROL Outputs]** selecteert u de velden die u wilt uitvoeren in de module. Selecteer in dit voorbeeld de optie **[!UICONTROL ID]** en **[!UICONTROL Name]** velden.

   >[!TIP]
   >
   >U kunt **Cmd+F** ([!DNL Mac] (besturingssysteem) of **Ctrl-F** ([!DNL Windows] OS) om snel een veld te vinden.

1. Klikken **[!UICONTROL OK]** om de moduleconfiguratie te bewaren.

1. Klik met de rechtermuisknop op de module en klik op **[!UICONTROL Rename]**, dan typ een naam beschrijft wat u de module wilt doen (zoals &quot;Onderzoek naar taak),&quot;dan klik **[!UICONTROL OK]**.

   De naam wordt net onder de module weergegeven. Hieronder: [!DNL Workfront Fusion] bevat een korte beschrijving van het type actie dat door de module wordt uitgevoerd.

   ![](assets/module-renamed-wf.png)

1. Doorgaan met [De tweede module toevoegen en configureren](#add-and-configure-the-second-module).

## De tweede module toevoegen en configureren

1. Houd de muis boven de gedeeltelijke cirkel rechts van de module en klik vervolgens op **[!UICONTROL Add another module]**.
1. Selecteren [!DNL Adobe Workfront] van de lijst van toepassingen, dan kies de module **[!UICONTROL Convert object]**.
1. In de [!UICONTROL Connection] selecteert u dezelfde Workfront-verbinding die u in de vorige module hebt gebruikt.
1. In de **[!UICONTROL Record type]** veld, selecteren **[!UICONTROL Task]**, omdat de module een taak converteert.
1. In de **[!UICONTROL Convert to]** veld, selecteren **Project**.
1. Klik naast het veld Taak-id op de kaarthandeling om deze in te schakelen.

   De schakeloptie wordt blauw als deze is ingeschakeld. Hierdoor kunt u de taak-id uit de vorige module toewijzen.

   ![Kaarten schakelen](assets/map-toggle.png)
1. Klik op de knop **[!UICONTROL Task ID]** veld.

   Er wordt een deelvenster geopend waarin u kunt selecteren wat u wilt gebruiken als de id van de taak die u naar een project wilt converteren. Omdat u toewijzing hebt ingeschakeld, bevat het deelvenster uitvoer van eerdere modules. U hebt de id geselecteerd als uitvoer van de vorige module, zodat deze nu beschikbaar is in het deelvenster.

   Dit deelvenster wordt het deelvenster Toewijzing genoemd. Zie voor meer informatie over het deelvenster Toewijzing [De informatie van de kaart van één module aan een andere](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. Selecteren **ID** in het deelvenster Toewijzing.

   Er wordt een ID-blok weergegeven in het veld Id. Het toont het aantal van de module het van in kaart wordt gebracht, en het gebied dat in kaart wordt gebracht.

   ![Kaart-id](assets/map-id.png)

1. Klik op de knop **Sjabloon-id** veld, typt u de naam van de Workfront-sjabloon die u voor dit project wilt gebruiken en selecteert u deze sjabloon wanneer deze in de lijst wordt weergegeven.
1. Klikken **[!UICONTROL OK]** om de moduleconfiguratie te bewaren.

1. Klik met de rechtermuisknop op de module en klik op **[!UICONTROL Rename]**, dan typ een naam beschrijft wat u de module wilt doen (zoals &quot;Omzetten in project),&quot;dan klik **[!UICONTROL OK]**.

1. Doorgaan naar [Het scenario testen](#test-the-scenario).

## Het scenario testen

Alvorens u uw scenario activeert, is het belangrijk om het te testen door het minstens eens in werking te stellen en de resultaten te bekijken. Dit helpt u begrijpen hoe de gegevens door het scenario stromen en om het even welke fouten vinden.

Voor dit scenario, zou een succesvolle test in de plaats bepalen van de nieuwe taak en het omzetten in een project resulteren.

1. Klikken **[!UICONTROL Run once]** in de linkerbenedenhoek van de scenario-editor.
1. Nadat het scenario eindigt lopend, klik de bel boven de eerste module om informatie over de bundel van gegevens te bekijken die de module, met inbegrip van gegevens verwerkte die van de taak worden getrokken die de module terugkeerde.

1. Klik op de bel met de uitvoeringscontrole boven de tweede module om de invoer (de taak) en de uitvoer (het omgezette project) weer te geven.

   Zie voor meer informatie over de gegevens in de inspectiepbellen:

   * Zie voor algemene informatie [Uitvoeringsstroom scenario in [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-flow.md).
   * Voor informatie over verwerkte bundels, zie [Uitvoering van scenario&#39;s, cycli en fasen in [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. In [!DNL Workfront Fusion], klikt u op **[!UICONTROL Save]** in de linkerbenedenhoek om de voortgang van het scenario op te slaan.

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
>    U kunt meerdere notities toevoegen voor een module.
>
>1. Sluit het dialoogvenster **[!UICONTROL Notes]** gebied.
>
>     Nadat u een notitie aan een scenario hebt toegevoegd, wordt een oranje stip weergegeven op het tabblad **[!UICONTROL Notes]** pictogram ![](assets/notes-icon-w-dot.png) onder aan de scenario-editor.
>
>1. Klik op de knop **[!UICONTROL Notes]** pictogram ![](assets/notes-icon-w-dot.png) om uw notities weer te geven.
>

## Het scenario activeren

De laatste stap in het creëren van een scenario is het activeren.

Omdat dit scenario naar een specifieke taak zoekt, is er geen behoefte om het te activeren. Wanneer u een scenario activeert, wordt het uitgevoerd volgens een schema of wanneer een specifieke actie in een toepassing plaatsvindt. Nadat u een scenario activeert, door gebrek, loopt het om de 15 minuten. U kunt dit veranderen door te bepalen wanneer en hoe vaak u het wilt lopen.

Voor meer informatie over het activeren van scenario&#39;s, zie [Een scenario activeren of deactiveren in [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Voor informatie over programma&#39;s, zie [Een scenario plannen in [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md).

## Volgende stappen

* [Een triggermodule toevoegen](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/add-trigger-to-simple-scenario.md) om het scenario toe te staan om periodiek naar nieuwe verzoeken te zoeken en hen in projecten om te zetten.
* Voeg een webhaak toe om het scenario toe te staan om uit te voeren telkens als een verzoek is ingegaan.
* Voeg een filter toe om ervoor te zorgen dat slechts bepaalde verzoeken in projecten worden omgezet.
* Voeg een functie toe die de naam van het nieuwe project aanpast.
* Voeg foutafhandeling toe om ervoor te zorgen dat het scenario bestand is tegen fouten.

