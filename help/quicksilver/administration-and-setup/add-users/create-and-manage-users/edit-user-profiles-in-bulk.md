---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Gebruikersprofielen bulksgewijs bewerken
description: Als Adobe Workfront-beheerder kunt u gebruikersaccounts bulksgewijs bewerken.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: 1a81c1becfc0866b92dbd1358af23671e5302266
workflow-type: tm+mt
source-wordcount: '2610'
ht-degree: 0%

---

# Gebruikersprofielen bulksgewijs bewerken

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Bulk Upload Users](https://helpx.adobe.com/nl/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

Je kunt gebruikersaccounts bulksgewijs bewerken. Bij gebruikers die bulkbewerkingen uitvoeren, worden alleen de velden die u specifiek selecteert, bijgewerkt met dezelfde gegevens voor alle geselecteerde gebruikers. Alle andere velden die u niet selecteert, blijven gelijk voor elke afzonderlijke gebruiker, zelfs als deze voor elke gebruiker anders zijn.

>[!NOTE]
>
>* U kunt het gedeelte Persoonlijke gegevens van gebruikersprofielen niet in bulk bewerken, omdat deze gegevens uniek moeten zijn voor elke gebruiker.
>* Om de nauwkeurigheid van gegevens en optimale prestaties te garanderen, raden we u aan niet meer dan 2000 gebruikers tegelijk te selecteren voor een bulkbewerking.
>

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p><p>of</p><p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>Het toegangsniveau voor systeembeheerders. </li> 
     <li> <p><b> Gebruikers </b> het plaatsen in uw toegangsniveau dat aan <b> wordt gevormd geeft </b> toegang uit, met <b> creeert </b> en minstens één van de twee <b> die gebruikers Admin </b> opties onder <b> worden toegelaten verfijnen uw montages </b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Van deze twee opties, als <b> Admin van de Gebruiker (de Gebruikers van de Groep) </b> wordt toegelaten, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gebruikersaccounts bulksgewijs bewerken

{{step-1-to-users}}

1. Selecteer meer dan één gebruiker, dan klik **uitgeven** pictogram ![&#x200B; pictogram &#x200B;](assets/edit-icon.png) uitgeeft.

1. In **geef Gebruiker** doos uit, verander de informatie in om het even welke secties, en klik **sparen** op elk ogenblik.

### Voorkeuren

* **Zone van de Tijd**: De tijdzone van de gebruiker.

  Voor informatie over het helpen van gebruikers samenwerken in Workfront over tijdzones, zie [&#x200B; Werkend over tijdzones &#x200B;](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

* **Landinstelling E-mail**: De aangewezen e-maillandinstelling van de gebruiker. Dit is van invloed op de notatie van getallen en datums in de e-mails die van Workfront naar deze gebruiker komen.

  >[!NOTE]
  >
  >Wanneer uw organisatie zich op de Adobe Unified Experience bevindt, worden de taalvoorkeuren van de gebruiker opgeslagen in het Adobe-profiel en wordt de e-maillandinstelling niet gebruikt. Voor informatie over de toegang tot van deze voorkeur, zie [&#x200B; Adobe Verenigde Ervaring voor Workfront &#x200B;](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

### Meldingen

Selecteer de e-mailberichten die voor de gebruikers moeten worden ingeschakeld.

U kunt zowel expresberichten als dagelijkse samenvattingsmeldingen selecteren. Alle dagelijkse samenvattingsmeldingen worden ergens na hetzelfde tijdstip verzonden voor alle gebruikers die u hebt geselecteerd.

Voor meer informatie, zie [&#x200B; gebeurtenisberichten voor iedereen in het systeem &#x200B;](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md) vormen.

### Toegang

* **Gebruiker is actief**: Laat deze optie toe om erop te wijzen dat de gebruikers actief zijn. Actieve gebruikers gebruiken een Workfront-licentie. Als u het veld uitschakelt, worden de gebruikers gedeactiveerd en wordt voorkomen dat zij zich aanmelden bij Workfront.

* **Niveau van de Toegang**: Selecteer het toegangsniveau om aan deze gebruikers toe te wijzen. Alle gebruikers die u hebt geselecteerd, hebben hetzelfde toegangsniveau.

  Wanneer u een toegangsniveau aan gebruikers toewijst, kunt u een niveau gelijk aan of lager dan uw eigen toegangsniveau toewijzen. (Als uw toegangsniveau bijvoorbeeld Standaard is, kunt u het toegangsniveau voor beheerders niet toewijzen.)

  Nochtans, kunt u geen toegangsniveau toewijzen dat door gebrek lager is dan uw eigen toegangsniveau als de beheerder van Workfront niet-standaardtoestemmingen op het toegangsniveau heeft toegelaten die niet ook in uw eigen toegangsniveau worden toegelaten.

  Als u bijvoorbeeld een standaardlicentie hebt zonder toegang tot verwijderingstaken, kunt u geen licentie voor licht toewijzen met toegang tot verwijderingstaken, hoewel de licentie voor licht lager is dan de licentie Standaard. Voor meer informatie, zie [&#x200B; tot douanetoegangsniveaus &#x200B;](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.

  Voor meer informatie over toegangsniveaus, zie [&#x200B; toegang tot Adobe Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md) vormen.

  >[!NOTE]
  >
  >Als uw organisatie het nieuwe toegangsmodel (Norm/Licht/Medewerker) gebruikt, kunt u geen Standaard of Lichte gebruiker aan een niveau van de Toegang van de Medewerker opnieuw toewijzen als die gebruiker hun beslissingsgrens voor de maand reeds heeft bereikt.
  >
  >Voor meer informatie over het nieuwe toegangsmodel, zie [&#x200B; Nieuw overzicht van toegangsniveaus &#x200B;](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).
  >
  >Voor informatie over besluitvormingsgrenzen, zie [&#x200B; Beperkt document en bewijsbesluit voor niet-betaalde gebruikers overzicht &#x200B;](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

* **Malplaatje van de Lay-out**: Kies een lay-outmalplaatje voor de gebruikers. deze lay-outmalplaatje heeft belangrijkheid over om het even welk lay-outmalplaatje dat aan hun Groep van het Huis, Team van het Huis, of Primaire Rol wordt toegewezen. Voor meer informatie over de taakprioriteit van lay-outmalplaatjes, zie [&#x200B; lay-outmalplaatjes &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) creëren en beheren.

  In de volgende lijst wordt beschreven hoe de lijst met sjablonen die u in dit veld hebt, afhankelijk is van uw toegang:

   * Als beheerder van Workfront, kunt u alle systeem-vlakke en groep-vlakke lay-outmalplaatjes zien.
   * Als groepsbeheerder, kunt u systeem-vlakke lay-outmalplaatje, evenals die zien verbonden aan de groepen die u beheert.
   * Als gebruiker met een Standard- of Plan-licentie en toegang om gebruikers te bewerken, kunt u alleen lay-outsjablonen op systeemniveau zien.

     Voor meer informatie over groep-vlakke lay-outmalplaatjes, zie [&#x200B; creëren en wijzigen de lay-outmalplaatjes van een groep &#x200B;](/help/quicksilver/administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

### Organisatie

* **Bedrijf**: Het bedrijf van de gebruikers. Gebruikers kunnen slechts met één bedrijf worden geassocieerd. U moet een bedrijf creëren alvorens u het met een gebruiker kunt associëren. Alleen actieve bedrijven worden in de lijst weergegeven. Voor informatie over het creëren van bedrijven, zie [&#x200B; bedrijven &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md) creëren en uitgeven.
* **Team van het Huis**: Specificeer het huisteam voor de gebruikers. Gebruikers kunnen slechts één huisteam hebben.
* **Andere Teams**: De gebruikers kunnen tot veelvoudige teams behoren.
* **Huidige Groep van het Huis**: Selecteer een aangewezen groep om de gebruikers toe te wijzen. Dit geeft de gebruikers de capaciteit om tot voorwerpen toegang te hebben die met de groep worden gedeeld. U kunt lay-outmalplaatjes met een Groep van het Huis ook delen.

  Dit is een verplicht veld. Elke gebruiker moet met een homegroep worden geassocieerd. Als u geen selecteert, wordt uw Groep van het Huis toegewezen als Groep van het Huis.

  U kunt een groep alleen aan een gebruiker toewijzen als een van de volgende situaties true is:

   * u bent een Workfront-beheerder
   * u bent de beheerder van de groep
   * de groep is openbaar

* **Andere Groepen**: De gebruikers kunnen tot veelvoudige groepen behoren. U kunt een groep alleen aan een gebruiker toewijzen als u een Workfront-beheerder, de beheerder van de groep of de groep openbaar is.

  >[!IMPORTANT]
  >
  >Als u een gebruiker toevoegt aan meer dan 100 groepen, kunnen er prestatieproblemen optreden in elk gebied van Workfront dat de lijst met groepen laadt.

  Voor meer informatie over openbare groepen, zie [&#x200B; een groep &#x200B;](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) creëren.

  Voor meer informatie over groepen, zie [&#x200B; Overzicht van Groepen &#x200B;](/help/quicksilver/administration-and-setup/manage-groups/groups-overview/groups.md).

### Bronplanning

* **Tijd van het Werk**: Vertegenwoordigt het percentage van de Volledige tijd Equivalente (FTE) tijd dat de gebruikers voor werkelijk werk, exclusief overheadkosten beschikbaar zijn. De Tijd van het werk moet een decimaal aantal tot 1 zijn, en het kan niet 0 zijn. Een beschikbaarheid van 20% voor werkelijk werk zou bijvoorbeeld 0,2 zijn.

  Het gebrek van het gebied is 1, erop wijzend dat een gebruiker hun volledige VTE op werkelijk besteedt, project-verwant werk.

  Het systeem gebruikt dit aantal om de beschikbaarheid van de gebruiker voor daadwerkelijke, op project betrekking hebbende werk te berekenen.

  Voor meer informatie over het creëren van programma&#39;s in Workfront, zie [&#x200B; een programma &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.

  De uitzonderingen van het programma en de onderbreking zouden de capaciteit van de gebruiker kunnen ook beïnvloeden.

  Workfront berekent de beschikbaarheid van een gebruiker afhankelijk van de voorkeuren voor het beheer van bronnen in uw installatiegebied. Voor meer informatie, zie [&#x200B; de voorkeur van het Beheer van het Middel &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md) vormen.

  >[!TIP]
  >
  >Plaats de waarde van de Tijd van het Werk aan 1 om erop te wijzen dat de gebruiker voor project-verwant werk hun volledig-tijdequivalent beschikbaar is.

* **plaats deactiveringsdatum**: Klik deze knoop als u deze gebruikers wilt plannen om op een bepaalde datum en op een bepaald tijdstip worden gedeactiveerd.
* **Datum van Deactivering**: De datum en de tijd waarop de gebruikers worden gedeactiveerd. Voor informatie over het plannen van gebruikers voor deactivering, zie [&#x200B; gebruikers van het Programma voor deactivering &#x200B;](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation) in [&#x200B; Deactivate of een gebruiker &#x200B;](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) opnieuw activeren.
* **Primaire Rol**: Dit is de primaire baanrol die de gebruikers in Workfront kunnen vervullen. Elke taak en kwestie waaraan de gebruikers worden toegewezen wordt ook toegewezen aan deze baanrol. Functies zijn essentieel voor het beheer van hulpbronnen. U kunt dit veld alleen bijwerken als u een Standard- of Plan-licentie hebt met beheerdersrechten voor gebruikers, of als u een Workfront-beheerder bent. Voor meer informatie over vestiging gebruikers met administratieve gebruikerstoegang, zie [&#x200B; Toegang van de Verlening tot gebruikers &#x200B;](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

  Alleen actieve taakrollen worden in de lijst weergegeven.

* (Voorwaardelijk) als u a **Primaire Rol** selecteerde, **Percentage van FTE het gebiedsvertoningen van de Beschikbaarheid**. Geef op welk percentage van de tijd van de planningen van de gebruikers aan deze taakrol wordt toegewezen. De standaardwaarde voor het Percentage van de Beschikbaarheid van VTE voor de Primaire Rol is 100%.
* **Andere Rollen**: De gebruikers kunnen veelvoudige baanrollen in Workfront hebben. Functies zijn essentieel voor het beheer van hulpbronnen. Er is geen limiet voor het aantal taakrollen dat een gebruiker kan uitvoeren. Nochtans, adviseren wij om één gebruiker aan een bovenmatig groot aantal baanrollen niet toe te wijzen, omdat het middelbeheer voor deze gebruikers te complex zou kunnen worden.

  Alleen actieve taakrollen worden in de lijst weergegeven. Voor meer informatie over baanrollen, zie [&#x200B; baanrollen &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md) creëren en beheren.

  U kunt dit veld alleen bijwerken als u een Standard- of Plan-licentie hebt met beheerdersrechten voor gebruikers, of als u een Workfront-beheerder bent.

  Voor meer informatie over vestiging gebruikers met administratieve gebruikerstoegang, zie [&#x200B; Toegang van de Verlening tot gebruikers &#x200B;](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

* (Voorwaardelijk) als u één of veelvoudige **Andere Rollen** selecteerde, **Percentage van FTE de gebiedsvertoningen van de Beschikbaarheid** voor elke rol. Geef op welk percentage van de tijd van de planningen van de gebruikers wordt toegewezen aan elke taakrol. De standaardwaarde voor het Percentage van VTE Beschikbaarheid voor de Andere Rollen is 0%.

  Als Andere Rollen een Beschikbaarheid van 0% FTE hebben, tonen zij niet in de Planner van het Middel, tenzij de gebruikers aan taken in deze rollen worden toegewezen.

  De som alle **Percentages van VTE Beschikbaarheid** voor alle rollen moet 100% gelijk zijn. Elk percentage van FTE Beschikbaarheid berekent de Beschikbare Uren voor elke rol per gebruiker in de Planner van het Middel. De beschikbare uren voor elke rol per gebruiker hangt van de beschikbare tijd voor de gebruiker af.

  De beschikbare tijd voor de gebruiker wordt door Workfront berekend afhankelijk van de methode die door de beheerder van Workfront is geselecteerd om FTE in de Voorkeur van het Beheer van het Middel te berekenen.

  Voor informatie over het berekenen van beschikbaarheid voor de gebruiker, zie [&#x200B; Overzicht van het berekenen van uren en FTE voor gebruikers en rollen in de Planner van het Middel &#x200B;](/help/quicksilver/resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

  Voor informatie over het vormen van de voorkeur van het Beheer van het Middel, zie [&#x200B; de voorkeur van het Beheer van het Middel &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md) vormen.

* **Programma**: Verwante een programma met de gebruikers. Het programma van de gebruikers berekent de chronologie van de taken de gebruikers worden toegewezen aan.

  U moet een schema creëren alvorens u het met gebruikers kunt associëren. Voor meer informatie over het creëren van programma&#39;s, zie [&#x200B; een programma &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.

  >[!IMPORTANT]
  >
  >Workfront gebruikt het programma van een gebruiker slechts wanneer de **Berekende Beschikbaarheid van het Middel die** plaatsen wordt geplaatst aan **het Programma van de Gebruiker**. Voor informatie over hoe dit het plaatsen beïnvloedt welk programma voor het Beheer van het Middel wordt gebruikt, zie [&#x200B; de voorkeur van het Beheer van het Middel &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md) vormen.

* **het Profiel van de Tijdopnemer**: Associeer een Profiel van de Tijdopnemer met de gebruikers om ervoor te zorgen dat timesheets automatisch produceren.

  De lijst met profielen die beschikbaar zijn in dit veld, is afhankelijk van uw toegang:

   * Als Workfront-beheerder kunt u alle tijdbladprofielen op systeemniveau en op groepsniveau zien.
   * Als groepsbeheerder, kunt u systeem-vlakke Profielen van de Chronologie, evenals die zien verbonden aan de groepen die u beheert.
   * Als gebruiker met een Standard- of Plan-licentie en toegang om gebruikers te bewerken, kunt u alleen tijdbladprofielen op systeemniveau zien. Voor meer informatie over groep-vlakke Profielen van de Chronologie, zie [&#x200B; creëren, uitgeven, en toewijzen timesheet profielen &#x200B;](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **het Type van Uur Standaard**: Selecteer het standaarduurtype voor de gebruikers. Dit is het uurtype dat door gebrek wordt gebruikt wanneer de gebruikers tijd registreren.
* **Beschikbare Types van Uur**: Selecteer de uurtypes die aan de gebruikers beschikbaar zouden moeten zijn. Deze uurtypen zijn overal zichtbaar in Workfront waar de gebruikers de tijd kunnen registreren. De gebruikers kunnen de uurtypes slechts zien die op het projectniveau evenals het gebruikersniveau worden toegelaten. Voor meer informatie over welke uurtypes aan gebruikers beschikbaar zijn, zie [&#x200B; de types en beschikbaarheid van uren bepalen &#x200B;](/help/quicksilver/timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
* **FTE**: Dit is het Volledige Gelijkwaardige van de Tijd van de gebruikers. Workfront gebruikt dit aantal om de beschikbaarheid van de gebruikers te berekenen die op het StandaardProgramma slechts worden gebaseerd wanneer de Voorkeur van het Beheer van het Middel op het systeemniveau aan het StandaardProgramma wordt geplaatst.

  De FTE geeft de hoeveelheid tijd aan die de gebruikers op het werk kunnen doorbrengen. Dit omvat overheadkosten, evenals tijd die aan projectwerk wordt doorgebracht. Bijvoorbeeld, tijd die in vergaderingen wordt doorgebracht, of de opleiding is ook inbegrepen in FTE.

  De FTE moet een decimaal getal tot en met 1 zijn en mag niet 0 zijn. Als de FTE-waarde bijvoorbeeld 0,5 is en de standaardplanning in Workfront 40 uur, zijn de gebruikers 20 uur per week beschikbaar.

  De standaardwaarde van het veld is 1.

  De uitzonderingen van het programma, de onderbreking, en de waarde van de Tijd van het Werk kunnen de beschikbaarheid van de gebruikers beïnvloeden.

  Workfront berekent de beschikbaarheid van een gebruiker afhankelijk van de voorkeuren voor het beheer van bronnen in uw installatiegebied.

  Als de Voorkeur van het Beheer van het Middel op het systeemniveau aan het Programma van de Gebruiker wordt geplaatst, wordt de waarde u hier specificeert genegeerd en de gebruiker wordt beschouwd als beschikbaar volgens wat in hun programma wordt gespecificeerd.

  Voor meer informatie, zie [&#x200B; de voorkeur van het Beheer van het Middel &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md) vormen.

  Voor meer informatie over het creëren van programma&#39;s in Workfront, zie [&#x200B; een programma &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.

* **Pools van het Middel**: Vennoot de gebruikers met de Pools van het Middel.

  >[!NOTE]
  >
  >Alleen de bronnenpools die alle geselecteerde gebruikers gemeen hebben, worden in dit veld weergegeven. Als de geselecteerde gebruikers geen gedeelde bronnenpools hebben, is dit veld leeg. Als dit veld leeg is, overschrijven de hier opgegeven bronnenpools hun afzonderlijke bronnenpools.

  Voor meer informatie over middelpools, zie [&#x200B; het middelpools van de Vereniging met gebruikers &#x200B;](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

* **Tarief van Kosten**: De hoeveelheid kosten per uur voor de gebruiker.

  Voor datum efficiënte kostentarieven, klik **toevoegen Tarief**. Voer de waarde van de kostenvoet voor de tijdsperiode in en wijs zo nodig een begindatum en einddatum toe. Kostenpercentage 1 heeft geen begindatum en de laatste kostenvoet heeft geen einddatum.

  Sommige datums worden automatisch toegevoegd. Bijvoorbeeld, als Kostentarief 1 geen einddatum heeft, en u Kostentarief 2 met een begindatum van 1 mei 2023 toevoegt, wordt een einddatum van 30 april, 2023 toegevoegd aan Kostentarief 1 zodat geen hiaten bestaan.

* **het Factureren Tarief**: De hoeveelheid het factureren per uur voor de gebruiker.

  Voor datum daadwerkelijke het factureren tarieven, klik **voegt Tarief** toe. Voer de waarde van de factureringssnelheid voor de tijdsperiode in en wijs zo nodig een begindatum en einddatum toe. Factureringsgraad 1 zal geen begindatum hebben en het laatste factureringstarief zal geen einddatum hebben.

  Sommige datums worden automatisch toegevoegd. Bijvoorbeeld, als het Facturerings Tarief 1 geen einddatum heeft, en u voegt een tweede met een begindatum van 1 Mei, 2023 toe, wordt een einddatum van 30 April, 2023 toegevoegd aan het Facturerings Tarief 1 zodat geen hiaten bestaan.

### Aangepaste Forms

Koppel een bestaand aangepast gebruikersformulier aan de gebruikers. U moet een aangepast formulier maken voordat u het aan een gebruiker kunt koppelen. Alleen actieve aangepaste formulieren worden in de lijst weergegeven. Velden die u niet kunt bewerken, worden niet weergegeven in een afzonderlijk aangepast formulier.

>[!NOTE]
>
>Geavanceerde aangepaste formulierfuncties, zoals Externe opzoekvelden en eigen Workfront-velden, zijn alleen beschikbaar wanneer u de gebruikersrecord opent op de detailpagina en niet in het dialoogvenster Gebruiker bewerken. (Klik in de lijst met gebruikers op de gebruikersnaam om de details te openen.)

U kunt naar keuze selecteren **herberekent de optie van de Uitdrukkingen van de Douane** om ervoor te zorgen dat alle berekende douanegebieden in douaneformulieren die aan de geselecteerde gebruikers in bijlage zijn bijgewerkt zijn.

Voor informatie over het creëren van douaneformulieren, zie [&#x200B; een douaneformulier &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

### Opmerking

Typ de opmerking die u naar de gebruikers en naar het gedeelte Updates van hun gebruikersprofielen wilt verzenden.

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Preferences</td> 
      <td> 
       <ul> 
        <li><b>Time Zone:</b> The users' time zone.</li> 
        <li><b>Locale</b>: The users' preferred locale. This affects the format of numbers and dates in the emails that come from Workfront.</li> 
        <li><b>Send work I assign to myself to my Working On tab</b>: This setting refers to a deprecated feature that has been removed from Workfront.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td>Select the email notifications which should be enabled for the new user.<p>You can select instant as well as daily digest notifications. All the daily digest notifications are delivered sometime after the same time for all the users selected. For more information, see <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configure event notifications for everyone in the system</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access</td> 
      <td> 
       <ul> 
        <li><b>Is Active:</b> Select this field to indicate whether the users are active. Active users use a Workfront license. Deselecting the field deactivates the users.</li> 
        <li> 
        <p><b>Access Level:</b> Select the access level to assign to these users. All users selected will have the same access level.
        </p> 
        <p>When you assign an access level to users, you can assign a level equal to or less than your own access level. (For example, if your access level is Planner, you cannot assign the Administrator access level.) </p>
        <p>However, you cannot assign an access level that is lower than your own if the Workfront administrator has enabled permissions on the access level that are not also enabled in your own (via the Fine-Tune settings, as described in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>).</p> 
        <p>For more information about access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configure access to Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Layout Template</b>: Choose a layout template for the users. The layout template assigned to the users will take precedence over any layout template assigned to their Home Group, Home Team or primary job role. For more information about the assignment priority of layout template, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> 
        <p><b>NOTE</b>:  The list of layout templates you have available in this field depends on your access:
          <ul>
           <li>As a Workfront administrator, you can see all system-level and group-level layout templates.</li>
           <li>As a group administrator, you can see system-level layout templates, as well as those associated with the groups that you manage.</li>
           <li><p>As a user with a Planner license and access to edit users, you can see only system-level layout templates. </p>
           <p>For information about group-level layout templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organization</td> 
      <td> 
       <ul> 
        <li><b>Company</b>: The company of the users. Users can be associated only with one company. You must create a company before you can associate it with a user. Only active companies display in the list. For information about creating companies, see Understanding and Managing Companies.</li> 
        <li><b>Home Team</b>: Specify the home team for the users. Users can only have one home team. </li> 
        <li><b>Other Teams</b>: Users can belong to multiple teams. </li> 
        <li> <p><b>Home Group:</b> Select an appropriate group to assign the users as their Home Group. This gives the user the ability to access objects that are shared with the group.</p> <p><b>NOTE</b>:  This is a required field. You cannot have users not associated with a Home Group.</p> <p>You can assign a group to users only in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li>The group is public.</li> 
         </ul> </li> 
        <li> <p><b>Other Groups</b>: Users can belong to multiple groups. You can assign a group to a user only  in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li> <p>The group is public. </p> 
          <p>For more information about public groups, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> 
          <p>For more information about groups, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Planning</td> 
      <td> 
       <ul> 
      
      <li>
       <b>Work Time</b>: Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.

      The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work. 

      The system uses this number to calculate the availability of the user for actual, project-related work. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.

      Schedule exceptions and time off might also affect the user capacity. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      <b>TIP</b>

      Set the Work Time value to  1 to indicate that the user is available for project-related work their entire full-time equivalent.
      </li> 

      <li><b>Schedule Deactivation</b>: Check this box if you want to schedule users to be deactivated after a period of time.</li> 
       <li><b>Scheduled Deactivation Date</b>: The date after which the users become deactivated. For more information about scheduling users for deactivation, see the section <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schedule users for deactivation</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</li> 
       <li> <p><b>Primary Role</b>: This is the primary job role that a user has in Workfront. Every task and issue that the users are assigned to is also assigned to this job role, by default. Job roles are essential in resource management. For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a></p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li>(Conditional) If you selected a <b>Primary Role</b>, the <b>Percentage of FTE Availability</b> field displays. Specify what percentage of time of the users' schedules is allocated to this job role. The default value for the Percentage of FTE Availability for the Primary Role is 100%.</li> 
       <li> <p><b>Other Roles</b>: Users can have multiple job roles in Workfront. Job roles are essential in resource management. There is no limit for how many job roles a user can fulfill. However, we recommend to not assign one user to an excessively large number of job roles, because resource management might become too complex for these users.</p> <p>For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li> <p>(Conditional) If you selected one or multiple <b>Other Roles</b>, the <b>Percentage of FTE Availability</b> field displays for each role. Specify what percentage of time of the users' schedules is allocated to each job role. The default value for the Percentage of FTE Availability for the Other Roles is 0%.</p> <p><b>NOTE</b>:  
       <ul> 
       <li>If Other Roles have a 0% FTE Availability, they do not display in the Resource Planner, unless the users are assigned to tasks in these roles.</li> 
       <li> <p>The sum of all Percentages of FTE Availability for all roles must equal 100%. Each Percentage of FTE Availability calculates the Available Hours for each role per user in the Resource Planner. The Available Hours for each role per user depends on the available time for the user.</p> <p>The available time for the user is calculated by Workfront depending on the method that has been selected by the Workfront administrator to calculate the FTE in the Resource Management Preferences.</p> <p>For more information about calculating availability for the user, see <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> <p>For more information about configuring Resource Management preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Schedule</b>: Associate a schedule with the users. The schedule of the users calculates the timeline of the tasks the users are assigned to.</p> <p>A Workfront administrator or a group administrator must create a schedule before it can be associated with users.</p> <p>Select a system-level or a group schedule to assign it to the selected users.</p> <p>For more information about system-level and group schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p><b>IMPORTANT</b>: Workfront uses the schedule of a user only when the Calculate Resource Availability Using setting is set to The User's Schedule. For information about how the Calculate Resource Availability Using setting affects which schedule is used for Resource Management, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       <li> <p><b>Timesheet Profile</b>: Associate a Timesheet Profile with the users. This ensures that timesheets generate automatically for the users.</p> 
       <p><b>NOTE</b>:  
       <ul> 
       <li>The list of timesheet profiles you have available in this field depends on your access:
       <ul>
       <li>As a Workfront administrator, you can see all system-level and group-level timesheet profiles.</li>
       <li><p>As a group administrator, you can see system-level timesheet profiles, as well as those associated with the groups that you manage.</p></li>
       <li><p>As a user with a Planner license and access to edit users, you can see only system-level timesheet profiles.</p></li>
       </ul></li> 
       <li>If you are a group administrator, all of the users you are editing must be members of a group that you administer.</li> 
       </ul> </p> </li> 
       <li><b>Default Hour Type</b>: Select the default hour type for the users. This is the hour type that is used by default when the users log time.</li> 
       <li> <p><b>Available Hour Types</b>: Select the hour types that should be available to the user. These hour types are visible everywhere in Workfront where the users can log time. A user can only see the hour types that are enabled at the project level as well as the user level.</p> 
       <p>For more information about what hour types are available to users, see <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Define hour types and availability</a>.</p> 
       </li> 
       <li> <b>FTE</b>: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. 

      <p>The FTE indicates the amount of time that the user can spend at work. This includes overhead, as well as time spent on project work. For example, time that is spent in meetings, or training is also included in the FTE.</p> 

      The FTE must be a decimal number up to 1, and it cannot be 0. For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

      The field's default is 1.

      Schedule exceptions, time off might, and the value of Work Time may affect the availability of the user. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area.

      If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

      For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.
      </li> 
       <li> <p><b>Resource Pools</b>: Associate the users with resource pools.</p> <p><b>NOTE</b>:  Only the resource pools that are common to all the users selected appear in this field. If the users selected have no shared resource pools, this field is empty. If this field is empty, the resource pools you specify here will overwrite their individual resource pools.</p> 
       <p>For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> </li> 
       <li><b>Cost Per Hour</b>: The amount of cost per hour for the user. </li> 
       <li><b>Billing Per Hour</b>: The amount of billing per hour for the user.</li> 
       <li><b>Custom Forms</b>: Associate an existing user custom form with the users. You must create a custom form before you can associate it with a user. Only active custom forms display in the list. For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>.</li> 
       <li><b>Comment</b>: Enter a comment in the field provided. All users selected will receive an in-app notification as well as an email notification with your comment. The comment shows in the Updates tab of the users' profile.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
-->

