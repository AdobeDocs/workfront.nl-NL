---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Systeembrede projectvoorkeuren configureren
description: Als  [!DNL Adobe Workfront]  beheerder, kunt u de standaardvoorkeur voor alle projecten vormen die door het systeem worden gecreeerd. Deze voorkeuren zijn van invloed op het project, de taak en het gedrag van problemen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: 90405d79f605d788331cb7a04ebf354dc4379bf5
workflow-type: tm+mt
source-wordcount: '2249'
ht-degree: 0%

---

# Projectvoorkeuren voor het hele systeem configureren

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


Als [!DNL Adobe Workfront] beheerder, kunt u de standaardvoorkeur voor alle projecten vormen die door het systeem worden gecreeerd. Deze voorkeuren zijn van invloed op het project, de taak en het gedrag van problemen.

>[!NOTE]
>
>Deze voorkeuren zijn standaard vergrendeld en groepsbeheerders kunnen deze op groepsniveau niet wijzigen, tenzij u ze voor alle groepen in het systeem ontgrendelt. Voor meer informatie, zie [ het Slot of ontgrendelt projectvoorkeur voor alle groepen in het systeem ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] plan</p></td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td><p>Nieuw: [!UICONTROL Standard]</p>
   of
   <p>Huidige: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Projectvoorkeuren configureren voor de gehele organisatie

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **[!UICONTROL Project Preferences]** > **[!UICONTROL Projects]** .

1. Op de **pagina van de Voorkeur van het Project**, ga met één van de 4 hieronder vermelde secties verder om voorkeur voor [!UICONTROL Project Status], [!UICONTROL Timelines], [!UICONTROL Business Cases], en [!UICONTROL Life after Death] te vormen.
1. Als u wilt dat alle groepen in de hele organisatie dezelfde projectvoorkeuren gebruiken, controleert u of elke voorkeur is vergrendeld ![](assets/lock-toggle-button.png) (dit is de standaardinstelling).

   >[!IMPORTANT]
   >
   >Als een projectvoorkeur is vergrendeld, worden alle wijzigingen die u in die voorkeur aanbrengt, overgeërfd door alle groepen in het systeem. Het is belangrijk om met de gebruikers en de groepen door uw organisatie te communiceren om ervoor te zorgen dat alle behoeften rekenschap worden gegeven in de manier u projectvoorkeur vormt.

   Voor informatie over het ontgrendelen van een voorkeur zodat alle groepen het op hun kunnen vormen en beheren, zie [ Vergrendelen of projectvoorkeur voor alle groepen in het systeem ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md) ontgrendelen.

1. Klik op **[!UICONTROL Save]**.

* [[!UICONTROL Project Status]](#project-status)
* [[!UICONTROL Timelines]](#timelines)
* [[!UICONTROL Business Cases]](#business-cases)
* [[!UICONTROL Life After Death]](#life-after-death)

### Projectstatus {#project-status}

Configureer een of meer van de volgende voorkeuren voor nieuwe projecten in het hele systeem:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Allow users to create projects without using a template]</td> 
   <td>  <p>Deze voorkeur staat gebruikers toe om projecten tot stand te brengen zonder een malplaatje te gebruiken wanneer het creëren van een project van de volgende gebieden: </p>
      <ul>
        <li>
        <p>De optie [!UICONTROL New Project] gebruiken in een lijst met projecten</p>
        </li>
          <li>
          <p>Een uitgave converteren naar een project vanaf de pagina van de uitgave</p>
          </li>
         </ul>
        <p>Deze voorkeur is standaard ingeschakeld. </p> 
        <p><b>OPMERKING</b></p>
        <p> Een groepsbeheerder kan deze voorkeur voor een groep wijzigen. Wanneer een gebruiker tot veelvoudige groepen met verschillende voorkeur behoort, kan de gebruiker een project zonder een malplaatje tot stand brengen als hun Groep van het Huis deze toegelaten voorkeur heeft.</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Set new project's status to]</td> 
   <td> <p>Bepaal de status van nieuwe projecten.</p>  <p><b> NOTA </b>  
     <ul> 
      <li>Als u of een andere [!DNL Workfront] beheerder de hier geselecteerde status verbergt, verandert de standaardstatus in de eerste status in de statuslijst.</li> 
     </ul> 
     <ul> 
      <li> <p>Als een vergrendeld systeem of een vergrendelde groepsstatus is ingesteld als de standaardstatus en later door iemand wordt ontgrendeld, probeert het systeem deze te vervangen door een vergrendelde status van hetzelfde type status.</p> <p>Als het niet kan vinden, zoekt het naar een vereiste status:</p> 
       <ul> 
        <li>Als er een vereiste status is die gelijk is aan de niet-vergrendelde standaardstatus, wordt de vereiste status de standaardstatus, zelfs als de status ontgrendeld is.</li> 
        <li>Als geen van de vereiste statussen overeenkomt met de niet-vergrendelde standaardstatus, wordt de eerste vereiste status in de statuslijst de standaardstatus.</li> 
       </ul> <p>Voor informatie over vereiste statussen, zie de artikelen <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override=""> Toegang tot de lijst van de statussen van het systeemproject </a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override=""> toegang tot de lijst van de statussen van de systeemtaak </a>, en <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override=""> heb toegang tot de lijst van de statussen van de systeemkwestie </a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calculate Percent Complete based on]</td> 
   <td> <p>Workfront berekent het percentage voltooide van een project of oudertaak gebruikend het percentage voltooide van elke taak in het project en of de Duur of de Geplande Uren van elke taak.</p><p>Het percentage voltooide van elke taak wordt manueel geplaatst door taaktoewijzing.</p><p>U kunt hier selecteren of Workfront de Duur of de Geplande Uren van taken zal gebruiken om het percentage te berekenen voltooide projecten.</p> <p>Als u [!UICONTROL Duration] selecteert, bepaalt de Duur van elke taak in een project het algemene percentage volledig voor het project, en de Duur van elke subtaak bepaalt het algemene percentage volledig voor zijn oudertaak.</p> <p>Als u [!UICONTROL Duration] selecteert, moet u de secties [!UICONTROL Typical hours per work day] en [!UICONTROL Typical work days per week] opgeven in de sectie [!UICONTROL Timelines] . [!DNL Workfront] gebruikt deze informatie wanneer het berekenen van het voltooide van een taak die op Duur wordt gebaseerd. </p> <p>Als u [!UICONTROL Planned Hours] selecteert, moet u ervoor zorgen dat voor alle taken in elk project de hoeveelheid [!UICONTROL Planned Hours] is gedefinieerd en dat de hoeveelheid niet nul is.</p><p>Voor meer informatie, zie <a href="/help/quicksilver/manage-work/tasks/task-information/project-percent-complete.md"> Volledige overzicht van de Percentage van het Project </a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Automatically set the project's Condition based on the Progress Status]</td> 
   <td> <p>Met deze voorkeur kunnen gebruikers de [!UICONTROL Condition] van een project handmatig instellen op ( [!UICONTROL On Target] , [!UICONTROL At Risk] , [!UICONTROL In Trouble] ) of [!DNL Workfront] de [!UICONTROL Condition] (Voortgangsstatus) automatisch laten instellen op basis van de voortgang van het project op de tijdlijn. Voor meer informatie over de Voorwaarde van projecten, zie <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override=""> Overzicht van het Type van de Voorwaarde en van de Voorwaarde van het Project </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Create baselines automatically]</p> </td> 
   <td> <p>Deze voorkeur leidt automatisch tot een basislijn (momentopname) van taak en projectdetails wanneer de status van het project in [!UICONTROL Current] verandert. Voor informatie over het creëren van basislijnen, zie <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override=""> projectbasislijnen </a> creëren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Performance Index Method] </p> </td> 
   <td> <p>De methode van de Index van Prestaties (PIM) voor het project controleert de methode [!DNL Workfront] gebruikt om de Vereiste metriek van de Waarde zoals [!UICONTROL Cost Performance Index] (CPI) en [!UICONTROL Estimate At Completion] (EAC) te berekenen. Voor meer informatie, zie <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override=""> [!UICONTROL Cost Performance Index] berekenen (CPI) </a> en <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Calculate Estimate At Completion] (EAC) </a></p> 
    <ul> 
     <li><strong>[!UICONTROL Hour-based]</strong>: [!DNL Workfront] gebruikt [!UICONTROL Planned Hours] om prestatiemetriek zoals EAC en CPI te berekenen. Wanneer de PIM wordt berekend op basis van uren, wordt de EAC weergegeven als een aantal uren. Zorg ervoor dat u een andere waarde voor [!UICONTROL Planned Hours] hebt dan nul.</li> 
     <li> <p><strong>[!UICONTROL Cost-based]</strong>: [!DNL Workfront] gebruikt [!UICONTROL Planned Labor Cost] om prestatiemetriek zoals EAC en CPI te berekenen. Zorg ervoor dat uw taakrollen of gebruikers zijn gekoppeld aan kosten per uur. Wanneer de PIM wordt berekend op basis van kosten, wordt de EAC weergegeven als een valutawaarde.</p> <p>De projectmanager kan deze instelling op projectniveau wijzigen met behulp van het [!UICONTROL Finance] -gebied in [!UICONTROL Project Details] . Voor meer informatie, zie <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override=""> informatie in het project [!UICONTROL Finance] gebied </a> beheren.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estimate at Completion ]</p> </td> 
   <td> <p>Bepaal welke gegevens [!DNL Workfront] gebruikt om [!UICONTROL Estimate at Completion] (EAC) te berekenen die de geprojecteerde totale kosten van een project vertegenwoordigt.</p> 
    <ul> 
     <li><strong>[!UICONTROL Calculate at project level]</strong>: EAC voor de bovenliggende taak en het bovenliggende project worden bepaald door [!UICONTROL Actual Hours] of [!UICONTROL Actual Labor Cost] in te voeren in de EAC-indelingen. Deze berekening bevat [!UICONTROL Actual Hours] of [!UICONTROL Costs and Expenses] die rechtstreeks aan de bovenliggende taak of het bovenliggende project zijn toegevoegd.</li> 
     <li> <p><strong>[!UICONTROL Roll up from tasks/subtasks]</strong>: EAC voor de oudertaak en het project worden bepaald door EAC voor elke kindtaak samen te vatten. Deze berekening sluit [!UICONTROL Actual Hours] of [!UICONTROL Actual Costs and Expenses] uit die rechtstreeks aan de bovenliggende taak of het bovenliggende project worden toegevoegd.</p> <p>De projectmanager kan dit het plaatsen op het projectniveau wijzigen, gebruikend het [!UICONTROL Finance] gebied in [!UICONTROL Project Details].Voor meer informatie, zie <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override=""> informatie in het project [!UICONTROL Finance] gebied </a> leiden.</p> </li> 
    </ul> <p>Voor meer informatie over hoe EAC berekent, zie <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override=""> [!UICONTROL Estimate At Completion] berekenen (EAC) </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Tijdlijnen {#timelines}

Configureer een of meer van de volgende voorkeuren voor nieuwe projecten in het hele systeem:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Schedule From]</td> 
   <td> <p>Bepaal of de nieuwe projecten van de Datum van het Begin of van de Datum van de Voltooiing gepland zijn wanneer zij worden gecreeerd.</p> 
    <ul> 
     <li><strong>[!UICONTROL Start Date]</strong>: Nieuwe taken worden standaard ingesteld op de taakbeperking van [!UICONTROL As Soon As Possible] en projectmanagers. Er wordt dan gevraagd een [!UICONTROL Planned Start Date] voor het project op te geven.</li> 
     <li><strong>[!UICONTROL Completion Date]</strong>: Nieuwe taken worden standaard ingesteld op de taakbeperking van [!UICONTROL As Late As Possible] en projectmanagers. Er wordt dan gevraagd een [!UICONTROL Planned Completion Date] voor het project op te geven.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User Time Off]</td> 
   <td> <p>Bepaal of de tijd van de Primaire Ontvanger van een taak de geplande data voor die taak op een project aanpast.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Consider user time off in task durations]</strong>: Om het even welke tijd van gepland voor Primaire Assignee van een taak past de geplande data van de taak aan als de tijd van weg tijdens de duur van de taak voorkomt. Dit is de standaardinstelling. </p> <p>Als een taak met een beperking van [!UICONTROL As Soon As Possible] bijvoorbeeld op 1 juni moet beginnen en op 3 juni moet worden voltooid, en de primaire ontvanger op 2 juni als een tijdelijke taak moet worden aangemerkt, worden de geplande datums van de taak aangepast aan 1 juni tot en met 4 juni.</p> <p><b> BELANGRIJK </b>:</p> <p>De duur van de taak verandert niet wanneer u deze instelling selecteert. Alleen de geplande datums veranderen, afhankelijk van de Taakbeperking.</p> </li> 
     <li><strong>[!UICONTROL Ignore user time off in task durations]</strong>: De geplande data van elke taak voor een project blijven zoals oorspronkelijk gepland, zelfs als de primaire ontvanger van een taak tijd van tijd heeft tijdens zijn duur.</li> 
    </ul> <p>Houd rekening met het volgende wanneer u opties voor deze instelling selecteert:</p> 
    <ul> 
     <li>Wanneer u deze instelling wijzigt, nemen alleen de projecten en sjablonen die na de wijziging zijn gemaakt de bijgewerkte instelling over. </li> 
     <li> <p>De waarde van de Beperking van de Taak van de taak bepaalt welke geplande taakdata om aan te passen: </p> 
      <ul> 
       <li>De geplande begindatum</li> 
       <li>De geplande afsluitdatum</li> 
       <li>Beide datums</li> 
       <li>Geen van beide datums. </li> 
      </ul> <p>Als een taak bijvoorbeeld een beperking [!UICONTROL Fixed Dates] heeft, worden de datums niet aangepast wanneer de primaire ontvanger de tijd uit heeft, zelfs als de optie [!UICONTROL Consider user time off in task duration] is geselecteerd. Voor informatie over taakbeperkingen, zie <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override=""> Overzicht van de Beperking van de Taak </a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Project timelines are automatically re-calculated]</p> </td> 
   <td> <p>Bepaal wanneer de tijdlijn van een project opnieuw wordt berekend. Voor informatie over het opnieuw berekenen van de projectchronologie, zie <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override=""> projectchronologie </a> opnieuw berekenen.</p> <p>De volgende opties zijn standaard ingeschakeld. U kunt een of meer van de volgende instellingen selecteren:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Every night]</strong>: Selecteer deze optie om de projecttijdlijnen elke avond opnieuw te berekenen. Wijzigingen die u aanbrengt in het project en die van invloed kunnen zijn op de tijdlijn, worden niet direct weergegeven. [!DNL Workfront​​​] herberekent tijdlijnen 's nachts alleen voor projecten waarbij aan beide volgende voorwaarden is voldaan:</p> <p> 
       <ul> 
        <li>een status hebben van [!UICONTROL Current]</li> 
        <li>Heeft in de afgelopen drie maanden een update</li> 
        <li>hebben een updatetype van één van het volgende gehad:</li>
        <ul>
        <li>Automatisch en bij wijziging</li>
        <li>Alleen wijzigen</li>
        <li>Alleen automatisch</li> 
      </ul>       
    <b> TIP:</b>
    <p>Deze instelling is niet van invloed op projecten met alleen het updatetype Handmatig.</p>
    <li> <p><strong> wanneer het werkingsgebied van een project </strong> verandert: Selecteer dit om projectchronologie onmiddellijk opnieuw te berekenen aangezien een verandering van het projectwerkingsgebied voorkomt. Voor informatie over wat een verandering van het projectwerkingsgebied vormt, zie <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override=""> projectchronologie </a> opnieuw berekenen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL When multiple users are assigned to a task use the schedule of the]</p> </td> 
   <td> <p>Als een project geen toegewezen programma heeft of als de gebruikers die aan zijn taken worden toegewezen geen Programma hebben dat aan hen wordt toegewezen, [!DNL Workfront] gebruikt het systeem standaardprogramma om de chronologie van de taken te berekenen.</p> <p>Als u veelvoudige gebruikers aan de zelfde taak in een project toewijst en het project een toegewezen programma heeft en de gebruikers die aan de taken worden toegewezen ook een programma hebben dat aan hen wordt toegewezen, [!UICONTROL Workfront] gebruikt de volgende programma's:</p> 
    <ul> 
     <li><strong>[!UICONTROL Primary Assignment]</strong>: [!DNL Workfront] gebruikt het schema van de primaire toewijzing voor de taak om tijdlijnen te berekenen.</li> 
     <li><strong>[!UICONTROL Project]</strong>: [!DNL Workfront] gebruikt het schema van het project om de tijdlijn van elke taak te berekenen.</li> 
    </ul> <p>Voor meer informatie over programma's, zie <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override=""> een programma </a> creëren.</p> </td> 
  </tr>

</tr> 
  <tr> 
   <td role="rowheader"> <p>Wanneer één gebruiker aan een taak wordt toegewezen, gebruik het programma van..</p> </td> 
   <td> 
<p>Als een project geen toegewezen programma heeft of als de gebruikers die aan zijn taken worden toegewezen geen Programma hebben dat aan hen wordt toegewezen, [!DNL Workfront] gebruikt het systeem standaardprogramma om de chronologie van de taken te berekenen.</p>

<p>Als u één gebruiker aan een taak in een project toewijst en zowel het project als de gebruiker die aan de taken wordt toegewezen hebben programma's verbonden aan hen, [!UICONTROL Workfront] gebruikt de volgende programma's:</p> 
    <ul> 
     <li><strong>[!UICONTROL User]</strong>: [!DNL Workfront] gebruikt het schema van de toegewezen gebruiker op de taak om tijdlijnen te berekenen.</li> 
     <li><strong>[!UICONTROL Project]</strong>: [!DNL Workfront] gebruikt het schema van het project om de tijdlijn van de taak te berekenen.</li> 
    </ul> <p>Voor meer informatie over programma's, zie <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override=""> een programma </a> creëren.</p>
</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Timeline Calculations] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Typical hours per work day]</strong>: Stel het aantal uren op een typische werkdag in voor de gebruikers die aan projecten gaan werken. De standaardwaarde is 8 uur.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL Typical work days per week]</strong>: Stel de standaardwerkweek in voor de gebruikers die aan projecten werken. De standaardwaarde is 5 dagen.</li> 
    </ul> <p>Deze twee opties zetten dagen om in uren, of weken in dagen.</p> <p>Als u bijvoorbeeld een taak hebt met 8 geplande uren en de duur wordt berekend op basis van de geplande uren, zet [!DNL Workfront] die uren om in dagen om de Duur weer te geven als dagen.</p> <p>In het veld [!UICONTROL work days per week] Normaal berekent [!DNL Workfront] de waarde FTE (Full Time Equivalent) voor uw systeem. Dit is wat [!DNL Workfront] gebruikt bij het berekenen van toewijzingen voor gebruikers.</p> <p>Deze waarden worden gebruikt wanneer u projectchronologie, het in de begroting opnemen voor middelen, of het registreren tijd tegen projecten plant. </p> <p>Zij worden niet gebruikt wanneer u timesheets voor gebruikers in het systeem, zoals die in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Configure] timesheet en uurvoorkeur </a> wordt beschreven.</p> <p><b> NOTA </b>:</p> <p>[!DNL Workfront] beheerders kunnen [!UICONTROL Timeline Calculations] -voorkeuren niet ontgrendelen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Custom Quarters]</p> </td> 
   <td> <p>Aangepaste jaarlijkse kwartalen configureren voor de gebruikers die aan projecten zullen werken. Aangepaste kwartalen zijn gewoonlijk kwartalen die niet overeenkomen met de traditionele uitsplitsing van kwartalen gedurende een kalenderjaar. U kunt meerdere aangepaste kwarten toevoegen. Voor meer informatie, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override=""> douanekwartalen voor projecten </a> toelaten.</p>  <p><b> NOTA </b>: </p><p>[!DNL Workfront] beheerders kunnen [!UICONTROL Custom Quarters] -voorkeuren niet ontgrendelen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Business Cases] {#business-cases}

U kunt een BedrijfsGeval voor pas gecreëerde projecten door het systeem tot stand brengen om projectverzoeken voor te leggen. U kunt voorkeuren definiëren om te bepalen welke gebieden zichtbaar zijn op het **[!UICONTROL Business Case]** -formulier. We raden u aan deze opties in te schakelen, zodat andere gereedschappen, zoals de [!UICONTROL Portfolio Optimizer] , correct worden bijgewerkt. Voor meer informatie over wat elke gebiedsvertoningen, zie [ een BedrijfsGeval bepalen: artikelindex ](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Nadat de [!DNL Workfront] beheerder de secties op [!UICONTROL Business Case] toelaat, kan een Eigenaar van het Project een BedrijfsGeval op het projectniveau tot stand brengen. Voor informatie over het creëren van een BedrijfsGeval, zie [ een BedrijfsGeval voor een project ](../../../manage-work/projects/define-a-business-case/create-business-case.md) creëren.

### [!UICONTROL Life After Death] {#life-after-death}

Configureer een of meer van de volgende voorkeuren voor nieuwe projecten in het hele systeem:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL After a project has been marked as Complete, people can still] </p> </td> 
   <td> <p>Bepaal de regels voor uw organisatie (of groep, als u projectvoorkeur voor een groep) betreffende vormt of een taak of een kwestie kan worden geschrapt nadat de projectstatus duidelijk is geworden [!UICONTROL Complete].</p> 
    <ul> 
     <li><strong>[!UICONTROL Delete Tasks]</strong>: Hiermee kunnen gebruikers taken uit een project verwijderen nadat het project is gemarkeerd als [!UICONTROL Complete] .<br></li> 
     <li><strong>[!UICONTROL Delete Issues]</strong>: Hiermee kunnen gebruikers uitgaven uit een project verwijderen nadat het project is gemarkeerd als [!UICONTROL Complete] .</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL After a Project is marked Complete, Dead, or it is Pending Approval, people can still]</p> </td> 
   <td> <p>Bepaal de regels voor uw organisatie (of groep, als u projectvoorkeur voor een groep) betreffende wat met taken, kwesties, documenten, en andere voorwerpen in een project gebeurt nadat de projectstatus <strong>[!UICONTROL Complete]</strong> is gemerkt, <strong>[!UICONTROL Dead]</strong>, of is <strong>[!UICONTROL Pending Approval]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL Add and edit tasks:]</strong> Hiermee kunnen gebruikers:
      <ul>
       <li><p>Taken in een project bewerken nadat het project is gemarkeerd als [!UICONTROL Complete] , [!UICONTROL Dead] of [!UICONTROL Pending Approval] .</p>
           <p>Opmerking: zelfs als deze optie niet is geselecteerd, kunnen gebruikers uitgaven-items toevoegen en bewerken. Logboekuren hebben een andere instelling. Om gebruikers toe te staan of te verhinderen tijd op projecten met een Volledige of Dode status te registreren, zie <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md"> timesheet en uurvoorkeur </a> vormen.</p></li>
       <li>Voeg taken aan een project toe.</li>
      </ul></li>
     <li><strong>[!UICONTROL Add and edit issues]</strong>: Hiermee kunnen gebruikers:
      <ul>
       <li>Bewerk problemen in een project nadat het project is gemarkeerd als [!UICONTROL Complete] , [!UICONTROL Dead] of [!UICONTROL Pending Approval] .</li>
       <li>Voeg uitgaven aan een project toe nadat het project [!UICONTROL Complete] of [!UICONTROL Dead] is gemerkt. (U kunt geen uitgaven aan een project toevoegen dat [!UICONTROL Pending Approval] is.)</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Add documents to the project and to its tasks and issues]</strong>: Hiermee kunnen gebruikers documenten toevoegen aan een project (of documenten toevoegen aan taken en problemen binnen het project) nadat het project is gemarkeerd als [!UICONTROL Complete] of [!UICONTROL Dead] .</p> <p>Deze optie is niet van toepassing op projecten die in afwachting zijn van goedkeuring.</p> </li> 
     <li> <p><strong>[!UICONTROL Attach templates]</strong>: Hiermee kunnen gebruikers sjablonen aan een project koppelen nadat het project is gemarkeerd als [!UICONTROL Complete] of [!UICONTROL Dead] .</p> <p>Deze optie is niet van toepassing op projecten die in afwachting zijn van goedkeuring.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
