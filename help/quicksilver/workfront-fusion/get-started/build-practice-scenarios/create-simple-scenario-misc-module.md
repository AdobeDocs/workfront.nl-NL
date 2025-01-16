---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Creeer een eenvoudig scenario in  [!DNL Adobe Workfront Fusion]
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
hide: true
hidefromtoc: true
feature: Workfront Fusion
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1232'
ht-degree: 0%

---

# Een basisscenario maken in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ creeer een basisscenario ](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/create-basic-scenario.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

De rol van [!DNL Adobe Workfront Fusion] is om uw processen te automatiseren zodat u zich op nieuwe taken kunt concentreren eerder dan het herhalen van de zelfde taken opnieuw en opnieuw. Het werkt door acties binnen en tussen apps en de diensten te verbinden om een scenario tot stand te brengen dat uw gegevens automatisch overbrengt en transformeert. Het scenario dat u voor gegevens in een app of service maakt, verwerkt die gegevens om het gewenste resultaat te verkrijgen.

In dit voorbeeld wordt u door het proces geleid voor het maken van een scenario waarin wordt gezocht naar een uitgave in Workfront. De methode zet deze om in een project.

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

1. In het **gebied van Scenario&#39;s**, klik **creeer een nieuw scenario**.

   <!--To locate the Scenarios area, see navigation article-->

   De vertoningen van de scenario redacteur, die een lege module in het centrum bevatten.

   <!--picture?-->

1. Selecteer de naam van de tijdelijke aanduiding **[!UICONTROL New scenario]** in de linkerbovenhoek en voer een naam in.
1. Ga met [ verder voeg en vorm de eerste hieronder module ](#add-and-configure-the-first-module) toe.

### De eerste module toevoegen en configureren

1. Klik op de lege module om de app te kiezen waaruit u een module wilt selecteren.

   Rechts van de module wordt een lijst met apps weergegeven.

1. Selecteer **[!DNL Adobe Workfront]** . Als deze niet zichtbaar is, klikt u op de zoekbalk onder aan de lijst, typt u &quot;Workfront&quot; en selecteert u deze wanneer deze wordt weergegeven in de lijst.

   In de lijst worden alle modules weergegeven die u kunt gebruiken. [!DNL Workfront]

1. Klik op de module **[!UICONTROL Search]** .

   Het venster van de moduleconfiguratie opent.

1. Selecteer in het vak [!UICONTROL Connection] de Workfront-verbinding.

   Als u geen verbinding van Workfront hebt, zie [ een verbinding tot stand brengen  [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. Selecteer **[!UICONTROL Issue]** in het vak [!UICONTROL Record Type] . Hiermee stelt u de module in om alleen problemen te zoeken.

   U kunt **[!UICONTROL Issue]** in de lijst vinden als u begint het woord &quot;[!UICONTROL issue]&quot; te typen.

1. Selecteer **[!UICONTROL First Matching Record]** in het vak **[!UICONTROL Result Set]** .

   Dit plaatst de module om slechts het eerste verslag terug te keren het vindt dat aan de criteria voldoet.
1. Configureer in het gebied **[!UICONTROL Search criteria]** de criteria om het specifieke probleem te retourneren.

   1. Selecteer in het eerste vak onder [!UICONTROL Search Criteria] het veld dat u in de zoekopdracht wilt opnemen. Selecteer **[!UICONTROL Name]** voor dit voorbeeld.

      U kunt **[!UICONTROL Name]** in de lijst vinden als u begint het woord &quot;[!UICONTROL name]&quot; te typen.
   1. Voor de exploitant, klik de dropdown pijl naast **bestaat** en verander het in [!UICONTROL **Bevat (geval ongevoelig)**].

      Hierdoor kan de module projecten zoeken met de door u gekozen woorden in de naam, zelfs als u niet de volledige naam invoert of de naam met het onjuiste geval invoert (zoals alle hoofdletters).
   1. Voer in het laatste veld onder [!UICONTROL Search Criteria] een woord of woordgroep in waarvan u weet dat deze voorkomt in de naam van de uitgave waarnaar u zoekt.

1. Selecteer in de lijst **[!UICONTROL Outputs]** de velden die de module moet uitvoeren. Selecteer in dit voorbeeld de velden **[!UICONTROL ID]** en **[!UICONTROL Name]** .

   >[!TIP]
   >
   >U kunt **Cmd+F** gebruiken ([!DNL Mac] OS) of **CTRL-F** ([!DNL Windows] OS) om een gebied snel te vinden.

1. Klik **[!UICONTROL OK]** om de moduleconfiguratie te bewaren.

1. Klik met de rechtermuisknop op de module, klik op **[!UICONTROL Rename]** en typ een naam met een beschrijving van wat de module moet doen (bijvoorbeeld &#39;Uitgave zoeken&#39;). Klik vervolgens op **[!UICONTROL OK]** .

   De naam wordt net onder de module weergegeven. Hieronder bevat [!DNL Workfront Fusion] een korte beschrijving van het type actie dat door de module wordt uitgevoerd.

   ![](assets/)

1. Ga met [ verder toevoegen en vormen de tweede module ](#add-and-configure-the-second-module).

## De tweede module toevoegen en configureren

1. Beweeg de cursor over de gedeeltelijke cirkel rechts van de sectie van de module en klik vervolgens op **[!UICONTROL Add another module]** .
1. Selecteer [!DNL Adobe Workfront] in de lijst met toepassingen en kies vervolgens de module **[!UICONTROL Misc Action]** .

   In de module Handeling Misc kunt u handelingen uitvoeren in Workfront waarvoor geen speciale module beschikbaar is. In dit voorbeeld, wordt deze module gebruikt om de kwestie in een project om te zetten.
1. Selecteer in het veld [!UICONTROL Connection] dezelfde Workfront-verbinding als in de vorige module.
1. Selecteer **[!UICONTROL Issue]** in het veld **[!UICONTROL Record type]**, omdat de uit te voeren actie betrekking heeft op een probleem.
1. Op het **[!UICONTROL Action]** gebied, uitgezochte **convertToProject**. Dit is de actie die de geselecteerde kwestie in een Project zal omzetten.
1. Klik op het veld **[!UICONTROL ID]** .

   Er wordt een deelvenster geopend waarin u kunt selecteren wat u wilt gebruiken als de id van de uitgave die u naar een project wilt converteren. Het deelvenster bevat uitvoer uit vorige modules. Omdat u id hebt geselecteerd als uitvoer van de vorige module, is deze nu beschikbaar in het deelvenster.

   Dit deelvenster wordt het deelvenster Toewijzing genoemd. Voor meer informatie over het mappingpaneel, zie [ informatie van de Kaart van één module aan een andere ](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. Selecteer **identiteitskaart** in het mappingpaneel.

   Er wordt een ID-blok weergegeven in het veld Id. Het toont het aantal van de module het van in kaart wordt gebracht, en het gebied dat in kaart wordt gebracht.

   ![ identiteitskaart van de Kaart ](assets/map-id.png)

1. (Optioneel) Zoek in de sectie Project het veld Eigenaar-id op en typ uw naam in het veld en selecteer de naam wanneer deze wordt weergegeven. Hierdoor wordt u de eigenaar van het project en kunt u het gemakkelijker vinden in Workfront.

   >[!TIP]
   >
   >U kunt **Cmd+F** gebruiken ([!DNL Mac] OS) of **CTRL-F** ([!DNL Windows] OS) om een gebied snel te vinden.

1. Klik **[!UICONTROL OK]** om de moduleconfiguratie te bewaren.

1. Klik met de rechtermuisknop op de module, klik op **[!UICONTROL Rename]** en typ een naam om te beschrijven wat de module moet doen (bijvoorbeeld &quot;Omzetten in project)&quot;. Klik vervolgens op **[!UICONTROL OK]** .

1. Ga aan [ Test het scenario ](#test-the-scenario) verder.

## Het scenario testen

Alvorens u uw scenario activeert, is het belangrijk om het te testen door het minstens eens in werking te stellen en de resultaten te bekijken. Dit helpt u begrijpen hoe de gegevens door het scenario stromen en om het even welke fouten vinden.

Voor dit scenario, zou een succesvolle test in het bepalen van de plaats van de kwestie en het omzetten in een project resulteren.

1. Klik op **[!UICONTROL Run once]** in de linkerbenedenhoek van de scenarioeditor.
1. Nadat het scenario eindigt lopend, klik de bel boven de eerste module om informatie over de bundel van gegevens te bekijken die de module, met inbegrip van gegevens verwerkte die uit de kwestie worden gehaald die de module terugkeerde.

1. Klik op de bel met de uitvoeringcontrole boven de tweede module om de invoer (de uitgave) en de uitvoer (het omgezette project) weer te geven.

   Zie voor meer informatie over de gegevens in de inspectiepbellen:

   * Voor algemene informatie, zie [ de uitvoeringsstroom van het Scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Voor informatie over verwerkte bundels, zie [ uitvoering Scenario, cycli, en fasen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Klik in [!DNL Workfront Fusion] in de linkerbenedenhoek op **[!UICONTROL Save]** om de voortgang van het scenario op te slaan.

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

De laatste stap in het creëren van een scenario is het activeren.

Omdat dit scenario naar een specifieke kwestie zoekt, is er geen behoefte om het te activeren. Wanneer u een scenario activeert, wordt het uitgevoerd volgens een schema of wanneer een specifieke actie in een toepassing plaatsvindt. Nadat u een scenario activeert, door gebrek, loopt het om de 15 minuten. U kunt dit veranderen door te bepalen wanneer en hoe vaak u het wilt lopen.

Voor meer informatie over het activeren van scenario&#39;s, zie [ een scenario in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md) activeren of deactiveren.

Voor informatie over programma&#39;s, zie [ Plan een scenario in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
