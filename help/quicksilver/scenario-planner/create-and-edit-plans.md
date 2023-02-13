---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Abonnementen maken en bewerken in Scenario Planner
description: U kunt plannen als deel van het gebruiken van de Planner van het Scenario van Workfront tot stand brengen, wanneer het prioriteren van de strategie op hoog niveau van uw bedrijf. Voor meer informatie over plannen, zie het overzicht van Abonnementen in de Planner van het Scenario.
author: Alina
feature: Workfront Scenario Planner
exl-id: 15c0e519-0164-449d-84f3-470d0d4eb795
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '2244'
ht-degree: 0%

---

# Plannen maken en bewerken in het dialoogvenster [!DNL Scenario Planner]

U kunt plannen maken als onderdeel van het gebruik van de [!DNL Workfront Scenario Planner], bij het bepalen van de prioriteiten voor de strategie op hoger niveau van uw bedrijf. Voor meer informatie over plannen, zie [Overzicht van plannen in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: talk about:</p>
<p>- Show people conflicts >> this impacts the conflicts calculation for initiatives>> link to the conflicts article</p>
<p>- explain what hovering over the green upward-pointing arrow does, with screen shot)</p>
</div>
-->

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td>[!UICONTROL Business] of hoger</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licentie*</p> </td> 
   <td> <p>[!UICONTROL Review] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td>Product</td> 
   <td> <p>U moet een extra licentie aanschaffen voor de [!DNL Adobe Workfront Scenario Planner] voor toegang tot de functionaliteit die in dit artikel wordt beschreven.</p> <p>Voor informatie over het verkrijgen van de [!UICONTROL Workfront Scenario Planner], zie <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Toegang nodig om de [!UICONTROL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configuraties op toegangsniveau* </td> 
   <td> <p>[!UICONTROL Edit] toegang tot [!DNL Scenario Planner]</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau veranderen, zie <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objectmachtigingen </p> </td> 
   <td> <p>[!DNL Manage] machtigingen voor een abonnement</p> <p>Voor informatie over het vragen van om extra toegang tot een plan, zie <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Toegang aanvragen tot een abonnement in de [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Abonnementen maken of bewerken

U kunt een geheel nieuw plan maken of een bestaand plan bewerken dat met u is gedeeld.

>[!NOTE]
>
>Nadat u een plan creeert, wordt u beschouwd als de planmaker en de eigenaar. Wanneer een gebruiker wordt gedeactiveerd, heeft het plan geen eigenaar en is niet zichtbaar aan iedereen tenzij eerder gedeeld met een verbinding.

In dit artikel wordt beschreven hoe u een geheel nieuw plan kunt maken of hoe u een bestaand plan kunt bewerken.

Voor alle overwegingen over plannen, met inbegrip van de informatie beschikbaar voor een plan, zie [Overzicht van plannen in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

Voor informatie over het schrappen van plannen, zie [Plannen verwijderen in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

Een abonnement maken of bewerken:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png)en klik vervolgens op [!UICONTROL Scenarios].

   Een lijst met bestaande plannen die u hebt gemaakt, wordt weergegeven in het dialoogvenster [!DNL Workfront Scenario Planner].

1. (Optioneel) Klik op de knop **[!UICONTROL Filter]** pictogram ![](assets/filter-icon-34x37.png)in de rechterbovenhoek van de overzichtslijst en selecteer een van de volgende opties:

   | Filter | Beschrijving |
   |---|---|
   | [!UICONTROL All] | Toont alle plannen die u creeerde of die met u zijn gedeeld. |
   | [!UICONTROL My plans] | Geeft de plannen weer die u hebt gemaakt. |
   | [!UICONTROL Shared with me] | Hiermee geeft u plannen weer die met u worden gedeeld. |

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Optioneel) Klik op de knop **[!UICONTROL Search]** pictogram ![](assets/search-icon.png) om een sleutelwoord te typen en van een plan snel de plaats te bepalen in de lijst.

1. Klik op de naam van een bestaand abonnement om het te bewerken en door te gaan met stap 7.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate) </p>
   -->

   of

   Klikken **[!UICONTROL New Plan]** in de linkerbovenhoek om een plan te creëren en met stap 5 verder te gaan.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate)</p>
   -->

   ![](assets/new-plan-button.png)

   De [!UICONTROL New Plan] wordt weergegeven.

   ![](assets/new-plan-ui-adding-a-new-plan-350x306.png)

1. (Voorwaardelijk) Wanneer u een nieuw plan creeert, specificeer de volgende informatie:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Typ een naam voor het abonnement. Dit is een verplicht veld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p>Belangrijk: <span style="font-weight: normal;">U kunt de volgende selecties niet wijzigen nadat u het abonnement hebt gemaakt en opgeslagen.</span> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>FTE ([!UICONTROL Full Time Equivalent]) of [!UICONTROL Hours]</span> </td> 
      <td> <p><span>Selecteer een van de volgende opties om aan te geven hoe u de informatie over de rol van de taak voor dit abonnement wilt schatten:</span> </p> 
       <ul> 
        <li> <p><span><strong>FTE</strong>. Dit is de standaardinstelling </span> </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: snippet below: this is per Ani; it does NOT look at the system FTE.) </p>
         --> <p>Voor alle berekeningen in de [!DNL Scenario Planner], [!DNL Workfront] gebruikt de volgende waarde: 1 FTE = 8 uur. </p> </li> 
        <li> <p><strong>[!UICONTROL Hours]</strong> </p> </li> 
       </ul> <p>Belangrijk: <span>De optie u hier selecteert bepaalt hoe de informatie van de baanrol voor het plan, de scenario's van het plan, en initiatieven toont.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Start date]</td> 
      <td> <p>Selecteer de maand en het jaar waarin het abonnement moet worden gestart. U kunt slechts maanden selecteren in dit veld. [!DNL Workfront] gaat ervan uit dat de begindatum van het plan de eerste dag van de geselecteerde maand is en de einddatum de laatste dag van het einde van de maand in zijn duur is. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Duration]</td> 
      <td> <p>Selecteer een van de volgende tijdsduur in het keuzemenu:</p> 
       <ul> 
        <li>1 jaar. Dit is de standaardduur. </li> 
        <li>3 jaar</li> 
        <li> <p>5 jaar</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Voorwaardelijk) Klik **[!UICONTROL Next]**.

   De tijdlijn van het plan wordt weergegeven als de **[!UICONTROL Initial scenario]**.

   Voor informatie over het creëren van extra scenario&#39;s, zie [Plan-scenario&#39;s maken en vergelijken in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Optioneel) Selecteer in het keuzemenu Tijdlijn een van de opties in de volgende tabel om de manier te wijzigen waarop u de tijdlijn van het plan weergeeft.

   ![](assets/month-dropdown-with-all-options.png)

   | Vervolgkeuzemenu, optie | Beschrijving |
   |---|---|
   | [!UICONTROL Month] | Geeft de tijdlijn per maand weer. Dit is de standaardinstelling en de enige optie voor een jaarabonnement. |
   | [!UICONTROL Quarter] | Geeft de tijdlijn per kwartaal weer. Deze optie is alleen beschikbaar als de optie [!UICONTROL Duration] van het plan 3 of 5 jaar bedraagt. Dit is de standaardoptie voor een driejarenplan. |
   | [!UICONTROL Year] | Geeft de tijdlijn per jaar weer. Deze optie is alleen beschikbaar als de optie [!UICONTROL Duration] van het plan is 5 jaar . Dit is de standaardoptie voor een vijfjarenplan. |

1. (Optioneel) Schuif van links naar rechts om de volledige duur van het abonnement weer te geven.
1. (Optioneel) Klik op de knop **[!UICONTROL Today]** indicatorlijn om naar de huidige dag terug te keren.

   ![](assets/today-indicator-350x160.png)

1. Klik op de knop **[!UICONTROL Job Roles]** doos in de kopbal van het plan om baanrollen toe te voegen die beschikbaar zullen zijn om het plan uit te voeren.

   De details van de [!UICONTROL Job Roles] weergegeven.

   >[!TIP]
   >
   >De roltoewijzingseenheid (VTE of uren) die [!DNL Workfront] het gebruik voor dit plan toont tussen haakjes in de titel van de doos.

   ![](assets/adding-people-to-plan-350x206.png)

1. Klik op de knop **[!UICONTROL Start typing job role]** en selecteer een rol in de lijst of typ de naam van een actieve taakrol.

   Alle actieve baanrollen in het systeem zijn vermeld wanneer u dit gebied klikt.

   Hiermee voegt u de taakrol toe aan de kolom Taakrollen.

1. Werk de volgende informatie voor de taakrol bij of bekijk deze:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max available] (voor FTE) </p> <p role="rowheader">of </p> <p role="rowheader"><span>[!UICONTROL Total available] (voor uren)</span> </p> </td> 
      <td> <p><span>Afhankelijk van of u om uren of FTE voor uw plan selecteerde te gebruiken, type</span> het aantal functies voor VTE's <span>of uren</span> die beschikbaar zijn om de werkzaamheden aan het plan op de volgende gebieden uit te voeren: </p> 
       <ul> 
        <li> <p style="font-weight: normal;"><strong>[!UICONTROL Total available]</strong> (voor uren): Vermeld het totale aantal uren voor alle maanden gedurende de duur van het scenario. Standaard, [!DNL Workfront] verdeelt het Totaal beschikbare aantal gelijkelijk over alle maanden in de duur van het scenario. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span>Als u 1200 uur voor een Designer invoert, betekent dit dat de Designer gedurende elke maand tijdens de duur van het abonnement 100 uur beschikbaar is, wanneer het abonnement [!UICONTROL Duration] is 1 jaar. </p> </li> 
        <li> <p><b>[!UICONTROL Max available]</b> (voor FTE): Vermeld het aantal VTE's dat de functie beschikbaar is voor elke maand tijdens de duur van het plan. Standaard, <strong>Workfront</strong> wijst de [!UICONTROL Max available] aantal aan elke maand in de duur van het scenario.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span>Als u 1 VTE voor een Consultant ingaat, betekent dit dat de Consultant beschikbaar is voor 1 VTE voor elke maand tijdens de duur van het abonnement. </p> <p>U kunt een getal invoeren dat lager is dan 1 FTE. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span>Een 0,5 consultant zou betekenen dat een consultant de helft van zijn VTE (doorgaans 4 uur, waarbij 8 uur 1 VTE is) zou wijden aan het werken aan dit plan. Voor alle berekeningen in de Planner van het Scenario, gebruikt Workfront de volgende waarde: 1 FTE = 8 uur. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max required] (voor FTE)</p> <p role="rowheader">of </p> <p role="rowheader"><span>[!UICONTROL Total required] (voor uren)</span> </p> </td> 
      <td> <p><span>Afhankelijk van of u hebt geselecteerd om uren of FTE voor uw plan te gebruiken, herzie</span> het aantal functies voor VTE's <span>of uren</span> die nodig zijn om de initiatieven in het scenario te voltooien. Bekijk de volgende velden:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Total required]</strong> (voor uren): Het totale aantal uren dat gedurende alle maanden tijdens de looptijd van het plan is vereist.</p> </li> 
        <li> <p><strong>[!UICONTROL Max required]</strong> (voor FTE): Het maximumaantal VTE's dat gedurende een van de maanden tijdens de looptijd van het plan vereist is. </p> </li> 
       </ul> <p>Tip: De <span>maximum</span> aantal FTE's <span>of het totale aantal uren</span> vereist voor die taakrolvertoningen nadat u initiatieven begint toe te voegen. Voor informatie over het toevoegen van initiatieven aan een plan, zie <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">Initiatieven maken en bewerken in het dialoogvenster [!DNL Scenario Planner]</a>.</p> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">[!UICONTROL Avg utilization]</td> 
       <td> <p>(NOTE: this field was removed in 21.2 - May 2021) </p> <p>[!DNL Workfront] calculates the average utilization for each job role using the job role FTEs associated with initiatives (required) and the job role FTEs associated with the plan (available). </p> <p> [!DNL Workfront] calculates the job role utilization percentage for a plan using the following formula: </p> <p><code>Job role utilization percentage = Sum [(Required job roles for each month of the plan *100)/ (Available job roles for each month of the plan)] / Number of months in the Duration of the plan</code> </p> 
        <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Example: </b></span></span> 
         <p>For example, if you have a plan with a duration of 12 months and an initiative with the duration of 2 months, where you use 1 Designer for your initiative (required job role) and there are 2 Designers available on the plan (available), the Utilization percentage for the Designer job role is calculated as follows:</p> 
         <p><code>Designer utilization percentage = [(1/2 + 1/2) * 100] / 12 = 100 / 12 = 8.3%</code> </p> 
        </div> <p>As you add job roles to the plan and indicate the Available amount for each one, the [!UICONTROL Utilization] value for each role also updates and [!DNL Workfront] calculates a utilization percentage for the plan. For information about how [!DNL Workfront] calculates the Job Role Utilization for a plan, see <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Plans overview in the [!DNL Scenario Planner]</a>. </p> <p>Tip: The Utilization percentage is rounded and has one decimal. </p> </td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">[!UICONTROL Hourly rate]</td> 
      <td> <p>Dit is het [!UICONTROL Cost Hour] percentage voor de functie. De uurkoers wordt weergegeven in de valuta van uw systeem. Voor informatie over de Tarieven van de opstellingsUitwisseling voor uw systeem, zie <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Wisselkoersen instellen</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Houd de aanwijzer boven de naam van een taakrol of klik op de tab nadat u de rolinformatie hebt bijgewerkt. Klik vervolgens op de knop **[!UICONTROL trash can icon]** ![](assets/delete.png) om het uit het plan te verwijderen.
1. Klik op **[!UICONTROL Job role distribution]**.

   Het deelvenster voor taakverdeling wordt gedurende alle maanden in de duur van het scenario weergegeven.

   ![](assets/job-role-monthly-distribution-box-fte-350x144.png)

1. Typ de naam van een taakrol om deze toe te voegen aan het abonnement in het dialoogvenster **[!UICONTROL Start typing job role field]** en klikt u op Enter wanneer het wordt weergegeven in de lijst. Hiermee voegt u de rol van de taak toe aan de [!UICONTROL Job Roles] kolom.
1. Werk of herzie de volgende informatie voor elke maand van het scenario bij:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Job Roles] (VTE of uren)</td> 
      <td>Zowel de baanrol beschikbaar voor het scenario als die vereist voor de initiatieven op het scenario tonen in het paneel van de taakverdeling. Er is een aanwijzing of de ramingen van de baanrol in FTEs of uren in de kolomkopbal zijn. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Available] (max &lt;number of="" ftes=""&gt;) </p> 
       <div> 
        <p>of</p> 
        <p>[!UICONTROL Available] (totaal &lt;number of="" hours=""&gt;) </p> 
       </div> </td> 
      <td> <p><span>Afhankelijk van of u hebt geselecteerd om uren of FTE voor uw plan te gebruiken, herzie of werk bij</span> het maandelijks aantal vacatures <span>of uren</span> beschikbaar voor het scenario in de volgende gebieden:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Available] (max &lt;number of="" ftes=""&gt;)</strong>: Het aantal tussen haakjes toont het maximumaantal rollen beschikbaar voor om het even welk van de maanden voor het scenario. Controleer of werk het aantal VTE's voor elke maand van het scenario bij. Als u de maandelijkse toewijzing wijzigt, kan het aantal VTE's tussen de haakjes worden bijgewerkt. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Available] (totaal &lt;number of="" hours=""&gt;)</strong>: Het aantal tussen haakjes toont het totale aantal uren beschikbaar voor alle maanden in het scenario. Controleer of werk het aantal uren voor elke maand van het scenario bij. Als u de maandelijkse toewijzing wijzigt, wordt het aantal uren tussen de haakjes bijgewerkt.</span> </p> </li> 
       </ul> <p>Het handmatig bijwerken van de maandelijkse taakrollentoewijzingen is een andere manier om taakrolconflicten tussen initiatieven op het scenario op te lossen. </p> <p>Tip:   <p><span>Om de maandelijkse rolbeschikbaarheid voor verscheidene maanden bij te werken, typ het aantal uren of FTEs in [!UICONTROL Available] in het veld van een willekeurige maand en sleep vervolgens de hoek van het veld over de aangrenzende maanden om dezelfde waarde voor elke maand te kopiëren. Laat het vallen om alle maanden bij te werken.</span> </p> <p> <img src="assets/job-role-distribution-draggable-corner-highlighted-350x83.png" style="width: 350;height: 83;"> </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Required] (max &lt;number&gt;)</p> 
       <div> 
        <p role="rowheader">of</p> 
        <p role="rowheader">[!UICONTROL Required] (totaal &lt;number&gt;)</p> 
       </div> </td> 
      <td> <p><span>Afhankelijk van of u hebt geselecteerd om uren of FTE voor uw plan te gebruiken, herzie</span> het maandelijks aantal vacatures of uren dat voor het scenario is vereist op de volgende gebieden: </p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Required] (max &lt;number of="" ftes=""&gt;)</strong>: Het aantal tussen haakjes toont het maximumaantal rollen die voor om het even welk van de maanden voor het scenario worden vereist. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Required] (totaal &lt;number of="" hours=""&gt;)</strong>: Het getal tussen haakjes geeft het totale aantal uren weer dat voor alle maanden in het scenario is vereist.</span> </p> </li> 
       </ul> <p>Tip: U kunt het vereiste aantal FTE's niet wijzigen <span>of uren</span> voor de functie. Dit aantal bevolkt voor het scenario nadat u initiatieven en hun baanrolvereisten begint toe te voegen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Difference]</td> 
      <td> 
       <div> 
        <p>Het maandelijkse verschil tussen de bedragen van vereiste en beschikbare baanrollen voor het scenario. [!DNL Workfront] berekent het verschil voor elke baanrol voor elke maand gebruikend de volgende formule:</p> 
        <p><code>Monthly role difference = Monthly required roles - Monthly available roles</code> (in VTE's of uren) </p> 
        <p>Tip: Wanneer het verschil een negatief aantal toont, vereist het scenario meer baanrollen dan het plan beschikbaar heeft. Uw middelen zijn oververdeeld. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Utilization] %</td> 
      <td> 
       <div> 
        <p>Het percentage van gebruik toont hoeveel van de beschikbare baanrollen eigenlijk (of vereist) op de initiatieven in het scenario worden gebruikt. </p> 
        <p>[!DNL Workfront] berekent het gebruik per baanrol per maand gebruikend de volgende formule: </p> 
        <p><code>Monthly role utilization % = Monthly required roles / Monthly available roles * 100</code> </p> 
        <p>Het gebruikspercentage wordt mogelijk in de volgende kleuren weergegeven, afhankelijk van de toewijzing van uw bronnen:</p> 
        <ul> 
         <li> <p><b>Groen</b>: De beschikbare en vereiste aantallen taakrollen komen overeen. De middelen zijn volledig toegewezen en het gebruikspercentage is 100%. </p> </li> 
         <li> <p><b>Rood</b>: Er zijn meer vereiste baanrollen dan het plan beschikbaar heeft. De middelen zijn oververdeeld en het gebruikspercentage is hoger dan 100%.</p> </li> 
         <li> <p><b>Blauw</b>: Er zijn meer beschikbare baanrollen dan zij worden vereist. De middelen zijn onderverdeeld en het bestedingspercentage is lager dan 100%. </p> </li> 
        </ul> 
       </div> <p> <img src="assets/utilization-percent-colors-sp-350x61.png" style="width: 350;height: 61;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **[!UICONTROL Apply]** om de maandelijkse taakverdeling te behouden

   of

   Klikken **[!UICONTROL Cancel]** om de de distributielijst van de baanrol te sluiten en aan het scenario terug te keren.

1. Klik op de knop **[!UICONTROL Financial]** in de koptekst van het plan, om de begroting voor dit plan toe te voegen.

   De details van de [!UICONTROL Financial] weergegeven.

   >[!TIP]
   >
   >De valuta die [!DNL Workfront] het gebruik voor dit plan toont tussen haakjes in de titel van de doos.

1. Geef de **[!UICONTROL Yearly budget]**.

   >[!NOTE]
   >
   >Als uw plan meerdere jaren omvat, moet u een begrotingsbedrag voor elk jaar specificeren.

1. Druk op Enter om het jaarlijkse budget op te slaan, en [!UICONTROL Tab] naar het volgende jaar te gaan.

   De jaarlijkse begroting wordt automatisch gelijkelijk verdeeld voor elke maand van het geselecteerde jaar.

1. Klikken **[!UICONTROL Advanced]** de maandelijkse verdeling van de begroting te zien. De jaarlijkse en maandelijkse begrotingen zijn altijd afgerond. Wanneer het begrotingsbedrag wegens decimalen niet gelijkelijk over alle maanden binnen een jaar kan worden verdeeld **[!UICONTROL Remaining]** de indicator wordt weergegeven onder de jaarlijkse begrotingsverdeling.

   ![](assets/adanced-and-remaining-links-on-plan-budget-350x507.png)

1. Pas handmatig de maandelijkse budgetten aan om de overschrijdingen te voorkomen.

   Wanneer het totaal van alle maandelijkse begrotingsbedragen groter is dan de jaarlijkse begroting, **[!UICONTROL Exceeding]** de waarschuwingsindicator wordt weergegeven onder de jaarlijkse begrotingsverdeling. Pas de maandelijkse begrotingsbedragen handmatig aan totdat ze gelijk zijn aan of lager zijn dan het beschikbare budget voor het plan.

   ![](assets/exceeding-budget-warning-on-plan-350x483.png)

1. De opdracht **[!UICONTROL Include people costs]** vaststelling om de kosten in verband met de rol van een baan niet mee te tellen bij de totale kosten van het plan. Vaste kosten tellen altijd mee voor de totale kosten van de regeling. Dit plaatsen wordt toegelaten door gebrek en beïnvloedt alle scenario&#39;s op het plan.
1. Klik ergens buiten de [!UICONTROL Financial] om het te sluiten. De gegevens die u hebt ingevoerd, worden automatisch opgeslagen.

   U kunt nu de initiatieven voor het plan beginnen te creëren, en scenario&#39;s toevoegen.

1. (Aanbevolen) Klik op **[!UICONTROL New initiative]** een nieuw initiatief toe te voegen.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Should this include information on how to create scenarios - see also information about scenarios in Manage Plans?)</p>
   -->

   Raadpleeg het artikel voor informatie over het toevoegen van initiatieven [Initiatieven maken en bewerken in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Optioneel) Maak een kopie van het bestaande scenario om een nieuw scenario van hetzelfde plan te maken. Voor meer informatie over het creëren van en het werken met veelvoudige scenario&#39;s, zie [Plan-scenario&#39;s maken en vergelijken in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).
1. Klik op **[!UICONTROL Save Plan]**.

   Uw abonnement is gemaakt of bijgewerkt.

1. (Optioneel) Klik op de knop **[!UICONTROL Favorites icon]** ![](assets/favorites-icon-small.png) rechts van de plannaam om het plan aan uw lijst van Favorieten toe te voegen.

1. (Optioneel) Kopieer de URL van het abonnement en verstuur het naar een andere gebruiker die het mogelijk moet controleren of bijwerken. Zij moeten ten minste [!UICONTROL View] toegang in hun toegangsniveau om het plan te kunnen bekijken. Zij moeten [!UICONTROL Edit] toegang tot bewerken. Als zij financiële informatie over het plan moeten herzien, zoals begrotingen, kosten, en baanrolrentetarieven informatie, moeten zij ook toegang hebben tot [!UICONTROL Financial Data] in hun toegangsniveau. Voor informatie over de toegang die nodig is voor de [!DNL Scenario Planner], zie [Toegang nodig om de [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).
