---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Initiatiefstrijdigheden oplossen in de functie Scenario Planner
description: Wanneer initiatieven met elkaar in strijd zijn, concurreren zij om dezelfde middelen. De middelen u voor een scenario beschikbaar hebt zijn niet genoeg om alle middelen te behandelen die door alle initiatieven in het scenario worden vereist.
author: Alina
feature: Workfront Scenario Planner
exl-id: d3a3e177-bece-4e03-89d7-9cee6127bc55
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '2082'
ht-degree: 0%

---

# Initiatiefconflicten oplossen in de [!DNL Scenario Planner]

Wanneer initiatieven met elkaar in strijd zijn, concurreren zij om dezelfde middelen. De middelen u voor een scenario beschikbaar hebt zijn niet genoeg om alle middelen te behandelen die door alle initiatieven in het scenario worden vereist.

Dit kan in elk van de volgende gevallen gebeuren:

* Het aantal functies dat voor het initiatief vereist is, is groter dan het aantal rollen dat voor het plan in de begroting is opgenomen.
* De kosten van het initiatief zijn hoger dan het voor het plan beschikbare budget.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] of hoger</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licentie*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td><b>Product</b> </td> 
   <td> <p>U moet een extra licentie aanschaffen voor de [!DNL Adobe Workfront Scenario Planner] voor toegang tot de functionaliteit die in dit artikel wordt beschreven.</p> <p>Voor informatie over het verkrijgen van de [!DNL Workfront Scenario Planner], zie <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Toegang nodig om de [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraties op toegangsniveau*</strong> </td> 
   <td> <p>[!UICONTROL Edit] of hoger [!DNL Scenario Planner]</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau veranderen, zie <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objectmachtigingen</strong> </p> </td> 
   <td> <p>[!UICONTROL Manage] machtigingen voor een abonnement</p> <p>Voor informatie over het vragen van om extra toegang tot een plan, zie <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Toegang aanvragen tot een abonnement in de [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Overzicht van conflicten oplossen

* Een conflict wordt ook begrepen als een overmatige toewijzing van de functies of de begroting van een scenario.
* Wanneer [!DNL Workfront] detecteert een conflict. De balk die overeenkomt met de conflicterende maand tijdens de duur van het initiatief wordt in rood weergegeven. Dit kan in elk van de volgende gevallen gebeuren:

   * Het aantal functies dat maandelijks voor een initiatief vereist is, is groter dan het aantal rollen dat voor het plan in de begroting is opgenomen nadat alle vorige initiatieven de voor het plan begrote middelen hebben gebruikt.
   * De maandelijkse kosten van het initiatief zijn groter dan de begroting die voor het plan beschikbaar is, nadat alle eerdere initiatieven de begroting van het plan hebben gebruikt om hun kosten te dekken.

>[!TIP]
>
>Standaard worden de [!DNL Scenario Planner] gaat ervan uit dat u voor een scenario 0 taakrollen en $0 of het equivalent van $0 in de valuta van uw systeem hebt begroot, tenzij u anders hebt opgegeven. Het aantal functies geeft het aantal FTE&#39;s (voltijdequivalenten) of uren aan dat in de begroting is opgenomen voor de functie.
>
>Voor alle berekeningen in de Planner van het Scenario, gebruikt Workfront de volgende waarde: 1 FTE = 8 uur.
>
>Voor informatie over het bijwerken van de beschikbare rollen voor een plan en een begroting zie [Plannen maken en bewerken in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

* U kunt een conflict oplossen door één van het volgende te doen:

   * De ontbrekende vereiste middelen automatisch toevoegen uit de initiatieven op het scenario. In dit artikel wordt beschreven hoe conflicten met deze optie kunnen worden opgelost.
   * Het aanpassen van de functie en de begrotingsmiddelen voor het scenario, door het plan uit te geven. Zie voor meer informatie [Plannen maken en bewerken in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Conflicten tussen initiatieven oplossen

1. Ga naar een plan waarvoor u conflicten wilt oplossen.

   Voor informatie over het maken van plannen raadpleegt u [Plannen maken en bewerken in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   Voor informatie over het maken van initiatieven raadpleegt u [Initiatieven maken en bewerken in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Optioneel) Van de **[!DNL Initial scenario]** selecteert u het scenario dat u wilt bekijken.

   >[!TIP]
   >
   >Een plan kan verscheidene scenario&#39;s hebben. Als we naar de conflicten in het plan kijken, [!DNL Workfront] verwijst naar de middelen die momenteel beschikbaar zijn voor het geselecteerde scenario en naar de middelen die vereist zijn voor de initiatieven van dat scenario. Voor informatie over scenario&#39;s, zie [Plan-scenario&#39;s maken en vergelijken in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. Zorg ervoor dat **[!UICONTROL Show conflicts]** is ingeschakeld. Deze optie is standaard ingeschakeld.

   ![](assets/show-scenarios-toggle-on.png)

   Het eerste conflicterende initiatief geeft de maanden weer met rode conflicten en er verschijnt een waarschuwingspictogram naast de naam van het initiatief.

   De achtergrond van alle initiatieven die beginnen met het eerste conflicterende wordt in het rood weergegeven op het schema van het plan.

   Wanneer een initiatief een conflict vertoont, betekent dit dat het aantal functies voor minstens één specifieke rol, de gemaakte kosten of beide het aantal functies of het budget dat voor het plan voor een bepaalde maand is vastgesteld, overschrijden.

   ![](assets/initiatives-on-plan-with-conflicts-350x126.png)

1. Voer een van de volgende handelingen uit om meer te weten te komen over de conflicten die er kunnen zijn:

   * Houd de muisaanwijzer boven het waarschuwingspictogram naast de naam van het initiatief om te begrijpen of u een functie- of begrotingsconflict hebt.

      ![](assets/budget-job-role-conflict-tooltip-on-warning-icon-350x109.png)

      Afhankelijk van of u taakrollen te veel hebt toegewezen of te hoge kosten voor uw initiatief, ziet u mogelijk een van de volgende opties wanneer u de muisaanwijzer op het waarschuwingspictogram plaatst:

      * Conflictdetails voor taakrol tonen
      * Details begrotingsconflict tonen
      * Functie- en begrotingsgegevens weergeven
   * Wanneer het bekijken van het plan door maand, houd over een maand in de chronologie van het plan om de vereiste middelen voor die maand te bekijken en of de conflicten voor de maand mensen of op kosten-betrekking hebben zijn.

      ![](assets/details-of-conflicts-on-monthly-plan-timeline-pop-up-350x178.png)

      Controleer de volgende maandelijkse informatie op het planniveau:

      * Het aantal beschikbare, vereiste en overtoegewezen functies voor de maand voor alle initiatieven die voor die maand zijn gepland
      * De beschikbare, vereiste en overtoegewezen kosten voor de maand voor alle voor die maand geplande initiatieven

         >[!TIP]
         >
         >De [!UICONTROL Available] de kosten zijn de begroting van het scenario voor die maand .
   * Houd de muisaanwijzer gedurende een maand boven de rode balk van een initiatief om het extra informatievak weer te geven over het conflict dat zich die maand voordoet.

      ![](assets/details-of-conflicts-on-initiative-timeline-pop-up-350x113.png)

      Controleer de volgende velden in het vak Aanvullende informatie op het niveau van het initiatief:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Maand waarin het conflict optreedt</td> 
        <td>Dit wordt weergegeven in de titel van het vak Aanvullende informatie.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">De naam van het initiatief</td> 
        <td>Dit wordt weergegeven in de titel van het vak Aanvullende informatie.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">[!UICONTROL Job Roles]</td> 
        <td> <p>De functies die aan dit initiatief zijn gekoppeld en die voor de geselecteerde maand zijn oververdeeld. In de volgende kolommen wordt informatie weergegeven voor elke taakrol die voor de geselecteerde maand is vereist en die een conflict veroorzaakt met het aantal functies dat voor die maand beschikbaar is:</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Available]</strong>: Het aantal van elke baanrol beschikbaar bij het scenario voor de geselecteerde maand.</p> </li> 
          <li> <p><strong>[!UICONTROL Required]</strong>: Het aantal van elke baanrol die voor het initiatief voor de geselecteerde maand wordt vereist.</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Overallocated]:</strong> Het verschil tussen het op het initiatief vereiste aantal en het beschikbare aantal van het scenario. </p> </li> 
         </ul> <p>Tip: Het aantal [!UICONTROL Available] rollen komen overeen of is hoger dan het aantal [!UICONTROL Required] rollen, maar de [!DNL Scenario Planner] er is nog steeds sprake van een overtoewijzing . Dit betekent dat er hogere-rangschikkingsinitiatieven zijn die reeds de baanrollen gebruikten die in het plan voor dezelfde maand beschikbaar waren. </p> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Kosten</td> 
        <td> <p>De kosten van het initiatief voor de geselecteerde maand. De volgende kolommen bevatten informatie over de benodigde kosten en het beschikbare budget voor de geselecteerde maand:</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Available]</strong>: De begroting die beschikbaar is in het plan voor de geselecteerde maand.</p> </li> 
          <li> <p><strong>[!UICONTROL Required]</strong>: De kosten van dit initiatief voor de geselecteerde maand.</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Overallocated]:</strong> Het verschil tussen de kosten van het initiatief en de beschikbare begroting uit het plan. </p> </li> 
         </ul> <p>Tip: Soms wordt [!UICONTROL Available] kosten komen overeen of zijn hoger dan [!UICONTROL Required] de kosten van het initiatief voor de geselecteerde maand en de [!DNL Scenario Planner] er is nog steeds sprake van een overtoerekening van de kosten . Dit betekent dat er hogere initiatieven zijn die al dezelfde maand gebruikmaken van de beschikbare begroting voor het plan. </p> </td> 
       </tr> 
      </tbody> 
     </table>



1. Voer een van de volgende handelingen uit om het deelvenster met details over het initiatief te openen en meer informatie weer te geven over waar de conflicten zich voordoen en om deze op te lossen:

   * Klik op het waarschuwingspictogram naast de naam van het initiatief.
   * Klik op de balk van een initiatief.
   * Klik op de knop **[!UICONTROL More]** pictogram ![](assets/more-icon.png) rechts van de naam van het initiatief klikt u op **[!UICONTROL Edit]**.

      Rechts wordt het deelvenster met initiatiefdetails weergegeven.

      Wanneer u niet genoeg mensen of budget hebt voor uw initiatief, wordt een rood waarschuwingspictogram weergegeven naast de volgende secties:

   * [!UICONTROL Required Job Roles]
   * [!UICONTROL Costs]

1. (Voorwaardelijk) Ga voor initiatieven met een functieconflict naar de **[!UICONTROL Required Job Roles]** om alle functies weer te geven die voor uw initiatief zijn vereist. Identificeer welke baanrollen zouden kunnen worden oververdeeld. Herzie het aantal VTE of uren nodig voor elke baanrol voor elke maand van het initiatief. Het vak met de FTE of het aantal uren voor maanden met overtoewijzingen wordt in een rode omtrek weergegeven.

   ![](assets/details-panel-overallocated-roles-350x275.png)

1. (Optioneel) Klik op de pijl naar rechts naast de maanden in de tijdlijn van het initiatief om te zien welke extra maanden een taakrolconflict veroorzaken.

   ![](assets/right-arrow-initiative-months-inside-details-box-highlighted-350x145.png)

1. (Optioneel) Klik op **[!UICONTROL Show details]** onder de taakrol die een conflict toont om te zien waar de conflicten verschijnen en om de conflicterende maanden in het de grafiekgebied van het plan te benadrukken. Voor elke taakrol wordt aanvullende informatie weergegeven.

   De volgende velden worden weergegeven voor elke taakrol:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Available]</td> 
      <td> <p>Het aantal baanrollen beschikbaar bij het plan voor elke maand. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Previously allocated]</td> 
      <td>Het aantal functies dat al voor een bepaalde maand uit de begroting van het plan is toegewezen aan hoger opgeleide initiatieven. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Overallocated]</td> 
      <td> <p>Het verschil tussen het aantal verplichte functies op initiatief en het aantal dat beschikbaar is in het plan na initiatieven met een hogere rang gebruikte ook een aantal rollen. Workfront berekent het aantal [!UICONTROL Overallocated] taakrollen met behulp van de volgende formule:</p> <p><code>Overallocated roles = (Roles Previously Allocated to higher initiatives + Required roles for current initiative) - Monthly available roles from the plan</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Op de kaart van het plan geven de maanden waarin de functies worden toegewezen de naam en het aantal rollen weer die nodig zijn voor elk initiatief waar ze nodig zijn. U moet de [!UICONTROL Month] weergave om de naam van de taakrollen te zien

   ![](assets/conflicting-job-role-months-on-plan-after-clicking-show-details-350x158.png)

1. Voer een van de volgende handelingen uit om conflicten met taakrollen op te lossen:

   * Pas handmatig het aantal functies voor elke maand van het initiatief aan in een lager aantal.
   * Houd de aanwijzer boven de naam van de taakrol en klik op de knop **[!UICONTROL delete]pictogram** ![](assets/delete.png) het schrappen van de functie van baan uit het initiatief .
   * Selecteren **[!UICONTROL Add roles to the scenario's available resources]** en klik vervolgens op **[!UICONTROL Apply]**.

      Dit voegt het ontbrekende aantal baanrol FTEs of uren aan het scenario toe [!UICONTROL Available] veld.

      >[!NOTE]
      >
      >De rollen u toevoegt om de conflicten op te lossen wijzigen [!UICONTROL Available] de baanrollen voor het geselecteerde scenario en niet voor alle scenario&#39;s in het plan.

      Een naar boven wijzende groene pijl ![](assets/upward-green-arrow.png) vertoningen voor de maand in de chronologie van het plan om erop te wijzen dat meer middelen aan het plan die maand werden toegevoegd. U moet de [!UICONTROL Month] om deze indicator te zien.

   * (Voorwaardelijk) Sluit het detailpanel en geef het initiatief een hogere prioriteit om begrotingsmiddelen uit het plan te ontvangen, indien mogelijk. Zie voor informatie over het bijwerken van de prioriteit van initiatieven [Prioriteiten van initiatieven bijwerken in het scenario Scenario Planner](../scenario-planner/prioritize-initiatives.md).

1. (Optioneel) Klik op **[!UICONTROL Hide details]** als u het vak met aanvullende gegevens wilt sluiten, klikt u op **[!UICONTROL Apply]** om de wijzigingen op te slaan die u aanbrengt in taakrollen.

1. (Voorwaardelijk) Ga voor initiatieven met kostenconflicten naar de **[!UICONTROL Costs]** in het informatieblad over het initiatief om de kosten voor elke maand van de duur van het initiatief te beoordelen . Geef aan welke maanden mogelijk niet genoeg geld in de begroting van het plan hebben om de kosten voor het geselecteerde initiatief te dekken. De doos met de ontoereikende beschikbare begroting toont in een rood overzicht.
1. (Optioneel) Klik op de naar rechts wijzende pijl naast de maanden in de tijdlijn van het initiatief om extra maanden weer te geven die onvoldoende budget hebben om de kosten te dekken.

   ![](assets/details-panel-insufficient-costs-350x239.png)

1. (Optioneel) Klik op **[!UICONTROL Show details]** onder de kostprijs om te zien waar het conflict zich voordoet en om de tegenstrijdige maanden op de kaart van het plan te plaatsen. De volgende extra gebieden tonen voor elk type van kosten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Available]</td> 
      <td> <p>De kosten die in de begroting van het plan voor elke maand beschikbaar zijn. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Previously allocated]</td> 
      <td>Het bedrag dat al uit de begroting van het plan is toegewezen aan hoger opgeleide initiatieven. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Overallocated]</td> 
      <td> <p>Het maandelijkse verschil tussen de kosten die nodig zijn voor het initiatief en het bedrag dat beschikbaar is uit de begroting van het plan na initiatieven met een hogere rang gebruikte ook een deel van de beschikbare begroting. [!DNL Workfront] berekent het aantal overtoegerekende kosten aan de hand van de volgende formule:</p> <p><code>Overallocated costs = (Costs Previously Allocated to higher initiatives + Required costs for the current initiative) - Monthly available budget from the plan</code> </p> <p>[!DNL Workfront] berekent de vereiste kosten voor het huidige initiatief voor elke maand met behulp van de volgende formule:</p> <p><code>Required initiative costs = Initiative Fixed Costs + Initiative People Costs</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Op de kaart van het plan geven de maanden waarin de kosten ontoereikend zijn de naam en het aantal rollen weer die nog nodig zijn voor het initiatief. U moet de Maandweergave selecteren om de kostenbedragen weer te geven.

   ![](assets/conflicting-costs-months-on-plan-after-clicking-show-details-350x139.png)

   >[!NOTE]
   >
   >Als u de optie [!UICONTROL Include people cost] vaststelling van de [!UICONTROL Budget] de doos toen u het plan creeerde, [!UICONTROL People Costs] In geen enkel scenario wordt een regel voor een initiatief weergegeven. In dit geval neemt Workfront geen berekeningen van Personeelskosten om kostenconflicten vast te stellen. Voor informatie over het creëren van een plan, zie [Plannen maken en bewerken in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

1. Voer een van de volgende handelingen uit om kostenconflicten op te lossen:

   * Pas handmatig het aantal [!UICONTROL Fixed Costs] voor elke maand van het initiatief tot een lager aantal.
   * In de **[!UICONTROL Required Job Roles]** , indien mogelijk het aantal functies voor de maand handmatig aanpassen met een budget voor Personeelskosten. Dit vermindert het aantal Personeelskosten.

      >[!TIP]
      >
      >U kunt Personeelskosten niet handmatig aanpassen.

   * Selecteren **[!UICONTROL Add amount to the scenario's budget]** en klik vervolgens op **[!UICONTROL Apply]**.

      Dit voegt toe dat het ontoereikende bedrag van de begroting van het scenario voor de maanden waarin het ontbrak, ook de totale begroting van het scenario bijwerkt.

      >[!NOTE]
      >
      >Het bedrag u toevoegt om de kostenconflicten op te lossen wijzigt de Begroting voor het geselecteerde scenario en niet voor alle scenario&#39;s in het plan.

   * (Voorwaardelijk) Sluit het detailpanel en geef het initiatief een hogere prioriteit om begrotingsmiddelen uit het plan te ontvangen, indien mogelijk. Zie voor informatie over het bijwerken van de prioriteit van initiatieven [Prioriteiten van initiatieven bijwerken in het [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Klikken **[!UICONTROL Apply]** wanneer u wijzigingen aanbrengt in de sectie Kosten.
1. Klikken **[!UICONTROL Save plan]** om uw wijzigingen op te slaan.


