---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Overzicht van de statussen van het Project van het Systeem
description: Workfront heeft 9 ingebouwde status van systeemprojecten. De eerste 3 in de tabel hieronder zijn vereist. Dit betekent dat u de clips kunt ontgrendelen, hernoemen en opnieuw ordenen, maar dat u ze niet kunt verbergen of verwijderen. Het wijzigen van de projectstatus is doorgaans een handmatig proces. Soms wordt de status van een project echter automatisch gewijzigd, afhankelijk van andere activiteiten die in het systeem plaatsvinden.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 6b8dd52b-1696-4e5d-bcbb-5b6d3b736df0
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1607'
ht-degree: 0%

---

# Overzicht van de status van systeemprojecten

<!--Audited: 12/2023-->

Workfront heeft 9 ingebouwde status van systeemprojecten.

De eerste 3 in de tabel hieronder zijn vereist. Dit betekent dat u de clips kunt ontgrendelen, hernoemen en opnieuw ordenen, maar dat u ze niet kunt verbergen of verwijderen.

Het wijzigen van de projectstatus is doorgaans een handmatig proces. Nochtans, zijn er sommige scenario&#39;s die in de volgende lijst worden geschetst wanneer een projectstatus automatisch, afhankelijk van andere activiteiten wordt veranderd die in het systeem gebeuren.

Workfront verschaft de volgende projectstatussen met uw Adobe Workfront-exemplaar:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th>Status van systeemproject</th> 
   <th>Deze projectstatus treedt op wanneer</th> 
   <th>Wat gebeurt er in deze status</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planning (vereiste status)</td> 
   <td> <p>De projectmanager plant de chronologie van het project, de taak van de taken, en de goedkeuringen. De projectmanager plaatst deze status manueel op een project.</p> <p><b>TIP</p> <p> Wij adviseren dat u de standaardstatus voor nieuwe projecten in Workfront aan Planning plaatst. Als beheerder van Workfront, kunt u de standaardstatus voor al uw nieuwe projecten op het gebied van Projecten van de Voorkeur van het Project veranderen.</p> <p>Voor meer informatie, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md"> systeem-brede projectvoorkeur </a> vormen.</p></td> 
   <td> <p>De gebruikers op het projectteam kunnen het project op hun lijsten van Projecten door gebrek (zonder een douanefilter), in het gebied van Projecten van Workfront zien. De taken en de kwesties die aan hen op het project worden toegewezen bevolken niet hun Lijst van het Werk. Alleen goedkeuringen en geaccepteerde werkitems worden weergegeven in de lijst Home Work.</p> <p>Er worden geen meldingen verzonden terwijl een project deze status heeft.</p> <p>Wij adviseren dat u alle veranderingen aanbrengt die een update aan de chronologie van het project, of om het even welke veranderingen in taken kunnen teweegbrengen en taken uitgeven terwijl het project in de status van de Planning is. Hierdoor wordt het aantal meldingen dat gebruikers ontvangen, tot een minimum beperkt.</p> <p>De tijdlijn van het project wordt niet automatisch berekend door het systeem.</p> </td> 
  </tr> 
  <tr> 
   <td>Huidige (vereiste status)</td> 
   <td> <p>Gebruikers werken aan taken en problemen in het project. De projectmanager zou een project aan Huidig moeten draaien om aan te geven dat het is begonnen.</p> <p>Dit is de standaardstatus voor nieuwe projecten in Workfront.</p> <p><b>TIP</b></p>

<p> Als beheerder van Workfront, kunt u de standaardstatus voor nieuwe projecten op het gebied van Projecten van de Voorkeur van het Project veranderen. Voor meer informatie, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref"> systeem-brede projectvoorkeur </a> vormen.</p> </td> 
   <td> <p>De gebruikers op het projectteam kunnen het project op hun lijsten van Projecten door gebrek (zonder een douanefilter), in het gebied van Projecten van Workfront zien. De taken en de kwesties die aan hen op het project worden toegewezen bevolken hun Lijst van het Werk. Ze kunnen beginnen met het accepteren van taken en problemen en ze verplaatsen naar de lijst Werken aan.</p> <p>Voor een Huidig project, worden alle berichten over chronologieveranderingen, taken, noodzakelijke acties, en goedkeuringen verzonden naar gebruikers op het projectteam.</p> <p>De chronologie van het project wordt automatisch berekend door het systeem, als het Type van Update van het project aan Automatisch, bij Verandering, of Automatisch en bij Verandering wordt geplaatst.</p> <p><b>TIP</b></p> <p> Het is een goed idee om de aanpassingen van het projectplan tot een minimum te houden wanneer een project in deze status is zodat de gebruikers niet teveel berichten ontvangen.</p> </td> 
  </tr> 
  <tr> 
   <td>Voltooid (vereiste status)</td> 
   <td> <p> Alle taken en problemen met het project worden voltooid en het project is voltooid.</p> 
     <p>Als de Wijze van de Voltooiing van het project aan Handboek wordt geplaatst, verkiest de projectmanager deze status manueel om gebruikers op het projectteam te informeren ophouden werkend aan het project.</p> 
    <p>Als de Voltooiingswijze van het project aan Automatisch wordt geplaatst, merkt Workfront automatisch een project als Voltooid wanneer alle taken en kwesties in het project als Voltooid worden gemerkt. 
    <p><b> BELANGRIJK </b> </p>
    <p>U kunt een project als Voltooid merken slechts wanneer alle taken, kwesties, en goedkeuringen op het project worden opgelost.</p> </td> 
   <td>
    <p>De gebruikers op het projectteam kunnen niet het project op hun lijsten van Projecten door gebrek (zonder een douanefilter), in het gebied van Projecten van Workfront zien. De taken en de kwesties die aan hen op het project worden toegewezen bevolken niet hun Verzoeken van het Werk of het Werken aan lijsten. </p>
    <p>Alle berichten met betrekking tot het project, behalve een bericht van de statusverandering, houden op worden verzonden naar de gebruikers op het projectteam.</p>
    <p>De tijdlijn van het project wordt niet meer berekend door het systeem. </p>
    <p>Kan het project niet kopiëren.</p>
    <p>U kunt voorkomen dat gebruikers extra handelingen uitvoeren wanneer een project is gemarkeerd als Voltooid. </p><p>Voor meer informatie over hoe te om acties op projecten te beperken die als Voltooid duidelijk zijn, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref"> systeem-brede projectvoorkeur </a> vormen.</p></td> 
  </tr> 
  <tr> 
   <td>Dead</td> 
   <td>Het project is nog niet voltooid, maar vanwege wegblokkades of wijzigingen in het bereik kan het project niet verder worden bewerkt en is het verlaten. De projectmanager verandert de status in Dead om de gebruikers op het projectteam te waarschuwen dat dit project nooit zal eindigen en zij zouden niet meer aan het moeten werken.</td> 
   <td> <p>De gebruikers op het projectteam kunnen niet het project op hun lijsten van Projecten door gebrek (zonder een douanefilter), in het gebied van Projecten van Workfront zien. De taken en de kwesties die aan hen op het project worden toegewezen verdwijnen uit hun Lijst van het Werk.</p> <p>Goedkeuringsbesluiten kunnen niet worden toegekend aan taken of kwesties.</p> <p>Meldingen over tijdlijnwijzigingen, toewijzingen, benodigde acties en goedkeuringen worden niet verzonden naar gebruikers in het projectteam.</p> <p>De tijdslijn van het project wordt niet automatisch berekend door het systeem, aangezien het project als voltooid wordt ervaren.</p> <p>U kunt gebruikers verhinderen bepaalde acties uit te voeren wanneer een project als Dode wordt gemerkt. Voor meer informatie over hoe te om acties op Dode projecten te beperken, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref"> systeem-brede projectvoorkeur </a> vormen.</p> </td> 
  </tr> 
  <tr> 
   <td>In de wachtstand</td> 
   <td>Het project is nog niet voltooid, maar vanwege enige vertraging moet het project tijdelijk worden opgeschort. De projectmanager verkiest om deze status te gebruiken om gebruikers in het projectteam te waarschuwen ophouden werkend aan het project, in de huidige tijd.</td> 
   <td> <p>De gebruikers op het projectteam kunnen niet het project op hun lijsten van Projecten door gebrek (zonder een douanefilter), in het gebied van Projecten van Workfront zien. De taken en de kwesties die aan hen op het project worden toegewezen verdwijnen uit hun Lijst van het Werk. </p> <p>Goedkeuringsbesluiten kunnen niet worden toegekend aan taken of kwesties.</p> <p>Meldingen over tijdlijnwijzigingen, toewijzingen, benodigde acties en goedkeuringen worden niet verzonden naar gebruikers in het projectteam.</p> <p> <p><b>OPMERKING</b></p>  <p>Wanneer u een project in de wachtstand plaatst, stopt de tijdlijn van het project niet. Het project kan nog steeds als Op Risico of In Problemen worden getoond, zelfs als niemand actief aan het project werkt. Het kan nodig zijn de datums van de resterende open taken handmatig aan te passen wanneer u het project weer terugzet op Current, zodat de voortgang van het project kan worden weergegeven.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>Gevraagd</td> 
   <td>De projectstatus wordt automatisch gemarkeerd als Gevraagd door het systeem, wanneer de bedrijfscase op een projectverzoek is voltooid en ter goedkeuring is voorgelegd. Voor meer informatie over het verzoeken van een project gebruikend een bedrijfsgeval, zie <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref"> Overzicht Gevraagde Projecten </a>.</td> 
   <td> <p>De gebruikers op het projectteam kunnen niet het project op hun lijsten van Projecten door gebrek (zonder een douanefilter), in het gebied van Projecten van Workfront zien. De taken en de kwesties op het project die aan hen worden toegewezen bevolken niet hun Lijst van het Werk.</p> <p>Alle meldingen met betrekking tot het project, met uitzondering van meldingen over statuswijziging, worden niet naar gebruikers verzonden.</p> <p>De tijdlijn van het project wordt niet automatisch berekend door het systeem.</p> </td> 
  </tr> 
  <tr> 
   <td>Goedgekeurd</td> 
   <td>De projectstatus wordt automatisch gemarkeerd als Goedgekeurd, wanneer de bedrijfscase op een projectverzoek is goedgekeurd. Voor meer informatie over het verzoeken van een project gebruikend een bedrijfsgeval, zie <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref"> Overzicht Gevraagde Projecten </a>.</td> 
   <td> <p>De gebruikers op het projectteam kunnen het project op hun lijsten van Projecten door gebrek (zonder een douanefilter), in het gebied van Projecten van Workfront zien. De taken en de kwesties die aan hen op het project worden toegewezen bevolken niet hun Lijst van het Werk.</p> <p>Alle meldingen met betrekking tot het project, met uitzondering van meldingen over statuswijziging, worden niet naar gebruikers verzonden.</p> <p>De tijdlijn van het project wordt niet automatisch berekend door het systeem. </p> </td> 
  </tr> 
  <tr> 
   <td>Geweigerd</td> 
   <td>De projectstatus wordt automatisch gemarkeerd als Geweigerd, wanneer de bedrijfscase op een projectverzoek is verworpen. Voor meer informatie over het verzoeken van een project gebruikend een bedrijfsgeval, zie <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref"> Overzicht Gevraagde Projecten </a>.</td> 
   <td> <p>De gebruikers op het projectteam kunnen niet het project op hun lijsten van Projecten door gebrek (zonder een douanefilter), in het gebied van Projecten van Workfront zien. De taken en de kwesties die aan hen op het project worden toegewezen bevolken niet hun Lijst van het Werk.</p> <p>Alle meldingen met betrekking tot het project, met uitzondering van meldingen over statuswijziging, worden niet naar gebruikers verzonden.</p> <p>De tijdlijn van het project wordt niet automatisch berekend door het systeem.</p> </td> 
  </tr> 
  <tr> 
   <td>Idea</td> 
   <td>De projectstatus wordt automatisch gemarkeerd als Idea wanneer u een projectverzoek indient, alvorens u de BedrijfsGeval voltooit. Voor meer informatie over het verzoeken van een project gebruikend een bedrijfsgeval, zie <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref"> Overzicht Gevraagde Projecten </a>.</td> 
   <td> <p>De gebruikers op het projectteam kunnen niet het project op hun lijsten van Projecten door gebrek (zonder een douanefilter), in het gebied van Projecten van Workfront zien. De taken en de kwesties die aan hen op het project worden toegewezen bevolken niet hun Lijst van het Werk.</p> <p>Alle meldingen met betrekking tot het project, met uitzondering van meldingen over statuswijziging, worden niet naar gebruikers verzonden.</p> <p>De tijdlijn van het project wordt niet automatisch berekend door het systeem.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>De volgende projectstatussen kunnen niet worden veranderd in een Dead, On Hold, of de Volledige status:
>
>* Gevraagd
>* Idea
>* Goedgekeurd
>* Afgewezen (of gelijkwaardig)
>
