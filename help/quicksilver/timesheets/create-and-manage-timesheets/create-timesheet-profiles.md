---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Werkbladprofielen maken, bewerken en toewijzen
description: U kunt timesheet-profielen maken, bewerken en toewijzen die terugkerende tijdbladen voor uw gebruikers genereren zonder tussenkomst van u. Zo bespaart u tijd en bent u verzekerd van consistentie tussen gebruikers.
author: Lisa
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 939407f56b39617441f669d11b9439e445ceaf6e
workflow-type: tm+mt
source-wordcount: '1641'
ht-degree: 0%

---

# Werkbladprofielen maken, bewerken en toewijzen

{{highlighted-preview}}

<!--Audited: 06/2025-->

U kunt timesheet-profielen maken, bewerken en toewijzen die terugkerende tijdbladen voor uw gebruikers genereren zonder tussenkomst van u. Dit bespaart u tijd en zorgt ervoor dat het volgende tussen gebruikers verenigbaar is:

* Tijdschema tijdpagina
* Fiatteurs
* Algemene uurtypen

Voor meer informatie over het creëren van manueel timesheet, zie [ een enig-gebruiktimesheet ](../../timesheets/create-and-manage-timesheets/create-tmshts.md) creëren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Nieuw: Standaard </p>
 <p>of</p> 
<p>Huidig: Plan </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet administratieve toegang tot Chronologie hebben. </p> </td> 
  </tr> 
 </tbody> 
</table>

*For meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een tijdbladprofiel maken of bewerken

<!--Old info: 
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>Als u wijzigingen in het tijdlijnprofiel in de huidige tijdbladen wilt inschakelen, moet u de bestaande tijdbladen verwijderen voordat u de wijzigingen in de tijdlijnprofielen aanbrengt en vervolgens nieuwe tijdbladen genereren. Voor instructies, zie [ timesheets van de Schrapping in Adobe Workfront ](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) en [ produceren manueel timesheets ](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

{{step-1-to-setup}}

1. Als u creeert of een timesheet profiel voor gebruik door het systeem uitgeeft, klik **Chronologie &amp; Uren**.

   of

   Als u creeert of een timesheet profiel voor een groep uitgeeft, klik **Groepen**, dan klik de naam van de groep.

1. Klik **Profielen van de Chronologie**.
1. Om een timesheet profiel tot stand te brengen, klik **Nieuw Profiel**.

   of

   Om een bestaand timesheet profiel uit te geven, selecteer het timesheet profiel u wilt uitgeven, dan klik **uitgeven**.

   De nieuwe of bestaande pagina van het timesheet- profiel toont.

1. Werk de volgende gegevens bij:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong> Naam </strong> </td> 
      <td> <p> Voeg een naam voor het timesheet profiel toe. Het zou de naam van een team of een groep kunnen zijn waarvan de mensen het zelfde tijdsbestek voor hun timesheets delen. </p> <p>Dit is een verplicht veld.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong> Beschrijving </strong> </td> 
      <td> <p> Voeg meer informatie toe over het tijdlijnprofiel.     
      </p> </td> 
     </tr>

   <tr> 
   <td role="rowheader"><strong> Groep met de Toegang van het Beleid </strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>Laat dit veld leeg als u een tijdbladprofiel op systeemniveau maakt.</p> <p>Om het even welke gebruiker die gebruikersrekeningen kan uitgeven kan een systeem-vlakke timesheet aan andere gebruikers vastmaken.</p> <p>Alleen een Workfront-beheerder kan een tijdbladprofiel op systeemniveau bewerken.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>Als u een timesheet-profiel maakt voor een groep die u beheert, moet u hier de groep identificeren.</p> <p>Hiermee wordt het tijdlijnprofiel niet toegewezen aan de gebruikers in de groep. De beheerders van de groep kunnen het tijdbladprofiel alleen wijzigen. In Stap 6 wijst u het profiel aan gebruikers toe.</p>

   <p><b> NOTA </b>: Wanneer de gebruikers buiten de groep timesheet profielen aan andere gebruikers vastmaken, zullen zij niet dit timesheet profiel kunnen zien of vastmaken.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> creeer timesheets </strong> </td> 
      <td> <p> <p>Geef op wanneer het tijdbladprofiel de tijdbladen moet genereren. Een timesheet kan worden geplaatst om automatisch op wekelijkse, bi-wekelijkse, halfmaandelijkse, of maandbasis te produceren. Selecteer de dag van de week waarop u het tijdspad wilt maken.</p>
      <p>Een wekelijkse timesheet begint op de datum het wordt geproduceerd. Als u bijvoorbeeld elke donderdag wekelijkse tijdbladen maakt, is de eerste dag van de week op het tijdsplaat donderdag.</p>


   <p><b> NOTA </b>: Workfront leidt altijd tot twee timesheets in een tijd: eerste timesheet omvat altijd de huidige datum, en tweede timesheet begint wanneer het tijdkader van eerste beëindigt.</p> </p> </td> 
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Fiatteurs</strong></p> </td> 
      <td> <p> <p>Approvers zijn gebruikers die timesheet voor de gebruikers goedkeuren verbonden aan timesheet. U kunt maximaal 7 gebruikers identificeren als fiatteurs op een timesheet. Het identificeren van veelvoudige gebruikers is nuttig om een fiatteur beschikbaar te verzekeren wanneer iemand uit het bureau is. Alle fiatteurs worden op de hoogte gesteld wanneer een gebruiker het tijdspad ter goedkeuring indient. Slechts één gebruiker wordt vereist om timesheet goed te keuren om het te worden goedgekeurd.</p> <p>Alleen gebruikers met beheerdersrechten voor tijdschriften kunnen worden ingesteld als fiatteurs. Voor meer informatie over timesheet administratieve rechten, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref"> gebruikers administratieve toegang van de Verlening tot bepaalde gebieden </a>.</p> <p>Gebruik het drop-down menu om fiatteur voor timesheet (als een fiatteur wordt vereist) te selecteren. U kunt uit de volgende opties selecteren:</p> 
      <ul> 
      <li><strong> niets </strong>: De timesheet te hoeven niet worden goedgekeurd.</li> 
      <li><strong> Hun Manager </strong>: Dit is de standaardfiatteur, die door het systeem wordt geplaatst. In dit geval, keurt de gebruiker die als hun manager wordt aangewezen timesheet goed wanneer het ter goedkeuring wordt voorgelegd.</li> 
      <li><strong> Specifieke Mensen:</strong> u kunt specifieke gebruikers, door naam, als timesheet fiatteurs aanwijzen. U kunt veelvoudige fiatteurs op een timesheet hebben. In dit geval, nadat één van de fiatteurs timesheet goedkeurt, wordt timesheet duidelijk als <strong> Gesloten </strong> en het verdwijnt van de lijst van timesheet goedkeuringen van alle resterende fiatteurs.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Kan tijd bewerken </strong> </td> 
      <td> <p> <p>Selecteer deze optie als de fiatteurs de uren op het tijdblad mogen bewerken.

   <p>Deze optie werkt samen met de instelling **Tijdschema's bewerken beperken tot eigenaars en beheerders** in het gebied Voorkeuren &gt; Instellen &gt; Timesheet &amp; uur. Voor meer informatie, zie <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md"> timesheet en uurvoorkeur </a> vormen.</p>

   <p>De volgende scenario's bestaan: </p>

   <ul>
      <li>Wanneer <b> timesheet het uitgeven aan eigenaars en beheert </b> optie wordt toegelaten:</li>
      <ul><li>De fiatteurs kunnen timesheet slechts goedkeuren en verwerpen, ongeacht of <b> tijd </b> kan uitgeven of niet wordt toegelaten. </li>
      <li>De managers van timesheet-eigenaars kunnen alleen de tijdbladen van hun directe rapporten bekijken.</li></ul>
      <li>Wanneer <b> timesheet het uitgeven aan eigenaars en beheert </b> optie wordt onbruikbaar gemaakt:</li>
    <ul><li>Wanneer <b> tijd </b> kan uitgeven wordt toegelaten, kunnen de fiatteurs voorleggen, opnieuw openen of sluiten timesheet en kunnen de tijd uitgeven.</li>
      <li>Wanneer <b> tijd </b> kan uitgeven wordt onbruikbaar gemaakt, kunnen de fiatteurs niet voorleggen, heropenen of sluiten timesheet en kunnen niet de tijd uitgeven. De fiatteurs kunnen timesheet slechts goedkeuren of verwerpen. </li>
      <li>De managers van de eigenaars van de chronologie van chronologie kunnen voorleggen, terugroepen, heropenen en hun directe rapporten uitgeven.</li></ul>
      </ul>

   <p>

   <b> NOTA </b>: Zodra u een timesheet voor goedkeuring voorlegt, kunt u niet meer de uren uitgeven. Om een voorgelegde timesheet aan een editable staat terug te keren, wijs timesheet terug of hebben fiatteur de timesheet verwerpen. Voor meer informatie, zie <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md"> een timesheet voor goedkeuring </a> voorleggen en <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md"> goedkeuren timesheet </a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong> Overtime </strong> </td> 
      <td>U kunt het vak Overwerk verbergen in tijdbladen. Deze optie is standaard uitgeschakeld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Beschikbare Types van Uur </strong> </td> 
      <td><p>Deze instelling verwijst alleen naar Algemene uurtypen en niet naar projectspecifieke uurtypen. </p>
      <p>Door gebrek, zien de gebruikers alle algemene uren op een timesheet. Nochtans, als uw organisatie slechts specifieke algemene uren voor een bepaalde reeks gebruikers wil worden getoond, kunt u de algemene uren selecteren die zij in hun timesheets moeten zien door hen in hun timesheet profiel op dit gebied te selecteren. Als u alle algemene uren wilt onbruikbaar maken, schrap alle uurtypes om timesheet zonder een sectie voor algemene uren te produceren.</p></td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong> de berichten van de Herinnering </strong> </td> 
      <td> <p> Voeg een herinneringsmelding toe. Workfront stuurt herinneringen naar gebruikers om hen te vragen hun tijdbladen in te vullen of goed te keuren. U moet herinneringsberichten tot stand brengen alvorens u hen met een timesheet profiel kunt associëren.  </p> </td> 
     </tr>

1. Wanneer het creëren van groep-vlakke timesheet profielen in Productie, klik **toewijzen de Mensen** tabel om het timesheet profiel met specifieke gebruikers, groepen, of (als u een beheerder van Workfront) teams bent te associëren. <!--Keep the reference to the group upon release to Prod, for now, until they unshim the group Timesheet Profiles-->

   <span class="preview"> wanneer het creëren van groep-vlakke timesheet profielen in Voorproef, scrol naar de bodem van de pagina en vind **toewijzen Mensen** sectie.</span>

   Wanneer het creëren van timesheet profielen voor het systeem, scrol naar de bodem van de pagina en vind **toewijzen de 1&rbrace; sectie van Mensen**. <!--Keep the reference to the system when releasing to Prod, until they unshim the group Timesheet Profile-->

   Typ de naam van de gebruiker, groep of team en klik vervolgens op de naam wanneer deze in de vervolgkeuzelijst wordt weergegeven.

   Als u een groepsbeheerder bent, kunt u het timesheet-profiel toewijzen aan groepen die u beheert, maar niet aan teams. Voor meer informatie, zie [ Beperkingen voor een groepsbeheerder die een timesheet profiel ](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) in dit artikel toewijst.

   >[!NOTE]
   >
   >* U kunt een gebruiker ook aan een tijdlijnprofiel koppelen door het gebruikersprofiel te bewerken. Voor meer informatie, zie [ het profiel van een gebruiker ](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.
   >* Wanneer u een groep toevoegt, wordt alleen de groepsnaam weergegeven op het tabblad Personen toewijzen, niet de lijst met groepsleden. Als u de hier vermelde groepsleden wilt zien, klik sparen Veranderingen, dan klik de naam van het timesheet profiel u enkel creeerde.
   >* Wanneer u deze stappen beëindigt, produceert het timesheet profiel timesheets slechts voor de toegewezen gebruikers of groepsleden die geen bestaande timesheets voor de huidige periode hebben.

1. Klik **sparen**.

1. Bij de bovenkant van de lijst van het timesheet profiel, klik **Meer** pictogram ![ Meer pictogram ](assets/more-icon.png), dan klik **produceert timesheets**.

   Onder aan het scherm wordt bevestigd dat tijdbladen zijn gegenereerd. Nieuwe tijdbladen worden gegenereerd op basis van de nieuwe profielen die u hebt gemaakt.

   Voor meer informatie, zie [ manueel timesheets ](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md) produceren.

   De eerste keer wordt het timesheet profiel timesheets geproduceerd, twee timesheets gecreeerd voor elke gebruiker, zowel voor het timeframe dat de huidige tijd evenals voor het volgende timeframe omvat.

   Daarna, telkens als het nieuwe timesheets produceert, wordt één timesheet gecreeerd per gebruiker.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## Beperkingen voor een groepsbeheerder die een timesheet-profiel toewijst {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

Als u een groepsbeheerder bent en de beheertoegangsoptie Timesheets &amp; de uren in uw toegangsniveau wordt onbruikbaar gemaakt, kunt u timesheet profielen tot stand brengen, maar u kunt hen slechts toewijzen aan:

* Groepen die u beheert
* Afzonderlijke gebruikers die u kunt bewerken en die deel uitmaken van een groep die u beheert

Voor deze groepen en gebruikers, zult u geen toegang tot timesheets hebben die het timesheet profiel produceert.

Als de optie Gebruikersbeheer (Groepgebruikers) ook is uitgeschakeld in uw toegangsniveau, kunt u het tijdbladprofiel toewijzen aan een groep die u beheert, maar dit heeft alleen invloed op de gebruikers in de groep die u toegang hebt om te bewerken. Als de groep gebruikers bevat die u geen toegang hebt om te bewerken, wordt aan deze gebruikers niet het tijdbladprofiel en de rest van de groep toegewezen.

Voor informatie over de optiesTijdopnemers &amp; uren in uw toegangsniveau, zie [ gebruikers administratieve toegang van de Verlening tot bepaalde gebieden ](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Voor informatie over de optieGebruiker Admin (de Gebruikers van de Groep) in uw toegangsniveau, zie [ Toegang van de Verlening tot gebruikers ](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Meerdere terugkerende tijdbladprofielen

U kunt meer dan één timesheet profiel voor uw organisatie hebben als er zijn:

* Unieke betalingstermijnen voor verschillende groepen gebruikers
* Unieke fiatteurs voor verschillende groepen gebruikers
* Unieke algemene urenvereisten voor verschillende gebruikersgroepen

Eén gebruiker kan niet aan meerdere tijdlijnprofielen tegelijk worden gekoppeld.
