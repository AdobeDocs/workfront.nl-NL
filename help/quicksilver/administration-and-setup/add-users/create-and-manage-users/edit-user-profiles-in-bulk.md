---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Gebruikersprofielen bulksgewijs bewerken
description: Als Adobe Workfront-beheerder kunt u gebruikersaccounts bulksgewijs bewerken.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: 5433008d93e99d69f8116e222bfce02411b77825
workflow-type: tm+mt
source-wordcount: '2194'
ht-degree: 0%

---

# Gebruikersprofielen bulksgewijs bewerken

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
>Voor instructies over het bewerken van het profiel van een gebruiker in de Adobe Admin Console raadpleegt u de sectie &quot;Gebruikersgegevens bewerken&quot; in het artikel [Gebruikers voor uploaden van bulken](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) of neem contact op met uw Adobe Admin Console-beheerder.
>
>Voor een lijst met procedures die verschillen afhankelijk van de vraag of uw organisatie al dan niet is aangemeld bij de Adobe Admin Console, raadpleegt u [Op Platform gebaseerde verschillen in beheer (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Je kunt gebruikersaccounts bulksgewijs bewerken. Bij gebruikers die bulkbewerkingen uitvoeren, worden alleen de velden die u specifiek selecteert, bijgewerkt met dezelfde gegevens voor alle geselecteerde gebruikers. Alle andere velden die u niet selecteert, blijven gelijk voor elke afzonderlijke gebruiker, zelfs als deze voor elke gebruiker anders zijn.

>[!NOTE]
>
>* U kunt het gedeelte Persoonlijke gegevens van gebruikersprofielen niet in bulk bewerken, omdat deze gegevens uniek moeten zijn voor elke gebruiker.
>* Om de nauwkeurigheid van gegevens en optimale prestaties te garanderen, raden we u aan niet meer dan 2000 gebruikers tegelijk te selecteren voor een bulkbewerking.
>


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

## Gebruikersaccounts bulksgewijs bewerken

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Gebruikers** ![](assets/users-icon-in-main-menu.png).

1. Selecteer meerdere gebruikers en klik op het pictogram Bewerken ![](assets/edit-icon.png).

1. In de **Gebruiker bewerken** Wijzig de volgende opties in het vak dat wordt weergegeven:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Voorkeuren</td> 
      <td> 
       <ul> 
        <li><b>Tijdzone:</b> De tijdzone van de gebruikers.</li> 
        <li><b>Landinstelling</b>: De voorkeurslandinstelling van de gebruiker. Dit is van invloed op de notatie van getallen en datums in de e-mails van Workfront.</li> 
        <li><b>Percentage volledig tonen bij updatestatus</b>: Schakel deze optie in als u een procent volledige balk wilt weergeven in de updatestroom van taken voor alle gebruikers.</li> 
        <li><b>Werk dat ik toewees aan mezelf verzenden naar het tabblad Werken aan</b>: Schakel deze optie in als u alles wat de gebruikers aan zichzelf toewijzen, rechtstreeks op het tabblad Werken aan wilt weergeven. Standaard wordt alles weergegeven dat aan een gebruiker is toegewezen op het tabblad Werkaanvraag.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Meldingen</td> 
      <td>Selecteer de e-mailberichten die moeten worden ingeschakeld voor de nieuwe gebruiker.<p>U kunt zowel expresberichten als dagelijkse samenvattingsmeldingen selecteren. Alle dagelijkse samenvattingsmeldingen worden enige tijd na hetzelfde tijdstip voor alle geselecteerde gebruikers verzonden. Zie voor meer informatie <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Gebeurtenismeldingen configureren voor iedereen in het systeem</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Toegang</td> 
      <td> 
       <ul> 
        <li><b>Is actief:</b> Selecteer dit veld om aan te geven of de gebruikers actief zijn. Actieve gebruikers gebruiken een Workfront-licentie. Als u de selectie van het veld opheft, worden de gebruikers gedeactiveerd.</li> 
        <li> 
        <p><b>Toegangsniveau:</b> Selecteer het toegangsniveau om aan deze gebruikers toe te wijzen. Alle geselecteerde gebruikers hebben hetzelfde toegangsniveau.
        </p> 
        <p>Wanneer u een toegangsniveau aan gebruikers toewijst, kunt u een niveau gelijk aan of minder dan uw eigen toegangsniveau toewijzen. (Als uw toegangsniveau bijvoorbeeld Planner is, kunt u het toegangsniveau voor beheerders niet toewijzen.) </p>
        <p>U kunt echter geen toegangsniveau toewijzen dat lager is dan uw eigen niveau als de Workfront-beheerder machtigingen op toegangsniveau heeft ingeschakeld die niet ook in uw eigen niveau zijn ingeschakeld (via de instellingen voor Fine-Tune, zoals beschreven in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>).</p> 
        <p>Voor meer informatie over toegangsniveaus, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Toegang tot Adobe Workfront configureren</a>.</p> 
         </li> 
        <li> 
        <p><b>Lay-outsjabloon</b>: Kies een lay-outsjabloon voor de gebruikers. Het lay-outmalplaatje dat aan de gebruikers wordt toegewezen zal belangrijkheid over om het even welk lay-outmalplaatje nemen dat aan hun Groep van het Huis, Team van het Huis of primaire baanrol wordt toegewezen. Zie voor meer informatie over de toewijzingsprioriteit van een lay-outsjabloon <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Lay-outsjablonen maken en beheren</a>.</p> 
        <p><b>OPMERKING</b>: De lijst met lay-outsjablonen die u in dit veld hebt, is afhankelijk van uw toegang:
          <ul>
           <li>Als beheerder van Workfront, kunt u alle systeem-vlakke en groep-vlakke lay-outmalplaatjes zien.</li>
           <li>Als groepsbeheerder, kunt u systeem-vlakke lay-outmalplaatjes, evenals die zien verbonden aan de groepen die u beheert.</li>
           <li><p>Als gebruiker met een Planner-licentie en toegang om gebruikers te bewerken, kunt u alleen lay-outsjablonen op systeemniveau zien. </p>
           <p>Voor informatie over lay-outsjablonen op groepsniveau raadpleegt u <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Lay-outsjablonen maken en beheren</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organisatie</td> 
      <td> 
       <ul> 
        <li><b>Bedrijf</b>: Het bedrijf van de gebruikers. Gebruikers kunnen slechts met één bedrijf worden geassocieerd. U moet een bedrijf creëren alvorens u het met een gebruiker kunt associëren. Alleen actieve bedrijven worden in de lijst weergegeven. Voor informatie over het creëren van bedrijven, zie het Begrip en het Leiden Bedrijven.</li> 
        <li><b>Thuisteam</b>: Geef het home team voor de gebruikers op. Gebruikers kunnen slechts één huisteam hebben. </li> 
        <li><b>Andere teams</b>: Gebruikers kunnen tot meerdere teams behoren. </li> 
        <li> <p><b>Thuisgroep:</b> Selecteer een geschikte groep om de gebruikers toe te wijzen als hun thuisgroep. Hierdoor heeft de gebruiker toegang tot objecten die met de groep worden gedeeld.</p> <p><b>OPMERKING</b>: Dit is een verplicht veld. Gebruikers kunnen niet aan een thuisgroep zijn gekoppeld.</p> <p>U kunt een groep alleen in de volgende situaties aan gebruikers toewijzen:</p> 
         <ul> 
          <li>U bent Workfront-beheerder.</li> 
          <li>U bent de beheerder van die groep.</li> 
          <li>De groep is openbaar.</li> 
         </ul> </li> 
        <li> <p><b>Overige groepen</b>: Gebruikers kunnen tot meerdere groepen behoren. U kunt alleen in de volgende situaties een groep aan een gebruiker toewijzen:</p> 
         <ul> 
          <li>U bent Workfront-beheerder.</li> 
          <li>U bent de beheerder van die groep.</li> 
          <li> <p>De groep is openbaar. </p> 
          <p>Zie voor meer informatie over openbare groepen <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Een groep maken</a>.</p> 
          <p>Voor meer informatie over groepen raadpleegt u <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Overzicht van groepen</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bronplanning</td> 
      <td> 
       <ul> 
        <li><b>Deactivering van schema</b>: Schakel dit selectievakje in als u wilt plannen dat gebruikers na een bepaalde periode worden gedeactiveerd.</li> 
        <li><b>Geplande datum van deactivering</b>: De datum waarna de gebruikers worden gedeactiveerd. Zie de sectie voor meer informatie over het plannen van gebruikers voor deactivering <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Gebruikers plannen voor deactivering</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Een gebruiker deactiveren of opnieuw activeren</a>.</li> 
        <li> <p><b>Primaire rol</b>: Dit is de primaire taakrol die een gebruiker in Workfront heeft. Elke taak en kwestie waaraan de gebruikers worden toegewezen wordt ook toegewezen aan deze baanrol, door gebrek. Functies zijn essentieel voor het beheer van hulpbronnen. Voor meer informatie over baanrollen, zie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Taakrollen maken en beheren</a></p> <p>U kunt dit gebied slechts bijwerken als u een vergunning van het Plan met administratieve gebruikerstoegang hebt, of als u een beheerder van Workfront bent. Voor meer informatie over vestiging gebruikers met administratieve gebruikerstoegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Toegang verlenen aan gebruikers</a>.</p> </li> 
        <li>(Voorwaardelijk) Als u een <b>Primaire rol</b>de <b>Percentage van de beschikbaarheid van VTE</b> wordt weergegeven. Geef op welk percentage van de tijd van de planningen van de gebruikers aan deze taakrol wordt toegewezen. De standaardwaarde voor het Percentage van de Beschikbaarheid van VTE voor de Primaire Rol is 100%.</li> 
        <li> <p><b>Andere rollen</b>: Gebruikers kunnen in Workfront meerdere functies hebben. Functies zijn essentieel voor het beheer van hulpbronnen. Er is geen limiet voor het aantal taakrollen dat een gebruiker kan uitvoeren. Nochtans, adviseren wij om één gebruiker aan een bovenmatig groot aantal baanrollen niet toe te wijzen, omdat het middelbeheer voor deze gebruikers te complex zou kunnen worden.</p> <p>Voor meer informatie over baanrollen, zie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Taakrollen maken en beheren</a>.</p> <p>U kunt dit gebied slechts bijwerken als u een vergunning van het Plan met administratieve gebruikerstoegang hebt, of als u een beheerder van Workfront bent. Voor meer informatie over vestiging gebruikers met administratieve gebruikerstoegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Toegang verlenen aan gebruikers</a>.</p> </li> 
        <li> <p>(Voorwaardelijk) Als u een of meerdere <b>Andere rollen</b>de <b>Percentage van de beschikbaarheid van VTE</b> wordt voor elke rol weergegeven. Geef op welk percentage van de tijd van de planningen van de gebruikers wordt toegewezen aan elke taakrol. De standaardwaarde voor het Percentage van VTE Beschikbaarheid voor de Andere Rollen is 0%.</p> <p><b>OPMERKING</b>:  
          <ul> 
           <li>Als Andere Rollen een Beschikbaarheid van 0% FTE hebben, tonen zij niet in de Planner van het Middel, tenzij de gebruikers aan taken in deze rollen worden toegewezen.</li> 
           <li> <p>De som van alle Percentages van VTE Beschikbaarheid voor alle rollen moet 100% gelijk zijn. Elk percentage van FTE Beschikbaarheid berekent de Beschikbare Uren voor elke rol per gebruiker in de Planner van het Middel. De beschikbare uren voor elke rol per gebruiker hangt van de beschikbare tijd voor de gebruiker af.</p> <p>De beschikbare tijd voor de gebruiker wordt door Workfront berekend afhankelijk van de methode die door de beheerder van Workfront is geselecteerd om FTE in de Voorkeur van het Beheer van het Middel te berekenen.</p> <p>Voor meer informatie over het berekenen van beschikbaarheid voor de gebruiker, zie <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overzicht van het berekenen van uren en FTE voor gebruikers en rollen in de Planner van het Middel</a>.</p> <p>Voor meer informatie over het vormen van de voorkeur van het Beheer van het Middel, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Voorkeuren voor beheer van bronnen configureren</a>.</p> </li> 
          </ul> </p> </li> 
        <li> <p><b>Schema</b>: Koppel een programma aan de gebruikers. Het programma van de gebruikers berekent de chronologie van de taken de gebruikers worden toegewezen aan.</p> <p>Een beheerder van Workfront of een groepsbeheerder moet een programma tot stand brengen alvorens het met gebruikers kan worden geassocieerd.</p> <p>Selecteer een systeem- of groepsschema om dit aan de geselecteerde gebruikers toe te wijzen.</p> <p>Voor meer informatie over systeem-niveau en groepsprogramma's, zie <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Een schema maken</a>.</p> <p><b>BELANGRIJK</b>: Workfront gebruikt het programma van een gebruiker slechts wanneer de Calculate Beschikbaarheid van het Middel Gebruikend het plaatsen aan het Programma van de Gebruiker wordt geplaatst. Voor informatie over hoe de Berekende Beschikbaarheid van het Middel die het plaatsen gebruikt beïnvloedt welk programma voor het Beheer van het Middel wordt gebruikt, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Voorkeuren voor beheer van bronnen configureren</a>.</p> </li> 
        <li> <p><b>Tijdbladprofiel</b>: Koppel een tijdbladprofiel aan de gebruikers. Dit zorgt ervoor dat timesheets automatisch voor de gebruikers produceren.</p> 
        <p><b>OPMERKING</b>:  
          <ul> 
           <li>De lijst met tijdlijnprofielen die beschikbaar zijn in dit veld, is afhankelijk van uw toegang:
            <ul>
             <li>Als beheerder van Workfront, kunt u alle systeem-niveau en groep-vlakke timesheet profielen zien.</li>
             <li><p>Als groepsbeheerder, kunt u systeem-vlakke timesheet profielen, evenals die zien verbonden aan de groepen die u beheert.</p></li>
             <li><p>Als gebruiker met een Planner-licentie en toegang tot het bewerken van gebruikers, kunt u alleen tijdbladprofielen op systeemniveau zien.</p></li>
            </ul></li> 
           <li>Als u een groepsbeheerder bent, moeten alle gebruikers u uitgeeft lid van een groep zijn die u beheert.</li> 
          </ul> </p> </li> 
        <li><b>Standaarduurtype</b>: Selecteer het standaarduurtype voor de gebruikers. Dit is het uurtype dat door gebrek wordt gebruikt wanneer de gebruikers tijd registreren.</li> 
        <li> <p><b>Beschikbare uurtypen</b>: Selecteer de uurtypen die voor de gebruiker beschikbaar zouden moeten zijn. Deze uurtypen zijn overal zichtbaar in Workfront waar de gebruikers de tijd kunnen registreren. Een gebruiker kan de uurtypes slechts zien die op het projectniveau evenals het gebruikersniveau worden toegelaten.</p> 
        <p>Voor meer informatie over welke uurtypes aan gebruikers beschikbaar zijn, zie <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Bepaal uurtypes en beschikbaarheid voor timesheets</a>.</p> 
        </li> 
        <li> <p><b>FTE</b>: Het aantal u hier specificeert wordt in aanmerking genomen om de beschikbaarheid te berekenen van de gebruiker die op het StandaardProgramma slechts wordt gebaseerd wanneer de Voorkeur van het Beheer van het Middel op het systeemniveau wordt geplaatst aan <b>Het standaardschema</b>.</p> 
        <p>Als de FTE-waarde bijvoorbeeld 0,5 is en de standaardplanning 40 uur, kan de gebruiker 20 uur per week werken. Voor meer informatie over hoe de programmauitzonderingen of de onderbreking gebruikersbeschikbaarheid zouden kunnen beïnvloeden wanneer het Standaard Programma wordt geselecteerd, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Voorkeuren voor beheer van bronnen configureren</a>. </p> 
        <p>Als de voorkeuren voor het beheer van bronnen op systeemniveau zijn ingesteld op <b>Het schema van de gebruiker</b>, wordt de waarde die u hier opgeeft genegeerd en wordt de gebruiker beschouwd als beschikbaar volgens wat in zijn programma is opgegeven. In dit geval wordt de FTE van de gebruiker voor de Resource Planner berekend met de volgende formule:</p>
        <p><code style="font-style: normal;">User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code> </p> <p>Voor meer informatie over het berekenen van gebruiker FTE, zie <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overzicht van het berekenen van uren en FTE voor gebruikers en rollen in de Planner van het Middel</a>.</p> <p>Voor meer informatie over het maken van planningen in Workfront raadpleegt u <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Een schema maken</a>.</p> <p>Voor meer informatie over het vormen van de Voorkeur van het Beheer van het Middel, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Voorkeuren voor beheer van bronnen configureren</a>.</p> 
        </li> 
        <li> <p><b>Brongroepen</b>: Koppel de gebruikers aan bronnenpools.</p> <p><b>OPMERKING</b>: Alleen de bronnenpools die alle geselecteerde gebruikers gemeen hebben, worden in dit veld weergegeven. Als de geselecteerde gebruikers geen gedeelde bronnenpools hebben, is dit veld leeg. Als dit veld leeg is, overschrijven de hier opgegeven bronnenpools hun afzonderlijke bronnenpools.</p> 
        <p>Voor meer informatie over middelpools, zie <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Overzicht van bronnenpools </a>.</p> </li> 
        <li><b>Kosten per uur</b>: De hoeveelheid kosten per uur voor de gebruiker. </li> 
        <li><b>Facturering per uur</b>: De hoeveelheid facturering per uur voor de gebruiker.</li> 
        <li><b>Aangepaste Forms</b>: Koppel een bestaand aangepast gebruikersformulier aan de gebruikers. U moet een aangepast formulier maken voordat u het aan een gebruiker kunt koppelen. Alleen actieve aangepaste formulieren worden in de lijst weergegeven. Voor informatie over het maken van aangepaste formulieren raadpleegt u <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Een aangepast formulier maken of bewerken</a>.</li> 
        <li><b>Opmerking</b>: Voer een opmerking in het veld in dat wordt weergegeven. Alle geselecteerde gebruikers ontvangen zowel een melding in de app als een e-mailbericht met uw opmerking. De opmerking wordt weergegeven op het tabblad Updates van het gebruikersprofiel.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) In het dialoogvenster **Aangepaste Forms** selecteert u de **Aangepaste expressies opnieuw berekenen** gebruiken om ervoor te zorgen dat alle berekende aangepaste velden in aangepaste formulieren die aan de geselecteerde gebruikers zijn gekoppeld, up-to-date zijn.

1. Klikken **Wijzigingen opslaan**.
