---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Overzicht van uren, FTE, en kosteninformatie in de mening van het Project en van de Rol van de Planner van het Middel
description: Overzicht van uren, FTE, en kosteninformatie in de mening van het Project en van de Rol van de Planner van het Middel
author: Alina
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '2958'
ht-degree: 0%

---

# Overzicht van uren, FTE, en kosteninformatie in de mening van het Project en van de Rol van de Planner van het Middel

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

Het begroten van uw middelen voor het werk zij aan een project moeten verwezenlijken is de belangrijkste functie van de Planner van het Middel. U kunt de beschikbare tijd van uw bronnen weergeven en de tijd toewijzen aan de projecten waaraan deze zijn toegewezen.

Voor informatie over het opnemen van middelen in de Planner van het Middel, zie [De middelen van de begroting in de Planner van het Middel gebruikend de meningen van het Project en van de Rol](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)

Dit artikel beschrijft enkele zeer belangrijke concepten die u moet kennen alvorens om uw middelen in de Planner van het Middel te beginnen begroten.

## Overzicht van begrotingsmiddelen

Houd rekening met het volgende wanneer u bronnen in de begroting opneemt met de functie voor middelentoewijzing:

* U kunt de toewijzing van uw middelen begroten door een hoeveelheid uren, VTE, of Kosten te specificeren die uw middelen kunnen gebruiken om het werk aan projecten te voltooien. Wanneer u tijd of kosten voor een middel begroot, vermindert de Beschikbare Uren, VTE, of Kosten voor het middel met het begrote bedrag. Dientengevolge de Beschikbare Uren, VTE, of bedragen van Kosten voor de projecten die het project volgen waarvoor u in de begroting vermindert voor die gebruikers en rollen op die projecten.

   >[!IMPORTANT]
   >
   >U kunt uw middelen voor een periode van 15 jaar begroten. Als u middelen begroot voor een project met een looptijd van meer dan 15 jaar, is de begrotingsinformatie misschien niet correct.

* U kunt Uren, FTE, of Kosten voor uw middelen voor om het even welk tijdkader begroten dat in de Planner van het Middel, onafhankelijk van de chronologie van het project wordt getoond. Als u bijvoorbeeld wilt aangeven dat uw bronnen mogelijk niet beschikbaar zijn tijdens de tijdlijn van het project (waar ze zijn gekoppeld aan geplande uren), maar wel op een ander tijdstip beschikbaar zijn, kunt u dit doen door de bronnen in te voegen voor tijdframes waarin de geplande uren nul zijn, als dat het moment is waarop ze beschikbaar zijn om te werken. U kunt de chronologie van het project manueel veranderen om uw middelbeschikbaarheid aan te passen nadat u dit doet.

   >[!NOTE]
   >
   >Wij adviseren dat u manueel uw Uren, FTE, of Kosten voor baanrollen of voor gebruikers eerst begroot. U kunt de automatische opties gebruiken om tijd voor uw projecten en middelen slechts te begroten wanneer u zeker bent dat de hoeveelheid Geplande Uren, VTE, of Kosten altijd uw Gefabriceerde Uren, FTE, of Kosten zou moeten aanpassen.\
   >Voor informatie over het gebruiken van de automatische opties voor het opnemen in de Planner van het Middel, zie de sectie &quot;het project en de rollen van de Begroting automatisch&quot;in het artikel [Beschikbaarheid en toewijzing van bronnen controleren met de Adobe Workfront Resource Planner](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

* FTE of kosten worden op dezelfde wijze begroot als de begrotingsuren, waarbij Adobe Workfront de FTE en de kostenwaarden gebruikt in plaats van de uren voor de middelen die u begroot.

   Voor meer informatie over het begrijpen hoe de Kosten in de Planner van het Middel worden berekend, zie [Kosten berekenen in de bronnenplanner](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

* Het begroten van toewijzingen voor uw middelen in de Planner van het Middel wordt gedaan op de volgende manieren:

   * Handmatig

      of

   * Automatisch, door de project en rolopties in te gebruiken **Weergeven op project** en **Weergeven op rol** weergaven.
   Zie voor meer informatie [De middelen van de begroting in de Planner van het Middel gebruikend de meningen van het Project en van de Rol](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

* Wanneer een gebruiker baanrollen verandert, wordt geschrapt, gedeactiveerd, of uit een Pool van het Middel verwijderd, veranderen de uren die voor de rol worden begroot niet en zij worden opnieuw verdeeld aan de resterende gebruikers in de rol. Als geen gebruiker meer met de baanrol wordt geassocieerd, worden de Begroeide Uren voor de rol nul.

Zie de sectie voor meer informatie over de project- en rolopties [Begrijp de waarden van Uren, FTE, en Kosten in de Planner van het Middel](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner) in dit artikel.

## Begrijp de waarden van Uren, FTE, en Kosten in de Planner van het Middel {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

Voordat u de bronnen in de begroting opneemt en de informatie over de begrote uren uren in de functie Bronnen bijwerkt, moet u bekend zijn met de volgende concepten

* **Geplande uren, VTE of Kosten**: Het werk dat moet worden verricht zoals gedefinieerd voor taken en kwesties.
* **Beschikbare uren, VTE of Kosten**: De hoeveelheid tijd dat de gebruikers of baanrollen aan het werk, volgens de programma&#39;s verbonden aan de gebruikers beschikbaar zijn.

Deze informatie toont in de Planner van het Middel voor elk middel (gebruiker of rol) en voor elk project.

Raadpleeg het artikel voor informatie over wat wordt weergegeven in de projectweergaven en de weergave Rol van het project [Overzicht van de navigatie in de bronnenplanner](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Voor informatie over het begrijpen hoe de Kosten in de Planner van het Middel worden berekend, zie het artikel [Kosten berekenen in de bronnenplanner](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

>[!NOTE]
>
>Het begroten door Kosten is identiek aan het begroten door Uren of VTE, maar u moet begrijpen hoe Workfront Kosten voor de Planner van het Middel berekent.
>
>Voor informatie over hoe de kosten in de Planner van het Middel worden berekend, zie het artikel [Kosten berekenen in de bronnenplanner](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

De volgende lijsten tonen de toewijzing en beschikbaarheidsinformatie die in de Planner van het Middel wanneer het toepassen van of het Project of de mening van de Rol toont. U kunt deze informatie op Uren, VTE, of Kosten bekijken:

* [De kolom AVL (Beschikbaar)](#the-avl-available-column)
* [De kolom PLN (gepland)](#the-pln-planned-column)
* [De BDG-kolom (begroot)](#the-bdg-budgeted-column)
* [De kolom VAR (Variantie)](#the-var-variance-column)
* [De kolom NET](#the-net-column)

### De kolom AVL (Beschikbaar) {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Weergegeven door</strong> </td> 
   <td><strong>Beschrijving</strong> </td> 
  </tr> 
  <tr> 
   <td>Project </td> 
   <td> <p>Het totaal van Uren, FTEs, of Kosten waarvoor alle gebruikers op het project beschikbaar zijn om volgens hun programma, voor het geselecteerde tijdkader te werken. </p> </td> 
  </tr> 
  <tr> 
   <td>Rol</td> 
   <td> <p>Het totaal van Uren, VTEs, of Kosten waarvoor alle gebruikers verbonden aan deze rol beschikbaar zijn om volgens hun programma en hun <strong>Percentage van de beschikbaarheid van VTE</strong> voor die specifieke rol, voor het geselecteerde tijdkader. </p> <p>Overweeg het volgende: </p> 
    <ul> 
     <li>Als geen gebruiker aan een baanrol wordt geassocieerd, dan is de waarde voor de Beschikbare Uren voor de baanrol nul. </li> 
     <li>Als een gebruiker aan een Primaire Rol van de Baan wordt geassocieerd, maar <strong>Percentage van de beschikbaarheid van VTE</strong> voor de rol 0% is, is de waarde voor Beschikbare uren van de baanrol nul.</li> 
     <li>Als de gebruiker aan Andere Rollen en wordt geassocieerd <strong>Percentage van de beschikbaarheid van VTE</strong> voor de rollen 0% is, zijn de Andere Rollen niet vermeld in de Planner van het Middel en de gebruiker toont slechts onder hun Primaire Rol.</li> 
    </ul> <p>Voor meer informatie over de <strong>Percentage van de beschikbaarheid van VTE</strong> zie het artikel voor een taakrol <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Gebruikersprofiel bewerken</a>.</p> <p>Voor meer informatie over hoe de baanrolbeschikbaarheid in de Planner van het Middel wordt berekend, zie de sectie "de Beschikbare Uren en FTE voor een baanrol in de Planner van het Middel"in het artikel berekenen <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overzicht van het berekenen van uren en FTE voor gebruikers en rollen in de Planner van het Middel</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Gebruiker</td> 
   <td> <p>Uren, FTEs, of Kosten dat de gebruiker beschikbaar is om, volgens hun programma, voor het geselecteerde tijdkader te werken. Dit aantal trekt de uren verbonden aan het volgende af:</p> 
    <ul> 
     <li>uitzonderingen programmeren</li> 
     <li>time off van de gebruiker</li> 
     <li>de voor andere projecten begrote uren. </li> 
    </ul> <p>De Beschikbare Uren, FTEs, of Kosten voor een gebruiker veranderen volgens het volgende: </p> 
    <ul> 
     <li>hoe hun programma en FTE gebaseerd op de Voorkeur van het Beheer van het Middel op het systeemniveau worden berekend.<br>Raadpleeg het artikel voor meer informatie over het berekenen van de beschikbaarheid van gebruikers en functies <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overzicht van het berekenen van uren en FTE voor gebruikers en rollen in de Planner van het Middel</a>.</li> 
    </ul> 
    <ul> 
     <li>de <strong>Prioriteit projectplanning</strong>, als de gebruiker voor het werk in de begroting wordt opgenomen.<br>Voor meer informatie over hoe de Prioriteit van de Planning van het Project de Beschikbare Uren van een gebruiker beïnvloedt, zie <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Overzicht van de navigatie in de bronnenplanner </a>. </li> 
    </ul> <p>Als de gebruiker voor deactivering is gepland, zijn de Beschikbare Uren, VTEs, of Kosten voor de dagen na de deactiveringsdatum nul. <br>Raadpleeg het artikel voor meer informatie over het deactiveren van gebruikers <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Een gebruiker deactiveren of opnieuw activeren</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### De kolom PLN (gepland) {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Weergegeven door</strong> </td> 
   <td><strong>Beschrijving</strong> </td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td> <p>Het totaal van de geplande uren, VTE's of kosten van alle functies of gebruikers die in het kader van het project worden vermeld, inclusief in de <strong>Geen rol</strong> of <strong>Geen gebruiker</strong> secties, voor het geselecteerde tijdkader, en zoals getoond in het lusje van de Details van het Project van het project. </p> <p><b>OPMERKING</b>

Handmatige aanpassingen van de dagelijkse gebruikerstoewijzingen kunnen de waarde van de geplande wekelijkse, maandelijkse of driemaandelijkse uren in het bronnenplan wijzigen. Met Workload Balancer kunt u dagelijkse gebruikerstoewijzingen voor taken en problemen handmatig aanpassen. Zie voor meer informatie <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Toewijzingen van gebruikers beheren in Workload Balancer</a>.</p> </td>
</tr> 
  <tr> 
   <td>Rol</td> 
   <td> <p>Het totaal van de Geplande Uren van alle taken die aan de rol worden toegewezen, tijdens het geselecteerde tijdkader. </p> <p>De <strong>Geen rol</strong> de sectie zal de Geplande Uren verbonden aan taken tonen die of unassigned zijn, die aan teams worden toegewezen (de waarvan uren in <strong>Geen gebruiker</strong> (sectie), of toegewezen aan gebruikers die niet zijn gekoppeld aan een taakrol. </p> </td> 
  </tr> 
  <tr> 
   <td>Gebruiker</td> 
   <td> <p>De geplande uren van alle taken die aan de gebruiker in een specifieke rol worden toegewezen, tijdens het geselecteerde tijdkader. </p> <p>De <strong>Geen gebruiker</strong> de sectie zal de Geplande Uren verbonden aan taken tonen die of unassigned of toegewezen aan teams zijn. </p> </td> 
  </tr> 
 </tbody> 
</table>

Houd rekening met het volgende wanneer u geplande uren bekijkt:

* Hoewel u geen informatie over taaktoewijzingen in de Planner van het Middel in de mening van het Project en van de Rol kunt zien, komt de hoeveelheid Geplande Uren op de taken in de projecten.
* De geplande uren worden gelijkelijk verdeeld aan elke dag binnen de Duur van taken, voor elk middel dat aan hen wordt toegewezen. De taakduur is gebaseerd op de geplande start- en voltooiingsdatums van de taak en omvat elke kalenderdag binnen die tijdsperiode.\
   Workfront houdt rekening met het programma van de gebruiker of van het project wanneer het verdelen van Geplande Uren aan gebruikers of projecten. In dit geval, worden de Geplande Uren gelijkelijk verdeeld aan elke dag binnen de Duur van taken exclusief weekends, tijd-off dagen, en planningsuitzonderingen.\
   Als u de Planner van het Middel door Week, bijvoorbeeld toont, en u taken hebt die veelvoudige weken op projecten overspannen, hangt het aantal Geplande Uren per week af van hoeveel dagen binnen die week deel van de taakDuur uitmaken. Dit werkt op dezelfde manier wanneer het tonen van de Planner van het Middel door Maand of Kwart en wanneer de taken veelvoudige maanden of kwartalen overspannen.\
   De dagen van het weekeinde, de programmauitzonderingen, en de tijd-off dagen worden uitgesloten van deze distributie.
* De volgende taakcategorieën worden opgenomen in de berekening van de geplande uren voor elke bron:

   * taken die aan gebruikers in de Groepen van het Middel, baanrollen, of teams op het project worden toegewezen\
      Als de taken aan teams worden toegewezen, zal hun toewijzing onder **Geen rol** en **Geen gebruiker** secties. U kunt de Geplande Uren zien verbonden aan teams, maar u kunt niet de uren begroten, omdat geen rollen noch gebruikers met de taken worden geassocieerd.

   * niet toegewezen taken

* De geplande uren in de Planner van het Middel omvatten geen Geplande Uren verbonden aan het volgende:

   * bovenliggende taken
   * taken toegewezen aan gebruikers zonder bronnenpools
   * , wanneer de **Uren opnemen uit uitgaven** instellen is uitgeschakeld.

* De geplande Uren tonen niet in de Planner van het Middel als de taakDuur nul is.
* De geplande uren die zijn gekoppeld aan gedeactiveerde gebruikers worden niet weergegeven.

### De BDG-kolom (begroot) {#the-bdg-budgeted-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Weergegeven door</strong> </td> 
   <td><strong>Beschrijving</strong> </td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td> <p>Een handmatige ingang om te schatten hoeveel uren, FTE, of Kosten u voor een project, voor een geselecteerd tijdkader begroot. </p> <p>In de mening van het Project, worden de uren u voor het project begroot verdeeld aan de baanrollen die onder het project worden vermeld. De hoeveelheid geplande uren voor elke rol bepaalt hoe de begrote uren uren over de rollen worden verdeeld. De begrotingsuren worden verdeeld over de rollen met hogere Geplande waarden van Uren. </p> <p>In de mening van de Rol, worden de uren u voor het project begroot niet verdeeld aan de rollen of de gebruikers op het project. </p> </td> 
  </tr> 
  <tr> 
   <td>Rol</td> 
   <td> <p>Een handmatige ingang om te schatten hoeveel uren u voor een rol, voor een geselecteerd tijdkader begroot. </p> <p>Als geen gebruiker met de baanrol wordt geassocieerd, kunt u niet de Begroeide Uren voor de baanrol schatten. </p> <p>In de weergave Rol worden de uren die u voor de rol begroot, verdeeld over de projecten die onder de rol worden vermeld. De hoeveelheid geplande uren voor elk project bepaalt hoe de begrote uren uren worden verdeeld over de projecten. De begrotingsuren worden verdeeld over de projecten met hogere waarden voor de geplande uren.</p> <p>In de mening van het Project, worden de uren u voor de rol begroot niet verdeeld aan de projecten of de gebruikers verbonden aan de rol. </p> </td> 
  </tr> 
  <tr> 
   <td>Gebruiker</td> 
   <td> <p>Een handmatige invoer om te schatten hoeveel uren u voor een gebruiker, voor een geselecteerd tijdkader begroot. </p> <p> <p><b>OPMERKING</b>   U kunt de Begroeide Uren voor gebruikers schatten die niet aan taken worden toegewezen, maar met een Pool van het Middel op een project worden geassocieerd omdat deze gebruikers ook in de Planner van het Middel verschijnen. Hun geplande uren zouden echter nul moeten zijn, als zij niet aan taken worden toegewezen. </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Houd rekening met het volgende wanneer u werkt met Budgeted Hours:

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(Duplicated below ??)
</MadCap:conditionalText>
-->

* U kunt middelen slechts begroten wanneer u Edit toegang tot het Beheer van het Middel en Financiële Gegevens en beheer de toestemmingen van de Financiën op de projecten hebt.

   Zie het artikel voor informatie over de toegang die nodig is voor het begroten van middelen [Toegang tot begrotingsmiddelen in Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Door gebrek, zijn de begrotingsuren in de Planner van het Middel nul voor alle middelen en voor alle projecten.
* U kunt de begrotingsuren voor gebruikers en rollen manueel schatten, of u kunt één van de verbindingen in het Project of de Rol van de Taak gebruiken **Meer** menu&#39;s om deze bij te werken op basis van het aantal geplande uren.\
   Voor meer informatie over project en rolopties, zie de sectie [Overzicht van uren, FTE, en kosteninformatie in de mening van het Project en van de Rol van de Planner van het Middel](#Budget) in dit artikel.

* De kleinste periode u uren, VTE, of Kosten voor kunt begroten is een week. U kunt geen uren, VTE, of Kosten voor een dag begroten.
* De begrotingsuren worden gelijkelijk verdeeld aan elke dag binnen de Duur van taken, voor elke middelen die aan hen worden toegewezen. De taakduur is gebaseerd op de geplande start- en voltooiingsdatums van de taak en omvat elke kalenderdag binnen die tijdsperiode.\
   Workfront houdt rekening met het programma van de gebruiker of van het project wanneer het verdelen van begrotingsuren aan gebruikers of projecten. In dit geval worden de begrote uren uren gelijkelijk verdeeld over elke dag binnen de Duur van taken exclusief weekends, maar met inbegrip van tijd-off en planningsuitzonderingen.\
   Als u de Planner van het Middel door Week, bijvoorbeeld toont, en u taken hebt die veelvoudige weken overspannen, hangt het aantal Begrotingshuren per week van hoeveel dagen binnen die week deel van de taakDuur af. Deze verdeling geldt niet voor weekenddagen. Dit werkt op dezelfde manier wanneer het tonen van de Planner van het Middel door Maand of Kwart en wanneer de taken veelvoudige maanden of kwartalen overspannen.

* U kunt over begrotingsuren rapporteren door Budgeted Hour als uw rapportvoorwerp voor een nieuw rapport te selecteren.\
   Zie de sectie &#39;Rapport over objecten&#39; in het artikel voor informatie over de objecten waarover u in Workfront kunt rapporteren [Objecten in Adobe Workfront begrijpen](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
   Zie het artikel voor informatie over het bouwen van een rapport over een Budgeted Hour [Rapport: Budgeted Hour](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md).

* De uren die eerder in de begroting zijn opgenomen voor gebruikers die later zijn gedeactiveerd, worden niet weergegeven.

### De kolom VAR (Variantie) {#the-var-variance-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Weergegeven door</strong> </td> 
   <td><strong>Beschrijving</strong> </td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td> <p>De uren, FTE, of de Variantie van Kosten tonen of u genoeg begrotingsuren voor het project hebt om alle Geplande Uren voor het project te verwezenlijken. </p> <p>De de Uur, FTE, of Variantie van de Kosten van het Project wordt berekend gebruikend de volgende formule:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Rol</td> 
   <td> <p>De uren, VTE, of de Variantie van Kosten toont of u genoeg begrote Uren, VTE, of Kosten voor de rol hebt om de Geplande die Uren te verwezenlijken aan het worden toegewezen. </p> <p>De de Uur van de Rol, FTE, of Variantie van de Kosten wordt berekend gebruikend de volgende formule:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Gebruiker</td> 
   <td> <p>De uren, FTE, of de Variantie van Kosten tonen of u genoeg begrotingsuren voor de gebruiker hebt om de Geplande die Uren te verwezenlijken aan hen worden toegewezen. </p> <p>De gebruikersuren, FTE, of de Variantie van Kosten worden berekend gebruikend de volgende formule:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Wanneer de Uren, VTE, of de Variantie van Kosten in rood toont, hebt u minder begrote Uren dan de Geplande Uren van het daadwerkelijke werk geschat dat moet worden voltooid. In dit geval zijn de begrotingsuren misschien niet genoeg om het werk af te ronden.

### De kolom NET  {#the-net-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Weergegeven door</strong> </td> 
   <td><strong>Beschrijving</strong> </td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td> 
    <div> 
     <p>Het project Netto Uren, FTE, of Kosten kunnen één van het volgende tonen: </p> 
     <ul> 
      <li> <p>Het verschil tussen de Beschikbare tijd of kosten en de begrote tijd of kosten voor het project:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>Het verschil tussen de Beschikbare tijd of de kosten en de Geplande tijd of kosten voor het project, wanneer het Geplande Gebruik (PLN) waarden in NETTO berekeningen het plaatsen wordt toegelaten: </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>TIP</b></p>        
  <p>Deze optie wordt alleen toegepast wanneer u de weergave aanpast in de sectie Geselecteerde items weergeven.</p>
  <p>Zie voor meer informatie <a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >Beschikbaarheid en toewijzing van bronnen controleren met de Adobe Workfront Resource Planner</a> </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>Rol</td> 
   <td> 
    <div> 
     <p>De rol Net Uren, VTE, of Kosten kan één van het volgende tonen: </p> 
     <ul> 
      <li> <p>Het verschil tussen de Beschikbare tijd of kosten en de begrote tijd of kosten voor de rol:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>Het verschil tussen de Beschikbare tijd of de kosten en de Geplande tijd of kosten voor de rol, wanneer het Geplande Gebruik (PLN) waarden in NETTO berekeningen het plaatsen wordt toegelaten:</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>TIP</b> <span>

Deze optie wordt alleen toegepast wanneer u de weergave aanpast in de sectie Geselecteerde items weergeven.</span> </p> <p><span>Zie voor meer informatie</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Beschikbaarheid en toewijzing van bronnen controleren met de Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>Gebruiker</td> 
   <td> 
    <div> 
     <p>De gebruikersNet Uren, VTE, of Kosten kunnen één van het volgende tonen: </p> 
     <ul> 
      <li> <p>Het verschil tussen de Beschikbare tijd of de kosten en de begrote tijd of kosten voor de gebruiker:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>Het verschil tussen de Beschikbare tijd of de kosten en de Geplande tijd of kosten voor de gebruiker, wanneer het Geplande Gebruik (PLN) waarden in NETTO berekeningen het plaatsen wordt toegelaten:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>TIP</b> <span>

Deze optie wordt alleen toegepast wanneer u de weergave aanpast in de sectie Geselecteerde items weergeven.</span> </p> <p><span>Zie voor meer informatie</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Beschikbaarheid en toewijzing van bronnen controleren met de Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Wanneer de NETTO Uren, VTE, of de vertoning van Kosten in rood, er niet genoeg Beschikbare tijd of begroting is om of de Beoogde begroting te dekken** of de geplande tijd of kosten in verband met het werk. In dit geval worden de middelen oververdeeld.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the table below is ideal but it does not transfer to Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours, FTE, or Cost)</strong> </td>
<td><strong>Displayed by</strong> </td>
<td><strong>Description</strong> </td>
</tr>
<tr>
<td rowspan="3">AVL <br>(Available Hours, FTE, or Cost)</td>
<td>Project </td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users on the project are available to work according to their schedule, for the time frame selected. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users associated with this role are available to work according to their schedule and their <strong>Percentage of FTE Availability</strong> for that specific role, for the time frame selected. </p> <p>Consider the following: </p>
<ul>
<li>If no user is associated with a job role, then the value for the Available Hours for the job role is zero. </li>
<li>If a user is associated with a Primary Job Role, but the <strong>Percentage of FTE Availability</strong> for the role is 0%, the job role Available Hours value is zero.</li>
<li>If the user is associated with Other Roles and the <strong>Percentage of FTE Availability</strong> for the roles is 0%, the Other Roles are not listed in the Resource Planner and the user displays only under their Primary Role.</li>
</ul> <p>For more information about the <strong>Percentage of FTE Availability</strong> for a job role, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> <p>For more information about how the job role availability is calculated in the Resource Planner, see the section "Calculate the Available Hours and FTE for a job role in the Resource Planner" in the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>Hours, FTEs, or Cost that the user is available to work, according to their schedule, for the time frame selected. This number subtracts the hours associated with the following:</p>
<ul>
<li>schedule exceptions</li>
<li>time off of the user</li>
<li>hours budgeted for other projects. </li>
</ul> <p>The Available Hours, FTEs, or Cost for a user change according the following: </p>
<ul>
<li>how their schedule and FTE are calculated based on the Resource Management Preferences at the system level.<br>For more information about calculating user and job role availability, see the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</li>
</ul>
<ul>
<li>the <strong>Project Planning Priority</strong>, if the user is budgeted for work.<br>For more information about how Project Planning Priority affects the Available Hours of a user, see <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Resource Planner navigation overview </a>. </li>
</ul> <p>If the user is scheduled for deactivation, the Available Hours, FTEs, or Cost for the days after the deactivation date are zero. <br>For more information about deactivating users, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</p> </td>
</tr>
<tr>
<td rowspan="4">PLN <br>(Planned Hours, FTE, or Cost)</td>
<td>Project</td>
<td> <p>The total of the Planned Hours, FTEs, or Cost from all the job roles or users listed under the project, including in the <strong>No Role</strong> or <strong>No User</strong> sections, for the time frame selected, and as displayed in the Project Details tab of the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of the Planned Hours from all the tasks assigned to the role, during the time frame selected. </p> <p>The <strong>No Role</strong> section will show the Planned Hours associated with tasks that are either unassigned, assigned to teams (whose hours are listed in the <strong>No User</strong> section), or assigned to users who are not associated with a job role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Planned Hours from all the tasks assigned to the user in a specific role, during the time frame selected. </p> <p>The <strong>No User</strong> section will show the Planned Hours associated with tasks that are either unassigned or assigned to teams. </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<ul>
<li>Although you cannot see information about task allocations in the Resource Planner in the Project and Role views, the amount of Planned Hours comes from the Planned Hours on the tasks in the projects. </li>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks excluding weekends, time-off days, and schedule exceptions.<br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> The following categories of tasks are included in calculating the Planned Hours for each resource:
<ul>
<li> tasks assigned to users in Resource Pools, job roles, or teams on the project<br>If tasks are assigned to teams, their allocation will appear under <strong>No Role</strong> and <strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks. </li>
<li> unassigned tasks </li>
</ul></li>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>tasks assigned to users with no Resource Pools</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> </td>
</tr>
<tr>
<td rowspan="4"> BDG <br>(BudgetedHours, FTE, or Cost) </td>
<td>Project</td>
<td> <p>A manual entry to estimate how many hours, FTE, or Cost you budget for a project, for a selected time frame. </p> <p>In the Project view, the hours you budget for the project are distributed to the job roles listed under the project. The amount of Planned Hours for each role determines how the Budgeted Hours are distributed to the roles. The Budgeted Hours are distributed to the roles with higher Planned Hours values. </p> <p>In the Role view, the hours you budget for the project are not distributed to the roles or the users on the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>A manual entry to estimate how many hours you budget for a role, for a selected time frame. </p> <p>If no user is associated with the job role, you cannot estimate the Budgeted Hours for the job role. </p> <p>In the Role view, the hours you budget for the role are distributed to the projects listed under the role. The amount of Planned Hours for each project determines how the Budgeted Hours are distributed to the projects. The Budgeted Hours are distributed to the projects with higher Planned Hours values.</p> <p>In the Project view, the hours you budget for the role are not distributed to the projects or the users associated with the role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>A manual entry to estimate how many hours you budget for a user, for a selected time frame. </p> <p> <note type="note">  You can estimate the Budgeted Hours for users who are not assigned to tasks, but are associated with a Resource Pool on a project because these users also appear in the Resource Planner. Their Planned Hours should be zero, however, if they are not assigned to tasks.
</note> </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when working with Budgeted Hours:</p> <li>
<ul>
<li> <p>You can budget resources only when you have Edit access to Resource Management and Financial Data and Manage Finance permissions on the projects.</p> <p>For information about the access needed for budgeting resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this bullet: Duplicated below)</p>
</li>
</ul> </li>
<ul>
<li>By default, the Budgeted Hours in the Resource Planner are zero for all resources and for all the projects.</li>
<li>You can manually estimate the Budgeted Hours for users and roles, or you can use one of the links in the Project or Job Role <strong>More</strong> menus to update them according to the number of Planned Hours.<br>For more information about project and role options, see the section <a href="#Budget" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a> in this article.</li>
<li> The smallest period of time you can budget hours, FTE, or Cost for is a week. You cannot budget hours, FTE, or Cost for a day. </li>
<li> Budgeted Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time. <br>Workfront takes into account the schedule of the user or of the project when distributing Budgeted Hours to users or projects. In this case, Budgeted Hours are equally distributed to each day within the Duration of tasks excluding weekends, but including time-off and schedule exceptions. <br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks, the number of Budgeted Hours per week depends on how many days within that week are part of the task Duration. Weekend days are excluded from this distribution. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters. </li>
<li>You can report on Budgeted Hours, by selecting Budgeted Hour as your report object for a new report.<br>For information about what objects you can report on in Workfront, see the section "Report on objects" in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. <br>For information about building a Budgeted Hour report, see the article <a href="../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Report: Budgeted Hour</a>.</li>
<li>Hours previously budgeted for users who were later deactivated do not display. <br></li>
</ul> </td>
</tr>
<tr>
<td rowspan="4">VAR <br>(Hour, FTE, or ,Cost Variance)</td>
<td>Project</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the project to accomplish all the Planned Hours for the project. </p> <p>The Project Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours, FTE, or Cost for the role to accomplish the Planned Hours assigned to it. </p> <p>The Role Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Hours, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the user to accomplish the Planned Hours assigned to them. </p> <p>The User Hours, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
When the Hours, FTE, or Cost Variance displays in red, you have estimated less Budgeted Hours than the Planned Hours of the actual work that needs to be completed. In this case, the Budgeted Hours might not be enough to complete the work.
</note> </td>
</tr>
<tr>
<td rowspan="4"> NET <br>(Net Hours, FTEs, or Cost) </td>
<td>Project</td>
<td>
<div>
<p>The project Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the project:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the project, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>Role</td>
<td>
<div>
<p>The role Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the role:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the role, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span class="preview"><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>User</td>
<td>
<div>
<p>The user Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the user:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the user, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
<span>When the NET Hours,&nbsp;FTE, or Cost display in red, there is not enough Available time or budget to cover either the Budgeted</span> or the Planned time or cost associated with the work. In this case, the resources are overallocated.
</note> </td>
</tr>
</tbody>
</table>
-->
