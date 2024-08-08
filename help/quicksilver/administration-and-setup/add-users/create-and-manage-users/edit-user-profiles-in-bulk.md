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
source-git-commit: 20cb940de1d42057ed11e4e7d59f1875cdba38bb
workflow-type: tm+mt
source-wordcount: '2242'
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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>Het toegangsniveau voor systeembeheerders. Voor informatie, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> een gebruiker volledige administratieve toegang verlenen </a>. </p> </li> 
     <li> <p><b> Gebruikers </b> het plaatsen in uw toegangsniveau dat aan <b> wordt gevormd geeft </b> toegang uit, met <b> creeert </b> en minstens één van de twee <b> die gebruikers Admin </b> opties onder <b> worden toegelaten verfijnen uw montages </b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Van deze twee opties, als Gebruiker <b> Admin (de Gebruikers van de Groep) </b> wordt toegelaten, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> <p>Voor meer informatie over <b> Gebruikers </b> die in een toegangsniveau plaatsen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> de toegang van de Verlening tot gebruikers </a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Gebruikersaccounts bulksgewijs bewerken

{{step-1-to-users}}

1. Selecteer meerdere gebruikers en klik op het pictogram Bewerken ![](assets/edit-icon.png) .

1. In **geef Gebruiker** doos uit die verschijnt, verander om het even welke volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Voorkeuren</td> 
      <td> 
       <ul> 
        <li><b> Tijdzone van de Tijd:</b> de tijdzone van de gebruikers.</li> 
        <li><b> Landinstelling </b>: De geprefereerde landinstelling van de gebruikers. Dit is van invloed op de notatie van getallen en datums in de e-mails van Workfront.</li> 
        <li><b> verzend het werk ik aan mezelf toewijst aan mijn het Werken aan lusje </b>: Controleer deze optie als u alles wilt dat de gebruikers aan zich toewijzen om direct op hun het Werken aan tabel te verschijnen. Standaard wordt alles weergegeven dat aan een gebruiker is toegewezen op het tabblad Werkaanvraag.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Meldingen</td> 
      <td>Selecteer de e-mailberichten die moeten worden ingeschakeld voor de nieuwe gebruiker.<p>U kunt zowel expresberichten als dagelijkse samenvattingsmeldingen selecteren. Alle dagelijkse samenvattingsmeldingen worden enige tijd na hetzelfde tijdstip voor alle geselecteerde gebruikers verzonden. Voor meer informatie, zie <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref"> gebeurtenisberichten voor iedereen in het systeem </a> vormen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Toegang</td> 
      <td> 
       <ul> 
        <li><b> is Actief:</b> selecteer dit gebied om erop te wijzen of de gebruikers actief zijn. Actieve gebruikers gebruiken een Workfront-licentie. Als u de selectie van het veld opheft, worden de gebruikers gedeactiveerd.</li> 
        <li> 
        <p><b> Niveau van de Toegang:</b> selecteer het toegangsniveau om aan deze gebruikers toe te wijzen. Alle geselecteerde gebruikers hebben hetzelfde toegangsniveau.
        </p> 
        <p>Wanneer u een toegangsniveau aan gebruikers toewijst, kunt u een niveau gelijk aan of minder dan uw eigen toegangsniveau toewijzen. (Als uw toegangsniveau bijvoorbeeld Planner is, kunt u het toegangsniveau voor beheerders niet toewijzen.) </p>
        <p>Nochtans, kunt u geen toegangsniveau toewijzen dat lager is dan uw als de beheerder van Workfront toestemmingen op het toegangsniveau heeft toegelaten die niet ook in uw worden toegelaten (via de montages Fijne Toon, zoals die in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> worden beschreven creeer of wijzig douanetoegangsniveaus </a>).</p> 
        <p>Voor meer informatie over toegangsniveaus, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref"> toegang tot Adobe Workfront </a> vormen.</p> 
         </li> 
        <li> 
        <p><b> Malplaatje van de Lay-out </b>: Kies een lay-outmalplaatje voor de gebruikers. Het lay-outmalplaatje dat aan de gebruikers wordt toegewezen zal belangrijkheid over om het even welk lay-outmalplaatje nemen dat aan hun Groep van het Huis, Team van het Huis of primaire baanrol wordt toegewezen. Voor meer informatie over de taakprioriteit van lay-outmalplaatje, zie <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref"> lay-outmalplaatjes </a> creëren en beheren.</p> 
        <p><b> NOTA </b>: De lijst van lay-outmalplaatjes u op dit gebied beschikbaar hebt hangt van uw toegang af:
          <ul>
           <li>Als beheerder van Workfront, kunt u alle systeem-vlakke en groep-vlakke lay-outmalplaatjes zien.</li>
           <li>Als groepsbeheerder, kunt u systeem-vlakke lay-outmalplaatjes, evenals die zien verbonden aan de groepen die u beheert.</li>
           <li><p>Als gebruiker met een Planner-licentie en toegang om gebruikers te bewerken, kunt u alleen lay-outsjablonen op systeemniveau zien. </p>
           <p>Voor informatie over groep-vlakke lay-outmalplaatjes, zie <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref"> lay-outmalplaatjes </a> creëren en beheren.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organisatie</td> 
      <td> 
       <ul> 
        <li><b> Bedrijf </b>: Het bedrijf van de gebruikers. Gebruikers kunnen slechts met één bedrijf worden geassocieerd. U moet een bedrijf creëren alvorens u het met een gebruiker kunt associëren. Alleen actieve bedrijven worden in de lijst weergegeven. Voor informatie over het creëren van bedrijven, zie het Begrip en het Leiden Bedrijven.</li> 
        <li><b> Team van het Huis </b>: Specificeer het huisteam voor de gebruikers. Gebruikers kunnen slechts één huisteam hebben. </li> 
        <li><b> Andere Teams </b>: De gebruikers kunnen tot veelvoudige teams behoren. </li> 
        <li> <p><b> Groep van het Huis:</b> selecteer een aangewezen groep om de gebruikers als hun Groep van het Huis toe te wijzen. Hierdoor heeft de gebruiker toegang tot objecten die met de groep worden gedeeld.</p> <p><b> NOTA </b>: Dit is een vereist gebied. Gebruikers kunnen niet aan een thuisgroep zijn gekoppeld.</p> <p>U kunt een groep alleen in de volgende situaties aan gebruikers toewijzen:</p> 
         <ul> 
          <li>U bent Workfront-beheerder.</li> 
          <li>U bent de beheerder van die groep.</li> 
          <li>De groep is openbaar.</li> 
         </ul> </li> 
        <li> <p><b> Andere Groepen </b>: De gebruikers kunnen tot veelvoudige groepen behoren. U kunt alleen in de volgende situaties een groep aan een gebruiker toewijzen:</p> 
         <ul> 
          <li>U bent Workfront-beheerder.</li> 
          <li>U bent de beheerder van die groep.</li> 
          <li> <p>De groep is openbaar. </p> 
          <p>Voor meer informatie over openbare groepen, zie <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref"> een groep </a> creëren.</p> 
          <p>Voor meer informatie over groepen, zie <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref"> Overzicht van Groepen </a>.</p> 
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
       <b> Tijd van het Werk </b>: Vertegenwoordigt het percentage van de Volledige tijd Equivalente (FTE) tijd dat de gebruiker voor werkelijk werk, exclusief overheadkosten beschikbaar is. De Tijd van het werk moet een decimaal aantal tot 1 zijn, en het kan niet 0 zijn. Een beschikbaarheid van 20% voor werkelijk werk zou bijvoorbeeld 0,2 zijn.

   Het gebrek van het gebied is 1, erop wijzend dat een gebruiker hun volledige VTE op werkelijk besteedt, project-verwant werk.

   Het systeem gebruikt dit aantal om de beschikbaarheid van de gebruiker voor daadwerkelijke, op project betrekking hebbende werk te berekenen.

   Voor meer informatie over het creëren van programma&#39;s in Workfront, zie <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md"> een programma </a> creëren.

   De uitzonderingen van het programma en de onderbreking van het programma zouden ook de gebruikerscapaciteit kunnen beïnvloeden.

   Workfront berekent de beschikbaarheid van een gebruiker afhankelijk van de voorkeuren voor het beheer van bronnen in uw installatiegebied. Voor meer informatie, zie <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md"> de voorkeur van het Beheer van het Middel </a> vormen.

   <b> TIP </b>

   Plaats de waarde van de Tijd van het Werk aan 1 om erop te wijzen dat de gebruiker voor project-verwant werk hun volledig-tijdequivalent beschikbaar is.
   </li>

   <li><b> Deactivering van het Programma </b>: controleer dit vakje als u gebruikers wilt plannen om na een periode worden gedeactiveerd.</li> 
       <li><b> Geplande DeactiveringsDatum </b>: De datum waarna de gebruikers worden gedeactiveerd. Voor meer informatie over het plannen van gebruikers voor deactivering, zie de sectie <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref"> gebruikers van het Programma voor deactivering </a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref"> Deactivate of een gebruiker </a> opnieuw activeren.</li> 
       <li> <p><b> Primaire Rol </b>: Dit is de primaire baanrol die een gebruiker in Workfront heeft. Elke taak en kwestie waaraan de gebruikers worden toegewezen wordt ook toegewezen aan deze baanrol, door gebrek. Functies zijn essentieel voor het beheer van hulpbronnen. Voor meer informatie over baanrollen, zie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref"> baanrollen creëren en beheren </a></p> <p>U kunt dit gebied slechts bijwerken als u een vergunning van het Plan met administratieve gebruikerstoegang hebt, of als u een beheerder van Workfront bent. Voor meer informatie over vestiging gebruikers met administratieve gebruikerstoegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Toegang van de Verlening tot gebruikers </a>.</p> </li> 
       <li>(Voorwaardelijk) als u a <b> Primaire Rol </b> selecteerde, <b> Percentage van FTE het gebiedsvertoningen van de Beschikbaarheid </b>. Geef op welk percentage van de tijd van de planningen van de gebruikers aan deze taakrol wordt toegewezen. De standaardwaarde voor het Percentage van de Beschikbaarheid van VTE voor de Primaire Rol is 100%.</li> 
       <li> <p><b> Andere Rollen </b>: De gebruikers kunnen veelvoudige baanrollen in Workfront hebben. Functies zijn essentieel voor het beheer van hulpbronnen. Er is geen limiet voor het aantal taakrollen dat een gebruiker kan uitvoeren. Nochtans, adviseren wij om één gebruiker aan een bovenmatig groot aantal baanrollen niet toe te wijzen, omdat het middelbeheer voor deze gebruikers te complex zou kunnen worden.</p> <p>Voor meer informatie over baanrollen, zie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref"> baanrollen </a> creëren en beheren.</p> <p>U kunt dit gebied slechts bijwerken als u een vergunning van het Plan met administratieve gebruikerstoegang hebt, of als u een beheerder van Workfront bent. Voor meer informatie over vestiging gebruikers met administratieve gebruikerstoegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Toegang van de Verlening tot gebruikers </a>.</p> </li> 
       <li> <p>(Voorwaardelijk) als u één of veelvoudige <b> Andere Rollen </b> selecteerde, <b> Percentage van FTE de gebiedsvertoningen van de Beschikbaarheid </b> voor elke rol. Geef op welk percentage van de tijd van de planningen van de gebruikers wordt toegewezen aan elke taakrol. De standaardwaarde voor het Percentage van VTE Beschikbaarheid voor de Andere Rollen is 0%.</p> <p><b> NOTA </b>:  
       <ul> 
       <li>Als Andere Rollen een Beschikbaarheid van 0% FTE hebben, tonen zij niet in de Planner van het Middel, tenzij de gebruikers aan taken in deze rollen worden toegewezen.</li> 
       <li> <p>De som van alle Percentages van VTE Beschikbaarheid voor alle rollen moet 100% gelijk zijn. Elk percentage van FTE Beschikbaarheid berekent de Beschikbare Uren voor elke rol per gebruiker in de Planner van het Middel. De beschikbare uren voor elke rol per gebruiker hangt van de beschikbare tijd voor de gebruiker af.</p> <p>De beschikbare tijd voor de gebruiker wordt door Workfront berekend afhankelijk van de methode die door de beheerder van Workfront is geselecteerd om FTE in de Voorkeur van het Beheer van het Middel te berekenen.</p> <p>Voor meer informatie over het berekenen van beschikbaarheid voor de gebruiker, zie <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref"> Overzicht van het berekenen van uren en FTE voor gebruikers en rollen in de Planner van het Middel </a>.</p> <p>Voor meer informatie over het vormen van de voorkeur van het Beheer van het Middel, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref"> de voorkeur van het Beheer van het Middel </a> vormen.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b> Programma </b>: Verwante een programma met de gebruikers. Het programma van de gebruikers berekent de chronologie van de taken de gebruikers worden toegewezen aan.</p> <p>Een beheerder van Workfront of een groepsbeheerder moet een programma tot stand brengen alvorens het met gebruikers kan worden geassocieerd.</p> <p>Selecteer een systeem- of groepsschema om dit aan de geselecteerde gebruikers toe te wijzen.</p> <p>Voor meer informatie over systeem-niveau en groepsprogramma's, zie <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref"> een programma </a> creëren.</p> <p><b> BELANGRIJK </b>: Workfront gebruikt het programma van een gebruiker slechts wanneer de Berekende Beschikbaarheid van het Middel het plaatsen aan het Programma van de Gebruiker wordt geplaatst. Voor informatie over hoe de Berekende Beschikbaarheid van het Middel het plaatsen beïnvloedt welk programma voor het Beheer van het Middel wordt gebruikt, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref"> de voorkeur van het Beheer van het Middel </a> vormen.</p> </li> 
       <li> <p><b> het Profiel van de Tijdopnemer </b>: Koppel een Profiel van de Tijdopnemer met de gebruikers. Dit zorgt ervoor dat timesheets automatisch voor de gebruikers produceren.</p> 
       <p><b> NOTA </b>:  
       <ul> 
       <li>De lijst met tijdlijnprofielen die beschikbaar zijn in dit veld, is afhankelijk van uw toegang:
       <ul>
       <li>Als beheerder van Workfront, kunt u alle systeem-niveau en groep-vlakke timesheet profielen zien.</li>
       <li><p>Als groepsbeheerder, kunt u systeem-vlakke timesheet profielen, evenals die zien verbonden aan de groepen die u beheert.</p></li>
       <li><p>Als gebruiker met een Planner-licentie en toegang tot het bewerken van gebruikers, kunt u alleen tijdbladprofielen op systeemniveau zien.</p></li>
       </ul></li> 
       <li>Als u een groepsbeheerder bent, moeten alle gebruikers u uitgeeft lid van een groep zijn die u beheert.</li> 
       </ul> </p> </li> 
       <li><b> het Type van Uur Standaard </b>: Selecteer het standaarduurtype voor de gebruikers. Dit is het uurtype dat door gebrek wordt gebruikt wanneer de gebruikers tijd registreren.</li> 
       <li> <p><b> Beschikbare Types van Uur </b>: Selecteer de uurtypes die aan de gebruiker beschikbaar zouden moeten zijn. Deze uurtypen zijn overal zichtbaar in Workfront waar de gebruikers de tijd kunnen registreren. Een gebruiker kan de uurtypes slechts zien die op het projectniveau evenals het gebruikersniveau worden toegelaten.</p> 
       <p>Voor meer informatie over welke uurtypes aan gebruikers beschikbaar zijn, zie <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref"> de types en beschikbaarheid van uren bepalen </a>.</p> 
       </li> 
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
       <li> <p><b> Pools van het Middel </b>: Vennoot de gebruikers met middelpools.</p> <p><b> NOTA </b>: Slechts verschijnen de middelgroepen die voor alle geselecteerde gebruikers gemeenschappelijk zijn op dit gebied. Als de geselecteerde gebruikers geen gedeelde bronnenpools hebben, is dit veld leeg. Als dit veld leeg is, overschrijven de hier opgegeven bronnenpools hun afzonderlijke bronnenpools.</p> 
       <p>Zie <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Overzicht van bronnenpools </a> voor meer informatie over bronnenpools.</p> </li> 
       <li><b> Kosten per uur </b>: De hoeveelheid kosten per uur voor de gebruiker. </li> 
       <li><b> het Factureren per Uur </b>: De hoeveelheid het factureren per uur voor de gebruiker.</li> 
       <li><b> Aangepaste Forms </b>: Verwante een bestaande vorm van de gebruikersdouane met de gebruikers. U moet een aangepast formulier maken voordat u het aan een gebruiker kunt koppelen. Alleen actieve aangepaste formulieren worden in de lijst weergegeven. Voor informatie over het creëren van douaneformulieren, zie <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md"> Ontwerp een vorm met de vormontwerper </a>.</li> 
       <li><b> Commentaar </b>: ga een commentaar op het verstrekte gebied in. Alle geselecteerde gebruikers ontvangen zowel een melding in de app als een e-mailbericht met uw opmerking. De opmerking wordt weergegeven op het tabblad Updates van het gebruikersprofiel.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatief) in de **sectie van Forms van de Douane 0}, selecteer de** **optie van de Uitdrukkingen van de Douane opnieuw berekenen om ervoor te zorgen dat alle berekende douanegebieden in douanevormen die aan de geselecteerde gebruikers in bijlage zijn bijgewerkt zijn.**

1. Klik **sparen Veranderingen**.
