---
title: Projectvoorkeuren voor een groep configureren
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: Als u een groepsbeheerder en een beheerder van Adobe Workfront een projectvoorkeur voor alle groepen in het systeem ontgrendelt, kunt u die voorkeur voor uw groep vormen om alle verdere projecten te beïnvloeden die uw groep creeert.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: fb1c7ade6622db391e0dac54f37603efe9dc0a58
workflow-type: tm+mt
source-wordcount: '2658'
ht-degree: 0%

---

# Projectvoorkeuren voor een groep configureren

Als u een groepsbeheerder en een beheerder van Adobe Workfront een projectvoorkeur voor alle groepen in het systeem ontgrendelt, kunt u die voorkeur voor uw groep vormen om alle verdere projecten te beïnvloeden die uw groep creeert.

Als er groepen zijn boven de groep die u beheert, kunnen hun beheerders dit ook voor uw groep doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

>[!NOTE]
>
>* Een niet-vergrendelde voorkeur blijft meestal voor onbepaalde tijd ontgrendeld. Als de beheerder van Workfront het opnieuw sluit, wordt het systeem opnieuw plaatsend dat en de montages voor de voorkeur door de groepsbeheerders wordt gemaakt worden verloren.
>* De voorkeuren die zijn ingesteld voor de groep die is gekoppeld aan een project, hebben voorrang op de voorkeuren die zijn ingesteld voor de thuisgroep van de gebruiker die het project maakt.
>* Sommige voorkeuren op groepsniveau zijn van invloed op projectsjablonen die u voor de groep maakt. Zie de sectie voor meer informatie [Sjablonen voor uw groep weergeven, bewerken en maken vanuit het gebied Groepen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) in het artikel [De projectsjablonen van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Nadat een beheerder van Workfront een voorkeur op het systeemniveau ontgrendelt, kunt u het vormen en dan het sluiten om ervoor te zorgen dat iedereen in uw groep en in zijn subgroepen de zelfde configuratie gebruikt. Dit is parallel aan de mogelijkheid dat een Workfront-beheerder een voorkeur voor iedereen in het systeem moet configureren en vergrendelen. Zie voor meer informatie [Een project, taak of uitgave van subgroepen vergrendelen of ontgrendelen](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

Configuratie op groepsniveau is ook mogelijk voor taak- en uitgavenvoorkeuren en voor voorkeuren voor tijdbladen en uren. Zie voor meer informatie [Taak- en uitgavevoorkeuren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) en [Voorkeuren voor tijdschriften en uren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

Voor informatie over hoe een beheerder van Workfront een projectvoorkeur ontgrendelt, zie [Projectvoorkeuren voor alle groepen in het systeem vergrendelen of ontgrendelen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-abonnement*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> <p>U moet een groepsbeheerder van de groep of een beheerder van Workfront zijn. Zie voor meer informatie <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Groepbeheerders</a> en <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de Workfront-beheerder als u wilt weten welk abonnement- of licentietype u hebt.

## Een ontgrendelde projectvoorkeur voor een groep configureren

>[!TIP]
>
>Als u een beheerder van Workfront bent, kunt u stappen 1-4 overslaan door te gaan naar Opstelling > de Voorkeur van het Project > Projecten, dan zoekend naar de naam van de groep in de doos bij de bovenkant van de pagina.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Groepen** ![](assets/groups-icon.png).

1. Klik op de naam van de groep waarvan u de projectvoorkeuren wilt configureren.
1. Klik in het linkerdeelvenster op **Projectvoorkeuren**.
1. Op de pagina die wordt weergegeven, gaat u verder met een van de vier onderstaande secties om voorkeuren voor de projectstatus, tijdlijnen, Business Case en Life after Death in te stellen.

   >[!TIP]
   >
   >Als u de muisaanwijzer boven een voorkeur houdt en knopinfo wordt weergegeven om aan te geven dat deze vergrendeld is, kunt u de Workfront-beheerder vragen deze te ontgrendelen voor alle groepen in de organisatie.

* [Projectstatus](#project-status)
* [Tijdlijnen](#timelines)
* [Zakelijke zaken](#business-cases)
* [Na de dood](#life-after-death)

### Projectstatus {#project-status}

Configureer een of meer van de volgende voorkeuren voor nieuwe projecten die aan de groep zijn gekoppeld:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>Gebruikers toestaan projecten te maken zonder een sjabloon te gebruiken</td>
<td><p>Deze voorkeur staat gebruikers toe om projecten tot stand te brengen zonder een malplaatje te gebruiken wanneer het creëren van een project van de volgende gebieden:</p>
<ul>
<li><p>De optie Nieuw project gebruiken in een lijst met projecten</p></li>

<li><p>Een uitgave converteren naar een project vanaf de pagina van de uitgave</p></li>
</ul>

<p>Deze voorkeur is standaard ingeschakeld op systeemniveau.</p>
<p><b>OPMERKING</b></p>
<p>Wanneer een gebruiker tot veelvoudige groepen met verschillende voorkeur behoort, zal de gebruiker toegestaan zijn om een project zonder een malplaatje tot stand te brengen als minstens één van hun groepen deze voorkeur toegelaten heeft.</p>
</td></tr>
  <tr> 
   <td role="rowheader">Status van nieuw project instellen op</td> 
   <td> <p>Bepaal de status van nieuwe projecten.</p> <p><b>OPMERKING</b>   
     <ul> 
      <li>Als u of een andere Workfront-beheerder de hier geselecteerde status verbergt, verandert de standaardstatus in de eerste status in de statuslijst.</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">Voor groepsprojectvoorkeuren kunt u alleen een vergrendelde status of een vereiste status als standaardstatus selecteren.</li> 
      <li> <p>Als een vergrendeld systeem of een vergrendelde groepsstatus is ingesteld als de standaardstatus en later door iemand wordt ontgrendeld, probeert het systeem deze te vervangen door een vergrendelde status van hetzelfde type status.</p> <p>Als het niet kan vinden, zoekt het naar een vereiste status:</p> 
       <ul> 
        <li>Als er een vereiste status is die gelijk is aan de niet-vergrendelde standaardstatus, wordt de vereiste status de standaardstatus, zelfs als de status ontgrendeld is.</li> 
        <li>Als geen van de vereiste statussen overeenkomt met de niet-vergrendelde standaardstatus, wordt de eerste vereiste status in de statuslijst de standaardstatus.</li> 
       </ul> <p>Raadpleeg de artikelen voor meer informatie over de vereiste statussen <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Heb toegang tot de lijst van de statussen van het systeemproject</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">De lijst met taakstatussen van het systeem openen</a>, en <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Toegang krijgen tot de lijst met systeemuitgiftestatussen</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Percentage berekenen voltooid op basis van</td> 
   <td> <p>Het percentage voltooide van een project of oudertaak is gebaseerd op de algemene vooruitgang van de taken. Deze informatie kan op of de Duur of de Geplande Uren van de taken op een project worden berekend.</p> <p>Als u Duur selecteert, bepaalt de Duur van elke taak in een project het algemene percentage volledig voor het project, en de Duur van elke subtaak bepaalt het algemene percentage volledig voor zijn oudertaak.</p> <p>Als u Duur selecteert, moet u de Normale uren per werkdag en de Typische werkdagen per week opgeven in de sectie Tijdlijnen. Workfront gebruikt deze informatie wanneer het berekenen van het percentage van een taak volledig op Duur wordt gebaseerd. </p> <p>Als u Geplande Uren selecteert, zorg ervoor dat alle taken op elk project de hoeveelheid Geplande Uren bepaalde uren hebben, en dat de hoeveelheid niet nul is.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">De projectvoorwaarde automatisch instellen op basis van de status van de voortgang</td> 
   <td> <p>Met deze voorkeur kunnen gebruikers de voorwaarde van een project handmatig instellen (Op doel, Bij risico, In problemen) of Workfront de voorwaarde (Voortgangsstatus) automatisch laten instellen op basis van de voortgang van het project op de tijdlijn. Zie voor meer informatie over de voorwaarde van projecten <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Overzicht van het type Projectvoorwaarde en Voorwaarde</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Basislijnen automatisch maken</p> </td> 
   <td> <p>Deze voorkeur leidt automatisch tot een basislijn (momentopname) van taak en projectdetails wanneer de status van het project in Huidig verandert. Zie voor informatie over het maken van basislijnen <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Projectbasislijnen maken</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Prestatiesindexmethode </p> </td> 
   <td> <p>De methode van de Index van Prestaties (PIM) voor het project controleert de methode Workfront gebruikt om de Vereiste metriek van de Waarde zoals de Index van de Prestaties van de Kosten (CPI) en Schatting bij Voltooiing (EAC) te berekenen. Zie voor meer informatie <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Kostenprestatie-index (CPI) berekenen</a>en <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Schatting berekenen bij voltooiing (EAC)</a></p> 
    <ul> 
     <li><strong>Op basis van uren</strong>: Workfront gebruikt Geplande uren om prestatiemetriek zoals EAC en CPI te berekenen. Wanneer de PIM wordt berekend op basis van uren, wordt de EAC weergegeven als een aantal uren. Zorg ervoor dat u een waarde hebt voor Geplande Uren, behalve nul.</li> 
     <li> <p><strong>Op basis van kosten</strong>: Workfront gebruikt Geplande loonkosten om prestatiemetriek zoals EAC en CPI te berekenen. Zorg ervoor dat uw taakrollen of gebruikers zijn gekoppeld aan kosten per uur. Wanneer de PIM wordt berekend op basis van kosten, wordt de EAC weergegeven als een valutawaarde.</p> <p>De projectmanager kan dit het plaatsen op het projectniveau wijzigen, gebruikend het gebied van de Financiën in de Details van het Project.Voor meer informatie, zie <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Informatie beheren in het gebied Projectfinanciering</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Schatting bij voltooiing </p> </td> 
   <td> <p>Bepaal welke gegevens Workfront gebruikt om de schatting bij voltooiing (EAC) te berekenen die de geraamde totale kosten van een project vertegenwoordigt.</p> 
    <ul> 
     <li><strong>Berekenen op projectniveau</strong>:EAC voor de oudertaak en het project worden bepaald door Werkelijke Uren of Werkelijke Kosten van de Arbeid in de Formulas EAC in te gaan. Deze berekening omvat Werkelijke uren of Kosten en Uitgaven die rechtstreeks aan de oudertaak of het project worden toegevoegd.</li> 
     <li> <p><strong>Omhoog rollen vanuit taken/subtaken</strong>: EAC voor de oudertaak en het project worden bepaald door EAC voor elke kindtaak samen te vatten. Deze berekening sluit Werkelijke uren of Werkelijke Kosten en Uitgaven die rechtstreeks aan de oudertaak of het project worden toegevoegd uit.</p> <p>De projectmanager kan dit het plaatsen op het projectniveau wijzigen, gebruikend het gebied van de Financiën in de Details van het Project.Voor meer informatie, zie <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Informatie beheren in het gebied Projectfinanciering</a>.</p> </li> 
    </ul> <p>Voor meer informatie over hoe de EAC berekent, zie <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Schatting berekenen bij voltooiing (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Tijdlijnen {#timelines}

Configureer een of meer van de volgende voorkeuren voor nieuwe projecten die aan de groep zijn gekoppeld:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Schema vanuit</td> 
   <td> <p>Bepaal of de nieuwe projecten van de Datum van het Begin of van de Datum van de Voltooiing gepland zijn wanneer zij worden gecreeerd.</p> 
    <ul> 
     <li><strong>Begindatum</strong>: De nieuwe taken worden gebrek aan zo spoedig mogelijk de Beperking van de Taak en projectmanagers ertoe aangezet om een Geplande Datum van het Begin voor het project te verstrekken.</li> 
     <li><strong>Voltooiingsdatum</strong>: De nieuwe taken worden gebrek aan de ZO laat Mogelijke Beperking van de Taak en projectmanagers ertoe aangezet om een Geplande Datum van de Voltooiing voor het project te verstrekken.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Gebruikerstijd uit</td> 
   <td> <p>Bepaal of de tijd van de Primaire Ontvanger van een taak de geplande data voor die taak op een project aanpast.</p> 
    <ul> 
     <li> <p><strong>Overweeg de gebruikerstijd in taakduur</strong>: Om het even welke tijd van gepland voor Primaire Assignee van een taak past de geplande data van de taak aan als de tijd van weg tijdens de duur van de taak voorkomt. Dit is de standaardinstelling. </p> <p>Als bijvoorbeeld een taak met een beperking van zo snel mogelijk op 1 juni moet beginnen en op 3 juni moet worden voltooid, en de primaire ontvanger op 2 juni als tijdelijke taak moet worden aangemerkt, worden de geplande data van de taak aangepast aan 1 juni tot en met 4 juni.</p> <p><b>BELANGRIJK</b>: De duur van de taak verandert niet wanneer u deze instelling selecteert. Alleen de geplande datums veranderen, afhankelijk van de Taakbeperking.</p> </li> 
     <li><strong>Gebruikerstijd in taakduur negeren</strong>: De geplande data van elke taak voor een project blijven zoals oorspronkelijk gepland, zelfs als de primaire ontvanger van een taak tijd van tijd heeft tijdens zijn duur.</li> 
    </ul> <p>Houd rekening met het volgende wanneer u opties voor deze instelling selecteert:</p> 
    <ul> 
     <li>Wanneer u deze instelling wijzigt, nemen alleen de projecten en sjablonen die na de wijziging zijn gemaakt de bijgewerkte instelling over. </li> 
     <li> <p>De waarde van de Beperking van de Taak van de taak bepaalt welke geplande taakdata om aan te passen: </p> 
      <ul> 
       <li>De geplande begindatum</li> 
       <li>De geplande afsluitdatum</li> 
       <li>Beide datums</li> 
       <li>Geen van beide datums. </li> 
      </ul> <p>Bijvoorbeeld, als een taak een Beperking van Vaste Datums heeft, passen de data niet aan wanneer de Primaire Ontvanger tijd weg heeft, zelfs als de optie de tijd van de gebruiker in taakduur overweegt wordt geselecteerd. Voor informatie over taakbeperkingen, zie <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Overzicht van taakbeperking</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Projecttijdlijnen worden automatisch opnieuw berekend</strong> </p> </td> 
   <td> <p>Bepaal wanneer de tijdlijn van een project opnieuw wordt berekend. Zie voor informatie over het opnieuw berekenen van de projecttijdlijn <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Projecttijdlijnen opnieuw berekenen</a>.</p> <p>De volgende opties zijn standaard ingeschakeld. U kunt een of meer van de volgende instellingen selecteren:</p> 
    <ul> 
     <li> <p><strong>Elke avond</strong>: Selecteer deze optie om de projecttijdlijnen elke avond opnieuw te berekenen. Wijzigingen die u aanbrengt in het project en die van invloed kunnen zijn op de tijdlijn, worden niet direct weergegeven. Workfront ​ ​ de tijdlijnen alleen 's nachts opnieuw te berekenen voor projecten waarbij aan beide volgende voorwaarden is voldaan:</p> <p> 
       <ul> 
        <li>Huidige status hebben</li> 
        <li>Heeft in de afgelopen drie maanden een update</li> 
       </ul> </p> </li> 
     <li> <p><strong>Wanneer het bereik van een project verandert</strong>: Selecteer deze optie om de projecttijdlijnen onmiddellijk opnieuw te berekenen terwijl een wijziging in het projectbereik plaatsvindt. Voor informatie over wat een verandering van het projectwerkingsgebied betekent, zie <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Projecttijdlijnen opnieuw berekenen</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Wanneer de veelvoudige gebruikers aan een taak worden toegewezen, gebruik het programma van</strong> </p> </td> 
   <td> <p>Als een project geen toegewezen programma heeft of als de gebruikers die aan zijn taken worden toegewezen geen Programma hebben dat aan hen wordt toegewezen, gebruikt Workfront het systeem standaardprogramma om de chronologie van de taken te berekenen.</p> <p>Als u veelvoudige gebruikers aan de zelfde taak in een project toewijst heeft toegewezen programma-en de gebruikers die aan de taken worden toegewezen hebben ook een programma toegewezen aan hen-Workfront gebruikt de volgende programma's:</p> 
    <ul> 
     <li><strong>Primaire toewijzing</strong>: Workfront gebruikt het schema van de primaire toewijzing voor de taak om tijdlijnen te berekenen.</li> 
     <li><strong>Project</strong>: Workfront gebruikt het programma van het project om de chronologie van elke taak te berekenen.</li> 
    </ul> <p>Voor meer informatie over programma's, zie <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Een schema maken</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Tijdlijnberekeningen </p> </td> 
   <td> 
    <ul> 
     <li><strong>Normaal aantal uren per werkdag</strong>: Stel het aantal uren op een typische werkdag in voor de gebruikers die aan projecten gaan werken. De standaardwaarde is 8 uur.</li> 
    </ul> 
    <ul> 
     <li><strong>Gemiddeld aantal werkdagen per week</strong>: Stel de standaardwerkweek in voor de gebruikers die aan projecten gaan werken. De standaardwaarde is 5 dagen.</li> 
    </ul> <p>Deze twee opties zetten dagen om in uren, of weken in dagen.</p> <p>Als u bijvoorbeeld een taak hebt met 8 geplande uren en de duur wordt berekend op basis van de geplande uren, zet Workfront die uren om in dagen om de Duur weer te geven als dagen.</p> <p>Vanuit het veld Normaal aantal werkdagen per week berekent Workfront de waarde FTE (Full Time Equivalent) voor uw systeem. Dit is wat Workfront gebruikt bij het berekenen van toewijzingen voor gebruikers.</p> <p>Deze waarden worden gebruikt wanneer u projectchronologie, het in de begroting opnemen voor middelen, of het registreren tijd tegen projecten plant. </p> <p>Ze worden niet gebruikt wanneer u tijdbladen voor gebruikers in het systeem opstelt, zoals beschreven in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Voorkeuren voor tijdpagina's en uren configureren</a>.</p> <p><b>OPMERKING</b>: Workfront-beheerders kunnen voorkeuren voor tijdlijnberekeningen niet ontgrendelen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>Aangepaste tekens</strong> </p> </td> 
   <td> <p>Aangepaste jaarlijkse kwartalen configureren voor de gebruikers die aan projecten zullen werken. Aangepaste kwartalen zijn gewoonlijk kwartalen die niet overeenkomen met de traditionele uitsplitsing van kwartalen gedurende een kalenderjaar. U kunt meerdere aangepaste kwarten toevoegen. Zie voor meer informatie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Aangepaste kwartalen inschakelen voor projecten</a>.</p> <p><b>OPMERKING</b>: Workfront-beheerders kunnen de voorkeuren voor aangepaste tekens niet ontgrendelen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Zakelijke zaken {#business-cases}

U kunt een BedrijfsGeval voor pas gecreëerde projecten tot stand brengen verbonden aan de groep om projectverzoeken voor te leggen. U kunt voorkeuren definiëren om te bepalen welke gebieden zichtbaar zijn in het dialoogvenster **Bedrijfs-case** formulier. Wij adviseren dat u deze opties toelaat zodat andere hulpmiddelen, zoals Portfolio Optimizer, behoorlijk bijwerken. Voor meer informatie over wat elk gebied toont, zie [Een bedrijfscase definiëren: artikelindex](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Nadat de beheerder van Workfront de secties op het BedrijfsGeval toelaat, kan een Eigenaar van het Project een BedrijfsGeval op het projectniveau dan creëren. Voor informatie over het creëren van een BedrijfsGeval, zie [Een bedrijfscase maken voor een project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### Na de dood  {#life-after-death}

Configureer een of meer van de volgende voorkeuren voor nieuwe projecten die aan de groep zijn gekoppeld:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>Nadat een project als Voltooid is gemarkeerd, kunnen mensen nog</strong> </p> </td> 
   <td> <p>Bepaal de regels voor uw organisatie (of groep, als u projectvoorkeur voor een groep) betreffende vormt of een taak of een kwestie kan worden geschrapt nadat de projectstatus is duidelijk Voltooid.</p> 
    <ul> 
     <li><strong>Taken verwijderen</strong>: Hiermee kunnen gebruikers taken uit een project verwijderen nadat het project is gemarkeerd als Voltooid.<br></li> 
     <li><strong>Problemen verwijderen</strong>: Hiermee kunnen gebruikers uitgaven uit een project verwijderen nadat het project is gemarkeerd als Voltooid.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Nadat een project is gemarkeerd als Voltooid, Dead of In afwachting van goedkeuring, kunnen mensen nog steeds</strong> </p> </td> 
   <td> <p>Bepaal de regels voor uw organisatie (of groep, als u projectvoorkeur voor een groep) betreffende wat aan taken, kwesties, documenten, en andere voorwerpen in een project vormt nadat de projectstatus is duidelijk gemaakt <strong>Voltooid</strong>, <strong>Dead</strong>, of <strong>In behandeling</strong>.</p> 
    <ul> 
     <li><strong>Taken toevoegen en bewerken</strong> Hiermee kunnen gebruikers: 
      <ul> 
       <li>Bewerk taken binnen een project nadat het project is gemarkeerd als Voltooid, Dode of In afwachting van goedkeuring. Dit omvat het toevoegen van uren en het veranderen van uitgaveningangen op een taak.</li> 
       <li>Voeg taken aan een project toe.</li> 
      </ul></li> 
     <li><strong>Uitgaven toevoegen en bewerken</strong>: Hiermee kunnen gebruikers: 
      <ul> 
       <li>Geef kwesties binnen een project uit nadat het project is duidelijk Voltooid, Dead, of in afwachting van Goedkeuring.</li> 
       <li>Voeg kwesties aan een project toe nadat het project is duidelijk Voltooid of Dood. (U kunt geen kwesties aan een project toevoegen dat in afwachting van Goedkeuring is.)</li> 
      </ul></li> 
     <li> <p><strong>Documenten toevoegen aan het project en aan de taken en problemen ervan</strong>: Hiermee kunnen gebruikers documenten toevoegen aan een project (of documenten toevoegen aan taken en problemen binnen het project) nadat het project is gemarkeerd als Voltooid of Gedoekt.</p> <p>Deze optie is niet van toepassing op projecten die in afwachting zijn van goedkeuring.</p> </li> 
     <li> <p><strong>Sjablonen bijvoegen</strong>: Staat gebruikers toe om malplaatjes aan een project vast te maken nadat het project is duidelijk Voltooid of Dood.</p> <p>Deze optie is niet van toepassing op projecten die in afwachting zijn van goedkeuring.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
