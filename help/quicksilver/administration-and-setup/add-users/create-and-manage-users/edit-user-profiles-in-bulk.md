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
source-git-commit: 1949a0bb213553f1f1f252c4382a90514fcd0b5b
workflow-type: tm+mt
source-wordcount: '2285'
ht-degree: 0%

---

# Gebruikersprofielen bulksgewijs bewerken

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
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
     <li> <p>Het toegangsniveau voor systeembeheerders. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>. </p> </li> 
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
        <li><b>Percentage volledig tonen bij updatestatus</b>: Schakel deze optie in als u een procentuele volledige balk wilt weergeven in het gedeelte Bijwerken van alle taken van gebruikers wanneer u de oudere opmerkingervaring gebruikt. Zie voor meer informatie <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md">Nieuwe ervaring met opmerkingen</a>.</li> 
        <li><b>Werk dat ik toewees aan mezelf verzenden naar het tabblad Werken aan</b>: Schakel deze optie in als u wilt dat alles wat de gebruikers aan zichzelf toewijzen, rechtstreeks op het tabblad Werken aan wordt weergegeven. Standaard wordt alles weergegeven dat aan een gebruiker is toegewezen op het tabblad Werkaanvraag.</li> 
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
          <p>Voor meer informatie over openbare groepen raadpleegt u <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Een groep maken</a>.</p> 
          <p>Zie voor meer informatie over groepen <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Overzicht van groepen</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bronplanning</td> 
      <td> 
       <ul>

   <li>
       <b>Tijdstip</b>: Geeft het percentage aan van de FTE-tijd (Full Time Equivalent) dat de gebruiker beschikbaar is voor werkelijk werk, exclusief overhead. De Tijd van het werk moet een decimaal aantal tot 1 zijn, en het kan niet 0 zijn. Een beschikbaarheid van 20% voor werkelijk werk zou bijvoorbeeld 0,2 zijn.

   Het gebrek van het gebied is 1, erop wijzend dat een gebruiker hun volledige VTE op werkelijk besteedt, project-verwant werk.

   Het systeem gebruikt dit aantal om de beschikbaarheid van de gebruiker voor daadwerkelijke, op project betrekking hebbende werk te berekenen.

   Voor meer informatie over het maken van planningen in Workfront raadpleegt u <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Een schema maken</a>.

   De uitzonderingen van het programma en de onderbreking van het programma zouden ook de gebruikerscapaciteit kunnen beïnvloeden.

   Workfront berekent de beschikbaarheid van een gebruiker afhankelijk van de voorkeuren voor het beheer van bronnen in uw installatiegebied. Zie voor meer informatie <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Voorkeuren voor beheer van bronnen configureren</a>.

   <b>TIP</b>

   Plaats de waarde van de Tijd van het Werk aan 1 om erop te wijzen dat de gebruiker voor project-verwant werk hun volledig-tijdequivalent beschikbaar is.
   </li>

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
       <li> <p><b>Schema</b>: Koppel een programma aan de gebruikers. Het programma van de gebruikers berekent de chronologie van de taken de gebruikers worden toegewezen aan.</p> <p>Een beheerder van Workfront of een groepsbeheerder moet een programma tot stand brengen alvorens het met gebruikers kan worden geassocieerd.</p> <p>Selecteer een systeem- of groepsschema om dit aan de geselecteerde gebruikers toe te wijzen.</p> <p>Voor meer informatie over systeem-niveau en groepsprogramma's, zie <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Een schema maken</a>.</p> <p><b>BELANGRIJK</b>: Workfront gebruikt het programma van een gebruiker slechts wanneer het Berekende Gebruik van de Beschikbaarheid van het Middel plaatsen aan het Programma van de Gebruiker wordt geplaatst. Voor informatie over hoe de Berekende Beschikbaarheid van het Middel die het plaatsen gebruikt beïnvloedt welk programma voor het Beheer van het Middel wordt gebruikt, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Voorkeuren voor beheer van bronnen configureren</a>.</p> </li> 
       <li> <p><b>Tijdbladprofiel</b>: Koppel een tijdlijnprofiel aan de gebruikers. Dit zorgt ervoor dat timesheets automatisch voor de gebruikers produceren.</p> 
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
       <li> <p><b>Beschikbare uurtypen</b>: Selecteer de uurtypen die beschikbaar moeten zijn voor de gebruiker. Deze uurtypen zijn overal zichtbaar in Workfront waar de gebruikers de tijd kunnen registreren. Een gebruiker kan de uurtypes slechts zien die op het projectniveau evenals het gebruikersniveau worden toegelaten.</p> 
       <p>Voor meer informatie over welke uurtypes aan gebruikers beschikbaar zijn, zie <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Bepaal uurtypes en beschikbaarheid voor timesheets</a>.</p> 
       </li> 
       <li> <b>FTE</b>: Dit is het voltijdequivalent van de gebruiker. Workfront gebruikt dit aantal om de beschikbaarheid van de gebruiker te berekenen die op het StandaardProgramma wordt gebaseerd slechts wanneer de Voorkeur van het Beheer van het Middel op het systeemniveau aan het StandaardProgramma wordt geplaatst.

   <p>FTE wijst op de hoeveelheid tijd die de gebruiker op het werk kan doorbrengen. Dit omvat overheadkosten, evenals tijd die aan projectwerk wordt doorgebracht. Bijvoorbeeld, tijd die in vergaderingen wordt doorgebracht, of de opleiding is ook inbegrepen in FTE.</p>

   De FTE moet een decimaal getal tot en met 1 zijn en mag niet 0 zijn. Als de FTE-waarde bijvoorbeeld 0,5 is en de standaardplanning in Workfront 40 uur, is de gebruiker 20 uur per week beschikbaar.

   De standaardwaarde van het veld is 1.

   De uitzonderingen van het programma, de onderbreking, en de waarde van de Tijd van het Werk kunnen de beschikbaarheid van de gebruiker beïnvloeden.

   Workfront berekent de beschikbaarheid van een gebruiker afhankelijk van de voorkeuren voor het beheer van bronnen in uw installatiegebied.

   Als de Voorkeur van het Beheer van het Middel op het systeemniveau aan het Programma van de Gebruiker wordt geplaatst, wordt de waarde u hier specificeert genegeerd en de gebruiker wordt beschouwd als beschikbaar volgens wat in hun programma wordt gespecificeerd.

   Zie voor meer informatie <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Voorkeuren voor beheer van bronnen configureren</a>.

   Voor meer informatie over het maken van planningen in Workfront raadpleegt u <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Een schema maken</a>.
   </li> 
       <li> <p><b>Brongroepen</b>: Koppel de gebruikers aan bronnenpools.</p> <p><b>OPMERKING</b>: Alleen de bronnenpools die alle geselecteerde gebruikers gemeen hebben, worden in dit veld weergegeven. Als de geselecteerde gebruikers geen gedeelde bronnenpools hebben, is dit veld leeg. Als dit veld leeg is, overschrijven de hier opgegeven bronnenpools hun afzonderlijke bronnenpools.</p> 
       <p>Voor meer informatie over middelpools, zie <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Overzicht van bronnenpools </a>.</p> </li> 
       <li><b>Kosten per uur</b>: De hoeveelheid kosten per uur voor de gebruiker. </li> 
       <li><b>Facturering per uur</b>: De hoeveelheid facturering per uur voor de gebruiker.</li> 
       <li><b>Aangepaste Forms</b>: Koppel een bestaand aangepast gebruikersformulier aan de gebruikers. U moet een aangepast formulier maken voordat u het aan een gebruiker kunt koppelen. Alleen actieve aangepaste formulieren worden in de lijst weergegeven. Zie voor informatie over het maken van aangepaste formulieren <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Een aangepast formulier maken of bewerken</a>.</li> 
       <li><b>Opmerking</b>: Voer een opmerking in het opgegeven veld in. Alle geselecteerde gebruikers ontvangen zowel een melding in de app als een e-mailbericht met uw opmerking. De opmerking wordt weergegeven op het tabblad Updates van het gebruikersprofiel.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) In het dialoogvenster **Aangepaste Forms** selecteert u de **Aangepaste expressies opnieuw berekenen** gebruiken om ervoor te zorgen dat alle berekende aangepaste velden in aangepaste formulieren die aan de geselecteerde gebruikers zijn gekoppeld, up-to-date zijn.

1. Klikken **Wijzigingen opslaan**.
