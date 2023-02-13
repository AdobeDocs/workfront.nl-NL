---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Een timesheet voor eenmalig gebruik maken
description: U kunt manueel tot een enig-gebruik timesheet leiden als u een timesheet wilt die niet terugkeert. Wanneer de einddatum van timesheet wordt bereikt en u meer timesheets nodig hebt, moet u nieuwe degenen creëren.
author: Alina
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 0%

---

# Een timesheet voor eenmalig gebruik maken

U kunt manueel tot een enig-gebruik timesheet leiden als u een timesheet wilt die niet terugkeert. Wanneer de einddatum van timesheet wordt bereikt en u meer timesheets nodig hebt, moet u nieuwe degenen creëren.

Voor informatie over het creëren van een timesheet profiel dat terugkerende timesheets voor uw gebruikers zonder enige verdere interventie van u (geadviseerd) produceert, zie [Werkbladprofielen maken, bewerken en toewijzen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

>[!NOTE]
>
>* Tijdschema&#39;s voor eenmalig gebruik kunnen niet worden gemaakt voor groepen.

>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* Wanneer het creëren van enig-gebruik timesheet, kunt u geen specifieke algemene uurtypes selecteren om in uw timesheet te omvatten. Alle typen van algemene uren die in uw systeem worden geactiveerd, worden in handmatig gemaakte tijdbladen weergegeven.
>
>  Als u slechts bepaalde algemene uurtypes aan vertoning in uw timesheets wilt selecteren, gebruik een timesheet profiel. Voor meer informatie over timesheet-profielen raadpleegt u [Werkbladprofielen maken, bewerken en toewijzen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

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
   <td> <p>U moet administratieve toegang tot Timesheets hebben. </p> <p>Zie voor meer informatie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> <p><b> OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Een timesheet voor eenmalig gebruik maken

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront.

1. Klikken **Timesheets**. De **Alles** is standaard geselecteerd. Alle tijdbladen die u kunt bekijken, worden dan weergegeven.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Optioneel) Voer een van de volgende handelingen uit om het filter in de lijst met tijdbladen bij te werken:

   * Selecteren **Goedkeuringen van mijn tijdsplaat** in de rechterbovenhoek van de pagina om alleen de door u goedgekeurde tijdbladen weer te geven

      of

      Selecteren **Mijn tijdbladen** om alleen uw tijdbladen weer te geven.

      Dit past Mijn Goedkeuringen Timesheet of de Mijn filters Timesheet op de lijst van timesheets toe.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klik op het pictogram Filter ![](assets/filter-nwepng.png) om een ander filter toe te passen, of creeer nieuwe. Voor informatie over het maken of bijwerken van filters raadpleegt u [Filters maken of bewerken in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >De Mijn Goedkeuringen Timesheet en Mijn opties Timesheets tonen niet bij de bovenkant van timesheet lijst of in de lijst van filters als uw beheerder van Workfront of een groepsbeheerder de Mijn Goedkeuringen Timesheet en de Mijn filters van Timesheets van of de Controles van de Lijst in het gebied van de Opstelling of van uw Malplaatje van de Lay-out verwijderde. Zie de volgende artikelen voor meer informatie:
   > 
   >   * [Filters, weergaven en groepen aanpassen met een lay-outsjabloon](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)



1. (Optioneel) Klik op de knop **Zoeken** pictogram ![](assets/search-icon.png) om een sleutelwoord te typen en naar specifieke timesheet te zoeken. U kunt bijvoorbeeld zoeken naar een tijdlijntijdframe met de naam van de eigenaar.

1. (Optioneel) Klik op de knop **Weergave** ![](assets/view-icon.png) of **Groepering** ![](assets/grouping.png) pictogrammen om een andere weergave of groep toe te passen of om een nieuwe weergave of groep te maken.

   Zie de volgende artikelen voor informatie over het maken van filters, weergaven of groepen:

   * [Filters maken of bewerken in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Weergaven maken of bewerken in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Groepen maken in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Klikken **Nieuwe tijdpagina** boven aan de lijst van tijdbladen.

   Geef de volgende informatie op:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Tijdschema maken voor</strong> </td> 
      <td>Begin ingaand de naam van de gebruiker, een baanrol, of een team voor wie u timesheet creeert, en klik hen wanneer zij in de lijst tonen.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Begindatum</strong> </td> 
      <td>Dit is de begindatum van het tijdspad.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Einddatum</strong> </td> 
      <td> Dit is de einddatum van het tijdschema.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Fiatteurs</strong> </td> 
      <td>Approvers zijn gebruikers die timesheet voor de gebruikers goedkeuren verbonden aan timesheet. Alleen gebruikers met beheerdersrechten voor tijdschriften kunnen worden ingesteld als fiatteurs. Voor meer informatie over administratieve rechten op tijdspagina raadpleegt u <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.<br>Voer de namen van de fiatteurs van de tijdpagina in en klik op deze namen wanneer ze in de lijst worden weergegeven.<br>U kunt veelvoudige fiatteurs op een timesheet hebben. In dat geval wordt het tijdspad, nadat een van de fiatteurs het tijdsplaat heeft goedgekeurd, als volgt gemarkeerd <strong>Gesloten</strong> en verdwijnt uit de lijst van goedkeuringen volgens het tijdschema van alle resterende fiatteurs.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Kan tijd bewerken</strong> </td>

   <td> <p>Selecteer deze optie als fiatteurs de uren op het tijdblad mogen bewerken.</p>

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

   Nadat u een tijdspad ter goedkeuring hebt verzonden, kunt u de uren niet meer bewerken. Om een voorgelegde timesheet aan een editable staat terug te keren, wijs timesheet terug of hebben fiatteur de timesheet verwerpen. Zie voor meer informatie <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Een tijdschema ter goedkeuring indienen</a> en <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Een tijdschema goedkeuren</a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">Overwerk</span> </td> 
      <td>U kunt ervoor kiezen om het vak Overuren op het tijdblad te verbergen. Deze optie is standaard uitgeschakeld.</td> 
      </tr> 
      </tbody> 
   </table>

1. Klikken **Tijdschema maken**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## Wanneer taken en problemen worden weergegeven op de tijdbladen van de gebruiker

Een taak of een kwestie die aan een gebruiker wordt toegewezen verschijnt automatisch op timesheet van een gebruiker als de taak of de kwestie aan om het even welke volgende criteria voldoet:

* De gebruiker heeft uren op de taak of de kwestie het programma geopend
* De geplande datum van de taak of afgifte valt binnen het tijdschema
* De taak of kwestie heeft een Ware Datum van het Begin (de taak of de uitgiftestatus is lopend)
* De taak of kwestie wordt vastgezet aan timesheet
* De geplande datum van voltooiing valt binnen het datumbereik van het tijdschema en de status is bezig

Als de **Tijdopnamen vooraf invullen met ...** de voorkeuren (die u vindt in de voorkeuren voor Tijdsopgaven en uren) zijn uitgeschakeld. In het tijdvenster ziet u de problemen en taken met de status Bezig. Voor meer informatie over de voorkeuren voor tijdbladen en uren raadpleegt u [Voorkeuren voor tijdpagina&#39;s en uren configureren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
