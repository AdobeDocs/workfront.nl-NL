---
title: Gebruikersprofiel bewerken
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-beheerder kunt u nieuwe gebruikers maken en de profielen van bestaande gebruikers beheren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '3264'
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

Als Adobe Workfront-beheerder kunt u gebruikers maken en de profielen van bestaande gebruikers beheren. Voor informatie over het creëren van gebruikers, zie [ gebruikers ](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md) toevoegen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

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

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een gebruikersprofiel bewerken

{{step-1-to-users}}

1. Selecteer de gebruiker, dan klik **uitgeven** pictogram ![](assets/edit-icon.png).

   Het vak Gebruiker bewerken wordt weergegeven.

1. In **geef Gebruiker** doos uit, verander om het even welke volgende informatie, en klik **sparen Veranderingen** op elk ogenblik:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Persoonlijke gegevens </td> 
      <td> 
       <ul> 
        <li><p><b>Voornaam</b></p></li>
        <li><p><b>Achternaam</b></p></li> 
        <li> <p><b> E-mailadres:</b> het e-mailadres voor een gebruiker is ook hun gebruikersbenaming in Workfront. Dit veld is hoofdlettergevoelig en moet uniek zijn. Als een gebruiker drie keer probeert een niet-uniek e-mailadres toe te voegen binnen een venster van 10 minuten, wordt een reCAPTCHA-reactie weergegeven.</p> <p> Selecteer <b> ik ben geen robot </b> het plaatsen alvorens u kunt te werk gaan.</p><p>Als u de e-maillijst van gewenste personen gebruikt en een e-maildomein invoert dat niet in de lijst voorkomt, ontvangt de gebruiker geen e-mailberichten. Voor meer informatie over de lijst van gewenste personen, zie <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref"> uw e-maillijst van gewenste personen </a> vormen.</p> </li> 
        <li> <p><b> Wachtwoord van het Terugstellen </b>: Klik deze verbinding om het wachtwoord van de gebruiker terug te stellen. U moet uw eigen wachtwoord invoeren voordat u het wachtwoord van een andere gebruiker opnieuw kunt instellen.</p> <p>Als u het wachtwoord van een andere gebruiker opnieuw wilt instellen, moet u een Workfront-beheerder of een groepsbeheerder zijn.</p> <p><b> NOTA </b>:  
          <ul> 
           <li> <p>Als u een groepsbeheerder bent, kunt u wachtwoorden slechts voor gebruikers in de groepen terugstellen waar u als beheerder wordt aangewezen. Ook, moet de toestemming van Admin van de Gebruiker (de Gebruikers van de Groep) op uw toegangsniveau worden toegelaten:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>Deze instelling is standaard uitgeschakeld. Voor meer informatie, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </li> 
           <li> <p>U kunt het wachtwoord van een Workfront-beheerder niet opnieuw instellen.</p> </li> 
          </ul> </p> </li> 
        <li><b> &lt;SSO Configuration&gt; Gebruikersnaam </b>: Als uw Workfront-beheerder een SSO-integratie met Workfront heeft ingeschakeld, wordt de SSO-gebruikersnaam in dit veld weergegeven. Het type SSO-configuratie dat voor uw Workfront-instantie is ingeschakeld, is zichtbaar in dit veld. </li> 
        <li> <p><b> OnlyAllow &lt;SSO Configuration&gt; Authentificatie </b>: Als uw beheerder van Workfront een integratie SSO met Workfront toeliet en alle gebruikers voor SSO heeft bijgewerkt, wordt dit gebied geselecteerd door gebrek. Het type SSO-configuratie dat voor uw Workfront-instantie is ingeschakeld, is zichtbaar in dit veld.</p> <p>Wanneer dit veld is geselecteerd, moet de gebruiker zich bij Workfront aanmelden met de SSO-gegevens. Als deze optie wordt uitgeschakeld, kunnen ze zich met hun Workfront-gegevens aanmelden bij Workfront.</p> <p>Voor meer informatie over het vormen van Workfront met een oplossing SSO, zie <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref"> Overzicht van enig teken-op in Adobe Workfront </a></p> <p>Voor meer informatie over het bijwerken van gebruikers voor SSO, zie <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref"> de gebruikers van de Update voor enig teken-op </a>.</p> 
        <p><b> NOTA </b>:</p> 
        <p> Als u een groepsbeheerder bent, kunt u de &lt;SSO Configuration&gt; gebieden slechts voor gebruikers in de groepen uitgeven waar u als dusdanig wordt aangewezen. Ook, moet de toestemming van Admin van de Gebruiker (de Gebruikers van de Groep) op uw toegangsniveau worden toegelaten.
        <p>Als u een groepsbeheerder bent en u de toestemming van de Gebruiker Admin (Alle Gebruikers) op uw toegangsniveau wordt toegelaten, kunt u de &lt;SSO Configuratie&gt; gebieden voor alle gebruikers uitgeven.</p> </li> 
        <li><b> Info van de Baan:</b> Informatie over de baan, als de baantitel (op het <b> gebied van de Titel </b>), en welk gebied van deskundigheid de gebruiker verantwoordelijk is (in het <b> Bespreking aan me over </b> gebied).</li> 
        <li><p><b> Info van het Contact </b>: Het de telefoonaantal van de gebruiker (in het <b> aantal van de Telefoon, Ext.</b>, en <b> Mobiel aantal </b> gebieden) en adres (in het <b> Adres, Stad, Staat, Postcode, Land </b> gebieden).</p>
        <p>Als de gebruiker voor het Verenigde Beheer van de Gebruiker (UUM) of het Systeem van Identity Management van de Adobe (IMS) wordt toegelaten, keurt het </b> gebied van het Land <b> in de sectie van het Info van het Contact slechts landcodewaarden (bijvoorbeeld, US, GB, IN) goed.</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Voorkeuren </td> 
      <td> 
       <ul> 
      <li> <p><b> Tijdzone van de Tijd:</b> de tijdzone van de gebruiker.</p> <p>Voor informatie over het helpen van gebruikers samenwerken in Workfront over tijdzones, zie <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref"> Werkend over tijdzones </a>.</p> </li>

   <li><p><b> Landinstelling E-mail </b>: De aangewezen e-maillandinstelling van de gebruiker. Dit is van invloed op de notatie van getallen en datums in de e-mails die van Workfront naar deze gebruiker komen.</p>
      <p><b> NOTA:</b> wanneer uw organisatie op de Adobe Verenigde Ervaring is, worden de de taalvoorkeur van de gebruiker opgeslagen in hun profiel van de Adobe en e-mailscène wordt niet gebruikt. Voor informatie over de toegang tot van deze voorkeur, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>.</p></li>

   <li><b> ontvangt e-mails van dit testmilieu </b>: Controleer deze optie als u e-mailberichten van het milieu wilt ontvangen dat u momenteel het programma wordt geopend.
      <p><b>OPMERKING</b></p>
      <p>Deze optie is alleen beschikbaar in de omgeving van Voorvertoning en Sandbox. E-mailmeldingen zijn standaard ingeschakeld in de productieomgeving. </p>
      </li>

   </li> 
       <li><b> verzend het werk ik aan mezelf toewijs aan mijn het Werken op lusje </b>: Dit het plaatsen verwijst naar een verouderde eigenschap die uit Workfront is verwijderd.</li> 
       <li><b> produceert automatisch proeven wanneer het uploaden van documenten </b>: Controle deze optie als u de documenten wilt die de gebruiker uploadt om een proef onmiddellijk te produceren. </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Meldingen</td> 
      <td> <p>Selecteer de e-mailberichten die moeten worden ingeschakeld voor de nieuwe gebruiker.</p> <p>U kunt zowel expresberichten als dagelijkse samenvattingsmeldingen selecteren.</p> <p>Voor meer informatie, zie <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref"> gebeurtenisberichten voor iedereen in het systeem </a> vormen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Toegang</td> 
      <td> 
       <ul> 
      <li><b> is Actief:</b> selecteer dit vakje om erop te wijzen dat de gebruiker actief is. Actieve gebruikers gebruiken een Workfront-licentie. Als u de doos wist, wordt de gebruiker gedeactiveerd en wordt voorkomen dat deze zich aanmeldt bij Workfront.</li> 
       <li> <p><b> Niveau van de Toegang:</b> selecteer het toegangsniveau om aan deze gebruiker toe te wijzen.</p> 
       <p>Wanneer u een toegangsniveau aan een gebruiker toewijst, kunt u een niveau gelijk aan of lager dan uw eigen toegangsniveau toewijzen.</p>
       <p>Bijvoorbeeld, als uw toegangsniveau Plan is, kunt u niet het de toegangsniveau van de Beheerder toewijzen. Nochtans, kunt u geen toegangsniveau toewijzen dat door gebrek lager is dan uw eigen toegangsniveau als de beheerder van Workfront niet-standaardtoestemmingen op het toegangsniveau heeft toegelaten die niet ook in uw eigen toegangsniveau worden toegelaten. </p>
       <p>Bijvoorbeeld, als u een vergunning van het Plan zonder toegang hebt om taken te schrappen, kunt u niet iemand een vergunning van het Werk met toegang toewijzen om taken te schrappen, hoewel de vergunning van het Werk lager is dan de vergunning van het Plan. Voor meer informatie, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen. </p> 
       <p>Voor meer informatie over toegangsniveaus, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref"> toegang tot Adobe Workfront </a> vormen.</p>
       <p> <b> NOTA:</b></p> 
       <p> Als uw organisatie het nieuwe toegangsmodel (Norm/Licht/Medewerker) gebruikt, kunt u geen Standaard of Lichte gebruiker aan een niveau van de Toegang van de Medewerker opnieuw toewijzen als die gebruiker hun beslissingsgrens voor de maand reeds heeft bereikt. </p><p>Voor meer informatie over het nieuwe toegangsmodel, zie <a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref"> Nieuw overzicht van toegangsniveaus </a>. </p><p>Voor informatie over besluitvormingsgrenzen, zie <a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref"> Beperkt document en bewijsbesluit voor niet-betaalde gebruikers overzicht </a>.</p></li> 
       <li> <p><b> Malplaatje van de Lay-out </b>: Kies een Malplaatje van de Lay-out voor de gebruiker. Deze lay-outsjabloon heeft voorrang op elke lay-outsjabloon die aan de thuisgroep, het thuisteam of de primaire rol van de gebruiker is toegewezen. Voor meer informatie over de taakprioriteit van de Malplaatjes van de Lay-out, zie <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref"> lay-outmalplaatjes </a> creëren en beheren.</p> <p><b> NOTA </b>:  <p>In de volgende lijst wordt beschreven hoe de lijst met sjablonen die u in dit veld hebt, afhankelijk is van uw toegang:</p> 
       <ul> 
       <li>Als beheerder van Workfront, kunt u alle systeem-niveau en groep-vlakke Malplaatjes van de Lay-out zien.</li> 
       <li>Als groepsbeheerder, kunt u systeem-vlakke lay-outmalplaatje, evenals die zien verbonden aan de groepen die u beheert.</li> 
       <li>Als gebruiker met een licentie voor abonnementen en toegang tot het bewerken van gebruikers, kunt u alleen lay-outsjablonen op systeemniveau zien.</li> 
       </ul> <p>Voor meer informatie over groep-vlakke Malplaatjes van de Lay-out, zie <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref"> lay-outmalplaatjes </a> creëren en beheren.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organisatie </td> 
      <td> 
       <ul> 
      <li><b> Bedrijf </b>: Het bedrijf van de gebruiker. Gebruikers kunnen slechts met één bedrijf worden geassocieerd. U moet een bedrijf creëren alvorens u het met een gebruiker kunt associëren. Alleen actieve bedrijven worden in de lijst weergegeven. Voor informatie over het creëren van bedrijven, zie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref"> bedrijven </a> creëren en uitgeven.</li> 
      <li><b> Rapporten aan:</b> als u een bedrijf voor de gebruiker specificeerde, kunt u de directe manager van de gebruiker op dit gebied ook specificeren. Een gebruiker kan slechts één manager hebben. Dit veld wordt niet weergegeven als de gebruiker niet eerst aan een bedrijf is gekoppeld. </li> 
      <li><b> Directe Rapporten:</b> als u een bedrijf voor de gebruiker specificeerde, kunt u de directe rapporten van de gebruiker ook specificeren. Een gebruiker kan meerdere directe rapporten hebben. Dit veld wordt niet weergegeven als de gebruiker niet eerst aan een bedrijf is gekoppeld.</li> 
      <li><b> Team van het Huis </b>: Specificeer het huisteam voor de gebruiker. Gebruikers kunnen slechts één huisteam hebben. Het Team van het Huis is belangrijk wanneer het toewijzen van een lay-outmalplaatje of wanneer het bepalen van het Werk aan het knoop voor de taken en kwesties die aan de gebruiker worden toegewezen. </li> 
      <li><b> Andere Teams </b>: De gebruikers kunnen tot veelvoudige teams behoren. Een gebruiker kan werkitems bekijken die zijn toegewezen aan een van de teams in het thuisgebied. </li> 
      <li> <p><b> Groep van het Huis:</b> selecteer een aangewezen groep om de gebruiker toe te wijzen. Hierdoor heeft de gebruiker toegang tot objecten die met de groep worden gedeeld. U kunt lay-outsjablonen ook delen met de thuisgroep van de gebruiker.</p> <p>Dit is een verplicht veld. Elke gebruiker moet met een homegroep worden geassocieerd. Als u er geen selecteert, wordt de startgroep toegewezen als de startgroep van de nieuwe gebruiker.</p> <p><b> NOTA </b>:</p> 
      <p> U kunt een groep alleen aan een gebruiker toewijzen als een van de volgende situaties true is:</p>
      <ul><li>u bent een Workfront-beheerder</li>
      <li>u bent de beheerder van de groep</li>
      <li>de groep is openbaar .</li></ul> 
      <li> <p><b> Andere Groepen </b>: De gebruikers kunnen tot veelvoudige groepen behoren. U kunt een groep alleen aan een gebruiker toewijzen als u een Workfront-beheerder, de beheerder van de groep of de groep openbaar is.</p> <p><b> BELANGRIJK </b>:</p> 
      <p>Als u een gebruiker toevoegt aan meer dan 100 groepen, kunnen er prestatieproblemen optreden in elk gebied van Workfront dat de lijst met groepen laadt.</p> <p>Voor meer informatie over openbare groepen, zie <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref"> een groep </a> creëren.</p> <p>Voor meer informatie over groepen, zie <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref"> Overzicht van Groepen </a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bronplanning </td> 
      <td> 
       <ul>
       <li>
       <b> Tijd van het Werk </b>: Vertegenwoordigt het percentage van de Volledige tijd Equivalente (FTE) tijd dat de gebruiker voor werkelijk werk, exclusief overheadkosten beschikbaar is. De Tijd van het werk moet een decimaal aantal tot 1 zijn, en het kan niet 0 zijn. Een beschikbaarheid van 20% voor werkelijk werk zou bijvoorbeeld 0,2 zijn.

   Het gebrek van het gebied is 1, erop wijzend dat een gebruiker hun volledige VTE op werkelijk besteedt, project-verwant werk.

   Het systeem gebruikt dit aantal om de beschikbaarheid van de gebruiker voor daadwerkelijke, op project betrekking hebbende werk te berekenen.

   Voor meer informatie over het creëren van programma&#39;s in Workfront, zie <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md"> een programma </a> creëren.

   De uitzonderingen van het programma en de onderbreking zouden de capaciteit van de gebruiker kunnen ook beïnvloeden.

   Workfront berekent de beschikbaarheid van een gebruiker afhankelijk van de voorkeuren voor het beheer van bronnen in uw installatiegebied. Voor meer informatie, zie <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md"> de voorkeur van het Beheer van het Middel </a> vormen.

   <b> TIP </b>

   Plaats de waarde van de Tijd van het Werk aan 1 om erop te wijzen dat de gebruiker voor project-verwant werk hun volledig-tijdequivalent beschikbaar is.
   </li> 
      <li> <b> Deactivering van het Programma </b>: Controleer deze doos als u deze gebruiker wilt plannen om op een bepaalde datum en op een bepaald tijdstip worden gedeactiveerd. </li> 
       <li><b> Gepland DeactiveringsDatum </b>: De datum en de tijd waarop de gebruiker wordt gedeactiveerd. Voor informatie over het plannen van gebruikers voor deactivering, zie de <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref"> gebruikers van het Programma voor deactivering </a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref"> Deactivate of een gebruiker </a> opnieuw activeren.</li> 
       <li> <p><b> Primaire Rol </b>: Dit is de primaire baanrol die de gebruiker in Workfront kan vervullen. Elke taak en kwestie waaraan de gebruiker wordt toegewezen wordt ook toegewezen aan deze baanrol. Functies zijn essentieel voor het beheer van hulpbronnen. U kunt dit gebied slechts bijwerken als u een vergunning van het Plan met administratieve gebruikerstoegang hebt, of als u een beheerder van Workfront bent. Voor meer informatie over vestiging gebruikers met administratieve gebruikerstoegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Toegang van de Verlening tot gebruikers </a>.</p> <p>Alleen actieve taakrollen worden in de lijst weergegeven. </p> </li> 
       <li>Als u a <b> Primaire Rol </b> selecteerde, <b> Percentage van FTE de vertoningen van het 3} gebied van de Beschikbaarheid {. </b> Geef op welk percentage van de tijd van de planning van de gebruiker aan deze taakrol wordt toegewezen. De standaardwaarde voor het Percentage van de Beschikbaarheid van VTE voor de Primaire Rol is 100%. </li> 
       <li> <p><b> Andere Rollen </b>: Een gebruiker kan veelvoudige baanrollen in Workfront hebben. Functies zijn essentieel voor het beheer van hulpbronnen. Er is geen limiet voor het aantal taakrollen dat een gebruiker kan uitvoeren. Nochtans, adviseren wij om één gebruiker aan een bovenmatig groot aantal baanrollen niet toe te wijzen, omdat het middelbeheer voor deze gebruikers te complex zou kunnen worden.<p>Alleen actieve taakrollen worden in de lijst weergegeven. Voor meer informatie over baanrollen, zie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref"> baanrollen </a> creëren en beheren.</p> <p>U kunt dit gebied slechts bijwerken als u een vergunning van het Plan met administratieve gebruikerstoegang hebt, of als u een beheerder van Workfront bent. <br> voor meer informatie over vestiging gebruikers met administratieve gebruikerstoegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> de toegang van de Verlening tot gebruikers </a>.</p> </li> 
       <li> <p>(Voorwaardelijk) als u één of veelvoudige <b> Andere Rollen </b> selecteerde, <b> Percentage van FTE de gebiedsvertoningen van de Beschikbaarheid </b> voor elke rol. Geef op welk percentage van de tijd van de planning van de gebruiker wordt toegewezen aan elke taakrol. De standaardwaarde voor het Percentage van VTE Beschikbaarheid voor de Andere Rollen is 0%.</p> <p><b> NOTA </b>: Als Andere Rollen een 0% VTE Beschikbaarheid hebben, tonen zij niet in de Planner van het Middel, tenzij de gebruikers aan taken in deze rollen worden toegewezen.</p> <p> <img alt="user_settings_rollen_and_date_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b> NOTA </b>: <p>De som alle <b> Percentages van VTE Beschikbaarheid </b> voor alle rollen moet 100% gelijk zijn. Elk percentage van FTE Beschikbaarheid berekent de Beschikbare Uren voor elke rol per gebruiker in de Planner van het Middel. De beschikbare uren voor elke rol per gebruiker hangt van de beschikbare tijd voor de gebruiker af.</p> <p>De beschikbare tijd voor de gebruiker wordt door Workfront berekend afhankelijk van de methode die door de beheerder van Workfront is geselecteerd om FTE in de Voorkeur van het Beheer van het Middel te berekenen.</p> <p>Voor informatie over het berekenen van beschikbaarheid voor de gebruiker, zie <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref"> Overzicht van het berekenen van uren en FTE voor gebruikers en rollen in de Planner van het Middel </a>.</p> <p>Voor informatie over het vormen van de voorkeur van het Beheer van het Middel, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref"> de voorkeur van het Beheer van het Middel </a> vormen.</p> </p>
       <span class="preview"><p>(Optioneel) Datumeffectieve taakrolltoewijzingen worden gebruikt in financiële berekeningen als de taakrol van de gebruiker tijdens een project verandert.</p><p>Klik <b> bepalen rollen door datum </b>, selecteer de <b> Primaire Rol </b> en <b> Andere Rollen </b>, en ga het toewijzingspercentage voor elke rol in. De rollen zouden het zelfde als de bestaande rollen (gebruikend verschillende percentages), of nieuwe rollen kunnen zijn. Selecteer de <b> datum van het Begin </b> wanneer deze rollen actief worden. Dit kan een datum in de toekomst zijn. Wanneer de nieuwste rollen actief worden, kunt u <b> klikken tonen vorige rollen </b> om de vorige, inactieve rollen te zien.</p> </li></span>
       <li> <p><b> Programma </b>: Associeer een programma met de gebruiker. Het programma van de gebruiker berekent de chronologie van de taken de gebruiker aan wordt toegewezen.</p> <p>U moet een schema creëren alvorens u het met een gebruiker kunt associëren. Voor meer informatie over het creëren van programma's, zie <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref"> een programma </a> creëren.</p> <p><b> NOTA </b>: Wij adviseren dat het programma u met de gebruiker associeert de Zone van de Tijd van de gebruiker aanpast.</p> </li> 
       <li> <p><b> het Profiel van de Tijdopnemer </b>: Associeer een Profiel van de Tijdopnemer met de gebruiker om ervoor te zorgen dat timesheets automatisch voor de gebruiker produceren.</p> <p><b> NOTA </b>: De lijst van profielen u op dit gebied beschikbaar hebt hangt van uw toegang af:
       <ul>
       <li>Als Workfront-beheerder kunt u alle tijdbladprofielen op systeemniveau en op groepsniveau zien.</li>
       <li>Als groepsbeheerder, kunt u systeem-vlakke Profielen van de Chronologie, evenals die zien verbonden aan de groepen die u beheert.</li>
       <li>Als gebruiker met een licentie voor abonnementen en toegang tot het bewerken van gebruikers, kunt u alleen tijdbladprofielen op systeemniveau zien. Voor meer informatie over groep-vlakke Profielen van de Chronologie, zie <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref"> creëren, uitgeven, en toewijzen timesheet profielen </a>.</li>
      </ul></p> </li> 
       <li><b> het Type van Uur Standaard </b>: Selecteer het standaarduurtype voor de gebruiker. Dit is het uurtype dat door gebrek wordt gebruikt wanneer de gebruiker tijd registreert.</li> 
       <li><b> Beschikbare Types van Uur </b>: Selecteer de uurtypes die aan de gebruiker beschikbaar zouden moeten zijn. Deze uurtypen zijn overal zichtbaar in Workfront waar de gebruiker tijd kan registreren. Een gebruiker kan de uurtypes slechts zien die op het projectniveau evenals het gebruikersniveau worden toegelaten. Voor meer informatie over welke uurtypes aan gebruikers beschikbaar zijn, zie <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref"> de types en beschikbaarheid van uren bepalen </a>.</li> 
       <li><b> Tijd van het Logboek binnen:</b> selecteer of de gebruiker tijd op het werkpunten in uren of dagen zou moeten registreren. Voor meer informatie, zie <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref"> vormen of de tijd uren of dagen </a> het programma wordt geopend.</li>

   <li> <b> FTE </b>: Dit is het Volledige Gelijkwaardige van de Tijd van de gebruiker. Workfront gebruikt dit aantal om de beschikbaarheid van de gebruiker te berekenen die op het StandaardProgramma wordt gebaseerd slechts wanneer de Voorkeur van het Beheer van het Middel op het systeemniveau aan het StandaardProgramma wordt geplaatst.

   <p>FTE wijst op de hoeveelheid tijd die de gebruiker op het werk kan doorbrengen. Dit omvat overheadkosten, evenals tijd die aan projectwerk wordt doorgebracht. Bijvoorbeeld, tijd die in vergaderingen wordt doorgebracht, of de opleiding is ook inbegrepen in FTE.</p>

   De FTE moet een decimaal getal tot en met 1 zijn en mag niet 0 zijn. Als de FTE-waarde bijvoorbeeld 0,5 is en de standaardplanning in Workfront 40 uur, is de gebruiker 20 uur per week beschikbaar.

   De standaardwaarde van het veld is 1.

   De uitzonderingen van het programma, de onderbreking, en de waarde van de Tijd van het Werk kunnen de beschikbaarheid van de gebruiker beïnvloeden.

   Workfront berekent de beschikbaarheid van een gebruiker afhankelijk van de voorkeuren voor het beheer van bronnen in uw installatiegebied.

   Als de Voorkeur van het Beheer van het Middel op het systeemniveau aan het Programma van de Gebruiker wordt geplaatst, wordt de waarde u hier specificeert genegeerd en de gebruiker wordt beschouwd als beschikbaar volgens wat in hun programma wordt gespecificeerd.

   Voor meer informatie, zie <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md"> de voorkeur van het Beheer van het Middel </a> vormen.

   Voor meer informatie over het creëren van programma&#39;s in Workfront, zie <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md"> een programma </a> creëren.
   </li>

   <li><b> Pools van het Middel </b>: Vennoot de gebruiker met de Pools van het Middel. Voor meer informatie, zie <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref"> middelpools met gebruikers associëren </a>.</li>

   <li><b> Tarief van Kosten </b>: De hoeveelheid kosten per uur voor de gebruiker.
      <p>Voor datum efficiënte kostentarieven, klik <strong> toevoegen Tarief </strong>. Voer de waarde van de kostenvoet voor de tijdsperiode in en wijs zo nodig een begindatum en einddatum toe. Kostenpercentage 1 heeft geen begindatum en de laatste kostenvoet heeft geen einddatum.</p><p>Sommige datums worden automatisch toegevoegd. Bijvoorbeeld, als Kostentarief 1 geen einddatum heeft, en u Kostentarief 2 met een begindatum van 1 mei 2023 toevoegt, wordt een einddatum van 30 april, 2023 toegevoegd aan Kostentarief 1 zodat geen hiaten bestaan.</p></li>

   <li><b> het Factureren Tarief </b>: De hoeveelheid het factureren per uur voor de gebruiker.
      <p>Voor datum daadwerkelijke het factureren tarieven, klik <strong> voegt Tarief </strong> toe. Voer de waarde van de factureringssnelheid voor de tijdsperiode in en wijs zo nodig een begindatum en einddatum toe. Factureringsgraad 1 zal geen begindatum hebben en het laatste factureringstarief zal geen einddatum hebben.</p> <p>Sommige datums worden automatisch toegevoegd. Bijvoorbeeld, als het Facturerings Tarief 1 geen einddatum heeft, en u voegt een tweede met een begindatum van 1 Mei, 2023 toe, wordt een einddatum van 30 April, 2023 toegevoegd aan het Facturerings Tarief 1 zodat geen hiaten bestaan.</p><p> <img alt="Kosten voor gebruikers en factureringstarieven" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

   </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aangepaste Forms</td> 
      <td><p>Koppel een bestaand aangepast gebruikersformulier aan deze gebruiker. U moet een aangepast formulier maken voordat u het aan een gebruiker kunt koppelen. Alleen actieve aangepaste formulieren worden in de lijst weergegeven. Velden die u niet kunt bewerken, worden niet weergegeven in een afzonderlijk aangepast formulier.</p> <p><strong> Nota:</strong> de Geavanceerde eigenschappen van de douanevorm zoals Externe raadplegingsgebieden en de inheemse gebieden van Workfront zijn slechts beschikbaar wanneer u het gebruikersverslag op de detailspagina, niet op de Edit dialoog van de Gebruiker opent. (Klik in de lijst met gebruikers op de gebruikersnaam om de details te openen.)</p> <p>Voor informatie over het creëren van douaneformulieren, zie <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md" class="MCXref xref"> Ontwerp een vorm met de vormontwerper </a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Opmerking</td> 
      <td>Typ de opmerking die u naar de gebruikers en naar het gedeelte Updates van hun gebruikersprofielen wilt verzenden.</td> 
     </tr> 
    </tbody> 
   </table>
