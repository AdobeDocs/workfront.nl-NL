---
title: Gebruikersprofiel bewerken
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-beheerder kunt u nieuwe gebruikers maken en de profielen van bestaande gebruikers beheren.
author: Courtney, Alina
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 5433008d93e99d69f8116e222bfce02411b77825
workflow-type: tm+mt
source-wordcount: '2557'
ht-degree: 0%

---

# Gebruikersprofiel bewerken

<!--drafted for Work Time field: 
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

In the table below, under Resource Planning, add the "Work Time" field and update the "FTE" field:

<b><span class="preview">Work Time</span></b>: <span class="preview">Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.</span> 

<span class="preview">The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work.</span>  

<span class="preview">The system uses this number to calculate the availability of the user for actual, project-related work.</span> 

<span class="preview">For more information about creating schedules in Workfront, see Create a schedule.</span>

<span class="preview">Schedule exceptions and time off might also affect the user capacity. 

Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see Configure Resource Management preferences. (*****INSERT LINK****)


***UPDATED FTE FIELD***

FTE: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. The FTE indicates the amount of time that the user can spend at work. This includes overhead, and  time that is not spent on project work, but on other type of work. For example, time that is spent in meetings, or training is also included in the FTE. 

The FTE must be a decimal number up to 1, and it cannot be 0. 
The field's default is 1.

For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

Schedule exceptions, time off might, <span class="preview">and the value of Work Time</span> may affect the amount of available hours or the FTE. 

Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see Configure Resource Management preferences. (*****INSERT LINK****)

If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

For more information about creating schedules in Workfront, see Create a schedule. (*****INSERT LINK*****)
-->

>[!IMPORTANT]
>
>De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet aan boord van de Admin Console zijn gegaan. Als uw organisatie is aangemeld bij de Adobe Admin Console, moet u deze handeling uitvoeren via de Adobe Admin Console.
>
>Voor instructies over het bewerken van het profiel van een gebruiker in de Adobe Admin Console raadpleegt u de sectie &quot;Gebruikersgegevens bewerken&quot; in het artikel [Gebruikers individueel beheren](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) of neem contact op met uw Adobe Admin Console-beheerder.
>
>Voor een lijst met procedures die verschillen afhankelijk van de vraag of uw organisatie al dan niet is aangemeld bij de Adobe Admin Console, raadpleegt u [Op Platform gebaseerde verschillen in beheer (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Als Adobe Workfront-beheerder kunt u nieuwe gebruikers maken en de profielen van bestaande gebruikers beheren. Voor informatie over het maken van gebruikers raadpleegt u [Gebruikers toevoegen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Gebruikers met een licentie voor abonnementen kunnen ook gebruikers maken en beheren. Voor informatie over de toegang nodig om gebruikers uit te geven, zie [Toegang verlenen aan gebruikers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Toegangsvereisten

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>Het toegangsniveau van de Beheerder van het Systeem. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>. </p> </li> 
     <li> <p><b>Gebruikers</b> het plaatsen in uw toegangsniveau dat wordt gevormd aan <b>Bewerken</b> toegang, met <b>Maken</b> en ten minste één van beide <b>Gebruikersbeheerder</b> opties ingeschakeld onder <b>Uw instellingen nauwkeurig afstellen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Van deze twee opties, als Gebruiker <b>Admin (Groepgebruikers)</b> wordt toegelaten, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> <p>Voor meer informatie over de <b>Gebruikers</b> het plaatsen in een toegangsniveau, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Toegang verlenen aan gebruikers</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Een gebruikersprofiel bewerken

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Gebruikers** ![](assets/users-icon-in-main-menu.png).
1. Selecteer de gebruiker en klik op het pictogram Bewerken ![](assets/edit-icon.png).

1. In de **Gebruiker bewerken** de doos die toont, om het even welke volgende informatie verandert, dan klik **Wijzigingen opslaan**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Persoonlijke gegevens </td> 
      <td> 
       <ul> 
        <li><b>Voornaam</b>, <b>Achternaam</b></li> 
        <li> <p><b>E-mailadres:</b> Het e-mailadres van een gebruiker is ook zijn gebruikersnaam in Workfront. Dit veld is hoofdlettergevoelig en moet uniek zijn. Als een gebruiker drie keer probeert een niet-uniek e-mailadres toe te voegen binnen een venster van 10 minuten, wordt een reCAPTCHA-reactie weergegeven.</p> <p>Als u de e-maillijst van gewenste personen gebruikt en een e-maildomein invoert dat niet in de lijst voorkomt, ontvangt de gebruiker geen e-mailberichten. Voor meer informatie over de lijst van gewenste personen, zie <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Uw e-maillijst van gewenste personen configureren</a>.</p> </li> 
        <li> <p><b>Wachtwoord opnieuw instellen</b>: Klik op deze koppeling om het wachtwoord van de gebruiker opnieuw in te stellen. U wordt om uw eigen wachtwoord gevraagd alvorens u het wachtwoord van een gebruiker kunt terugstellen.</p> <p>Als u het wachtwoord van een andere gebruiker opnieuw wilt instellen, moet u een Workfront-beheerder of een groepsbeheerder zijn.</p> <p><b>OPMERKING</b>:  
          <ul> 
           <li> <p>Als u een groepsbeheerder bent, kunt u wachtwoorden slechts voor gebruikers in de groepen terugstellen waar u als dusdanig wordt aangewezen. Ook, moet de toestemming van Admin van de Gebruiker (de Gebruikers van de Groep) op uw toegangsniveau worden toegelaten:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>Deze instelling is standaard uitgeschakeld. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </li> 
           <li> <p>U kunt het wachtwoord van een Workfront-beheerder niet opnieuw instellen.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;sso configuration=""&gt; Gebruikersnaam</b>: Als uw Workfront-beheerder een SSO-integratie met Workfront heeft ingeschakeld, wordt de SSO-gebruikersnaam in dit veld weergegeven. Het type SSO-configuratie dat voor uw Workfront-instantie is ingeschakeld, is zichtbaar in dit veld. </li> 
        <li> <p><b>OnlyAllow &lt;sso configuration=""&gt; Verificatie</b>: Als uw Workfront-beheerder een SSO-integratie met Workfront heeft ingeschakeld en alle gebruikers voor SSO heeft bijgewerkt, is dit veld standaard geselecteerd. Het type SSO-configuratie dat voor uw Workfront-instantie is ingeschakeld, is zichtbaar in dit veld.</p> <p>Wanneer dit veld is geselecteerd, moet de gebruiker zich bij Workfront aanmelden met de SSO-gegevens. Als deze optie wordt uitgeschakeld, kunnen ze zich met hun Workfront-gegevens aanmelden bij Workfront.</p> <p>Voor meer informatie over het vormen van Workfront met een oplossing SSO, zie <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Overzicht van Single Sign-On in Adobe Workfront</a></p> <p>Voor meer informatie over het bijwerken van gebruikers voor SSO, zie <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Gebruikers bijwerken voor eenmalige aanmelding</a>.</p> <p><b>OPMERKING</b>: Als u een groepsbeheerder bent, kunt u het dialoogvenster &lt;sso configuration=""&gt; velden alleen voor gebruikers in de groepen waar u als zodanig bent aangewezen. Ook, moet de toestemming van Admin van de Gebruiker (de Gebruikers van de Groep) op uw toegangsniveau worden toegelaten.
        <p>Als u een groepsbeheerder bent en u de machtiging Gebruikersbeheer (Alle gebruikers) hebt ingeschakeld op uw toegangsniveau, kunt u de opdracht &lt;sso configuration=""&gt; voor alle gebruikers.</p> </li> 
        <li><b>Taakgegevens:</b> Informatie over de taak, zoals de functie en het expertisegebied waarvoor de gebruiker verantwoordelijk is.</li> 
        <li><p><b>Contactinfo</b>: Het telefoonnummer en het adres van de gebruiker.</p>
        <p>Als de gebruiker voor Verenigd Gebruikersbeheer (UUM) of het Systeem van Adobe Identity Management (IMS) wordt toegelaten, <b>Land</b> in het gedeelte Contactinfo worden alleen landcodewaarden geaccepteerd (bijvoorbeeld VS, GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Voorkeuren </td> 
      <td> 
       <ul> 
        <li> <p><b>Tijdzone:</b> De tijdzone van de gebruiker.</p> <p>Voor informatie over hoe u gebruikers kunt helpen in Workfront samen te werken in verschillende tijdzones raadpleegt u <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Werken in tijdzones</a>.</p> </li> 
        <li><b>Landinstelling e-mail</b>: De e-maillandinstelling van de voorkeur van de gebruiker. Dit is van invloed op de notatie van getallen en datums in de e-mails van Workfront.</li> 
        <li><b>Percentage volledig tonen bij updatestatus</b>: Schakel deze optie in als u een procentuele volledige balk wilt weergeven in het gedeelte Bijwerken van de taken van deze gebruiker.</li> 
        <li><b>Werk dat ik toewees aan mezelf verzenden naar het tabblad Werken aan</b>: Schakel deze optie in als u wilt dat alles wat de gebruiker aan zichzelf toewijst, rechtstreeks op het tabblad Werken aan wordt weergegeven. Standaard wordt alles weergegeven dat aan een gebruiker is toegewezen op het tabblad Werkaanvraag.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Meldingen</td> 
      <td> <p>Selecteer de e-mailberichten die moeten worden ingeschakeld voor de nieuwe gebruiker.</p> <p>U kunt zowel expresberichten als dagelijkse samenvattingsmeldingen selecteren.</p> <p>Zie voor meer informatie <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Gebeurtenismeldingen configureren voor iedereen in het systeem</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Toegang</td> 
      <td> 
       <ul> 
        <li><b>Is actief:</b> Selecteer dit vakje om aan te geven dat de gebruiker actief is. Actieve gebruikers gebruiken een Workfront-licentie. Als u het vak wist, wordt de gebruiker gedeactiveerd.</li> 
        <li> <p><b>Toegangsniveau:</b> Selecteer het toegangsniveau dat u aan deze gebruiker wilt toewijzen.</p> 
        <p>Wanneer u een toegangsniveau aan een gebruiker toewijst, kunt u een niveau gelijk aan of minder dan uw eigen toegangsniveau toewijzen. (Als uw toegangsniveau bijvoorbeeld Planner is, kunt u het toegangsniveau voor beheerders niet toewijzen.) U kunt echter geen toegangsniveau toewijzen dat standaard lager is dan uw eigen toegangsniveau als de Workfront-beheerder niet-standaardmachtigingen op het toegangsniveau heeft ingeschakeld die niet ook in uw eigen toegangsniveau zijn ingeschakeld (via de instellingen voor Fine-Tune, zoals beschreven in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>). </p> 
        <p>Voor meer informatie over toegangsniveaus, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Toegang tot Adobe Workfront configureren</a>.</p> </li> 
        <li> <p><b>Lay-outsjabloon</b>: Kies een lay-outsjabloon voor de gebruiker. Deze lay-outsjabloon heeft voorrang op elke lay-outsjabloon die is toegewezen aan de thuisgroep, het thuisteam of de primaire taakrol van de gebruiker. Voor meer informatie over de toewijzingsprioriteit van Lay-outsjablonen raadpleegt u <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Lay-outsjablonen maken en beheren</a>.</p> <p><b>OPMERKING</b>:  <p>De lijst met sjablonen die u in dit veld hebt, is afhankelijk van uw toegang:</p> 
          <ul> 
           <li>Als beheerder van Workfront, kunt u alle systeem-niveau en groep-vlakke Malplaatjes van de Lay-out zien.</li> 
           <li>Als groepsbeheerder, kunt u systeem-vlakke lay-outmalplaatje, evenals die zien verbonden aan de groepen die u beheert.</li> 
           <li>Als gebruiker met een licentie voor abonnementen en toegang tot het bewerken van gebruikers, kunt u alleen lay-outsjablonen op systeemniveau zien.</li> 
          </ul> <p>Zie voor meer informatie over lay-outsjablonen op groepsniveau <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Lay-outsjablonen maken en beheren</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organisatie </td> 
      <td> 
       <ul> 
      <li><b>Bedrijf</b>: Het bedrijf van de gebruiker. Gebruikers kunnen slechts met één bedrijf worden geassocieerd. U moet een bedrijf creëren alvorens u het met een gebruiker kunt associëren. Alleen actieve bedrijven worden in de lijst weergegeven. Voor informatie over het creëren van bedrijven, zie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Bedrijven maken en bewerken</a>.</li> 
      <li><b>Rapporten aan:</b> Als u een bedrijf voor de gebruiker hebt opgegeven, kunt u in dit veld ook de directe manager van de gebruiker opgeven. Een gebruiker kan slechts één manager hebben.</li> 
      <li><b>Directe rapporten:</b> Als u een bedrijf voor de gebruiker specificeerde, kunt u de directe rapporten van de gebruiker ook specificeren. Een gebruiker kan meerdere directe rapporten hebben.</li> 
      <li><b>Thuisteam</b>: Geef het home team voor de gebruiker op. Gebruikers kunnen slechts één huisteam hebben.</li> 
      <li><b>Andere teams</b>: Gebruikers kunnen tot meerdere teams behoren.</li> 
      <li> <p><b>Thuisgroep:</b> Selecteer een geschikte groep om de gebruiker toe te wijzen. Hierdoor heeft de gebruiker toegang tot objecten die met de groep worden gedeeld.</p> <p>Dit is een verplicht veld. Elke gebruiker moet met een homegroep worden geassocieerd. Als u geen selecteert, wordt uw groep toegewezen als homegroep van de nieuwe gebruiker.</p> <p><b>OPMERKING</b>: U kunt een groep alleen aan een gebruiker toewijzen als u een Workfront-beheerder, de beheerder van de groep of de groep openbaar is.</p> </li> 
      <li> <p><b>Overige groepen</b>: Gebruikers kunnen tot meerdere groepen behoren. U kunt een groep alleen aan een gebruiker toewijzen als u een Workfront-beheerder, de beheerder van de groep of de groep openbaar is.</p> <p><b>BELANGRIJK</b>: Als u een gebruiker toevoegt aan meer dan 100 groepen, kunnen er prestatieproblemen optreden in elk gebied van Workfront dat de lijst met groepen laadt.</p> <p>Zie voor meer informatie over openbare groepen <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Een groep maken</a>.</p> <p>Voor meer informatie over groepen raadpleegt u <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Overzicht van groepen</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bronplanning </td> 
      <td> 
       <ul>
       <li><b>Deactivering van schema</b>: Schakel dit selectievakje in als u wilt plannen dat deze gebruiker na een bepaalde periode wordt gedeactiveerd. </li> 
       <li><b>Geplande datum van deactivering</b>: De datum waarna de gebruiker wordt gedeactiveerd. Voor informatie over het plannen van gebruikers voor deactivering, zie <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Gebruikers plannen voor deactivering</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Een gebruiker deactiveren of opnieuw activeren</a>.</li> 
       <li> <p><b>Primaire rol</b>: Dit is de primaire taakrol die de gebruiker in Workfront kan vervullen. Elke taak en kwestie waaraan de gebruiker wordt toegewezen wordt ook toegewezen aan deze baanrol. Functies zijn essentieel voor het beheer van hulpbronnen. U kunt dit gebied slechts bijwerken als u een vergunning van het Plan met administratieve gebruikerstoegang hebt, of als u een beheerder van Workfront bent. Voor meer informatie over vestiging gebruikers met administratieve gebruikerstoegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Toegang verlenen aan gebruikers</a>.</p> <p>Alleen actieve taakrollen worden in de lijst weergegeven. </p> </li> 
       <li>Als u een <b>Primaire rol</b>de <b>Percentage van de beschikbaarheid van VTE</b> wordt weergegeven. Geef op welk percentage van de tijd van de planning van de gebruiker aan deze taakrol wordt toegewezen. De standaardwaarde voor het Percentage van de Beschikbaarheid van VTE voor de Primaire Rol is 100%. </li> 
       <li> <p><b>Andere rollen</b>: Een gebruiker kan meerdere taakrollen hebben in Workfront. Functies zijn essentieel voor het beheer van hulpbronnen. Er is geen limiet voor het aantal taakrollen dat een gebruiker kan uitvoeren. Nochtans, adviseren wij om één gebruiker aan een bovenmatig groot aantal baanrollen niet toe te wijzen, omdat het middelbeheer voor deze gebruikers te complex zou kunnen worden.<p>Alleen actieve taakrollen worden in de lijst weergegeven. Voor meer informatie over baanrollen, zie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Taakrollen maken en beheren</a>.</p> <p>U kunt dit gebied slechts bijwerken als u een vergunning van het Plan met administratieve gebruikerstoegang hebt, of als u een beheerder van Workfront bent. <br>Voor meer informatie over vestiging gebruikers met administratieve gebruikerstoegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Toegang verlenen aan gebruikers</a>.</p> </li> 
       <li> <p>(Voorwaardelijk) Als u een of meerdere <b>Andere rollen</b>de <b>Percentage van de beschikbaarheid van VTE</b> wordt voor elke rol weergegeven. Geef op welk percentage van de tijd van de planning van de gebruiker wordt toegewezen aan elke taakrol. De standaardwaarde voor het Percentage van VTE Beschikbaarheid voor de Andere Rollen is 0%.</p> <p><b>OPMERKING</b>: Als Andere Rollen een Beschikbaarheid van 0% FTE hebben, tonen zij niet in de Planner van het Middel, tenzij de gebruikers aan taken in deze rollen worden toegewezen.</p> <p> <img alt="user_settings_rollen_and_date_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>OPMERKING</b>: <p>De som van alle <b>Percentage van de beschikbaarheid van FTE</b> voor alle rollen moet 100 % gelijk zijn . Elk percentage van FTE Beschikbaarheid berekent de Beschikbare Uren voor elke rol per gebruiker in de Planner van het Middel. De beschikbare uren voor elke rol per gebruiker hangt van de beschikbare tijd voor de gebruiker af.</p> <p>De beschikbare tijd voor de gebruiker wordt door Workfront berekend afhankelijk van de methode die door de beheerder van Workfront is geselecteerd om FTE in de Voorkeur van het Beheer van het Middel te berekenen.</p> <p>Voor informatie over het berekenen van beschikbaarheid voor de gebruiker, zie <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overzicht van het berekenen van uren en FTE voor gebruikers en rollen in de Planner van het Middel</a>.</p> <p>Voor informatie over het vormen van de voorkeur van het Beheer van het Middel, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Voorkeuren voor beheer van bronnen configureren</a>.</p> </p> </li> 
       <li> <p><b>Schema</b>: Koppel een schema aan de gebruiker. Het programma van de gebruiker berekent de chronologie van de taken de gebruiker aan wordt toegewezen.</p> <p>U moet een schema creëren alvorens u het met een gebruiker kunt associëren. Voor meer informatie over het creëren van programma's, zie <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Een schema maken</a>.</p> <p><b>OPMERKING</b>: Wij adviseren dat het programma u met de gebruiker associeert de Zone van de Tijd van de gebruiker aanpast.</p> </li> 
       <li> <p><b>Tijdbladprofiel</b>: Koppel een tijdbladprofiel aan de gebruiker om ervoor te zorgen dat tijdbladen automatisch voor de gebruiker worden gegenereerd.</p> <p><b>OPMERKING</b>: De lijst met profielen die beschikbaar zijn in dit veld, is afhankelijk van uw toegang:
       <ul>
       <li>Als Workfront-beheerder kunt u alle tijdbladprofielen op systeemniveau en op groepsniveau zien.</li>
       <li>Als groepsbeheerder, kunt u systeem-vlakke Profielen van de Chronologie, evenals die zien verbonden aan de groepen die u beheert.</li>
       <li>Als gebruiker met een licentie voor abonnementen en toegang tot het bewerken van gebruikers, kunt u alleen tijdbladprofielen op systeemniveau zien. Voor meer informatie over de profielen van de Chronologie op groepsniveau, zie <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Werkbladprofielen maken, bewerken en toewijzen</a>.</li>
      </ul></p> </li> 
       <li><b>Standaarduurtype</b>: Selecteer het standaarduurtype voor de gebruiker. Dit is het uurtype dat door gebrek wordt gebruikt wanneer de gebruiker tijd registreert.</li> 
       <li><b>Beschikbare uurtypen</b>: Selecteer de uurtypen die voor de gebruiker beschikbaar zouden moeten zijn. Deze uurtypen zijn overal zichtbaar in Workfront waar de gebruiker tijd kan registreren. Een gebruiker kan de uurtypes slechts zien die op het projectniveau evenals het gebruikersniveau worden toegelaten. Voor meer informatie over welke uurtypes aan gebruikers beschikbaar zijn, zie <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Bepaal uurtypes en beschikbaarheid voor timesheets</a>.</li> 
       <li><b>Aanmeldtijd:</b> Selecteer of de gebruiker de tijd op het werk in uren of dagen zou moeten registreren. Zie voor meer informatie <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Configureer of de tijd uren of dagen is aangemeld</a>.</li> 
       <li> <p><b>FTE</b>: Het systeem gebruikt dit aantal om de beschikbaarheid van de gebruiker te berekenen die op het StandaardProgramma slechts wordt gebaseerd wanneer de Voorkeur van het Beheer van het Middel op het systeemniveau wordt geplaatst aan <b>Het standaardschema</b>. De waarde moet <i>0</i> of tussen <i>1</i> en <i>1</i>.</p> <p>Als de FTE-waarde bijvoorbeeld 0,5 is en de standaardplanning 40 uur, kan de gebruiker 20 uur per week werken.</p> <p>Als de voorkeuren voor het beheer van bronnen op systeemniveau zijn ingesteld op <b>Het schema van de gebruiker</b>, wordt de waarde die u hier opgeeft genegeerd en wordt de gebruiker beschouwd als beschikbaar volgens wat in zijn programma is opgegeven. In dit geval wordt de FTE van de gebruiker voor de Resource Planner berekend met de volgende formule:</p> <p ><code>User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code><em><br></em> </p> <p>Voor meer informatie over het berekenen van gebruiker FTE, zie <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overzicht van het berekenen van uren en FTE voor gebruikers en rollen in de Planner van het Middel</a>.<br>Voor meer informatie over het maken van planningen in Workfront raadpleegt u <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Een schema maken</a>.</p> <p>De uitzonderingen van het programma en de onderbreking zouden de hoeveelheid Geplande Uren of VTE kunnen beïnvloeden. Zie voor meer informatie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Voorkeuren voor beheer van bronnen configureren</a>. </p> </li> 
        <li><b>Brongroepen</b>: Koppel de gebruiker aan bronnenpools. Zie voor meer informatie <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Brongroepen koppelen aan gebruikers </a>.</li> 
        <li><b>Kosten per uur</b>: De hoeveelheid kosten per uur voor de gebruiker. </li> 
        <li><b>Facturering per uur</b>: De hoeveelheid facturering per uur voor de gebruiker.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aangepaste Forms</td> 
      <td>Koppel een bestaand aangepast formulier aan deze gebruiker. U moet een aangepast formulier maken voordat u het aan een gebruiker kunt koppelen. Alleen actieve aangepaste formulieren worden in de lijst weergegeven. Voor informatie over het maken van aangepaste formulieren raadpleegt u <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Een aangepast formulier maken of bewerken</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Opmerking</td> 
      <td> <p>Typ de opmerking die u naar de gebruikers en naar het gedeelte Updates van hun gebruikersprofielen wilt verzenden.</p> </td> 
     </tr> 
    </tbody> 
   </table>
