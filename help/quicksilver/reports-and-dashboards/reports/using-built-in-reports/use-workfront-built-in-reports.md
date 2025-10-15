---
product-area: reporting
navigation-topic: using-built-in-reports
title: Ingebouwde Adobe Workfront-rapporten gebruiken
description: Adobe Workfront heeft een uitgebreide lijst met ingebouwde rapporten die klaar zijn om te gebruiken. Workfront-beheerders kunnen ingebouwde rapporten verbergen, zodat gebruikers er geen toegang toe hebben.
author: Nolan
feature: Reports and Dashboards
exl-id: 32a47c25-192a-4e97-9016-42e6b6e201b9
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '2978'
ht-degree: 0%

---

# Ingebouwde Adobe Workfront-rapporten gebruiken

<!--Audited: 11/2024-->

Adobe Workfront heeft een uitgebreide lijst met ingebouwde rapporten die u kunt gebruiken.

Workfront-beheerders kunnen ingebouwde rapporten verbergen, zodat gebruikers er geen toegang toe hebben. Voor meer informatie over hoe te om ingebouwde rapporten te verbergen, zie [ ingebouwde rapporten van de Huid ](../../../administration-and-setup/manage-workfront/configure-reports/hide-built-in-reports.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
      <p>Medewerker of hoger</p>
      <p>Aanvraag of hoger</p>
   </td>
  </tr>
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders weergeven of vergroten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten beheren voor een rapport om een filter toe te voegen aan of te bewerken in een rapport</p> <p>Machtigingen beheren voor een filter om het in een lijst te bewerken</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overzicht van ingebouwde rapporten {#overview-of-built-in-reports}

U kunt een exemplaar tot stand brengen een ingebouwd rapport en het bewaren als nieuw rapport. Voor meer informatie over het creëren van exemplaren van ingebouwde rapporten, zie [ een nieuwe versie van een rapport ](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#create-a-new-version-of-a-report) in het artikel [ creëren een exemplaar van een rapport ](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

De volgende verslagen gaan over het Workfront-pakket. De rapporten zijn beschikbaar aan alle gebruikers die minstens de rechten van de Mening aan ingebouwde rapporten in hun toegangsniveau hebben.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong> Naam van het Rapport </strong> </th> 
   <th><strong> Beschrijving van het Rapport </strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Feitelijke Portfolio-kosten per programma</td> 
   <td>Een projectrapport met de geplande kosten en de werkelijke kosten van de projecten. Het rapport wordt gegroepeerd door de Naam van het Programma, die door de Naam van Portfolio wordt veroorzaakt, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Werkelijke Portfolio-kosten per project</td> 
   <td>Een projectrapport met de geplande kosten en de werkelijke kosten van de projecten. Het rapport wordt gegroepeerd door de Naam van het Project, die door de Naam van Portfolio wordt veroorzaakt, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Werkelijke Portfolio-inkomsten per programma</td> 
   <td>Een projectrapport met de geplande inkomsten en de werkelijke inkomsten van de projecten. Het rapport wordt gegroepeerd door de Naam van het Programma, die door de Naam van Portfolio wordt veroorzaakt, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Werkelijke Portfolio-inkomsten per project</td> 
   <td>Een projectrapport met de geplande inkomsten en de werkelijke inkomsten van de projecten. Het rapport wordt gegroepeerd door de Naam van het Project, die door de Naam van Portfolio wordt veroorzaakt, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Werkelijke ontvangsten per onderneming</td> 
   <td>Een projectrapport met de werkelijke inkomsten en het bedrijf van de projecten. Het rapport wordt gegroepeerd door de Naam van het Bedrijf, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Werkelijke ontvangsten per groep</td> 
   <td>Een projectrapport met de werkelijke inkomsten en de groep van de projecten. Het rapport wordt gegroepeerd door de Naam van de Groep, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Alle geopende tijdbladen</td> 
   <td>Een rapport Tijdschema dat Open Timesheets toont. Het rapport geeft de volgende velden weer: Datumbereik, Naam eigenaar, Totaal aantal uren, Overwerk, Naam fiatteur en Status van de tijdbladen.</td> 
  </tr> 
  <tr> 
   <td>Goedkeuringstijdbladen (gevraagd)</td> 
   <td>Een rapport met een tijdlijnoverzicht waarin de ingediende of geweigerde tijdbladen met fiatteurs worden weergegeven. Het rapport geeft de volgende velden weer: Datumbereik, Eigenaar, Totaal aantal uren, Overwerk, Naam fiatteur en Status van de tijdbladen. Het rapport wordt veroorzaakt door: De Datum van het Begin van de Tijdopmaak, de Datum van het Eind van de Tijdopmaak, de Naam van de Approver van de Tijdopmaak, en Naam van de Gebruiker.</td> 
  </tr> 
  <tr> 
   <td>Risicoprojecten</td> 
   <td>Een rapport van het Project dat Huidige en Plannende projecten toont die een Voorwaarde van Bij Risico of in Problemen hebben. Het rapport bevat de volgende velden: Beschrijving, Geplande Voltooiingsdatum, Geprojecteerde Voltooiingsdatum, Percentage voltooid, Status en Prioriteit van de projecten. Het rapport is gegroepeerd op Portfolio Name.</td> 
  </tr> 
  <tr> 
   <td>Factureringsopbrengsten per onderneming</td> 
   <td>Een rapport van het Project dat het Bedrijf en de Inkomsten van de Facturering van de projecten toont. Het rapport wordt gegroepeerd door de Naam van het Bedrijf, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Factureringsontvangsten per groep</td> 
   <td>Een projectrapport met de factureringsinkomsten en de groep projecten. Het rapport wordt gegroepeerd door de Naam van de Groep, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Factureringsontvangsten per maand</td> 
   <td>Een rapport van het Verslag van de Facturering dat de Naam van het Project, de Inkomsten van de Facturering van het Project en de Datum van de Rekening van de factureringsverslagen toont. Het rapport wordt gegroepeerd door de maand van de FactureringsDatum van de het factureringsverslagen, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Voltooide problemen per week</td> 
   <td>An Issue report that displays the Actual Completion Date of the issues. Het rapport wordt gegroepeerd op de week van de Werkelijke Voltooiingsdatum van de kwesties en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Uitgaven per week door gebruiker voltooid</td> 
   <td>An Issue report that displays the Actual Completion Date and Astaken of the issues. Het rapport wordt gegroepeerd op de primaire toegewezen persoon en op de week van de werkelijke afsluitende datum van de emissies, en bevat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Huidige projecten</td> 
   <td>Een rapport van het Project dat alle Huidige projecten toont. Het rapport bevat de volgende velden: Beschrijving, Geplande Voltooiingsdatum, Geprojecteerde Voltooiingsdatum, Percentage voltooid, Status en Prioriteit van de projecten.</td> 
  </tr> 
  <tr> 
   <td>Kosten per uur per maand</td> 
   <td>Een matrixuurrapport waarin het aantal geregistreerde uren en hun werkelijke kosten worden weergegeven. Het rapport wordt gegroepeerd op Naam van Eigenaar en de maand van de Invoerdatum van de uren.</td> 
  </tr> 
  <tr> 
   <td>Uren per gebruiker</td> 
   <td>Een rapport van het Uur dat het aantal geregistreerde uren toont. Het rapport wordt gegroepeerd op Naam van Eigenaar en omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Uren per week</td> 
   <td>Een matrixuurrapport dat het aantal geregistreerde uren in de afgelopen vier weken en de Datum van de Ingang van de uren toont. Het rapport wordt veroorzaakt door de Datum van de Ingang van de uren en door de Naam van de Eigenaar en de maand van de Datum van de Ingang van de uren gegroepeerd.</td> 
  </tr> 
  <tr> 
   <td>Problemen op basis van status</td> 
   <td>An Issue report that displays the Status of issues. Het rapport wordt gegroepeerd door Status van de kwesties, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Problemen per status en project</td> 
   <td>Een matrixrapport van de Kwestie dat de Status van kwesties in Huidige projecten en de Naam van het Project toont. Het rapport wordt gegroepeerd door de Naam van het Project en Status van de kwesties.</td> 
  </tr> 
  <tr> 
   <td>Arbeidskosten vs. onkosten door Portfolio</td> 
   <td>Een projectrapport waarin de geplande loonkosten, de werkelijke loonkosten, de geplande onkostenkosten en de werkelijke kosten van de projecten worden weergegeven. Het rapport wordt gegroepeerd door de Naam van Portfolio, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Arbeidskosten vs. onkosten per programma</td> 
   <td>Een projectrapport waarin de geplande loonkosten, de werkelijke loonkosten, de geplande onkostenkosten en de werkelijke kosten van de projecten worden weergegeven. Het rapport wordt gegroepeerd door de Naam van Portfolio en de Naam van het Programma, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Maandelijkse geplande Portfolio-kosten in verhouding tot werkelijke kosten per project</td> 
   <td>Een matrixprojectrapport (financiële gegevens) met de datum van toewijzing, de totale geplande kosten, de totale werkelijke kosten en de totale kostenvariatie van de projecten. Het rapport wordt gegroepeerd op de Naam van het Project, het kwartaal en de maand van de Datum van Toewijzing.</td> 
  </tr> 
  <tr> 
   <td>Voorziene jaarlijkse Portfolio-inkomsten vs. Werkelijk per project</td> 
   <td>Een matrixprojectrapport (financiële gegevens) met de datum van toewijzing, de totale geplande inkomsten, de totale werkelijke inkomsten en de variatie van de totale opbrengsten van de projecten. Het rapport wordt gegroepeerd op de Naam van het Project, het kwartaal en de maand van de Datum van Toewijzing.</td> 
  </tr> 
  <tr> 
   <td>Voorziene maandelijkse projectkosten versus werkelijke kosten</td> 
   <td>Een matrixprojectrapport (financiële gegevens) met de datum van toewijzing, de totale geplande kosten, de totale werkelijke kosten en de totale kostenvariatie van de projecten. Het rapport wordt gegroepeerd door de Naam van het Project, het kwartaal en de maand van de Datum van de Toewijzing en door de Naam van het Project veroorzaakt.</td> 
  </tr> 
  <tr> 
   <td>Voorziene jaarlijkse inkomsten uit het project versus werkelijke inkomsten</td> 
   <td>Een matrixprojectrapport (financiële gegevens) met de datum van toewijzing, de totale geplande inkomsten, de totale werkelijke inkomsten en de variatie van de totale opbrengsten van de projecten. Het rapport wordt gegroepeerd door de Naam van het Project, het kwartaal en de maand van de Datum van de Toewijzing en door de Naam van het Project veroorzaakt.</td> 
  </tr> 
  <tr> 
   <td>Mijn documenten</td> 
   <td>Een documentrapport dat door de aangemelde gebruiker geüploade documenten weergeeft. In het rapport worden de volgende velden weergegeven: Naam eigenaar, Wijzigingsdatum, Grootte, Aantal versies, Source en Type van de documenten.</td> 
  </tr> 
  <tr> 
   <td>Mijn favorieten</td> 
   <td>Een rapport Favorieten waarin een lijst met objecten wordt weergegeven die door de aangemelde gebruiker als favorieten zijn gemarkeerd. In het rapport worden de volgende velden weergegeven: Objecttype en Naam van de favorieten.</td> 
  </tr> 
  <tr> 
   <td>Mijn problemen</td> 
   <td>Een rapport van de Kwestie dat onvolledige Kwesties toont die aan de gebruiker worden toegewezen die het programma wordt geopend. In het rapport worden de volgende velden weergegeven: Source-naam, Type uitgave, primaire toewijzing, Invoerdatum, Status en Prioriteit van de problemen.</td> 
  </tr> 
  <tr> 
   <td>Mijn portfolio's</td> 
   <td>Een Portfolio-rapport waarin actieve portfolio's worden weergegeven waarin de aangemelde gebruiker Portfolio Manager is.</td> 
  </tr> 
  <tr> 
   <td>Mijn programma's</td> 
   <td>Een rapport van het Programma dat Programma's en hun Beschrijving toont, waar de het programma geopende gebruiker de Manager van het Programma is.</td> 
  </tr> 
  <tr> 
   <td>Problemen met het openen van mijn project</td> 
   <td>Een rapport van de Kwestie dat onvolledige kwesties in projecten toont het waarvan Team van het Project de het programma geopende gebruiker omvat. In het rapport worden de volgende velden weergegeven: Source-naam, Type uitgave, primaire toewijzing, Invoerdatum, Status en Prioriteit van de problemen.</td> 
  </tr> 
  <tr> 
   <td>Mijn projecten</td> 
   <td>Een rapport van het Project dat Huidige projecten toont het waarvan Team van het Project de het programma geopende gebruiker omvat. Het rapport bevat de volgende velden: Beschrijving, Geplande Voltooiingsdatum, Geprojecteerde Voltooiingsdatum, Percentage voltooid, Status en Prioriteit van de projecten.</td> 
  </tr> 
  <tr> 
   <td>Mijn verzonden problemen</td> 
   <td>Een rapport van de Kwestie dat kwesties toont die door de geregistreerde gebruiker worden voorgelegd, die in de afgelopen drie maanden zijn gesloten of momenteel open zijn. Het rapport bevat de volgende velden: Source Name, Issue Type, Entry Date, Status en Priority van de problemen.</td> 
  </tr> 
  <tr> 
   <td>Mijn taken</td> 
   <td>Een rapport van de Taak dat onvolledige taken in Huidige Projecten toont die aan de het programma geopende gebruiker worden toegewezen. In het rapport worden de volgende velden weergegeven: Geplande duur, Projectnaam, primaire toewijzing, Geplande start, Geplande voltooiing, Percentage voltooiing en Prioriteit van de taken.</td> 
  </tr> 
  <tr> 
   <td>Mijn tijdbladen</td> 
   <td>Een rapport Timesheet dat alle timesheets van de het programma geopende gebruiker toont. Het rapport geeft de volgende velden weer: Datumbereik, Naam eigenaar, Totaal aantal uren, Overwerk, Naam fiatteur en Status van de tijdbladen.</td> 
  </tr> 
  <tr> 
   <td>Mijn niet-toegewezen problemen</td> 
   <td>Een rapport van de Kwestie dat open kwesties toont die aan om het even welke baanrollen van de aangemelde gebruiker worden toegewezen en die niet aan de gebruiker worden toegewezen. Het rapport bevat de volgende velden: Source Name, Issue Type, Entry Date, Status en Priority van de problemen.</td> 
  </tr> 
  <tr> 
   <td>Mijn niet toegewezen taken</td> 
   <td>Een rapport van de Taak dat onvolledige taken toont die aan om het even welke baan rollen van de het programma geopende gebruiker worden toegewezen en niet aan de gebruiker worden toegewezen. In het rapport worden de volgende velden weergegeven: Geplande duur, Projectnaam, primaire toewijzing, Geplande begindatum, Geplande voltooiingsdatum, Percentage voltooid en Prioriteit van de taken.</td> 
  </tr> 
  <tr> 
   <td>Mijn komende taken</td> 
   <td>Een rapport van de Taak dat onvolledige taken toont die in de volgende twee weken zouden moeten beginnen, is op Huidige projecten, en toegewezen aan de het programma geopende gebruiker. In het rapport worden de volgende velden weergegeven: Projectnaam, Geplande Voltooiingsdatum, Geprojecteerde Voltooiingsdatum, Percentage voltooid en Status van de taken.</td> 
  </tr> 
  <tr> 
   <td>Tijdbladen openen (gevraagd)</td> 
   <td>Een rapport Tijdschema dat Open Timesheets toont. Het rapport geeft de volgende velden weer: Datumbereik, Eigenaar, Totaal aantal uren, Overwerk, Naam fiatteur, Status van de tijdbladen. Het rapport wordt veroorzaakt door: De Datum van het Begin van de Tijdopmaak, de Datum van het Eind van de Tijdopmaak, de Naam van de Approver van de Tijdopmaak, en Naam van de Gebruiker.</td> 
  </tr> 
  <tr> 
   <td>Overdrachtsprojecten van Portfolio</td> 
   <td>Een projectrapport waarin de geplande kosten en de werkelijke kosten van de projecten worden weergegeven. Het rapport is gegroepeerd op Portfolio Name.</td> 
  </tr> 
  <tr> 
   <td>Geplande Portfolio-kosten per programma</td> 
   <td>Een projectrapport waarin de geplande kosten en de werkelijke kosten van de projecten worden weergegeven. Het rapport wordt veroorzaakt door de Naam van Portfolio, die door de Naam van het Programma wordt gegroepeerd, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Geplande Portfolio-kosten per project</td> 
   <td>Een projectrapport waarin de geplande kosten en de werkelijke kosten van de projecten worden weergegeven. Het rapport wordt veroorzaakt door de Naam van Portfolio, die door de Naam van het Project wordt gegroepeerd, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Geplande Portfolio-inkomsten per programma</td> 
   <td>Een projectrapport met de geplande inkomsten en werkelijke inkomsten van de projecten. Het rapport wordt veroorzaakt door de Naam van Portfolio, die door de Naam van het Programma wordt gegroepeerd, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Geplande Portfolio-inkomsten per project</td> 
   <td>Een projectrapport met de geplande inkomsten en werkelijke inkomsten van de projecten. Het rapport wordt veroorzaakt door de Naam van Portfolio, die door de Naam van het Project wordt gegroepeerd, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Geplande versus werkelijke kosten door Portfolio</td> 
   <td>Een projectrapport met de geplande kosten en werkelijke kosten van de projecten door Portfolio. Het rapport wordt gegroepeerd door de Naam van Portfolio, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Geplande versus werkelijke kosten per programma</td> 
   <td>Een projectrapport met de geplande kosten en werkelijke kosten van de projecten per programma. Het rapport wordt gegroepeerd door de Naam van Portfolio, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Geplande versus werkelijke inkomsten van Portfolio</td> 
   <td>Een projectrapport met de geplande inkomsten en de werkelijke inkomsten van de projecten. Het rapport wordt gegroepeerd door de Naam van Portfolio, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Geplande versus werkelijke inkomsten per programma</td> 
   <td>Een projectrapport met de geplande inkomsten en de werkelijke inkomsten van de projecten. Het rapport wordt gegroepeerd door de Naam van het Programma, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Portfolio-kosten per programma en per maand</td> 
   <td>Een matrixprojectrapport waarin de geplande kosten, de begrote kosten en de werkelijke kosten van de projecten worden weergegeven. Het rapport wordt gegroepeerd op Portfolio-naam, programmanaam en de maand van de geplande begindatum van de projecten.</td> 
  </tr> 
  <tr> 
   <td>Portfolio-projecten per status gegroepeerd op programma</td> 
   <td>Een rapport van het Project dat de Status van de projecten toont. Het rapport wordt gegroepeerd door de Naam van het Programma en de Status van het Project, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Portfolio Projecten gegroepeerd op Status en Portfolio</td> 
   <td>Een rapport van het Project dat de Naam van Portfolio en de Status van de projecten toont. Het rapport wordt gegroepeerd door de Naam van Portfolio en de Status van de projecten, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Portfolio-inkomsten per programma</td> 
   <td>Een projectrapport met de naam, de naam van het programma, de geplande inkomsten en de werkelijke inkomsten van de projecten. Het rapport wordt gegroepeerd door de Naam van Portfolio en de Naam van het Programma, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Portfolio Revenue gegroepeerd per programma en per maand</td> 
   <td>Een matrixprojectrapport met de geplande inkomsten, werkelijke inkomsten, Portfolio-naam en programmanaam. Het rapport wordt gegroepeerd op de naam van Portfolio, de naam van het programma en de maand van de geplande begindatum van de projecten.</td> 
  </tr> 
  <tr> 
   <td>Projectkosten en ontvangsten per taakstatus</td> 
   <td>Een matrixtaakrapport waarin de geplande kosten, werkelijke kosten, geplande inkomsten, werkelijke inkomsten en de projectnaam van de taken worden weergegeven. Het rapport wordt gegroepeerd door de Naam en Status van het Project van de taken.</td> 
  </tr> 
  <tr> 
   <td>Projectkosten versus inkomsten van Portfolio</td> 
   <td>Een projectrapport met de naam van de Portfolio, de werkelijke kosten en de werkelijke inkomsten van de projecten. Het rapport wordt gegroepeerd door de Naam van Portfolio, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Projectkosten per maand en per kwartaal</td> 
   <td>Een matrixkostenrapport met de invoerdatum, het geplande bedrag, het werkelijke bedrag en het project van de uitgaven. Het rapport wordt gegroepeerd op de projectnaam, het kwartaal en de maand van de datum van binnenkomst van de uitgaven.</td> 
  </tr> 
  <tr> 
   <td>Kosten per uur per maand voor project</td> 
   <td>Een matrixuurrapport waarin de volgende velden worden weergegeven: Uren, Datum van binnenkomst, Werkelijke kosten van de projecten, Type uur en Projectnaam. Het rapport wordt gegroepeerd door de Naam van het Project, maand van de Datum van de Ingang van de uren, en het Type van Uur.</td> 
  </tr> 
  <tr> 
   <td>Kosten van arbeidskosten en uitgaven per maand en per kwartaal voor projecten</td> 
   <td>Een matrixprojectrapport waarin de geplande loonkosten, de werkelijke loonkosten, de geplande onkostenkosten en de werkelijke kosten van de projecten worden weergegeven. Het rapport wordt gegroepeerd op de projectnaam en het kwartaal en de maand van de werkelijke begindatum van de projecten.</td> 
  </tr> 
  <tr> 
   <td>Projectprestaties</td> 
   <td>Een projectverslag met de volgende gebieden van de lopende projecten: Vervaldatum, CPI, SPI, CSI, geplande kosten, begroting, OAG en kosten van de projecten.</td> 
  </tr> 
  <tr> 
   <td>Projectverzoeken</td> 
   <td>Een rapport van het Project dat gevraagde projecten toont. Het rapport bevat de volgende velden: Beschrijving, Geplande Voltooiingsdatum, Geprojecteerde Voltooiingsdatum, Percentage voltooid, Status en Prioriteit van de projecten.</td> 
  </tr> 
  <tr> 
   <td>Projecten op voorwaarde</td> 
   <td>Een rapport van het Project dat de Voorwaarde van de projecten toont. Het rapport wordt gegroepeerd door Voorwaarde, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Projecten op voorwaarde per groep</td> 
   <td>Een rapport van het Project dat de Status van de Voortgang en de Groep van de projecten toont. Het rapport wordt gegroepeerd door de Naam van de Groep en de Status van de Voortgang, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Projecten per prioriteit</td> 
   <td>Een projectrapport waarin de prioriteit van projecten wordt weergegeven. Het rapport wordt gegroepeerd op Prioriteit, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Projecten met status Voortgang</td> 
   <td>Een rapport van het Project dat de Voortgangsstatus van de projecten toont. Het rapport wordt gegroepeerd door de Status van de Voortgang, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Taken door Voortgangsstatus</td> 
   <td>Een rapport van de Taak dat de Voortgangsstatus van alle Taken in Huidige Projecten toont. Het rapport wordt gegroepeerd door de Status van de Voortgang, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Taken op status</td> 
   <td>Een rapport van de Taak dat de Status van alle taken toont. Het rapport wordt gegroepeerd door Status, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Te controleren tijdbladen</td> 
   <td>Een rapport Timesheet dat Voorgelegde en Geweigerde chronologiebladen toont de waarvan fiatteur de het programma geopende gebruiker is. Het rapport geeft de volgende velden weer: Datumbereik, Eigenaar, Totaal aantal uren, Overwerk, Naam fiatteur en Status van de tijdbladen.</td> 
  </tr> 
  <tr> 
   <td>Problemen met taken</td> 
   <td>Een rapport van de Taak dat onvolledige taken met een Status van de Voortgang van Late of Achter, een Datum van Handoff vroeger dan morgen toont en waar de het programma geopende gebruiker deel van het Team van het Project van het project uitmaakt de taken zijn. In het rapport worden de volgende velden weergegeven: Geplande duur, Projectnaam, primaire toewijzing, Geplande start, Geplande voltooiing, Percentage voltooiing en Prioriteit van de taken.</td> 
  </tr> 
  <tr> 
   <td>Aanmeldingsgegevens gebruiker</td> 
   <td>Een gebruikersrapport waarin de volgende velden worden weergegeven: de unieke id, het aantal aanmeldingen (het aantal keren dat de gebruiker zich heeft aangemeld sinds het begin van Workfront), de laatste aanmeldingsdatum van de gebruikers. Het rapport wordt gegroepeerd door het Niveau van de Toegang van de gebruikers.</td> 
  </tr> 
 </tbody> 
 <p><span class="wysiwyg-color-pink"></span> </p> 
</table>

## Toegang tot ingebouwde rapporten

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Section directly linked to "Getting Started with Workfront Reporting." Do not change/ rename.) </p>
-->

{{step1-click-main-menu}}

1. Klik **Rapporten**.
1. Klik **Alle Rapporten**.
1. Breid het **drop-down menu van de Filter** uit, en selecteer **Nieuwe Filter**.

1. Klik **toevoegen een Regel van de Filter**.
1. Op het **Begin typend gebiedsnaam** gebied, begin **Globale identiteitskaart** te typen.

1. Onder het **voorwerp van het Rapport**, uitgezochte **Globale identiteitskaart**.

1. In het drop-down menu van de filterbepaling, uitgezocht **is niet Leeg**.\
   ![ Globale filter van identiteitskaart voor systeemrapporten ](assets/qs-global-id-filter-for-system-reports-350x179.png)

1. Klik **sparen Filter**.\
   De rapportenlijst toont slechts ingebouwde rapporten.\
   Voor meer informatie over welke ingebouwde rapporten beschikbaar zijn, zie het sectie [ Overzicht van ingebouwde rapporten ](#overview-of-built-in-reports) in dit artikel.
