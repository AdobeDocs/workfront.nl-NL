---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Initiatiefstrijdigheden oplossen in de functie Scenario Planner
description: Wanneer initiatieven met elkaar in strijd zijn, concurreren zij om dezelfde middelen. De middelen u voor een scenario beschikbaar hebt zijn niet genoeg om alle middelen te behandelen die door alle initiatieven in het scenario worden vereist.
author: Alina
feature: Workfront Scenario Planner
exl-id: d3a3e177-bece-4e03-89d7-9cee6127bc55
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '2119'
ht-degree: 0%

---

# Initiatiefconflicten oplossen in de [!DNL Scenario Planner]

Wanneer initiatieven met elkaar in strijd zijn, concurreren zij om dezelfde middelen. De middelen u voor een scenario beschikbaar hebt zijn niet genoeg om alle middelen te behandelen die door alle initiatieven in het scenario worden vereist.

Dit kan in elk van de volgende gevallen gebeuren:

* Het aantal functies dat voor het initiatief vereist is, is groter dan het aantal rollen dat voor het plan in de begroting is opgenomen.
* De kosten van het initiatief zijn hoger dan het voor het plan beschikbare budget.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>Nieuw: Ultimate </p></li>
   <p>De Scenario Planner is niet beschikbaar voor de nieuwe Workfront Select- of Workfront Prime-plannen. </p>
   <li><p>Huidig: [!UICONTROL Business] of hoger</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licentie*</p> </td> 
   <td> <p>Nieuw: Licht of hoger</p> 
   <p>Huidig: [!UICONTROL Review] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>Voor de nieuwe plannen van Workfront:</p><p> Adobe Workfront</li></p>
   <li><p>Voor de huidige plannen van Workfront: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>

<p>Voor meer informatie, zie <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref"> Toegang nodig om [!DNL Scenario Planner]</a> te gebruiken. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Toegangsniveau </td> 
   <td> <p>[!UICONTROL Edit] toegang tot de [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objectmachtigingen </p> </td> 
   <td> <p>[!UICONTROL Manage] machtigingen voor een abonnement</p> <p>Voor informatie bij het vragen van om extra toegang tot een plan, zie <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref"> de toegang van het Verzoek tot een plan in [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang tot de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overzicht van conflicten oplossen

* Een conflict wordt ook begrepen als een overmatige toewijzing van de functies of de begroting van een scenario.
* Wanneer [!DNL Workfront] een conflict ontdekt, verschijnt de bar die aan de conflicterende maand tijdens de duur van het initiatief beantwoordt in rood. Dit kan in elk van de volgende gevallen gebeuren:

   * Het aantal functies dat maandelijks voor een initiatief vereist is, is groter dan het aantal rollen dat voor het plan in de begroting is opgenomen nadat alle vorige initiatieven de voor het plan begrote middelen hebben gebruikt.
   * De maandelijkse kosten van het initiatief zijn groter dan de begroting die voor het plan beschikbaar is, nadat alle eerdere initiatieven de begroting van het plan hebben gebruikt om hun kosten te dekken.

>[!TIP]
>
>Standaard gaat [!DNL Scenario Planner] ervan uit dat u voor een scenario een budget van 0 taakrollen en $0 of het equivalent van $0 in de systeemvaluta hebt opgenomen, tenzij u anders hebt opgegeven. Het aantal functies geeft het aantal FTE&#39;s (voltijdequivalenten) of uren aan dat in de begroting is opgenomen voor de functie.
>
>Voor alle berekeningen in de Planner van het Scenario, gebruikt Workfront de volgende waarde: 1 FTE = 8 Uren.
>
>Voor informatie over het bijwerken van de beschikbare rollen voor een plan en een begroting zie [ plannen in  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) creëren en uitgeven.

* U kunt een conflict oplossen door één van het volgende te doen:

   * De ontbrekende vereiste middelen automatisch toevoegen uit de initiatieven op het scenario. In dit artikel wordt beschreven hoe conflicten met deze optie kunnen worden opgelost.
   * Het aanpassen van de functie en de begrotingsmiddelen voor het scenario, door het plan uit te geven. Voor meer informatie, zie [ plannen in  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) creëren en uitgeven.

## Conflicten tussen initiatieven oplossen

1. Ga naar een plan waarvoor u conflicten wilt oplossen.

   Voor informatie over het creëren van plannen, zie [ plannen in  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) creëren en uitgeven.

   Voor informatie over het creëren van initiatieven, zie [ initiatieven in  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md) creëren en uitgeven.

1. (Optioneel) Selecteer in de vervolgkeuzelijst **[!DNL Initial scenario]** het scenario dat u wilt bekijken.

   >[!TIP]
   >
   >Een plan kan verscheidene scenario&#39;s hebben. Wanneer u de conflicten in het plan bekijkt, verwijst [!DNL Workfront] naar de bronnen die momenteel beschikbaar zijn voor het geselecteerde scenario en naar de bronnen die vereist zijn voor de initiatieven van dat scenario. Voor informatie over scenario&#39;s, zie [ planscenario&#39;s in  [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md) creëren en vergelijken.

1. Zorg ervoor dat **[!UICONTROL Show conflicts]** is ingeschakeld. Deze optie is standaard ingeschakeld.

   ![ toon scenario&#39;s knevel ](assets/show-scenarios-toggle-on.png)

   Het eerste conflicterende initiatief geeft de maanden weer met rode conflicten en er verschijnt een waarschuwingspictogram naast de naam van het initiatief.

   De achtergrond van alle initiatieven die beginnen met het eerste conflicterende wordt in het rood weergegeven op het schema van het plan.

   Wanneer een initiatief een conflict vertoont, betekent dit dat het aantal functies voor minstens één specifieke rol, de gemaakte kosten of beide het aantal functies of het budget dat voor het plan voor een bepaalde maand is vastgesteld, overschrijden.

   ![ Initiatieven op plan met conflict ](assets/initiatives-on-plan-with-conflicts-350x126.png)

1. Voer een van de volgende handelingen uit om meer te weten te komen over de conflicten die er kunnen zijn:

   * Houd de muisaanwijzer boven het waarschuwingspictogram naast de naam van het initiatief om te begrijpen of u een functie- of begrotingsconflict hebt.

     ![ conflict van de de baanrol van de Begroting ](assets/budget-job-role-conflict-tooltip-on-warning-icon-350x109.png)

     Afhankelijk van of u taakrollen te veel hebt toegewezen of te hoge kosten voor uw initiatief, ziet u mogelijk een van de volgende opties wanneer u de muisaanwijzer op het waarschuwingspictogram plaatst:

      * Conflictdetails voor taakrol tonen
      * Details begrotingsconflict tonen
      * Functie- en begrotingsgegevens weergeven

   * Wanneer het bekijken van het plan door maand, houd over een maand in de chronologie van het plan om de vereiste middelen voor die maand te bekijken en of de conflicten voor de maand mensen of op kosten-betrekking hebben zijn.

     ![ Details van conflicten op maandelijkse chronologie ](assets/details-of-conflicts-on-monthly-plan-timeline-pop-up-350x178.png)

     Controleer de volgende maandelijkse informatie op het niveau van de regeling:

      * Het aantal beschikbare, vereiste en overtoegewezen functies voor de maand voor alle initiatieven die voor die maand zijn gepland
      * De beschikbare, vereiste en overtoegewezen kosten voor de maand voor alle voor die maand geplande initiatieven

        >[!TIP]
        >
        >De [!UICONTROL Available] -kosten zijn de begroting van het scenario voor die maand.

   * Houd de muisaanwijzer gedurende een maand boven de rode balk van een initiatief om het extra informatievak weer te geven over het conflict dat die maand plaatsvindt.

     ![ Details van conflicten op initiatiefchronologie ](assets/details-of-conflicts-on-initiative-timeline-pop-up-350x113.png)

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
          <li> <p><strong>[!UICONTROL Required]</strong>: Het aantal functies dat voor het initiatief is vereist voor de geselecteerde maand.</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Overallocated]:</strong> Het verschil tussen het aantal dat op het initiatief wordt vereist en het aantal beschikbaar van het scenario. </p> </li> 
         </ul> <p>Tip: soms komt het aantal [!UICONTROL Available] rollen overeen met of is het hoger dan het aantal [!UICONTROL Required] rollen, maar in [!DNL Scenario Planner] wordt nog steeds een overtoewijzing weergegeven. Dit betekent dat er hogere-rangschikkingsinitiatieven zijn die reeds de baanrollen gebruikten die in het plan voor dezelfde maand beschikbaar waren. </p> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Kosten</td> 
        <td> <p>De kosten van het initiatief voor de geselecteerde maand. De volgende kolommen bevatten informatie over de benodigde kosten en het beschikbare budget voor de geselecteerde maand:</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Available]</strong>: De begroting die beschikbaar is in het plan voor de geselecteerde maand.</p> </li> 
          <li> <p><strong>[!UICONTROL Required]</strong>: De kosten van dit initiatief voor de geselecteerde maand.</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Overallocated]:</strong> Het verschil tussen de kosten van het initiatief en de begroting beschikbaar uit het plan. </p> </li> 
         </ul> <p>Tip: soms komen de [!UICONTROL Available] -kosten overeen met of zijn deze hoger dan de [!UICONTROL Required] -kosten van het initiatief voor de geselecteerde maand en toont de [!DNL Scenario Planner] nog steeds een te hoge kostenallocatie. Dit betekent dat er hogere initiatieven zijn die al dezelfde maand gebruikmaken van de beschikbare begroting voor het plan. </p> </td> 
       </tr> 
      </tbody> 
     </table>

1. Voer een van de volgende handelingen uit om het deelvenster met details over het initiatief te openen en meer informatie weer te geven over waar de conflicten zich voordoen en om deze op te lossen:

   * Klik op het waarschuwingspictogram naast de naam van het initiatief.
   * Klik op de balk van een initiatief.
   * Klik het **[!UICONTROL More]** pictogram ![ Meer pictogram ](assets/more-icon.png) aan het recht van de naam van het initiatief, dan klik **[!UICONTROL Edit]**.

     Rechts wordt het deelvenster met initiatiefdetails weergegeven.

     Wanneer u niet genoeg mensen of budget hebt voor uw initiatief, wordt een rood waarschuwingspictogram weergegeven naast de volgende secties:

   * [!UICONTROL Required Job Roles]
   * [!UICONTROL Costs]

1. (Voorwaardelijk) Ga voor initiatieven met een functieconflict naar de sectie **[!UICONTROL Required Job Roles]** om alle taakrollen weer te geven die voor uw initiatief zijn vereist. Identificeer welke baanrollen zouden kunnen worden oververdeeld. Herzie het aantal VTE of uren nodig voor elke baanrol voor elke maand van het initiatief. Het vak met de FTE of het aantal uren voor maanden met overtoewijzingen wordt in een rode omtrek weergegeven.

   ![ OverToegewezen rollen ](assets/details-panel-overallocated-roles-350x275.png)

1. (Optioneel) Klik op de pijl naar rechts naast de maanden in de tijdlijn van het initiatief om te zien welke extra maanden een taakrolconflict veroorzaken.

   ![ Juiste schuif binnen detailsdoos ](assets/right-arrow-initiative-months-inside-details-box-highlighted-350x145.png)

1. (Optioneel) Klik op **[!UICONTROL Show details]** onder de taakrol die een conflict weergeeft om te zien waar de conflicten verschijnen en om de conflicterende maanden in het grafiekgebied van het abonnement te markeren. Voor elke taakrol wordt aanvullende informatie weergegeven.

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
      <td> <p>Het verschil tussen het aantal verplichte functies op initiatief en het aantal dat beschikbaar is in het plan na initiatieven met een hogere rang gebruikte ook een aantal rollen. Workfront berekent het aantal [!UICONTROL Overallocated] taakrollen met de volgende formule:</p> <p><code>Overallocated roles = (Roles Previously Allocated to higher initiatives + Required roles for current initiative) - Monthly available roles from the plan</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Op de kaart van het plan geven de maanden waarin de functies worden toegewezen de naam en het aantal rollen weer die nodig zijn voor elk initiatief waar ze nodig zijn. U moet de weergave [!UICONTROL Month] selecteren om de naam van de taakrollen weer te geven

   ![ Conflicterend baanrollen ](assets/conflicting-job-role-months-on-plan-after-clicking-show-details-350x158.png)

1. Voer een van de volgende handelingen uit om conflicten met taakrollen op te lossen:

   * Pas handmatig het aantal functies voor elke maand van het initiatief aan in een lager aantal.
   * Beweeg over de naam van de baanrol en klik het **[!UICONTROL delete]pictogram** ![ pictogram van de Schrapping ](assets/delete.png) om de baanrol uit het initiatief te verwijderen.
   * Selecteer **[!UICONTROL Add roles to the scenario's available resources]** en klik op **[!UICONTROL Apply]** .

     Hiermee voegt u het ontbrekende aantal taakrol-FTE&#39;s of -uren toe aan het veld [!UICONTROL Available] van het scenario.

     >[!NOTE]
     >
     >De rollen u toevoegt om de conflicten op te lossen wijzigen de [!UICONTROL Available] baanrollen voor het geselecteerde scenario en niet voor alle scenario&#39;s in het plan.

     Een naar boven gericht groene pijl ![ naar boven wijzende groene pijl ](assets/upward-green-arrow.png) vertoningen voor de maand in de chronologie van het plan om erop te wijzen dat meer middelen aan het plan die maand werden toegevoegd. U moet de weergave [!UICONTROL Month] selecteren om deze indicator te zien.

   * (Voorwaardelijk) Sluit het detailpanel en geef het initiatief een hogere prioriteit om begrotingsmiddelen uit het plan te ontvangen, indien mogelijk. Voor informatie over het bijwerken van initiatiefprioriteit, zie [ de initiatiefprioriteiten van de Update in de Planner van het Scenario ](../scenario-planner/prioritize-initiatives.md).

1. (Optioneel) Klik op **[!UICONTROL Hide details]** om het vak Extra details te sluiten en klik vervolgens op **[!UICONTROL Apply]** om de wijzigingen in de taakrollen op te slaan.

1. (Voorwaardelijk) Voor initiatieven met kostenconflicten gaat u naar de sectie **[!UICONTROL Costs]** in het deelvenster met initiatiefdetails om de kosten voor elke maand van de duur van het initiatief te controleren. Geef aan welke maanden mogelijk niet genoeg geld in de begroting van het plan hebben om de kosten voor het geselecteerde initiatief te dekken. De doos met de ontoereikende beschikbare begroting toont in een rood overzicht.
1. (Optioneel) Klik op de naar rechts wijzende pijl naast de maanden in de tijdlijn van het initiatief om extra maanden weer te geven die onvoldoende budget hebben om de kosten te dekken.

   ![ Pijl voor ontoereikende kosten ](assets/details-panel-insufficient-costs-350x239.png)

1. (Optioneel) Klik op **[!UICONTROL Show details]** onder de kosteninformatie om te zien waar het conflict voorkomt en om de conflicterende maanden op het overzicht van het abonnement te benadrukken. De volgende extra gebieden tonen voor elk type van kosten:

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
      <td> <p>Het maandelijkse verschil tussen de kosten die nodig zijn voor het initiatief en het bedrag dat beschikbaar is uit de begroting van het plan na initiatieven met een hogere rang gebruikte ook een deel van de beschikbare begroting. [!DNL Workfront] berekent het aantal overtoegerekende kosten met behulp van de volgende formule:</p> <p><code>Overallocated costs = (Costs Previously Allocated to higher initiatives + Required costs for the current initiative) - Monthly available budget from the plan</code> </p> <p>[!DNL Workfront] berekent de vereiste kosten voor het huidige initiatief voor elke maand met behulp van de volgende formule:</p> <p><code>Required initiative costs = Initiative Fixed Costs + Initiative People Costs</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Op de kaart van het plan geven de maanden waarin de kosten ontoereikend zijn de naam en het aantal rollen weer die nog nodig zijn voor het initiatief. U moet de Maandweergave selecteren om de kostenbedragen weer te geven.

   ![ Conflicterende kosten ](assets/conflicting-costs-months-on-plan-after-clicking-show-details-350x139.png)

   >[!NOTE]
   >
   >Als u de instelling [!UICONTROL Include people cost] voor het vak [!UICONTROL Budget] van het abonnement hebt uitgeschakeld toen u het abonnement maakte, wordt de regel [!UICONTROL People Costs] in geen enkel scenario weergegeven voor initiatieven. In dit geval neemt Workfront geen berekeningen van Personeelskosten om kostenconflicten te bepalen. Voor informatie over het creëren van een plan, zie [ plannen in  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) creëren en uitgeven.

1. Voer een van de volgende handelingen uit om kostenconflicten op te lossen:

   * Stel handmatig het aantal [!UICONTROL Fixed Costs] voor elke maand van het initiatief in op een lager aantal.
   * Pas in de sectie **[!UICONTROL Required Job Roles]** indien mogelijk handmatig het aantal functies voor de maand aan met een budget voor personeelskosten. Dit vermindert het aantal Personeelskosten.

     >[!TIP]
     >
     >U kunt Personeelskosten niet handmatig aanpassen.

   * Selecteer **[!UICONTROL Add amount to the scenario's budget]** en klik op **[!UICONTROL Apply]** .

     Dit voegt toe dat het ontoereikende bedrag van de begroting van het scenario voor de maanden waarin het ontbrak, ook de totale begroting van het scenario bijwerkt.

     >[!NOTE]
     >
     >Het bedrag u toevoegt om de kostenconflicten op te lossen wijzigt de Begroting voor het geselecteerde scenario en niet voor alle scenario&#39;s in het plan.

   * (Voorwaardelijk) Sluit het detailpanel en geef het initiatief een hogere prioriteit om begrotingsmiddelen uit het plan te ontvangen, indien mogelijk. Voor informatie over het bijwerken van initiatiefprioriteit, zie [ de initiatiefprioriteiten van de Update in  [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Klik op **[!UICONTROL Apply]** wanneer u wijzigingen aanbrengt in de sectie Kosten.
1. Klik op **[!UICONTROL Save plan]** om de wijzigingen op te slaan.


