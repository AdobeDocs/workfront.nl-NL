---
product-area: reporting
navigation-topic: using-built-in-reports
title: Ingebouwde Adobe Workfront-rapporten gebruiken
description: Adobe Workfront heeft een uitgebreide lijst met ingebouwde rapporten die u kunt gebruiken.
author: Nolan
feature: Reports and Dashboards
exl-id: 32a47c25-192a-4e97-9016-42e6b6e201b9
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2997'
ht-degree: 0%

---

# Ingebouwde Adobe Workfront-rapporten gebruiken

Adobe Workfront heeft een uitgebreide lijst met ingebouwde rapporten die u kunt gebruiken.

Workfront-beheerders kunnen ingebouwde rapporten verbergen, zodat gebruikers er geen toegang toe hebben.\
Voor meer informatie over hoe te om ingebouwde rapporten te verbergen, zie [Ingebouwde rapporten verbergen](../../../administration-and-setup/manage-workfront/configure-reports/hide-built-in-reports.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Aanvraag of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders weergeven of vergroten</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten beheren voor een rapport om een filter toe te voegen aan of te bewerken in een rapport</p> <p>Machtigingen beheren voor een filter om het in een lijst te bewerken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Overzicht van ingebouwde rapporten {#overview-of-built-in-reports}

U kunt een ingebouwd rapport aanpassen en het opslaan als nieuw rapport. Voor meer informatie over het aanpassen van ingebouwde rapporten, zie [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

De volgende verslagen gaan over het Workfront-pakket. De rapporten zijn beschikbaar aan alle gebruikers die minstens de rechten van de Mening aan ingebouwde rapporten in hun toegangsniveau hebben.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Rapportnaam</strong> </th> 
   <th><strong>Beschrijving van rapport</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Werkelijke Portfolio-kosten per programma</td> 
   <td>Een projectrapport met de geplande kosten en de werkelijke kosten van de projecten. Het rapport wordt gegroepeerd door de Naam van het Programma, die door de Naam van de Portfolio wordt veroorzaakt, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Werkelijke Portfolio kosten per project</td> 
   <td>Een projectrapport met de geplande kosten en de werkelijke kosten van de projecten. Het rapport wordt gegroepeerd door de Naam van het Project, die door de Naam van Portfolio wordt veroorzaakt, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Werkelijke Portfolio ontvangsten per programma</td> 
   <td>Een projectverslag met de geplande inkomsten en de werkelijke inkomsten van de projecten. Het rapport wordt gegroepeerd door de Naam van het Programma, die door de Naam van de Portfolio wordt veroorzaakt, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Werkelijke Portfolio-inkomsten per project</td> 
   <td>Een projectverslag met de geplande inkomsten en de werkelijke inkomsten van de projecten. Het rapport wordt gegroepeerd door de Naam van het Project, die door de Naam van Portfolio wordt veroorzaakt, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Werkelijke ontvangsten per onderneming</td> 
   <td>Een projectverslag met de werkelijke inkomsten en de onderneming van de projecten. Het rapport wordt gegroepeerd door de Naam van het Bedrijf, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Werkelijke ontvangsten per groep</td> 
   <td>Een projectrapport met de werkelijke inkomsten en de groep van projecten. Het rapport wordt gegroepeerd door de Naam van de Groep, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Alle geopende tijdbladen</td> 
   <td>Een rapport met een tijdlijnoverzicht waarin de geopende tijdbladen worden weergegeven. Het rapport geeft de volgende velden weer: de Waaier van de Datum, Naam van de Eigenaar, Totale Uren, Overuren, Naam van de Fiatteur, en Status van timesheets.</td> 
  </tr> 
  <tr> 
   <td>Goedkeuringstijdbladen (gevraagd)</td> 
   <td>Een rapport met een tijdlijnrapport waarin de ingediende of geweigerde tijdbladen met fiatteurs worden weergegeven. Het rapport geeft de volgende velden weer: de Waaier van de Datum, Eigenaar, Totale Uren, Overuren, Naam van de Fiatteur, en Status van timesheets. Het rapport is ingegeven door: Begindatum tijdpagina, Einddatum tijdpagina, Naam tijdbladbeoordelaar en Gebruikersnaam.</td> 
  </tr> 
  <tr> 
   <td>Risicoprojecten</td> 
   <td>Een projectrapport waarin de huidige en planningsprojecten worden weergegeven met de status "Op risico" of "In Trouble". Het rapport geeft de volgende velden weer: de beschrijving, de geplande uitvoeringsdatum, de voorspelde uitvoeringsdatum, het percentage dat is voltooid, de status en de prioriteit van de projecten. Het rapport wordt gegroepeerd door de Naam van de Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Factureringsopbrengsten per onderneming</td> 
   <td>Een projectrapport waarin de inkomsten van het bedrijf en de facturering van de projecten worden weergegeven. Het rapport wordt gegroepeerd door de Naam van het Bedrijf, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Factureringsontvangsten per groep</td> 
   <td>Een projectrapport met de factuuropbrengsten en de groep projecten. Het rapport wordt gegroepeerd door de Naam van de Groep, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Factureringsontvangsten per maand</td> 
   <td>Een rapport van het Verslag van de Facturering dat de Naam van het Project, de Inkomsten van de Facturering van het Project en de Datum van de Rekening van de factureringsverslagen toont. Het rapport wordt gegroepeerd door de maand van de FactureringsDatum van de het factureringsverslagen, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Voltooide problemen per week</td> 
   <td>Een Issue-rapport met de Actual Completion Date of the issues. Het rapport wordt gegroepeerd op de week van de Werkelijke Voltooiingsdatum van de kwesties en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Uitgaven per week door gebruiker voltooid</td> 
   <td>Een Issue-rapport met de werkelijke afwerkingsdatum en toewijzingen van de problemen. Het rapport wordt gegroepeerd op de primaire toegewezen persoon en op de week van de werkelijke afsluitende datum van de emissies, en bevat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Huidige projecten</td> 
   <td>Een projectrapport waarin alle huidige projecten worden weergegeven. Het rapport geeft de volgende velden weer: de beschrijving, de geplande uitvoeringsdatum, de voorspelde uitvoeringsdatum, het percentage dat is voltooid, de status en de prioriteit van de projecten.</td> 
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
   <td>Problemen per status</td> 
   <td>Een Issue-rapport waarin de status van problemen wordt weergegeven. Het rapport wordt gegroepeerd door Status van de kwesties, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Problemen per status en project</td> 
   <td>Een matrixrapport van de Kwestie dat de Status van kwesties in Huidige projecten en de Naam van het Project toont. Het rapport wordt gegroepeerd door de Naam van het Project en Status van de kwesties.</td> 
  </tr> 
  <tr> 
   <td>Arbeidskosten vs. onkostenkosten per Portfolio</td> 
   <td>Een projectrapport waarin de geplande loonkosten, de werkelijke loonkosten, de geplande onkostenposten en de werkelijke kosten van de projecten worden weergegeven. Het rapport wordt gegroepeerd door de Naam van de Portfolio, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Arbeidskosten vs. onkosten per programma</td> 
   <td>Een projectrapport waarin de geplande loonkosten, de werkelijke loonkosten, de geplande onkostenposten en de werkelijke kosten van de projecten worden weergegeven. Het rapport wordt gegroepeerd door de Naam van de Portfolio en Naam van het Programma, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Voorziene maandelijkse Portfolio kosten in verhouding tot werkelijke kosten per project</td> 
   <td>Een matrixprojectrapport (financiële gegevens) met de datum van toewijzing, de totale geplande kosten, de totale werkelijke kosten en de totale kostenvariatie van de projecten. Het rapport wordt gegroepeerd op de Naam van het Project, het kwartaal en de maand van de Datum van de Toewijzing.</td> 
  </tr> 
  <tr> 
   <td>Voorziene maandelijkse Portfolio-inkomsten vs. Werkelijk per project</td> 
   <td>Een matrixprojectrapport (financiële gegevens) met de datum van toewijzing, de totale geplande inkomsten, de totale werkelijke inkomsten en de totale variatie in inkomsten van de projecten. Het rapport wordt gegroepeerd op de Naam van het Project, het kwartaal en de maand van de Datum van de Toewijzing.</td> 
  </tr> 
  <tr> 
   <td>Voorziene maandelijkse projectkosten versus werkelijke kosten</td> 
   <td>Een matrixprojectrapport (financiële gegevens) met de datum van toewijzing, de totale geplande kosten, de totale werkelijke kosten en de totale kostenvariatie van de projecten. Het rapport wordt gegroepeerd door de Naam van het Project, het kwartaal en de maand van de Datum van de Toewijzing en door de Naam van het Project veroorzaakt.</td> 
  </tr> 
  <tr> 
   <td>Voorziene jaarlijkse inkomsten uit het project versus werkelijke inkomsten</td> 
   <td>Een matrixprojectrapport (financiële gegevens) met de datum van toewijzing, de totale geplande inkomsten, de totale werkelijke inkomsten en de totale variatie in inkomsten van de projecten. Het rapport wordt gegroepeerd door de Naam van het Project, het kwartaal en de maand van de Datum van de Toewijzing en door de Naam van het Project veroorzaakt.</td> 
  </tr> 
  <tr> 
   <td>Mijn documenten</td> 
   <td>Een documentrapport waarin documenten worden weergegeven die door de aangemelde gebruiker zijn geüpload. Het rapport geeft de volgende velden weer: De naam van de eigenaar, Gewijzigde datum, Grootte, Aantal versies, Bron en Type van de documenten.</td> 
  </tr> 
  <tr> 
   <td>Mijn favorieten</td> 
   <td>Een rapport Favorieten waarin een lijst met objecten wordt weergegeven die door de aangemelde gebruiker als favorieten zijn gemarkeerd. Het rapport geeft de volgende velden weer: het Objecttype en de naam van de favorieten.</td> 
  </tr> 
  <tr> 
   <td>Mijn problemen</td> 
   <td>Een rapport van de Kwestie dat onvolledige Kwesties toont die aan de gebruiker worden toegewezen die het programma wordt geopend. Het rapport geeft de volgende velden weer: Bronnaam, Type uitgave, primaire ontvanger, Invoerdatum, Status en Prioriteit van de uitgaven.</td> 
  </tr> 
  <tr> 
   <td>Mijn Portfolio</td> 
   <td>Een rapport van Portfolio dat actieve Portfolio toont waar de het programma geopende gebruiker de Manager van de Portfolio is.</td> 
  </tr> 
  <tr> 
   <td>Mijn programma's</td> 
   <td>Een rapport van het Programma dat Programma's en hun Beschrijving toont, waar de het programma geopende gebruiker de Manager van het Programma is.</td> 
  </tr> 
  <tr> 
   <td>Problemen met het openen van mijn project</td> 
   <td>Een rapport van de Kwestie dat onvolledige kwesties in projecten toont het waarvan Team van het Project de het programma geopende gebruiker omvat. Het rapport geeft de volgende velden weer: Bronnaam, Type uitgave, primaire ontvanger, Invoerdatum, Status en Prioriteit van de uitgaven.</td> 
  </tr> 
  <tr> 
   <td>Mijn projecten</td> 
   <td>Een rapport van het Project dat Huidige projecten toont het waarvan Team van het Project de het programma geopende gebruiker omvat. Het rapport geeft de volgende velden weer: de beschrijving, de geplande uitvoeringsdatum, de voorspelde uitvoeringsdatum, het percentage dat is voltooid, de status en de prioriteit van de projecten.</td> 
  </tr> 
  <tr> 
   <td>Mijn verzonden problemen</td> 
   <td>Een Issue-rapport waarin de problemen worden weergegeven die zijn ingediend door de aangemelde gebruiker en die de afgelopen drie maanden zijn gesloten of momenteel zijn geopend. Het rapport geeft de volgende velden weer: Bronnaam, Type uitgave, Invoerdatum, Status en Prioriteit van de problemen.</td> 
  </tr> 
  <tr> 
   <td>Mijn taken</td> 
   <td>Een rapport van de Taak dat onvolledige taken in Huidige Projecten toont die aan de het programma geopende gebruiker worden toegewezen. Het rapport geeft de volgende velden weer: de geplande duur, de naam van het project, de primaire toegewezen persoon, het geplande begin, de geplande voltooiing, de Percentage van de voltooiing, en de Prioriteit van de taken.</td> 
  </tr> 
  <tr> 
   <td>Mijn tijdbladen</td> 
   <td>Een rapport Timesheet dat alle timesheets van de het programma geopende gebruiker toont. Het rapport geeft de volgende velden weer: de Waaier van de Datum, Naam van de Eigenaar, Totale Uren, Overuren, Naam van de Fiatteur, en Status van timesheets.</td> 
  </tr> 
  <tr> 
   <td>Mijn niet-toegewezen problemen</td> 
   <td>Een rapport van de Kwestie dat open kwesties toont die aan om het even welke baanrollen van de aangemelde gebruiker worden toegewezen en die niet aan de gebruiker worden toegewezen. Het rapport geeft de volgende velden weer: Bronnaam, Type uitgave, Invoerdatum, Status en Prioriteit van de problemen.</td> 
  </tr> 
  <tr> 
   <td>Mijn niet toegewezen taken</td> 
   <td>Een rapport van de Taak dat onvolledige taken toont die aan om het even welke baan rollen van de het programma geopende gebruiker worden toegewezen en niet aan de gebruiker worden toegewezen. Het rapport geeft de volgende velden weer: de geplande duur, de naam van het project, de primaire toewijzing, de geplande begindatum, de geplande uitvoeringsdatum, het percentage van de voltooiing en de prioriteit van de taken.</td> 
  </tr> 
  <tr> 
   <td>Mijn komende taken</td> 
   <td>Een rapport van de Taak dat onvolledige taken toont die in de volgende twee weken zouden moeten beginnen, is op Huidige projecten, en toegewezen aan de het programma geopende gebruiker. Het rapport geeft de volgende velden weer: de projectnaam, de geplande uitvoeringsdatum, de voorspelde uitvoeringsdatum, het percentage dat is voltooid en de status van de taken.</td> 
  </tr> 
  <tr> 
   <td>Tijdbladen openen (gevraagd)</td> 
   <td>Een rapport met een tijdlijnoverzicht waarin de geopende tijdbladen worden weergegeven. Het rapport geeft de volgende velden weer: de Waaier van de Datum, Eigenaar, Totale Uren, Overuren, Naam van de Fiatteur, Status van timesheets. Het rapport is ingegeven door: Begindatum tijdpagina, Einddatum tijdpagina, Naam tijdbladbeoordelaar en Gebruikersnaam.</td> 
  </tr> 
  <tr> 
   <td>Boekprojecten per Portfolio</td> 
   <td>Een projectrapport met de geplande kosten en de werkelijke kosten van de projecten. Het rapport wordt gegroepeerd door de Naam van de Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Voorziene Portfolio-kosten per programma</td> 
   <td>Een projectrapport met de geplande kosten en de werkelijke kosten van de projecten. Het rapport wordt veroorzaakt door de Naam van de Portfolio, die door de Naam van het Programma wordt gegroepeerd, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Voorziene Portfolio-kosten per project</td> 
   <td>Een projectrapport met de geplande kosten en de werkelijke kosten van de projecten. Het rapport wordt veroorzaakt door de Naam van de Portfolio, die door de Naam van het Project wordt gegroepeerd, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Geplande ontvangsten Portfolio per programma</td> 
   <td>Een projectverslag met de geplande inkomsten en werkelijke inkomsten van de projecten. Het rapport wordt veroorzaakt door de Naam van de Portfolio, die door de Naam van het Programma wordt gegroepeerd, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Geplande Portfolio-inkomsten per project</td> 
   <td>Een projectverslag met de geplande inkomsten en werkelijke inkomsten van de projecten. Het rapport wordt veroorzaakt door de Naam van de Portfolio, die door de Naam van het Project wordt gegroepeerd, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Geplande versus werkelijke kosten per Portfolio</td> 
   <td>Een projectrapport met de geplande kosten en werkelijke kosten van de projecten per Portfolio. Het rapport wordt gegroepeerd door de Naam van de Portfolio, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Geplande versus werkelijke kosten per programma</td> 
   <td>Een projectrapport met de geplande kosten en werkelijke kosten van de projecten per programma. Het rapport wordt gegroepeerd door de Naam van de Portfolio, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Geplande versus werkelijke inkomsten van Portfolio</td> 
   <td>Een projectverslag met de geplande inkomsten en de werkelijke inkomsten van de projecten. Het rapport wordt gegroepeerd door de Naam van de Portfolio, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Geplande versus werkelijke inkomsten per programma</td> 
   <td>Een projectverslag met de geplande inkomsten en de werkelijke inkomsten van de projecten. Het rapport wordt gegroepeerd door de Naam van het Programma, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Portfolio kosten gegroepeerd per programma en per maand</td> 
   <td>Een matrixprojectrapport waarin de geplande kosten, de begrote kosten en de werkelijke kosten van de projecten worden weergegeven. Het rapport wordt gegroepeerd op de Naam van Portfolio, de Naam van het Programma en de maand van de Geplande Datum van het Begin van de projecten.</td> 
  </tr> 
  <tr> 
   <td>Portfolio-projecten per status gegroepeerd op programma</td> 
   <td>Een projectrapport waarin de status van de projecten wordt weergegeven. Het rapport wordt gegroepeerd door de Naam van het Programma en de Status van het Project, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Portfolio Projecten gegroepeerd op status en Portfolio</td> 
   <td>Een projectrapport waarin de naam van de Portfolio en de status van de projecten worden weergegeven. Het rapport wordt gegroepeerd door de Naam van de Portfolio en de Status van de projecten, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Portfolio Ontvangsten per programma</td> 
   <td>Een projectverslag met de naam van de Portfolio, de naam van het programma, de geplande inkomsten en de werkelijke inkomsten van de projecten. Het rapport wordt gegroepeerd door de Naam van de Portfolio en de Naam van het Programma, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Portfolio Ontvangsten gegroepeerd per programma en per maand</td> 
   <td>Een matrixprojectrapport met de geplande inkomsten, werkelijke inkomsten, naam van de Portfolio en naam van het programma. Het rapport wordt gegroepeerd op de naam van de Portfolio, de naam van het programma en de maand van de geplande begindatum van de projecten.</td> 
  </tr> 
  <tr> 
   <td>Projectkosten en ontvangsten per taakstatus</td> 
   <td>Een matrixtaakrapport waarin de geplande kosten, werkelijke kosten, geplande inkomsten, werkelijke inkomsten en de projectnaam van de taken worden weergegeven. Het rapport wordt gegroepeerd door de Naam en Status van het Project van de taken.</td> 
  </tr> 
  <tr> 
   <td>Projectkosten vs. inkomsten van Portfolio</td> 
   <td>Een projectrapport met de naam van de Portfolio, de werkelijke kosten en de werkelijke inkomsten van de projecten. Het rapport wordt gegroepeerd door de Naam van de Portfolio, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Projectkosten per maand en per kwartaal</td> 
   <td>Een matrixkostenrapport met de datum van binnenkomst, het geplande bedrag, het werkelijke bedrag en het project van de uitgaven. Het rapport wordt gegroepeerd op de projectnaam, het kwartaal en de maand van de datum van binnenkomst van de uitgaven.</td> 
  </tr> 
  <tr> 
   <td>Kosten per uur per maand voor project</td> 
   <td>Een matrixuurrapport waarin de volgende velden worden weergegeven: Uren, Invoerdatum, Werkelijke kosten van de projecten, Uurtype, Projectnaam. Het rapport wordt gegroepeerd door de Naam van het Project, maand van de Datum van de Ingang van de uren, en het Type van Uur.</td> 
  </tr> 
  <tr> 
   <td>Kosten van arbeidskosten en uitgaven per maand en per kwartaal voor projecten</td> 
   <td>Een matrixprojectrapport waarin de geplande loonkosten, de werkelijke loonkosten, de geplande onkostenposten en de werkelijke kosten van de projecten worden weergegeven. Het rapport wordt gegroepeerd op de projectnaam en het kwartaal en de maand van de werkelijke begindatum van de projecten.</td> 
  </tr> 
  <tr> 
   <td>Projectprestaties</td> 
   <td>Een projectrapport dat de volgende gebieden van Huidige projecten toont: de uiterste datum, de CPI, de SPI, de CSI, de geplande kosten, de begroting, de OAG en de kosten van de projecten.</td> 
  </tr> 
  <tr> 
   <td>Projectverzoeken</td> 
   <td>Een rapport van het Project dat Gevraagde projecten toont. Het rapport geeft de volgende velden weer: de beschrijving, de geplande uitvoeringsdatum, de voorspelde uitvoeringsdatum, het percentage dat is voltooid, de status en de prioriteit van de projecten.</td> 
  </tr> 
  <tr> 
   <td>Projecten op voorwaarde</td> 
   <td>Een rapport van het Project dat de Voorwaarde van de projecten toont. Het rapport wordt gegroepeerd door Voorwaarde, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Projecten op voorwaarde per groep</td> 
   <td>Een projectrapport waarin de status van de voortgang en de groep projecten worden weergegeven. Het rapport wordt gegroepeerd door de Naam van de Groep en de Status van de Voortgang, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Projecten per prioriteit</td> 
   <td>Een projectrapport waarin de prioriteit van projecten wordt weergegeven. Het rapport wordt gegroepeerd op Prioriteit, en het omvat een grafiek.</td> 
  </tr> 
  <tr> 
   <td>Projecten met status Voortgang</td> 
   <td>Een projectrapport waarin de status van de voortgang van de projecten wordt weergegeven. Het rapport wordt gegroepeerd door de Status van de Voortgang, en het omvat een grafiek.</td> 
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
   <td>Een rapport Timesheet dat Voorgelegde en Geweigerde timesheets toont de waarvan fiatteur de het programma geopende gebruiker is. Het rapport geeft de volgende velden weer: de de Waaier van de Datum, Eigenaar, Totale Uren, Overuren, Naam van de Fiatteur en Status van timesheets.</td> 
  </tr> 
  <tr> 
   <td>Problemen met taken</td> 
   <td>Een rapport van de Taak dat onvolledige taken met een Status van de Voortgang van Late of Achter, een Datum van Handoff vroeger dan morgen toont en waar de het programma geopende gebruiker deel van het Team van het Project van het project uitmaakt de taken zijn. Het rapport geeft de volgende velden weer: Geplande duur, projectnaam, primaire toegewezen persoon, gepland begin, geplande voltooiing, percentage voltooid en prioriteit van de taken.</td> 
  </tr> 
  <tr> 
   <td>Aanmeldingsgegevens gebruiker</td> 
   <td>Een gebruikersrapport waarin de volgende velden worden weergegeven: de unieke id, Aantal aanmelding (het aantal keren dat de gebruiker zich heeft aangemeld vanaf Workfront), Datum laatste aanmelding van de gebruikers. Het rapport wordt gegroepeerd door het Niveau van de Toegang van de gebruikers.</td> 
  </tr> 
 </tbody> 
 <p><span class="wysiwyg-color-pink"></span> </p> 
</table>

## Toegang tot ingebouwde rapporten

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Section directly linked to "Getting Started with Workfront Reporting." Do not change/ rename.) </p>
-->

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront.
1. Klikken **Rapporten**.
1. Klikken **Alle rapporten**.
1. Breid uit **Filter** en selecteert u **Nieuw filter**.

1. Klikken **Filterregel toevoegen**.
1. In de **Typ de veldnaam** veld, beginnen met typen **Algemene id**.

1. Onder de **Rapport** object, selecteren **Algemene id**.

1. Selecteer in de keuzelijst met filteropties de optie **Is niet leeg**.\
   ![](assets/qs-global-id-filter-for-system-reports-350x179.png)

1. Klikken **Filter opslaan**.\
   De rapportenlijst toont slechts ingebouwde rapporten.\
   Voor meer informatie over welke ingebouwde rapporten beschikbaar zijn, zie [Overzicht van ingebouwde rapporten](#overview-of-built-in-reports).
