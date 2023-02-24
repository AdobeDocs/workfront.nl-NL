---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Werkbladprofielen maken, bewerken en toewijzen
description: U kunt timesheet-profielen maken, bewerken en toewijzen die terugkerende tijdbladen voor uw gebruikers genereren zonder tussenkomst van u. Zo bespaart u tijd en bent u verzekerd van consistentie tussen gebruikers.
author: Alina
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 43f1ad86784532ed3a5a3baa12d135ca35f16d21
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 0%

---

# Werkbladprofielen maken, bewerken en toewijzen

U kunt timesheet-profielen maken, bewerken en toewijzen die terugkerende tijdbladen voor uw gebruikers genereren zonder tussenkomst van u. Dit bespaart u tijd en zorgt ervoor dat het volgende tussen gebruikers verenigbaar is:

* Tijdschema tijdpagina
* Fiatteurs
* Algemene uurtypen

Voor meer informatie over het manueel creëren van een timesheet, zie [Een timesheet voor eenmalig gebruik maken](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>U moet administratieve toegang tot Timesheets hebben. </p> <p>Zie voor meer informatie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p>  <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Een tijdbladprofiel maken of bewerken

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>Als u wijzigingen in het tijdlijnprofiel wilt inschakelen in de huidige tijdbladen, moet u de bestaande tijdbladen verwijderen en vervolgens nieuwe tijdbladen genereren. Zie voor instructies [Tijdschema&#39;s in Adobe Workfront verwijderen](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) en [Tijdbladen handmatig genereren](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik op **Tijdschema en uren**.

   of

   Als u een tijdlijnprofiel voor een groep maakt of bewerkt, klikt u op **Groepen** en klikt u op de naam van de groep.

1. Klikken **Tijdbladprofielen**.
1. Klik op **Nieuw profiel**.

   of

   Als u een bestaand tijdbladprofiel wilt bewerken, selecteert u het tijdlijnprofiel dat u wilt bewerken en klikt u op **Bewerken**.

   Het nieuwe of bestaande tijdbladprofiel wordt weergegeven.


1. Op de **Details instellen** tab, typ een **Naam** en **Beschrijving** voor het tijdbladprofiel en de volgende informatie verstrekken:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Groep met de Toegang van het Beleid</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>Laat dit veld leeg als u een tijdbladprofiel op systeemniveau maakt.</p> <p>Om het even welke gebruiker die gebruikersrekeningen kan uitgeven kan een systeem-vlakke timesheet aan andere gebruikers vastmaken.</p> <p>Alleen een Workfront-beheerder kan een tijdbladprofiel op systeemniveau bewerken.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>Als u een timesheet-profiel maakt voor een groep die u beheert, moet u hier de groep identificeren.</p> <p>Hiermee wordt het tijdbladprofiel niet toegewezen aan de gebruikers in de groep. het staat slechts de beheerders van de groep toe om het timesheet profiel te wijzigen. In Stap 6 wijst u het profiel aan gebruikers toe.</p> <p><b>OPMERKING</b>

   Wanneer gebruikers buiten de groep timesheet-profielen aan andere gebruikers koppelen, kunnen ze dit tijdbladprofiel niet zien of koppelen.</p> </li>
   </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tijdschema's maken</strong> </td> 
      <td> <p> <p>Geef op wanneer het tijdbladprofiel de tijdbladen moet genereren. Een timesheet kan worden geplaatst om automatisch op wekelijkse, bi-wekelijkse, halfmaandelijkse, of maandbasis te produceren. Selecteer de dag van de week waarop u het tijdspad wilt maken.</p>
      <p>Een wekelijkse timesheet begint op de datum het wordt geproduceerd. Als u bijvoorbeeld elke donderdag wekelijkse tijdbladen maakt, is de eerste dag van de week op het tijdsplaat donderdag.</p>
      <p><b>OPMERKING</b></p>

   <p>Workfront maakt altijd twee tijdbladen tegelijk: het eerste tijdspad bevat altijd de huidige datum en het tweede tijdspad begint wanneer het tijdkader van de eerste termijn eindigt.</p> </p> </td> 
    </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Fiatteurs</strong></p> </td> 
      <td> <p> <p>Approvers zijn gebruikers die timesheet voor de gebruikers goedkeuren verbonden aan timesheet. U kunt maximaal 7 gebruikers identificeren als fiatteurs op een timesheet. Het identificeren van veelvoudige gebruikers is nuttig om een fiatteur beschikbaar te verzekeren wanneer iemand uit het bureau is. Alle fiatteurs worden op de hoogte gesteld wanneer een gebruiker het tijdspad ter goedkeuring indient. Slechts één gebruiker wordt vereist om timesheet goed te keuren om het te worden goedgekeurd.</p> <p>Alleen gebruikers met beheerdersrechten voor tijdschriften kunnen worden ingesteld als fiatteurs. Voor meer informatie over administratieve rechten op tijdspagina raadpleegt u <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> <p>Gebruik het drop-down menu om fiatteur voor timesheet (als een fiatteur wordt vereist) te selecteren. U kunt uit de volgende opties selecteren:</p> 
      <ul> 
      <li><strong>Geen</strong>: Het tijdschema hoeft niet te worden goedgekeurd.</li> 
      <li><strong>Hun manager</strong>: Dit is de standaardfiatteur, die door het systeem wordt geplaatst. In dit geval, keurt de gebruiker die als hun manager wordt aangewezen timesheet goed wanneer het ter goedkeuring wordt voorgelegd.</li> 
      <li><strong>Specifieke personen:</strong> U kunt specifieke gebruikers, door naam, als timesheet fiatteurs aanwijzen. U kunt veelvoudige fiatteurs op een timesheet hebben. In dat geval wordt het tijdspad, nadat een van de fiatteurs het tijdsplaat heeft goedgekeurd, als volgt gemarkeerd <strong>Gesloten</strong> en verdwijnt uit de lijst van goedkeuringen volgens het tijdschema van alle resterende fiatteurs.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Kan tijd bewerken </strong> </td> 
      <td> <p> <p>Selecteer deze optie als de fiatteurs de uren op het tijdblad mogen bewerken.

   Deze optie werkt samen met de **Tijdschema&#39;s bewerken beperken tot eigenaars en beheerders** het plaatsen in de Opstelling > de Tijdopmaak &amp; van Uren > het gebied van de Voorkeur. Zie voor meer informatie <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Voorkeuren voor tijdpagina&#39;s en uren configureren</a>.

   De volgende scenario&#39;s bestaan:

   <ul>
      <li>Wanneer de <b>Tijdschema's bewerken beperken tot eigenaars en beheerders</b> optie is ingeschakeld:</li>
      <ul><li>De fiatteurs kunnen slechts timesheet goedkeuren en verwerpen, ongeacht of <b>Kan tijd bewerken</b> is ingeschakeld of niet. </li>
      <li>De managers van timesheet-eigenaars kunnen alleen de tijdbladen van hun directe rapporten bekijken.</li></ul>
      <li>Wanneer de <b>Tijdschema's bewerken beperken tot eigenaars en beheerders</b> optie is uitgeschakeld:</li>
    <ul><li>Wanneer de <b>Kan tijd bewerken</b> is ingeschakeld, kunnen fiatteurs de tijdpagina verzenden, opnieuw openen of sluiten en de tijd bewerken.</li>
      <li>Wanneer de <b>Kan tijd bewerken</b> is uitgeschakeld, kunnen fiatteurs de tijdpagina niet verzenden, opnieuw openen of sluiten en kunnen de tijd niet bewerken. De fiatteurs kunnen timesheet slechts goedkeuren of verwerpen. </li>
      <li>De managers van de eigenaars van de chronologie van chronologie kunnen voorleggen, terugroepen, heropenen en hun directe rapporten uitgeven.</li></ul>
      </ul>

   <p><b>OPMERKING</b>

   Nadat u een tijdspad ter goedkeuring hebt verzonden, kunt u de uren niet meer bewerken. Om een voorgelegde timesheet aan een editable staat terug te keren, wijs timesheet terug of hebben fiatteur de timesheet verwerpen. Zie voor meer informatie <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Een tijdschema ter goedkeuring indienen</a> en<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Een tijdschema goedkeuren</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Beschikbare uurtypen</strong> </td> 
      <td>Door gebrek, zien de gebruikers alle algemene uren op een timesheet. Nochtans, als uw organisatie slechts specifieke algemene uren voor een bepaalde reeks gebruikers wil worden getoond, kunt u de algemene uren selecteren die zij in hun timesheets moeten zien door hen in hun timesheet profiel op dit gebied te selecteren. Als u alle algemene uren wilt onbruikbaar maken, schrap alle uurtypes om timesheet zonder een sectie voor algemene uren te produceren.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Overwerk</span> </td> 
      <td>U kunt het vak Overwerk verbergen in tijdbladen. Deze optie is standaard uitgeschakeld.</td> 
     </tr> 
    </tbody> 
    </table>

1. Klik op de knop **Personen toewijzen** om het tijdbladprofiel te koppelen aan specifieke gebruikers, groepen of (als u een Workfront-beheerder bent) teams. Typ de naam van de gebruiker, groep of team en klik vervolgens op de naam wanneer deze in de vervolgkeuzelijst wordt weergegeven.

   Als u een groepsbeheerder bent, kunt u het timesheet-profiel toewijzen aan groepen die u beheert, maar niet aan teams. Zie voor meer informatie [Beperkingen voor een groepsbeheerder die een timesheet-profiel toewijst](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) in dit artikel.

   >[!NOTE]
   >
   >* U kunt een gebruiker ook aan een tijdlijnprofiel koppelen door het gebruikersprofiel te bewerken. Zie voor meer informatie [Gebruikersprofiel bewerken](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* Wanneer u een groep toevoegt, wordt alleen de groepsnaam weergegeven op het tabblad Personen toewijzen, niet de lijst met groepsleden. Als u de hier vermelde groepsleden wilt zien, klik sparen Veranderingen, dan klik de naam van het timesheet profiel u enkel creeerde.
   >* Wanneer u deze stappen beëindigt, produceert het timesheet profiel timesheets slechts voor de toegewezen gebruikers of groepsleden die geen bestaande timesheets voor de huidige periode hebben.


1. Klikken **Wijzigingen opslaan**.

   De eerste keer het timesheet profiel produceert timesheets, worden 2 timesheets gecreeerd voor elke gebruiker. Daarna, telkens als het nieuwe timesheets produceert, op timesheet wordt gecreeerd per gebruiker.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## Beperkingen voor een groepsbeheerder die een timesheet-profiel toewijst {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

Als u een groepsbeheerder bent en de beheertoegangsoptie Timesheets &amp; de uren in uw toegangsniveau wordt onbruikbaar gemaakt, kunt u timesheet profielen tot stand brengen, maar u kunt hen slechts toewijzen aan:

* Groepen die u beheert
* Afzonderlijke gebruikers die u kunt bewerken en die deel uitmaken van een groep die u beheert

Voor deze groepen en gebruikers, zult u geen toegang tot timesheets hebben die het timesheet profiel produceert.

Als de optie Gebruikersbeheer (Groepgebruikers) ook is uitgeschakeld in uw toegangsniveau, kunt u het tijdbladprofiel toewijzen aan een groep die u beheert, maar dit heeft alleen invloed op de gebruikers in de groep die u toegang hebt om te bewerken. Als de groep gebruikers bevat die u geen toegang hebt om te bewerken, wordt aan deze gebruikers niet het tijdbladprofiel en de rest van de groep toegewezen.

Voor informatie over de optie Timesheets &amp; uren in uw toegangsniveau, zie [Gebruikers administratieve toegang verlenen tot bepaalde gebieden](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Voor informatie over de optie Gebruikersbeheer (Groepgebruikers) in uw toegangsniveau, zie [Toegang verlenen aan gebruikers](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Meerdere terugkerende tijdbladprofielen

U kunt meer dan één timesheet profiel voor uw organisatie hebben als er zijn:

* Unieke betalingstermijnen voor verschillende groepen gebruikers
* Unieke fiatteurs voor verschillende groepen gebruikers
* Unieke algemene urenvereisten voor verschillende gebruikersgroepen

Eén gebruiker kan niet aan meerdere tijdlijnprofielen tegelijk worden gekoppeld. 
