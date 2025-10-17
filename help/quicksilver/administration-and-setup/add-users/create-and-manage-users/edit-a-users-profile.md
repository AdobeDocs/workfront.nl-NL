---
title: Gebruikersprofiel bewerken
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-beheerder kunt u nieuwe gebruikers maken en de profielen van bestaande gebruikers beheren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '3403'
ht-degree: 0%

---

# Gebruikersprofiel bewerken

{{highlighted-preview}}

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

Als Adobe Workfront-beheerder kunt u gebruikers maken en de profielen van bestaande gebruikers beheren. Voor informatie over het creëren van gebruikers, zie [&#x200B; gebruikers &#x200B;](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md) toevoegen.

Voor informatie over gebruikers die hun eigen profielen bijwerken, zie [&#x200B; mijn montages &#x200B;](/help/quicksilver/workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) vormen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>Het toegangsniveau voor systeembeheerders. </li> 
     <li> <p><b> Gebruikers </b> het plaatsen in uw toegangsniveau dat aan <b> wordt gevormd geeft </b> toegang uit, met <b> creeert </b> en minstens één van de twee <b> die gebruikers Admin </b> opties onder <b> worden toegelaten verfijnen uw montages </b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Van deze twee opties, als <b> Admin van de Gebruiker (de Gebruikers van de Groep) </b> wordt toegelaten, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een gebruikersprofiel bewerken

{{step-1-to-users}}

1. Selecteer de gebruiker, dan klik **uitgeven** pictogram ![&#x200B; pictogram &#x200B;](assets/edit-icon.png) uitgeeft.

   Het vak Gebruiker bewerken wordt weergegeven.

1. In **geef Gebruiker** doos uit, verander de informatie in om het even welke secties, en klik **sparen** op elk ogenblik.

### Persoonlijke gegevens

* **Voornaam**
* **Achternaam**

  >[!NOTE]
  >
  >Als u de naam van een gebruiker bewerkt in Workfront, wordt de naam van de gebruiker niet bewerkt in de Adobe Admin Console.

* **E-mailadres**: Het e-mailadres voor een gebruiker is ook hun gebruikersbenaming in Workfront. Dit veld is hoofdlettergevoelig en moet uniek zijn. Als een gebruiker drie keer probeert een niet-uniek e-mailadres toe te voegen binnen een venster van 10 minuten, wordt een reCAPTCHA-reactie weergegeven.

  Selecteer **ik ben geen robot** het plaatsen alvorens u kunt te werk gaan.

  Als u de e-maillijst van gewenste personen gebruikt en een e-maildomein invoert dat niet in de lijst voorkomt, ontvangt de gebruiker geen e-mailberichten. Voor meer informatie over de lijst van gewenste personen, zie [&#x200B; uw e-maillijst van gewenste personen &#x200B;](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md) vormen.

  Als uw organisatie naar de Adobe Admin Console is gemigreerd, kunt u het e-mailadres van een gebruiker niet bewerken in Workfront. Het e-mailadres van de gebruiker wordt ingesteld in de Adobe Admin Console.

* **Wachtwoord van de Verandering**: Klik deze knoop om het wachtwoord van de gebruiker terug te stellen. U moet uw eigen wachtwoord invoeren voordat u het wachtwoord van een andere gebruiker opnieuw kunt instellen.

  Als u het wachtwoord van een andere gebruiker opnieuw wilt instellen, moet u een Workfront-beheerder of een groepsbeheerder zijn.

  Als u een groepsbeheerder bent, kunt u wachtwoorden slechts voor gebruikers in de groepen terugstellen waar u als beheerder wordt aangewezen. Ook, moet de toestemming van Admin van de Gebruiker (de Gebruikers van de Groep) op uw toegangsniveau worden toegelaten:

  ![&#x200B; het toegangsniveau dat van Admin van de Gebruiker &#x200B;](assets/group-admin-user.png) plaatst

  Deze instelling is standaard uitgeschakeld. Voor meer informatie, zie [&#x200B; tot douanetoegangsniveaus &#x200B;](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.

  U kunt het wachtwoord van een Workfront-beheerder niet opnieuw instellen.

* **&lt;SSO Configuration> Gebruikersnaam**: Als uw Workfront-beheerder een SSO-integratie met Workfront heeft ingeschakeld, wordt de SSO-gebruikersnaam in dit veld weergegeven. Het type SSO-configuratie dat voor uw Workfront-instantie is ingeschakeld, is zichtbaar in dit veld.
* **OnlyAllow &lt;SSO Configuration> Authentificatie**: Als uw beheerder van Workfront een integratie SSO met Workfront toeliet en alle gebruikers voor SSO heeft bijgewerkt, wordt dit gebied geselecteerd door gebrek. Het type SSO-configuratie dat voor uw Workfront-instantie is ingeschakeld, is zichtbaar in dit veld.

  Wanneer dit veld is geselecteerd, moet de gebruiker zich bij Workfront aanmelden met de SSO-gegevens. Als deze optie wordt uitgeschakeld, kunnen ze zich met hun Workfront-gegevens aanmelden bij Workfront.

  Voor meer informatie over het vormen van Workfront met een oplossing SSO, zie [&#x200B; Overzicht van enig teken-op in Adobe Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

  Voor meer informatie over het bijwerken van gebruikers voor SSO, zie [&#x200B; de gebruikers van de Update voor enig teken-op &#x200B;](/help/quicksilver/administration-and-setup/add-users/single-sign-on/update-users-sso.md).

  >[!NOTE]
  >
  >Als u een groepsbeheerder bent, kunt u de &lt;SSO Configuration> gebieden slechts voor gebruikers in de groepen uitgeven waar u als dusdanig wordt aangewezen. Ook, moet de toestemming van Admin van de Gebruiker (de Gebruikers van de Groep) op uw toegangsniveau worden toegelaten.
  >
  >Als u een groepsbeheerder bent en u de toestemming van de Gebruiker Admin (Alle Gebruikers) op uw toegangsniveau wordt toegelaten, kunt u de &lt;SSO Configuratie> gebieden voor alle gebruikers uitgeven.

* **de foto van het Profiel**: Klik **uploaden nieuw** om het het profielbeeld van de gebruiker te laden. U kunt een JPG-, GIF- of PNG-bestand uploaden. De maximale bestandsgrootte is 4 MB.

  Het profielbeeld wordt de avatar van de gebruiker en het is zichtbaar door het systeem van Workfront, waar de naam van de gebruiker wordt getoond.

* **Info van de Baan**: Informatie over de baan, als de baantitel (op het **gebied van de Titel**), en welk gebied van deskundigheid de gebruiker verantwoordelijk is (in het **Bespreking aan me over** gebied).
* **Info van het Contact**: Het de telefoonaantal van de gebruiker (in het **aantal van de Telefoon**, **Uitgang.**, en **Mobiel aantal** gebieden) en adres (in het **Adres**, **Stad**, **Staat**, **Postcode**, en **Land** gebieden).

  Als de gebruiker voor het Verenigde Beheer van de Gebruiker (UUM) of het Systeem van Adobe Identity Management (IMS) wordt toegelaten, keurt het **gebied van het Land** in de sectie van Info van het Contact slechts landcodewaarden (bijvoorbeeld, V.S., GB, IN) goed.

### Voorkeuren

* **Zone van de Tijd**: De tijdzone van de gebruiker.

  Voor informatie over het helpen van gebruikers samenwerken in Workfront over tijdzones, zie [&#x200B; Werkend over tijdzones &#x200B;](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

* **Landinstelling E-mail**: De aangewezen e-maillandinstelling van de gebruiker. Dit is van invloed op de notatie van getallen en datums in de e-mails die van Workfront naar deze gebruiker komen.

  >[!NOTE]
  >
  >Wanneer uw organisatie zich op de Adobe Unified Experience bevindt, worden de taalvoorkeuren van de gebruiker opgeslagen in het Adobe-profiel en wordt de e-maillandinstelling niet gebruikt. Voor informatie over de toegang tot van deze voorkeur, zie [&#x200B; Adobe Verenigde Ervaring voor Workfront &#x200B;](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* **ontvangt e-mails van dit testmilieu**: Controleer deze optie als u e-mailberichten van het milieu wilt ontvangen dat u momenteel het programma wordt geopend.

  >[!NOTE]
  >
  >Deze optie is alleen beschikbaar in de omgeving van Voorvertoning en Sandbox. E-mailmeldingen zijn standaard ingeschakeld in de productieomgeving.

* **plaatst automatisch de taakstatus aan Bezig wanneer de taken zelf-toegewezen** zijn: Wanneer deze optie wordt geselecteerd, het werk dat de gebruiker zelf-wijst automatisch aan Bezig status in plaats van Nieuw wordt geplaatst.

* **produceert automatisch proeven wanneer het uploaden van documenten**: Controle deze optie als u de documenten wilt die de gebruiker uploadt om een proef onmiddellijk te produceren.

### Meldingen

Selecteer de e-mailmeldingen die voor de nieuwe gebruiker moeten worden ingeschakeld.

U kunt zowel expresberichten als dagelijkse samenvattingsmeldingen selecteren.

Voor meer informatie, zie [&#x200B; gebeurtenisberichten voor iedereen in het systeem &#x200B;](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md) vormen.

### Toegang

* **Gebruiker is actief**: Laat deze optie toe om erop te wijzen dat de gebruiker actief is. Actieve gebruikers gebruiken een Workfront-licentie. Als u het veld uitschakelt, wordt de gebruiker gedeactiveerd en wordt voorkomen dat deze zich aanmeldt bij Workfront.

* **Niveau van de Toegang**: Selecteer het toegangsniveau om aan deze gebruiker toe te wijzen.

  Wanneer u een toegangsniveau aan een gebruiker toewijst, kunt u een niveau gelijk aan of lager dan uw eigen toegangsniveau toewijzen. (Als uw toegangsniveau bijvoorbeeld Standaard is, kunt u het toegangsniveau voor beheerders niet toewijzen.)

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

* **Malplaatje van de Lay-out**: Kies een lay-outmalplaatje voor de gebruiker. Deze lay-outmalplaatje heeft belangrijkheid over om het even welk lay-outmalplaatje dat aan de Groep van het Huis van de gebruiker, het Team van het Huis, of Primaire Rol wordt toegewezen. Voor meer informatie over de taakprioriteit van lay-outmalplaatjes, zie [&#x200B; lay-outmalplaatjes &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) creëren en beheren.

  In de volgende lijst wordt beschreven hoe de lijst met sjablonen die u in dit veld hebt, afhankelijk is van uw toegang:

   * Als beheerder van Workfront, kunt u alle systeem-vlakke en groep-vlakke lay-outmalplaatjes zien.
   * Als groepsbeheerder, kunt u systeem-vlakke lay-outmalplaatje, evenals die zien verbonden aan de groepen die u beheert.
   * Als gebruiker met een Standard- of Plan-licentie en toegang om gebruikers te bewerken, kunt u alleen lay-outsjablonen op systeemniveau zien.

     Voor meer informatie over groep-vlakke lay-outmalplaatjes, zie [&#x200B; creëren en wijzigen de lay-outmalplaatjes van een groep &#x200B;](/help/quicksilver/administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

### Organisatie

* **Bedrijf**: Het bedrijf van de gebruiker. Gebruikers kunnen slechts met één bedrijf worden geassocieerd. U moet een bedrijf creëren alvorens u het met een gebruiker kunt associëren. Alleen actieve bedrijven worden in de lijst weergegeven. Voor informatie over het creëren van bedrijven, zie [&#x200B; bedrijven &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md) creëren en uitgeven.
* **Rapporten aan**: Als u een bedrijf voor de gebruiker specificeerde, kunt u de directe manager van de gebruiker op dit gebied ook specificeren. Een gebruiker kan slechts één manager hebben. Dit veld wordt niet weergegeven als de gebruiker niet eerst aan een bedrijf is gekoppeld.
* **Directe Rapporten**: Als u een bedrijf voor de gebruiker specificeerde, kunt u de directe rapporten van de gebruiker ook specificeren. Een gebruiker kan meerdere directe rapporten hebben. Dit veld wordt niet weergegeven als de gebruiker niet eerst aan een bedrijf is gekoppeld.
* **Team van het Huis**: Specificeer het huisteam voor de gebruiker. Gebruikers kunnen slechts één huisteam hebben. Het Team van het Huis is belangrijk wanneer het toewijzen van een lay-outmalplaatje of wanneer het bepalen van het Werk aan het knoop voor de taken en kwesties die aan de gebruiker worden toegewezen.
* **Andere Teams**: De gebruikers kunnen tot veelvoudige teams behoren. Een gebruiker kan werkitems bekijken die zijn toegewezen aan een van de teams in het thuisgebied.
* **Huidige Groep van het Huis**: Selecteer een aangewezen groep om de gebruiker toe te wijzen. Hierdoor heeft de gebruiker toegang tot objecten die met de groep worden gedeeld. U kunt lay-outsjablonen ook delen met de thuisgroep van de gebruiker.

  Dit is een verplicht veld. Elke gebruiker moet met een homegroep worden geassocieerd. Als u er geen selecteert, wordt de startgroep toegewezen als de startgroep van de nieuwe gebruiker.

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

* **Tijd van het Werk**: Vertegenwoordigt het percentage van de Volledige tijd Equivalente (FTE) tijd dat de gebruiker voor werkelijk werk, exclusief overheadkosten beschikbaar is. De Tijd van het werk moet een decimaal aantal tot 1 zijn, en het kan niet 0 zijn. Een beschikbaarheid van 20% voor werkelijk werk zou bijvoorbeeld 0,2 zijn.

  Het gebrek van het gebied is 1, erop wijzend dat een gebruiker hun volledige VTE op werkelijk besteedt, project-verwant werk.

  Het systeem gebruikt dit aantal om de beschikbaarheid van de gebruiker voor daadwerkelijke, op project betrekking hebbende werk te berekenen.

  Voor meer informatie over het creëren van programma&#39;s in Workfront, zie [&#x200B; een programma &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.

  De uitzonderingen van het programma en de onderbreking zouden de capaciteit van de gebruiker kunnen ook beïnvloeden.

  Workfront berekent de beschikbaarheid van een gebruiker afhankelijk van de voorkeuren voor het beheer van bronnen in uw installatiegebied. Voor meer informatie, zie [&#x200B; de voorkeur van het Beheer van het Middel &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md) vormen.

  >[!TIP]
  >
  >Plaats de waarde van de Tijd van het Werk aan 1 om erop te wijzen dat de gebruiker voor project-verwant werk hun volledig-tijdequivalent beschikbaar is.

* **plaats deactiveringsdatum**: Klik deze knoop als u deze gebruiker wilt plannen om op een bepaalde datum en op een bepaald tijdstip worden gedeactiveerd.
* **Datum van Deactivering**: De datum en de tijd waarop de gebruiker wordt gedeactiveerd. Voor informatie over het plannen van gebruikers voor deactivering, zie [&#x200B; gebruikers van het Programma voor deactivering &#x200B;](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation) in [&#x200B; Deactivate of een gebruiker &#x200B;](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) opnieuw activeren.
* **Primaire Rol**: Dit is de primaire baanrol die de gebruiker in Workfront kan vervullen. Elke taak en kwestie waaraan de gebruiker wordt toegewezen wordt ook toegewezen aan deze baanrol. Functies zijn essentieel voor het beheer van hulpbronnen. U kunt dit veld alleen bijwerken als u een Standard- of Plan-licentie hebt met beheerdersrechten voor gebruikers, of als u een Workfront-beheerder bent. Voor meer informatie over vestiging gebruikers met administratieve gebruikerstoegang, zie [&#x200B; Toegang van de Verlening tot gebruikers &#x200B;](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

  Alleen actieve taakrollen worden in de lijst weergegeven.

* (Voorwaardelijk) als u a **Primaire Rol** selecteerde, **Percentage van FTE het gebiedsvertoningen van de Beschikbaarheid**. Geef op welk percentage van de tijd van de planning van de gebruiker aan deze taakrol wordt toegewezen. De standaardwaarde voor het Percentage van de Beschikbaarheid van VTE voor de Primaire Rol is 100%.
* **Andere Rollen**: Een gebruiker kan veelvoudige baanrollen in Workfront hebben. Functies zijn essentieel voor het beheer van hulpbronnen. Er is geen limiet voor het aantal taakrollen dat een gebruiker kan uitvoeren. Nochtans, adviseren wij om één gebruiker aan een bovenmatig groot aantal baanrollen niet toe te wijzen, omdat het middelbeheer voor deze gebruikers te complex zou kunnen worden.

  Alleen actieve taakrollen worden in de lijst weergegeven. Voor meer informatie over baanrollen, zie [&#x200B; baanrollen &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md) creëren en beheren.

  U kunt dit veld alleen bijwerken als u een Standard- of Plan-licentie hebt met beheerdersrechten voor gebruikers, of als u een Workfront-beheerder bent.

  Voor meer informatie over vestiging gebruikers met administratieve gebruikerstoegang, zie [&#x200B; Toegang van de Verlening tot gebruikers &#x200B;](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

* (Voorwaardelijk) als u één of veelvoudige **Andere Rollen** selecteerde, **Percentage van FTE de gebiedsvertoningen van de Beschikbaarheid** voor elke rol. Geef op welk percentage van de tijd van de planning van de gebruiker wordt toegewezen aan elke taakrol. De standaardwaarde voor het Percentage van VTE Beschikbaarheid voor de Andere Rollen is 0%.

  Als Andere Rollen een Beschikbaarheid van 0% FTE hebben, tonen zij niet in de Planner van het Middel, tenzij de gebruikers aan taken in deze rollen worden toegewezen.

  ![&#x200B; de rollen van de Gebruiker en FTE &#x200B;](assets/user-roles-fte-2025.png)

  De som alle **Percentages van VTE Beschikbaarheid** voor alle rollen moet 100% gelijk zijn. Elk percentage van FTE Beschikbaarheid berekent de Beschikbare Uren voor elke rol per gebruiker in de Planner van het Middel. De beschikbare uren voor elke rol per gebruiker hangt van de beschikbare tijd voor de gebruiker af.

  De beschikbare tijd voor de gebruiker wordt door Workfront berekend afhankelijk van de methode die door de beheerder van Workfront is geselecteerd om FTE in de Voorkeur van het Beheer van het Middel te berekenen.

  Voor informatie over het berekenen van beschikbaarheid voor de gebruiker, zie [&#x200B; Overzicht van het berekenen van uren en FTE voor gebruikers en rollen in de Planner van het Middel &#x200B;](/help/quicksilver/resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

  Voor informatie over het vormen van de voorkeur van het Beheer van het Middel, zie [&#x200B; de voorkeur van het Beheer van het Middel &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md) vormen.

  <span class="preview"> (Optioneel) Datumeffectieve taakroltoewijzingen worden gebruikt in financiële berekeningen als de taakrol van de gebruiker tijdens een project verandert. </span>

  <span class="preview"> klik **bepaalt rollen door datum**, selecteert de **Primaire Rol** en **Andere Rollen**, en gaat het toewijzingspercentage voor elke rol in. De rollen zouden het zelfde als de bestaande rollen (gebruikend verschillende percentages), of nieuwe rollen kunnen zijn. Selecteer de begindatum wanneer deze rollen actief worden. Dit kan een datum in de toekomst zijn. Wanneer de nieuwste rollen actief worden, kunt u **klikken tonen vorige rollen** om de vorige, inactieve rollen te zien.</span>

* **Programma**: Associeer een programma met de gebruiker. Het programma van de gebruiker berekent de chronologie van de taken de gebruiker aan wordt toegewezen.

  U moet een schema creëren alvorens u het met een gebruiker kunt associëren. Voor meer informatie over het creëren van programma&#39;s, zie [&#x200B; een programma &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.

  >[!NOTE]
  >
  >Wij adviseren dat het programma u met de gebruiker associeert de tijdzone van de gebruiker aanpast.

  >[!IMPORTANT]
  >
  >Workfront gebruikt het programma van een gebruiker slechts wanneer de **Berekende Beschikbaarheid van het Middel die** plaatsen wordt geplaatst aan **het Programma van de Gebruiker**. Voor informatie over hoe dit het plaatsen beïnvloedt welk programma voor het Beheer van het Middel wordt gebruikt, zie [&#x200B; de voorkeur van het Beheer van het Middel &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md) vormen.

* **het Profiel van de Tijdopnemer**: Associeer een Profiel van de Tijdopnemer met de gebruiker om ervoor te zorgen dat timesheets automatisch voor de gebruiker produceren.

  De lijst met profielen die beschikbaar zijn in dit veld, is afhankelijk van uw toegang:

   * Als Workfront-beheerder kunt u alle tijdbladprofielen op systeemniveau en op groepsniveau zien.
   * Als groepsbeheerder, kunt u systeem-vlakke Profielen van de Chronologie, evenals die zien verbonden aan de groepen die u beheert.
   * Als gebruiker met een Standard- of Plan-licentie en toegang om gebruikers te bewerken, kunt u alleen tijdbladprofielen op systeemniveau zien. Voor meer informatie over groep-vlakke Profielen van de Chronologie, zie [&#x200B; creëren, uitgeven, en toewijzen timesheet profielen &#x200B;](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **het Type van Uur Standaard**: Selecteer het standaarduurtype voor de gebruiker. Dit is het uurtype dat door gebrek wordt gebruikt wanneer de gebruiker tijd registreert.
* **Beschikbare Types van Uur**: Selecteer de uurtypes die aan de gebruiker beschikbaar zouden moeten zijn. Deze uurtypen zijn overal zichtbaar in Workfront waar de gebruiker tijd kan registreren. Een gebruiker kan de uurtypes slechts zien die op het projectniveau evenals het gebruikersniveau worden toegelaten. Voor meer informatie over welke uurtypes aan gebruikers beschikbaar zijn, zie [&#x200B; de types en beschikbaarheid van uren bepalen &#x200B;](/help/quicksilver/timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
* **Tijd van het Logboek binnen**: Selecteer of de gebruiker tijd op het werkpunten in uren of dagen zou moeten registreren. Voor meer informatie, zie [&#x200B; vormen of de tijd uren of dagen &#x200B;](/help/quicksilver/timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md) het programma wordt geopend.
* **FTE**: Dit is het Volledige Gelijkwaardige van de Tijd van de gebruiker. Workfront gebruikt dit aantal om de beschikbaarheid van de gebruiker te berekenen die op het StandaardProgramma wordt gebaseerd slechts wanneer de Voorkeur van het Beheer van het Middel op het systeemniveau aan het StandaardProgramma wordt geplaatst.

  FTE wijst op de hoeveelheid tijd die de gebruiker op het werk kan doorbrengen. Dit omvat overheadkosten, evenals tijd die aan projectwerk wordt doorgebracht. Bijvoorbeeld, tijd die in vergaderingen wordt doorgebracht, of de opleiding is ook inbegrepen in FTE.

  De FTE moet een decimaal getal tot en met 1 zijn en mag niet 0 zijn. Als de FTE-waarde bijvoorbeeld 0,5 is en de standaardplanning in Workfront 40 uur, is de gebruiker 20 uur per week beschikbaar.

  De standaardwaarde van het veld is 1.

  De uitzonderingen van het programma, de onderbreking, en de waarde van de Tijd van het Werk kunnen de beschikbaarheid van de gebruiker beïnvloeden.

  Workfront berekent de beschikbaarheid van een gebruiker afhankelijk van de voorkeuren voor het beheer van bronnen in uw installatiegebied.

  Als de Voorkeur van het Beheer van het Middel op het systeemniveau aan het Programma van de Gebruiker wordt geplaatst, wordt de waarde u hier specificeert genegeerd en de gebruiker wordt beschouwd als beschikbaar volgens wat in hun programma wordt gespecificeerd.

  Voor meer informatie, zie [&#x200B; de voorkeur van het Beheer van het Middel &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md) vormen.

  Voor meer informatie over het creëren van programma&#39;s in Workfront, zie [&#x200B; een programma &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.

* **Pools van het Middel**: Vennoot de gebruiker met de Pools van het Middel. Voor meer informatie, zie [&#x200B; hulpmiddelpools met gebruikers &#x200B;](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md) associëren.
* **Tarief van Kosten**: De hoeveelheid kosten per uur voor de gebruiker.

  Voor datum efficiënte kostentarieven, klik **toevoegen Tarief**. Voer de waarde van de kostenvoet voor de tijdsperiode in en wijs zo nodig een begindatum en einddatum toe. Kostenpercentage 1 heeft geen begindatum en de laatste kostenvoet heeft geen einddatum.

  Sommige datums worden automatisch toegevoegd. Bijvoorbeeld, als Kostentarief 1 geen einddatum heeft, en u Kostentarief 2 met een begindatum van 1 mei 2023 toevoegt, wordt een einddatum van 30 april, 2023 toegevoegd aan Kostentarief 1 zodat geen hiaten bestaan.

* **het Factureren Tarief**: De hoeveelheid het factureren per uur voor de gebruiker.

  Voor datum daadwerkelijke het factureren tarieven, klik **voegt Tarief** toe. Voer de waarde van de factureringssnelheid voor de tijdsperiode in en wijs zo nodig een begindatum en einddatum toe. Factureringsgraad 1 zal geen begindatum hebben en het laatste factureringstarief zal geen einddatum hebben.

  Sommige datums worden automatisch toegevoegd. Bijvoorbeeld, als het Facturerings Tarief 1 geen einddatum heeft, en u voegt een tweede met een begindatum van 1 Mei, 2023 toe, wordt een einddatum van 30 April, 2023 toegevoegd aan het Facturerings Tarief 1 zodat geen hiaten bestaan.

  ![&#x200B; de kosten en het factureren van de Gebruiker tarieven &#x200B;](assets/user-cost-billing-rates-2025.png)

### Aangepaste Forms

Koppel een bestaand aangepast gebruikersformulier aan deze gebruiker. U moet een aangepast formulier maken voordat u het aan een gebruiker kunt koppelen. Alleen actieve aangepaste formulieren worden in de lijst weergegeven. Velden die u niet kunt bewerken, worden niet weergegeven in een afzonderlijk aangepast formulier.

>[!NOTE]
>
>Geavanceerde aangepaste formulierfuncties, zoals Externe opzoekvelden en eigen Workfront-velden, zijn alleen beschikbaar wanneer u de gebruikersrecord opent op de detailpagina en niet in het dialoogvenster Gebruiker bewerken. (Klik in de lijst met gebruikers op de gebruikersnaam om de details te openen.)

Voor informatie over het creëren van douaneformulieren, zie [&#x200B; een douaneformulier &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

### Opmerking

Typ de opmerking die u naar de gebruiker en naar het gedeelte Updates van het gebruikersprofiel wilt verzenden.

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Personal Info </td> 
      <td> 
       <ul> 
        <li><p><b>First Name</b></p></li>
        <li><p><b>Last Name</b></p><p><b>NOTE:</b></p><p>Editing a user's name in Workfront does not edit the user's name in the Adobe Admin Console.</p></li> 
        <li> <p><b>Email Address:</b> The email address for a user is also their username in Workfront. This field is case-sensitive and must be unique. If any user attempts to add a non-unique email address 3 times within a 10-minute window, a reCAPTCHA response appears.</p> <p> Select the <b>I am not a robot</b> setting before you can proceed.</p><p>If you use the email allowlist and enter an email domain not on the list, the user will not receive email notifications. For more information about the allowlist, see <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Configure your email allowlist</a>.</p><p>If your organization has been migrated to the Adobe Admin Console, you cannot edit a user's email address in Workfront. The user's email address is set in the Adobe Admin Console. </li> 
        <li> <p><b>Reset Password</b>: Click this link to reset the user's password. You must enter your own password before you can reset another user's password.</p> <p>To reset another user's password, you must be a Workfront administrator, or a group administrator.</p> <p><b>NOTE</b>:  
          <ul> 
           <li> <p>If you are a group administrator, you can reset passwords only for users in the groups where you are designated as an administrator. Also, the User Admin (Group Users) permission must be enabled in your access level:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>This setting is disabled by default. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </li> 
           <li> <p>You cannot reset the password of a Workfront administrator.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;SSO Configuration&gt; Username</b>: If your Workfront administrator enabled an SSO integration with Workfront, the SSO Username displays in this field. The type of SSO configuration enabled for your Workfront instance is visible in this field. </li> 
        <li> <p><b>OnlyAllow &lt;SSO Configuration&gt; Authentication</b>: If your Workfront administrator enabled an SSO integration with Workfront and has updated all users for SSO, this field is selected by default. The type of SSO configuration enabled for your Workfront instance is visible in this field.</p> <p>When this field is selected, the user is required to log into Workfront with their SSO credentials. Unchecking it will allow them to log in to Workfront with their Workfront credentials.</p> <p>For more information about configuring Workfront with an SSO solution, see <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Overview of single sign-on in Adobe Workfront</a></p> <p>For more information about updating users for SSO, see <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Update users for single sign-on</a>.</p> 
        <p><b>NOTE</b>:</p> 
        <p> If you are a group administrator, you can edit the &lt;SSO Configuration&gt; fields only for users in the groups where you are designated as such. Also, the User Admin (Group Users) permission must be enabled in your access level.
        <p>If you are a group administrator and you have the User Admin (All Users) permission enabled in your access level, you can edit the &lt;SSO Configuration&gt; fields for all users.</p> </li> 
        <li><b>Job Info:</b> Information about the job, like the job title (in the <b>Title</b> field), and what area of expertise the user is responsible for (in the <b>Talk to Me About</b> field).</li> 
        <li><p><b>Contact Info</b>: The user's phone number (in the <b>Phone number, Ext.</b>, and <b>Mobile number</b> fields) and address (in the <b>Address, City, State, Postal Code, Country</b> fields ).</p>
        <p>If the user is enabled for Unified User Management (UUM) or Adobe Identity Management System (IMS), the <b>Country</b> field in the Contact Info section only accepts country code values (for example, US, GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Preferences </td> 
      <td> 
       <ul> 
      <li> <p><b>Time Zone:</b> The user's time zone.</p> <p>For information about helping users collaborate in Workfront across time zones, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Working across time zones</a>.</p> </li>

      <li><p><b>Email Locale</b>: The user's preferred email locale. This affects the format of numbers and dates in the emails that come from Workfront to this user.</p>
      <p><b>NOTE:</b> When your organization is on the Adobe Unified Experience, the user's language preferences are stored in their Adobe profile and the email locale is not used. For information about accessing these preferences, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></li> 
      
      <li><b>Receive emails from this test environment</b>: Check this option if you want to receive email notifications from the environment that you are currently logged in.
      <p><b>NOTE</b></p>
      <p>This option is available only in the Preview and Sandbox environments. Email notifications are enabled in the Production environment by default. </p>
      </li> 
      
      </li> 
       <li><b>Send work I assign to myself to my Working On tab</b>: This setting refers to a deprecated feature that has been removed from Workfront.</li> 
       <li><b>Automatically generate proofs when uploading documents</b>: Check this option if you want the documents that the user uploads to immediately generate a proof. </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td> <p>Select the email notifications which should be enabled for the new user.</p> <p>You can select instant as well as daily digest notifications.</p> <p>For more information, see <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configure event notifications for everyone in the system</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access</td> 
      <td> 
       <ul> 
      <li><b>Is Active:</b> Select this box to indicate that the user is active. Active users use a Workfront license. Clearing the box deactivates the user and prevents them from logging in to Workfront.</li> 
       <li> <p><b>Access Level:</b> Select the access level to assign to this user.</p> 
       <p>When you assign an access level to a user, you can assign a level equal to or lower than your own access level.</p>
       <p>For example, if your access level is Plan, you cannot assign the Administrator access level. However, you cannot assign an access level that by default is lower than your own access level if the Workfront administrator has enabled non-default permissions on the access level that are not also enabled in your own access level. </p>
       <p>For example, if you have a Plan license with no access to delete tasks, you cannot assign someone a Work license with access to delete tasks, although the Work license is lower than the Plan license. For more information, see  <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> 
       <p>For more information about access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configure access to Adobe Workfront</a>.</p>
       <p> <b>NOTE:</b></p> 
       <p> If your organization uses the new access model (Standard/Light/Contributor), you cannot reassign a Standard or Light user to a Contributor access level if that user has already reached their decision limit for the month. </p><p>For more information on the new access model, see <a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">New access levels overview</a>. </p><p>For information on decision limits, see <a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">Limited document and proof decision for non-paid users overview</a>.</p></li> 
       <li> <p><b>Layout Template</b>: Choose a Layout Template for the user. This Layout Template takes precedence over any Layout Template assigned to the user's Home Group, Home Team or Primary Role. For more information about the assignment priority of Layout Templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> <p><b>NOTE</b>:  <p>The following list describes how the list of templates you have available in this field depends on your access:</p> 
       <ul> 
       <li>As a Workfront administrator, you can see all system-level and group-level Layout Templates.</li> 
       <li>As a group administrator, you can see system-level layout template, as well as those associated with the groups that you manage.</li> 
       <li>As a user with a Plan license and access to edit users, you can see only system-level Layout Templates.</li> 
       </ul> <p>For more information about group-level Layout Templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organization </td> 
      <td> 
       <ul> 
      <li><b>Company</b>: The company of the user. Users can be associated only with one company. You must create a company before you can associate it with a user. Only active companies display in the list. For information about creating companies, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Create and edit companies</a>.</li> 
      <li><b>Reports to:</b> If you specified a company for the user, you can also specify the direct manager of the user in this field. A user can have only one manager. This field does not display if the user is not associated with a company first. </li> 
      <li><b>Direct Reports:</b> If you specified a company for the user, you can also specify the direct reports of the user. A user can have multiple direct reports. This field does not display if the user is not associated with a company first.</li> 
      <li><b>Home Team</b>: Specify the home team for the user. Users can only have one home team. The Home Team is important when assigning a layout template or when defining the Work On It button for the tasks and issues assigned to the user. </li> 
      <li><b>Other Teams</b>: Users can belong to multiple teams. A user can view work items assigned to any of their teams in their Home area. </li> 
      <li> <p><b>Home Group:</b> Select an appropriate group to assign the user. This gives the user the ability to access objects that are shared with the group. You can also share layout templates with the user's Home Group.</p> <p>This is a required field. Every user must be associated with a home group. If you don't select one, your Home Group is assigned as the new user's Home Group.</p> <p><b>NOTE</b>:</p> 
      <p> You can assign a group to a user only if one of the following is true:</p>
      <ul><li>you are a Workfront administrator</li>
      <li>you are the administrator of the group</li>
      <li>the group is public.</li></ul> 
      <li> <p><b>Other Groups</b>: Users can belong to multiple groups. You can assign a group to a user only if you are a Workfront administrator, you are the administrator of the group, or the group is public.</p> <p><b>IMPORTANT</b>:</p> 
      <p>Adding a user to more than 100 groups may cause performance issues in any area of Workfront that loads the list of groups.</p> <p>For more information about public groups, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> <p>For more information about groups, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Planning </td> 
      <td> 
       <ul>
       <li>
       <b>Work Time</b>: Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.

      The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work.  

      The system uses this number to calculate the availability of the user for actual, project-related work. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.

      Schedule exceptions and time off might also affect the user's capacity. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      <b>TIP</b>

      Set the Work Time value to 1 to indicate that the user is available for project-related work their entire full-time equivalent.
      </li> 
      <li> <b>Schedule Deactivation</b>: Check this box if you want to schedule this user to be deactivated on a certain date and at a certain time. </li> 
       <li><b>Scheduled Deactivation Date</b>: The date and time on which the user becomes deactivated. For information about scheduling users for deactivation, see the <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schedule users for deactivation</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</li> 
       <li> <p><b>Primary Role</b>: This is the primary job role that the user can fulfill in Workfront. Every task and issue that the user is assigned to is also assigned to this job role. Job roles are essential in resource management. You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> <p>Only active job roles display in the list. </p> </li> 
       <li>If you selected a <b>Primary Role</b>, the <b>Percentage of FTE Availability</b> field displays. Specify what percentage of time of the user's schedule is allocated to this job role. The default value for the Percentage of FTE Availability for the Primary Role is 100%. </li> 
       <li> <p><b>Other Roles</b>: A user can have multiple job roles in Workfront. Job roles are essential in resource management. There is no limit for how many job roles a user can fulfill. However, we recommend to not assign one user to an excessively large number of job roles, because resource management might become too complex for these users.<p>Only active job roles display in the list. For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. <br>For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li> <p>(Conditional) If you selected one or multiple <b>Other Roles</b>, the <b>Percentage of FTE Availability</b> field displays for each role. Specify what percentage of time of the user's schedule is allocated to each job role. The default value for the Percentage of FTE Availability for the Other Roles is 0%.</p> <p><b>NOTE</b>:  If Other Roles have a 0% FTE Availability, they do not display in the Resource Planner, unless the users are assigned to tasks in these roles.</p> <p> <img alt="user_settings_roles_and_dte_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>NOTE</b>: <p>The sum of all <b>Percentages of FTE Availability</b> for all roles must equal 100%. Each Percentage of FTE Availability calculates the Available Hours for each role per user in the Resource Planner. The Available Hours for each role per user depends on the available time for the user.</p> <p>The available time for the user is calculated by Workfront depending on the method that has been selected by the Workfront administrator to calculate the FTE in the Resource Management Preferences.</p> <p>For information about calculating availability for the user, see <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> <p>For information about configuring Resource Management preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </p>
       <span class="preview"><p>(Optional) Date effective job role assignments are used in financial calculations if the user's job role changes during a project.</p><p>Click <b>Define roles by date</b>, select the <b>Primary Role</b> and <b>Other Roles</b>, and enter the allocation percentage for each role. The roles could be the same as the existing roles (using different percentages), or new roles. Select the <b>Start date</b> when these roles become active. This can be a future date. When the newest roles become active, you can click <b>Show previous roles</b> to see the previous, inactive roles.</p> </li></span>
       <li> <p><b>Schedule</b>: Associate a schedule with the user. The schedule of the user calculates the timeline of the tasks the user is assigned to.</p> <p>You must create a schedule before you can associate it with a user. For more information about creating schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p><b>NOTE</b>: We recommend that the schedule you associate with the user matches the user's Time Zone.</p> </li> 
       <li> <p><b>Timesheet Profile</b>: Associate a Timesheet Profile with the user to ensure that timesheets generate automatically for the user.</p> <p><b>NOTE</b>:  The list of profiles you have available in this field depends on your access:
       <ul>
       <li>As a Workfront administrator, you can see all system-level and all group-level Timesheet Profiles.</li>
       <li>As a group administrator, you can see system-level Timesheet Profiles, as well as those associated with the groups that you manage.</li>
       <li>As a user with a Plan license and access to edit users, you can see only system-level Timesheet Profiles. For more information about group-level Timesheet Profiles, see <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Create, edit, and assign timesheet profiles</a>.</li>
      </ul></p> </li> 
       <li><b>Default Hour Type</b>: Select the default hour type for the user. This is the hour type that is used by default when the user logs time.</li> 
       <li><b>Available Hour Types</b>: Select the hour types that should be available to the user. These hour types are visible everywhere in Workfront where the user can log time. A user can only see the hour types that are enabled at the project level as well as the user level. For more information about what hour types are available to users, see <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Define hour types and availability</a>.</li> 
       <li><b>Log Time in:</b> Select whether the user should log time on work items in hours or days. For more information, see <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Configure whether time is logged in hours or days</a>.</li>
       
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
      
      <li><b>Resource Pools</b>: Associate the user with Resource Pools. For more information, see <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associate resource pools with users </a>.</li> 
      
      <li><b>Cost Rate</b>: The amount of cost per hour for the user.
      <p>For date effective cost rates, click <strong>Add Rate</strong>. Enter the value of the cost rate for the time period, and assign a Start Date and End Date as needed. Cost Rate 1 will not have a start date and the last cost rate will not have an end date.</p><p>Some dates are added automatically. For example, if Cost Rate 1 does not have an end date, and you add Cost Rate 2 with a start date of May 1, 2023, an end date of April 30, 2023 is added to Cost Rate 1 so that no gaps exist.</p></li> 
      
      <li><b>Billing Rate</b>: The amount of billing per hour for the user.
      <p>For date effective billing rates, click <strong>Add Rate</strong>. Enter the value of the billing rate for the time period, and assign a Start Date and End Date as needed. Billing Rate 1 will not have a start date and the last billing rate will not have an end date.</p> <p>Some dates are added automatically. For example, if Billing Rate 1 does not have an end date, and you add a second with a start date of May 1, 2023, an end date of April 30, 2023 is added to Billing Rate 1 so that no gaps exist.</p><p> <img alt="User cost and billing rates" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

      </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custom Forms</td> 
      <td><p>Associate an existing user custom form with this user. You must create a custom form before you can associate it with a user. Only active custom forms display in the list. Fields you do not have access to edit are not displayed in an individual custom form.</p> <p><strong>Note:</strong> Advanced custom form features such as External lookup fields and Workfront native fields are only available when you open the user record on the details page, not on the Edit User dialog. (From the list of users, click the user name to open the details.)</p> <p>For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md" class="MCXref xref">Create a custom form</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Comment</td> 
      <td>Type the comment you want to send to the users and to the Updates area of their user profiles.</td> 
     </tr> 
    </tbody> 
   </table>
-->
