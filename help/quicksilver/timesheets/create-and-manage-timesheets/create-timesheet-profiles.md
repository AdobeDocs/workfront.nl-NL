---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Werkbladprofielen maken, bewerken en toewijzen
description: U kunt timesheet-profielen maken, bewerken en toewijzen die terugkerende tijdbladen voor uw gebruikers genereren zonder tussenkomst van u. Zo bespaart u tijd en bent u verzekerd van consistentie tussen gebruikers.
author: Lisa
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 611c3c947855610cf86cdcbf96d1e9d847e34f38
workflow-type: tm+mt
source-wordcount: '1668'
ht-degree: 0%

---

# Werkbladprofielen maken, bewerken en toewijzen

<!--Audited: 06/2025-->

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Het is beschikbaar slechts in het milieu van de Sandbox van de Voorproef, en wordt vrijgegeven in gefaseerde uitrol aan Productie.</span>

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

   * **Naam**: Voeg een naam voor het timesheet profiel toe. Het zou de naam van een team of een groep kunnen zijn waarvan de mensen het zelfde tijdsbestek voor hun timesheets delen. Dit is een verplicht veld.
   * **Beschrijving**: Voeg meer informatie over het timesheet profiel toe.
   * **Groep met de Toegang van het Beleid**: Als u een systeem-vlakke timesheet profiel creeert, verlaat dit gebied leeg.

     Om het even welke gebruiker die gebruikersrekeningen kan uitgeven kan een systeem-vlakke timesheet aan andere gebruikers vastmaken.

     Alleen een Workfront-beheerder kan een tijdbladprofiel op systeemniveau bewerken.

     Als u een timesheet-profiel maakt voor een groep die u beheert, moet u hier de groep identificeren.

     Hiermee wordt het tijdlijnprofiel niet toegewezen aan de gebruikers in de groep. De beheerders van de groep kunnen het tijdbladprofiel alleen wijzigen. In Stap 6 wijst u het profiel aan gebruikers toe.

     >[!NOTE]
     >
     >Wanneer gebruikers buiten de groep timesheet-profielen aan andere gebruikers koppelen, kunnen ze dit tijdbladprofiel niet zien of koppelen.

   * **creeer timesheets**: Specificeer wanneer het timesheet profiel de timesheets zou moeten produceren. Een timesheet kan worden geplaatst om automatisch op wekelijkse, bi-wekelijkse, halfmaandelijkse, of maandbasis te produceren. Selecteer de dag van de week waarop u het tijdspad wilt maken.

     Een wekelijkse timesheet begint op de datum het wordt geproduceerd. Als u bijvoorbeeld elke donderdag wekelijkse tijdbladen maakt, is de eerste dag van de week op het tijdsplaat donderdag.

     >[!NOTE]
     >
     >Workfront maakt altijd twee tijdbladen tegelijk: de eerste tijdpagina bevat altijd de huidige datum en de tweede tijdpagina begint wanneer het tijdframe van de eerste eindigt.

   * **Approvers**: Approvers zijn gebruikers die timesheet voor de gebruikers goedkeuren verbonden aan timesheet. U kunt maximaal 7 gebruikers identificeren als fiatteurs op een timesheet. Het identificeren van veelvoudige gebruikers is nuttig om een fiatteur beschikbaar te verzekeren wanneer iemand uit het bureau is. Alle fiatteurs worden op de hoogte gesteld wanneer een gebruiker het tijdspad ter goedkeuring indient. Slechts één gebruiker wordt vereist om timesheet goed te keuren om het te worden goedgekeurd.

     Alleen gebruikers met beheerdersrechten voor tijdschriften kunnen worden ingesteld als fiatteurs. Voor meer informatie over timesheet administratieve rechten, zie [ gebruikers administratieve toegang van de Verlening tot bepaalde gebieden ](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

     Gebruik het drop-down menu om fiatteur voor timesheet (als een fiatteur wordt vereist) te selecteren. U kunt uit de volgende opties selecteren:

      * **niets**: De timesheet te hoeven niet worden goedgekeurd.
      * **Hun Manager**: Dit is de standaardfiatteur, die door het systeem wordt geplaatst. In dit geval, keurt de gebruiker die als hun manager wordt aangewezen timesheet goed wanneer het ter goedkeuring wordt voorgelegd.
      * **Specifieke Mensen**: U kunt specifieke gebruikers, door naam, als timesheet fiatteurs aanwijzen. U kunt veelvoudige fiatteurs op een timesheet hebben. In dit geval, nadat één van de fiatteurs timesheet goedkeurt, wordt timesheet duidelijk als **Gesloten** en het verdwijnt van de lijst van timesheet goedkeuringen van alle resterende fiatteurs.

   * **kan tijd** uitgeven: Selecteer deze optie om de fiatteurs toe te staan om uren op timesheet uit te geven.

     Deze optie werkt samen met **beperkt timesheet het uitgeven aan eigenaars en beheert** plaatsen in de Opstelling > de Tijdopmaak &amp; het gebied van de Uren > van de Voorkeur. Voor meer informatie, zie [ timesheet en uurvoorkeur ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) vormen.

     De volgende scenario&#39;s bestaan:

     Wanneer **timesheet het uitgeven aan eigenaars en beheert** optie wordt toegelaten:

      * De fiatteurs kunnen timesheet slechts goedkeuren en verwerpen, ongeacht of Can uitgeven tijd of niet wordt toegelaten.
      * De managers van timesheet-eigenaars kunnen alleen de tijdbladen van hun directe rapporten bekijken.

     Wanneer **timesheet het uitgeven aan eigenaars en beheert** optie wordt onbruikbaar gemaakt:

      * Wanneer **tijd** kan uitgeven wordt toegelaten, kunnen de fiatteurs voorleggen, opnieuw openen of sluiten timesheet en kunnen de tijd uitgeven.
      * Wanneer **tijd kan uitgeven** gehandicapt is, kunnen de fiatteurs niet voorleggen, heropenen of sluiten timesheet en kunnen niet de tijd uitgeven. De fiatteurs kunnen timesheet slechts goedkeuren of verwerpen.
      * De managers van de eigenaars van de chronologie van chronologie kunnen voorleggen, terugroepen, heropenen en hun directe rapporten uitgeven.

     >[!NOTE]
     >
     >Nadat u een tijdspad ter goedkeuring hebt verzonden, kunt u de uren niet meer bewerken. Om een voorgelegde timesheet aan een editable staat terug te keren, wijs timesheet terug of hebben fiatteur de timesheet verwerpen. Voor meer informatie, zie [ een timesheet voor goedkeuring ](/help/quicksilver/timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md) voorleggen en [ goedkeuren timesheet ](/help/quicksilver/timesheets/create-and-manage-timesheets/timesheet-approvals.md).

   * **Overtime**: U kunt verkiezen om de doos van Overuren in chronologiebladen te verbergen. Deze optie is standaard uitgeschakeld.
   * **Beschikbare Types van Uur**: Dit het plaatsen verwijst slechts naar de Algemene Types van Uur, en niet naar project-specifieke uurtypes.

     Door gebrek, zien de gebruikers alle algemene uren op een timesheet. Nochtans, als uw organisatie slechts specifieke algemene uren voor een bepaalde reeks gebruikers wil worden getoond, kunt u de algemene uren selecteren die zij in hun timesheets moeten zien door hen in hun timesheet profiel op dit gebied te selecteren. Als u alle algemene uren wilt onbruikbaar maken, schrap alle uurtypes om timesheet zonder een sectie voor algemene uren te produceren.

   * **Herinneringsberichten**: Voeg een herinnering bericht toe. Workfront stuurt herinneringen naar gebruikers om hen te vragen hun tijdbladen in te vullen of goed te keuren. U moet herinneringsberichten tot stand brengen alvorens u hen met een timesheet profiel kunt associëren.

1. Wanneer het creëren van groep-vlakke timesheet profielen in Productie, klik **toewijzen de Mensen** tabel om het timesheet profiel met specifieke gebruikers, groepen, of (als u een beheerder van Workfront) teams bent te associëren. <!--To associate the timesheet profile with specific users, groups, or (if you are a Workfront administrator) teams, scroll towards the bottom of the page and find the **Assign People** section.-->

   <span class="preview"> wanneer het creëren van groep-vlakke timesheet profielen in Voorproef, scrol naar de bodem van de pagina en vind **toewijzen Mensen** sectie.</span>

   Wanneer het creëren van timesheet profielen voor het systeem, scrol naar de bodem van de pagina en vind **toewijzen de 1} sectie van Mensen**.

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

<!--
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td> <p> Add a name for the timesheet profile. It could be the name of a team or a group whose people share the same timeframe for their timesheets. </p> <p>This ia a required field.</p> </td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td> <p> Add more information about the timesheet profile.     
      </p> </td> 
     </tr>

   <tr> 
   <td role="rowheader"><strong>Group with Administration Access</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>If you are creating a system-level timesheet profile, leave this field blank.</p> <p>Any user who can edit user accounts can attach a system-level timesheet to other users.</p> <p>Only a Workfront administrator can edit a system-level timesheet profile.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>If you are creating a timesheet profile for a group you administer, identify the group here.</p> <p>This does not assign the timesheet profile to the users in the group; it only allows the group's administrators to modify the timesheet profile. You will assign the profile to users in Step 6.</p>

   <p><b>NOTE</b>: When users outside the group are attaching timesheet profiles to other users, they won't be able to see or attach this timesheet profile.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Create timesheets</strong> </td> 
      <td> <p> <p>Specify when the timesheet profile should generate the timesheets. A timesheet can be set to automatically generate on a weekly, bi-weekly, semi-monthly, or monthly basis. Select the day of the week when you want the timesheet to be produced.</p>
      <p>A weekly timesheet begins on the date it is generated. For example, if you create weekly timesheets every Thursday, the first day of the week on the timesheet is Thursday.</p>
    
      
   <p><b>NOTE</b>: Workfront always creates two timesheets at a time: the first timesheet always includes the current date, and the second timesheet starts when the time frame of the first one ends.</p> </p> </td> 
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Approvers</strong></p> </td> 
      <td> <p> <p>Approvers are users who approve the timesheet for the users associated with the timesheet. You can identify up to 7 users as approvers on a timesheet. Identifying multiple users is useful to ensure an approver is available when someone is out of the office. All approvers are notified when a user submits the timesheet for approval. Only one user is required to approve the timesheet in order for it to be approved.</p> <p>Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Use the drop-down menu&nbsp;to select&nbsp;the approver&nbsp;for the timesheet (if an approver is required). You can select from the following options:</p> 
      <ul> 
      <li><strong>None</strong>: The timesheet does not need to&nbsp;be approved.</li> 
      <li><strong>Their Manager</strong>: This is the default approver, set by the system. In this case, the user designated as their manager approves the timesheet when it is submitted for approval.</li> 
      <li><strong>Specific People:</strong>&nbsp;You can designate specific users, by name, as timesheet approvers. You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as <strong>Closed</strong> and it disappears from the timesheet approvals list of all the remaining approvers.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Can edit time </strong> </td> 
      <td> <p> <p>Select this option to allow the approvers to edit hours on the timesheet. 

   <p>This option works together with the **Restrict timesheet editing to owners and admins** setting in the Setup > Timesheet & Hours > Preferences area. For more information, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configure timesheet and hour preferences</a>.</p>

   <p>The following scenarios exist: </p>

   <ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is enabled:</li>
      <ul><li>Approvers can only approve and reject timesheet, regardless of whether the <b>Can edit time</b> is enabled or not. </li>
      <li>Timesheet owners' managers can only view their direct reports' timesheets.</li></ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is disabled:</li>
    <ul><li>When the <b>Can edit time</b> is enabled, approvers can submit, reopen, or close the timesheet and can edit the time.</li>
      <li>When the <b>Can edit time</b> is disabled, approvers cannot submit, reopen, or close the timesheet and cannot edit the time. Approvers can only approve or reject the timesheet. </li>
      <li>Timesheet owners' managers can submit, recall, reopen, and edit their direct reports' timesheets.</li></ul>
      </ul>

   <p>

   <b>NOTE</b>: Once you submit a timesheet for approval, you can no longer edit the hours. To return a submitted timesheet to an editable state, recall the timesheet or have the approver reject the timesheet. For more information, see <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Submit a timesheet for approval</a> and <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approve a timesheet</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Overtime</strong> </td> 
      <td>You can choose to hide the Overtime box in timesheets. This option is disabled by default.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Available Hour Types</strong> </td> 
      <td><p>This setting refers only to General Hour Types, and not to project-specific hour types. </p>
      <p>By default, users see all general hours on a timesheet. However, if your organization wants only specific general hours to be shown for a particular set of users, you can select the general hours that they need to see in their timesheets by selecting them in their timesheet profile in this field. If you want to disable all general hours, deselect all hour types to generate the timesheet without a section for general hours.</p></td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Reminder notifications</strong> </td> 
      <td> <p> Add a reminder notification. Workfront will send reminders to users to ask them to complete or approve their timesheets. You must create reminder notifications before you can associate them with a timesheet profile.  </p> </td> 
     </tr>
    </tbody> 
   </table>
-->