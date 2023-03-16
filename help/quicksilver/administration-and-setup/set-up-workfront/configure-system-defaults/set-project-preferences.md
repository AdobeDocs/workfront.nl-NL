---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Projectvoorkeuren voor het hele systeem configureren
description: Als [!DNL Adobe Workfront] beheerder, kunt u de standaardvoorkeur voor alle projecten vormen die door het systeem worden gecreeerd. Deze voorkeuren zijn van invloed op project, taak en probleemgedrag.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '2072'
ht-degree: 0%

---

# Projectvoorkeuren voor het hele systeem configureren

Als [!DNL Adobe Workfront] beheerder, kunt u de standaardvoorkeur voor alle projecten vormen die door het systeem worden gecreeerd. Deze voorkeuren zijn van invloed op project, taak en probleemgedrag.

>[!NOTE]
>
>Deze voorkeuren zijn standaard vergrendeld en groepsbeheerders kunnen deze op groepsniveau niet wijzigen, tenzij u ze voor alle groepen in het systeem ontgrendelt. Zie voor meer informatie [Projectvoorkeuren voor alle groepen in het systeem vergrendelen of ontgrendelen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Projectvoorkeuren configureren voor de gehele organisatie

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **[!UICONTROL Project Preferences]** > **[!UICONTROL Projects]**.

1. Ga op de pagina die wordt weergegeven verder met een van de vier onderstaande secties om voorkeuren te configureren voor [!UICONTROL Project Status], [!UICONTROL Timelines], [!UICONTROL Business Cases], en [!UICONTROL Life after Death].
1. Als u wilt dat alle groepen in de organisatie dezelfde projectvoorkeuren gebruiken, moet elke voorkeur zijn vergrendeld ![](assets/lock-toggle-button.png) (dit is de standaardinstelling).

   >[!IMPORTANT]
   >
   >Als een projectvoorkeur is vergrendeld, worden alle wijzigingen die u in die voorkeur aanbrengt, overgeërfd door alle groepen in het systeem. Het is belangrijk om met de gebruikers en de groepen door uw organisatie te communiceren om ervoor te zorgen dat alle behoeften rekenschap worden gegeven in de manier u projectvoorkeur vormt.

   Voor informatie over het ontgrendelen van een voorkeur zodat alle groepen het op hun kunnen vormen en beheren, zie [Projectvoorkeuren voor alle groepen in het systeem vergrendelen of ontgrendelen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

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
        <p>Gebruik de [!UICONTROL New Project] optie in een lijst van projecten</p>
        </li>
          <li>
          <p>Een uitgave converteren naar een project vanaf de pagina van de uitgave</p>
          </li>
         </ul>
        <p>Deze voorkeur is standaard ingeschakeld. </p> 
        <p><b>OPMERKING</b></p>
        <p> Een groepsbeheerder kan deze voorkeur voor een groep wijzigen. Wanneer een gebruiker tot veelvoudige groepen met verschillende voorkeur behoort, zal de gebruiker een project zonder een malplaatje kunnen tot stand brengen als hun Groep van het Huis deze toegelaten voorkeur heeft.</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Set new project's status to]</td> 
   <td> <p>Bepaal de status van nieuwe projecten.</p>  <p><b>OPMERKING</b>  
     <ul> 
      <li>Als u of een andere [!DNL Workfront] de beheerder verbergt de hier geselecteerde status, verandert de standaardstatus in de eerste status in de statuslijst.</li> 
     </ul> 
     <ul> 
      <li> <p>Als een vergrendeld systeem of een vergrendelde groepsstatus is ingesteld als de standaardstatus en later door iemand wordt ontgrendeld, probeert het systeem deze te vervangen door een vergrendelde status van hetzelfde type status.</p> <p>Als het niet kan vinden, zoekt het naar een vereiste status:</p> 
       <ul> 
        <li>Als er een vereiste status is die gelijk is aan de niet-vergrendelde standaardstatus, wordt de vereiste status de standaardstatus, zelfs als de status ontgrendeld is.</li> 
        <li>Als geen van de vereiste statussen overeenkomt met de niet-vergrendelde standaardstatus, wordt de eerste vereiste status in de statuslijst de standaardstatus.</li> 
       </ul> <p>Raadpleeg de artikelen voor informatie over de vereiste statussen <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Heb toegang tot de lijst van de statussen van het systeemproject</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">De lijst met taakstatussen van het systeem openen</a>, en <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Toegang krijgen tot de lijst met systeemuitgiftestatussen</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calculate Percent Complete based on]</td> 
   <td> <p>Het percentage voltooide van een project of oudertaak is gebaseerd op de algemene vooruitgang van de taken. Deze informatie kan op of de Duur of de Geplande Uren van de taken op een project worden berekend.</p> <p>Als u [!UICONTROL Duration], bepaalt de Duur van elke taak in een project het algemene percentage volledig voor het project, en de Duur van elke subtaak bepaalt het algemene percentage volledig voor zijn oudertaak.</p> <p>Als u [!UICONTROL Duration], zorg ervoor dat u de [!UICONTROL Typical hours per work day] en [!UICONTROL Typical work days per week] in de [!UICONTROL Timelines] sectie. [!DNL Workfront] gebruikt deze informatie wanneer het berekenen van het volledige de percent van een taak die op Duur wordt gebaseerd. </p> <p>Als u [!UICONTROL Planned Hours]ervoor zorgen dat alle taken voor elk project de hoeveelheid [!UICONTROL Planned Hours] gedefinieerd en dat de waarde niet nul is.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Automatically set the project's Condition based on the Progress Status]</td> 
   <td> <p>Met deze voorkeur kunnen gebruikers de [!UICONTROL Condition] van een project handmatig ([!UICONTROL On Target], [!UICONTROL At Risk], [!UICONTROL In Trouble]) of [!DNL Workfront] instellen [!UICONTROL Condition] (Voortgangsstatus) wordt automatisch gebaseerd op de voortgang van het project op de tijdlijn. Voor meer informatie over de Voorwaarde van projecten, zie <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Overzicht van het type Projectvoorwaarde en Voorwaarde</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Create baselines automatically]</p> </td> 
   <td> <p>Deze voorkeur leidt automatisch tot een basislijn (momentopname) van taak en projectdetails wanneer de status van het project verandert in [!UICONTROL Current]. Voor informatie over het maken van basislijnen raadpleegt u <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Projectbasislijnen maken</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Performance Index Method] </p> </td> 
   <td> <p>De methode van de Index van Prestaties (PIM) voor het project controleert de methode [!DNL Workfront] gebruikt om de waarden van de verdiende waarde te berekenen, zoals [!UICONTROL Cost Performance Index] (CPI) en [!UICONTROL Estimate At Completion] (EAC). Zie voor meer informatie <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Berekenen [!UICONTROL Cost Performance Index] (CPI)</a> en <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Calculate Estimate At Completion] (EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL Hour-based]</strong>: [!DNL Workfront] gebruik [!UICONTROL Planned Hours] om prestatiemetriek zoals EAC en CPI te berekenen. Wanneer de PIM wordt berekend op basis van uren, wordt de EAC weergegeven als een aantal uren. Zorg ervoor dat u een waarde hebt voor [!UICONTROL Planned Hours], met uitzondering van nul.</li> 
     <li> <p><strong>[!UICONTROL Cost-based]</strong>: [!DNL Workfront] gebruik [!UICONTROL Planned Labor Cost] om prestatiemetriek zoals EAC en CPI te berekenen. Zorg ervoor dat uw taakrollen of gebruikers zijn gekoppeld aan kosten per uur. Wanneer de PIM wordt berekend op basis van kosten, wordt de EAC weergegeven als een valutawaarde.</p> <p>De projectmanager kan dit het plaatsen op het projectniveau wijzigen, gebruikend [!UICONTROL Finance] gebied in [!UICONTROL Project Details]. Zie voor meer informatie <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Informatie beheren in het project [!UICONTROL Finance] gebied</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estimate at Completion ]</p> </td> 
   <td> <p>Bepalen welke gegevens [!DNL Workfront] gebruikt voor het berekenen van de [!UICONTROL Estimate at Completion] (EAC) die de geraamde totale kosten van een project vertegenwoordigt.</p> 
    <ul> 
     <li><strong>[!UICONTROL Calculate at project level]</strong>:EAC voor de oudertaak en het project wordt bepaald door binnen te gaan [!UICONTROL Actual Hours] of [!UICONTROL Actual Labor Cost] in de EAC-formules. Deze berekening omvat [!UICONTROL Actual Hours] of [!UICONTROL Costs and Expenses] rechtstreeks toegevoegd aan de bovenliggende taak of het bovenliggende project.</li> 
     <li> <p><strong>[!UICONTROL Roll up from tasks/subtasks]</strong>: EAC voor de oudertaak en het project worden bepaald door EAC voor elke kindtaak samen te vatten. Deze berekening sluit uit [!UICONTROL Actual Hours] of [!UICONTROL Actual Costs and Expenses] rechtstreeks toegevoegd aan de bovenliggende taak of het bovenliggende project.</p> <p>De projectmanager kan dit het plaatsen op het projectniveau wijzigen, gebruikend [!UICONTROL Finance] gebied in [!UICONTROL Project Details].Zie voor meer informatie <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Informatie beheren in het project [!UICONTROL Finance] gebied</a>.</p> </li> 
    </ul> <p>Voor meer informatie over hoe de EAC berekent, raadpleegt u <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Berekenen [!UICONTROL Estimate At Completion] (EAC)</a>.</p> </td> 
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
     <li><strong>[!UICONTROL Start Date]</strong>: Nieuwe taken zijn standaard ingesteld op [!UICONTROL As Soon As Possible] De Beperking van de taak en projectmanagers worden ertoe aangezet om een [!UICONTROL Planned Start Date] voor het project.</li> 
     <li><strong>[!UICONTROL Completion Date]</strong>: Nieuwe taken zijn standaard ingesteld op [!UICONTROL As Late As Possible] De Beperking van de taak en projectmanagers worden ertoe aangezet om een [!UICONTROL Planned Completion Date] voor het project.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User Time Off]</td> 
   <td> <p>Bepaal of de tijd van de Primaire Ontvanger van een taak de geplande data voor die taak op een project aanpast.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Consider user time off in task durations]</strong>: Om het even welke tijd van gepland voor Primaire Assignee van een taak past de geplande data van de taak aan als de tijd van weg tijdens de duur van de taak voorkomt. Dit is de standaardinstelling. </p> <p>Bijvoorbeeld als een taak met een Beperking van [!UICONTROL As Soon As Possible] De eerste vergadering is gepland om op 1 juni te beginnen en op 3 juni af te sluiten. De eerste vergadering heeft op 2 juni de tijd om te vertrekken, en de geplande data van de taak worden op 1 juni tot en met 4 juni vastgesteld.</p> <p><b>BELANGRIJK</b>: De duur van de taak verandert niet wanneer u deze instelling selecteert. Alleen de geplande datums veranderen, afhankelijk van de Taakbeperking.</p> </li> 
     <li><strong>[!UICONTROL Ignore user time off in task durations]</strong>: De geplande data van elke taak op een project blijven zoals oorspronkelijk gepland, zelfs als de primaire ontvanger van een taak tijd van tijd heeft tijdens zijn duur.</li> 
    </ul> <p>Houd rekening met het volgende wanneer u opties voor deze instelling selecteert:</p> 
    <ul> 
     <li>Wanneer u deze instelling wijzigt, nemen alleen de projecten en sjablonen die na de wijziging zijn gemaakt de bijgewerkte instelling over. </li> 
     <li> <p>De waarde van de Beperking van de Taak van de taak bepaalt welke geplande taakdata om aan te passen: </p> 
      <ul> 
       <li>De geplande begindatum</li> 
       <li>De geplande afsluitdatum</li> 
       <li>Beide datums</li> 
       <li>Geen van beide datums. </li> 
      </ul> <p>Als een taak bijvoorbeeld een beperking heeft van [!UICONTROL Fixed Dates], worden de datums niet aangepast wanneer de primaire ontvanger over tijd beschikt, zelfs als de optie [!UICONTROL Consider user time off in task duration] is geselecteerd. Voor informatie over taakbeperkingen, zie <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Overzicht van taakbeperking</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Project timelines will be automatically re-calculated]</p> </td> 
   <td> <p>Bepaal wanneer de tijdlijn van een project opnieuw wordt berekend. Voor informatie over het opnieuw berekenen van de projecttijdlijn raadpleegt u <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Projecttijdlijnen opnieuw berekenen</a>.</p> <p>De volgende opties zijn standaard ingeschakeld. U kunt een of meer van de volgende instellingen selecteren:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Every night]</strong>: Selecteer deze optie om de projecttijdlijnen elke avond opnieuw te berekenen. Wijzigingen die u aanbrengt in het project en die van invloed kunnen zijn op de tijdlijn, worden niet direct weergegeven. [!DNL Workfront​​​] herberekent alleen tijdlijnen 's nachts voor projecten waarbij aan beide volgende voorwaarden is voldaan:</p> <p> 
       <ul> 
        <li>een status hebben van [!UICONTROL Current]</li> 
        <li>Heeft in de afgelopen drie maanden een update</li> 
        <li>hebben een updatetype van één van het volgende gehad:</li>
        <ul>
        <li>Automatisch en bij wijziging</li>
        <li>Alleen wijzigen</li>
        <li>Alleen automatisch</li> 
      </ul>       
    <b>TIP</b>
    <p>Deze instelling heeft geen invloed op projecten met alleen het updatetype Handmatig.</p>
    <li> <p><strong>Wanneer het bereik van een project verandert</strong>: Selecteer dit om projectchronologie onmiddellijk opnieuw te berekenen aangezien een verandering van het projectwerkingsgebied voorkomt. Voor informatie over wat een verandering van het projectwerkingsgebied betekent, zie <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Projecttijdlijnen opnieuw berekenen</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL When multiple users are assigned to a task use the schedule of the]</p> </td> 
   <td> <p>Als een project geen toegewezen programma heeft of als de gebruikers die aan zijn taken worden toegewezen geen Programma hebben dat aan hen wordt toegewezen; [!DNL Workfront] gebruikt het standaardschema van het systeem om de chronologie van de taken te berekenen.</p> <p>Als u veelvoudige gebruikers aan de zelfde taak in een project toewijst heeft toegewezen programma-en de gebruikers die aan de taken worden toegewezen hebben ook een programma dat aan hen wordt toegewezen—[!UICONTROL Workfront] gebruikt de volgende schema's:</p> 
    <ul> 
     <li><strong>[!UICONTROL Primary Assignment]</strong>: [!DNL Workfront] gebruikt het programma van de Primaire Taak op de taak om chronologie te berekenen.</li> 
     <li><strong>[!UICONTROL Project]</strong>: [!DNL Workfront] gebruikt het programma van het project om de chronologie van elke taak te berekenen.</li> 
    </ul> <p>Voor meer informatie over programma's, zie <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Een schema maken</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Timeline Calculations] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Typical hours per work day]</strong>: Stel het aantal uren op een typische werkdag in voor de gebruikers die aan projecten gaan werken. De standaardwaarde is 8 uur.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL Typical work days per week]</strong>: Stel de standaardwerkweek in voor de gebruikers die aan projecten gaan werken. De standaardwaarde is 5 dagen.</li> 
    </ul> <p>Deze twee opties zetten dagen om in uren, of weken in dagen.</p> <p>Als u bijvoorbeeld een taak hebt met 8 geplande uren en de duur wordt berekend op basis van de geplande uren, [!DNL Workfront] zet die uren in dagen om om de Duur als dagen te tonen.</p> <p>Van de standaard [!UICONTROL work days per week] veld, [!DNL Workfront] berekent de FTE-waarde (Full Time Equivalent) voor uw systeem. Dit is wat [!DNL Workfront] wordt gebruikt bij het berekenen van toewijzingen voor gebruikers.</p> <p>Deze waarden worden gebruikt wanneer u projectchronologie, het in de begroting opnemen voor middelen, of het registreren tijd tegen projecten plant. </p> <p>Ze worden niet gebruikt wanneer u tijdbladen voor gebruikers in het systeem opstelt, zoals beschreven in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Configure] voorkeuren voor tijdlijnen en uren</a>.</p> <p><b>OPMERKING</b>: [!DNL Workfront] beheerders kunnen niet ontgrendelen [!UICONTROL Timeline Calculations] voorkeuren.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Custom Quarters]</p> </td> 
   <td> <p>Aangepaste jaarlijkse kwartalen configureren voor de gebruikers die aan projecten zullen werken. Aangepaste kwartalen zijn gewoonlijk kwartalen die niet overeenkomen met de traditionele uitsplitsing van kwartalen gedurende een kalenderjaar. U kunt meerdere aangepaste kwarten toevoegen. Zie voor meer informatie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Aangepaste kwartalen inschakelen voor projecten</a>.</p>  <p><b>OPMERKING</b>: [!DNL Workfront] beheerders kunnen niet ontgrendelen [!UICONTROL Custom Quarters] voorkeuren.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Business Cases] {#business-cases}

U kunt een BedrijfsGeval voor pas gecreëerde projecten door het systeem tot stand brengen om projectverzoeken voor te leggen. U kunt voorkeuren definiëren om te bepalen welke gebieden zichtbaar zijn in het dialoogvenster **[!UICONTROL Business Case]** formulier. Wij adviseren dat u deze opties toelaat zodat andere hulpmiddelen, zoals [!UICONTROL Portfolio Optimizer], correct bijwerken. Voor meer informatie over wat elk gebied toont, zie [Een bedrijfscase definiëren](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Na de [!DNL Workfront] de beheerder laat de secties op toe [!UICONTROL Business Case], kan een Eigenaar van het Project een BedrijfsGeval op het projectniveau dan tot stand brengen. Voor informatie over het creëren van een BedrijfsGeval, zie [Een bedrijfscase maken voor een project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL Life After Death] {#life-after-death}

Configureer een of meer van de volgende voorkeuren voor nieuwe projecten in het hele systeem:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL After a project has been marked as Complete, people can still] </p> </td> 
   <td> <p>Bepaal de regels voor uw organisatie (of groep, als u projectvoorkeur voor een groep) betreffende vormt of een taak of een kwestie kan worden geschrapt nadat de projectstatus is duidelijk gemaakt [!UICONTROL Complete].</p> 
    <ul> 
     <li><strong>[!UICONTROL Delete Tasks]</strong>: Staat gebruikers toe om taken van een project te schrappen nadat het project is gemerkt [!UICONTROL Complete].<br></li> 
     <li><strong>[!UICONTROL Delete Issues]</strong>: Staat gebruikers toe om kwesties van een project te schrappen nadat het project is gemerkt [!UICONTROL Complete].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL After a Project is marked Complete, Dead, or it is Pending Approval, people can still]</p> </td> 
   <td> <p>Bepaal de regels voor uw organisatie (of groep, als u projectvoorkeur voor een groep) betreffende wat aan taken, kwesties, documenten, en andere voorwerpen in een project vormt nadat de projectstatus is duidelijk gemaakt <strong>[!UICONTROL Complete]</strong>, <strong>[!UICONTROL Dead]</strong>, of <strong>[!UICONTROL Pending Approval]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL Add and edit tasks]</strong> Hiermee kunnen gebruikers:
      <ul>
       <li>Taken in een project bewerken nadat het project is gemarkeerd [!UICONTROL Complete], [!UICONTROL Dead], of [!UICONTROL Pending Approval]. Dit omvat het toevoegen van uren en het veranderen van uitgaveningangen op een taak.</li>
       <li>Voeg taken aan een project toe.</li>
      </ul></li> 
     <li><strong>[!UICONTROL Add and edit issues]</strong>: Hiermee kunnen gebruikers:
      <ul>
       <li>Geef kwesties binnen een project uit nadat het project is gemerkt [!UICONTROL Complete], [!UICONTROL Dead], of [!UICONTROL Pending Approval].</li>
       <li>Voeg kwesties aan een project toe nadat het project is gemerkt [!UICONTROL Complete] of [!UICONTROL Dead]. (U kunt geen kwesties aan een project toevoegen dat [!UICONTROL Pending Approval].)</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Add documents to the project and to its tasks and issues]</strong>: Staat gebruikers toe om documenten aan een project (of om documenten aan taken en kwesties binnen het project toe te voegen) toe te voegen nadat het project is gemerkt [!UICONTROL Complete] of [!UICONTROL Dead].</p> <p>Deze optie is niet van toepassing op projecten die in afwachting zijn van goedkeuring.</p> </li> 
     <li> <p><strong>[!UICONTROL Attach templates]</strong>: Staat gebruikers toe om malplaatjes aan een project vast te maken nadat het project is gemerkt [!UICONTROL Complete] of [!UICONTROL Dead].</p> <p>Deze optie is niet van toepassing op projecten die in afwachting zijn van goedkeuring.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
