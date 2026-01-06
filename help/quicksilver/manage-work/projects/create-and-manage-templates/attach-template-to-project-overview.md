---
content-type: overview
product-area: templates
keywords: overschrijven,veld,overschrijven
navigation-topic: templates-navigation-topic
title: Overzicht van het koppelen van een sjabloon aan een project
description: Wanneer u een malplaatje aan een bestaand project vastmaakt, wijzigt u sommige informatie over het project volgens dat van het malplaatje. Een deel van de informatie over het project blijft ongewijzigd.
author: Alina
feature: Work Management
exl-id: 7f0137b6-ce8e-4b66-ad55-e6dc2aae09d9
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 0%

---

# Overzicht van het koppelen van een sjabloon aan een project

Wanneer u een malplaatje aan een bestaand project vastmaakt, wijzigt u sommige informatie over het project volgens dat van het malplaatje. Een deel van de informatie over het project blijft ongewijzigd.

Voor informatie over hoe te om een malplaatje aan een project vast te maken, zie [ een malplaatje aan een project ](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md) vastmaken.

## Overwegingen bij het toevoegen van sjablonen aan projecten

Overweeg het volgende wanneer het toevoegen van malplaatjes aan projecten:

* U kunt alleen actieve sjablonen aan projecten koppelen.
* U kunt een malplaatje aan een project vastmaken wanneer het project in een status van Voltooid, Dead, of in In afwachting van Goedkeuring is, slechts wanneer uw beheerder van Adobe Workfront of een groepsbeheerder deze functionaliteit op het gebied van de Voorkeur van het Project heeft toegelaten. Voor informatie over het plaatsen van projectvoorkeur, zie [ systeem-brede projectvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.
* Tenzij u specifieke malplaatjetaken van wordt toegevoegd in het gehechtheidsproces uitsluiten, worden alle malplaatjetaken toegevoegd aan het bestaande project.
* De meeste sjablooninstellingen worden toegevoegd aan het project. Sommige projectinstellingen blijven behouden. Voor informatie, zie de sectie [ veranderingen in projectgebieden begrijpen wanneer het vastmaken van een malplaatje ](#understand-changes-to-project-fields-when-attaching-a-template) in dit artikel.

## Wijzigingen in projectvelden begrijpen bij het koppelen van een sjabloon {#understand-changes-to-project-fields-when-attaching-a-template}

>[!IMPORTANT]
>
>Het vastmaken van een malplaatje aan een project is niet het zelfde als het creëren van een project van een malplaatje. Wanneer u een project van een malplaatje creeert, brengen alle malplaatjegebieden over naar het nieuwe project. Bij het koppelen van een sjabloon blijven enkele bestaande projectvelden ongewijzigd.

Sommige malplaatjemontages brengen automatisch over naar het project, tenzij u hen specifiek merkt om tijdens het proces van de malplaatjegehechtheid worden uitgesloten. Wanneer u hen merkt om worden uitgesloten, worden de waarden van het projectgebied bewaard.

Nochtans, zijn niet alle projectgebieden beschikbaar om in het proces te leiden om een malplaatje aan een project vast te maken. Voor informatie, zie [ een malplaatje aan een project ](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md) vastmaken.

De volgende lijst beschrijft het gebrek voor wat met projectgebieden gebeurt wanneer u een malplaatje vastmaakt en welke gebieden u tijdens het gehechtheidsproces kunt beheren om het standaardgedrag met voeten te treden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Veld</td> 
   <td>Wat gebeurt er standaard tijdens het koppelen van een sjabloon?</td> 
   <td>Mogelijkheid om de veldupdates te beheren in het bijlageproces </td> 
  </tr> 
  <tr> 
   <td>Beschrijving</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Status</p> </td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td>Wordt overgedragen van een sjabloon als het veld leeg is in het project</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Prioriteit</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Type voorwaarde</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Planningsmodus</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Geplande data</td> 
   <td>Wijzigen op basis van de toegevoegde taken</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Werkelijke datums</td> 
   <td>Wijzigen op basis van de toegevoegde taken</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programma</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Groep</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bedrijf</td> 
   <td>Wordt overgedragen van een sjabloon als het veld leeg is in het project</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Geplande uren</td> 
   <td>Wijzigen op basis van de toegevoegde taken</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Projecteigenaar</td> 
   <td>Wordt overgedragen van een sjabloon als het veld leeg is in het project</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Projectsponsor</td> 
   <td>Wordt overgedragen van een sjabloon als het veld leeg is in het project</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Resource Manager</td> 
   <td>Toegevoegd aan de lijst van bestaande middelmanagers op het project</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aangepaste Forms</td> 
   <td>Toegevoegd aan het project, naast formulieren die al in het project staan</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Begroting</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Valuta</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>PIM</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>EAC</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gepland voordeel</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Werkelijk voordeel</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mijlpad</td> 
   <td>Wordt overgedragen van een sjabloon als het veld leeg is in het project</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Voltooiingsmodus</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Samenvattingsmodus</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Type update</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Schema</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gebruikerstijd uit</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modus Bronniveaus</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risico (projectveld)</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Brongroepen</td> 
   <td>Toegevoegd aan de lijst met bestaande bronnenpools in het project</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Uurtypen</td> 
   <td> <p>Als deze optie tijdens het bijlageproces niet is geselecteerd, blijft de instelling Uurtypen voor het project ongewijzigd. </p> <p>Indien geselecteerd, brengt het malplaatje het plaatsen over naar het project. Als het filtreren van het Type van Uur aan ja zowel op het project als het malplaatje wordt geplaatst, worden de uurtypes van het malplaatje toegevoegd aan degenen op het project.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Herinneringsmeldingen</td> 
   <td> <p>Toegevoegd aan de lijst met bestaande herinneringen voor het project. </p> <p>Als deze optie tijdens het bijlageproces is uitgeschakeld, blijven de meldingen voor de herinnering aan het project ongewijzigd. </p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Standaardgoedkeuringsproces taak</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Standaard aangepaste Forms</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Werkinspanning</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span> staat gebruikers toe om kwesties inline toe te voegen </span> </td> 
   <td><span> de informatie van het Project wordt bewaard </span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Alle instellingen</td> 
   <td>De montages van het malplaatje beschrijven die van het project</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Taken</td> 
   <td>Toegevoegd aan de bodem van de taaklijst, naast de bestaande projecttaken</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Documenten</td> 
   <td>Toegevoegd aan het project, naast bestaande projectdocumenten</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Risico's (objecten in het risicogebied van het project)</td> 
   <td>Toegevoegd aan het project, naast bestaande projectrisico's </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Goedkeuringsproces</td> 
   <td>Van sjabloon overgedragen</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Factureringstarieven</td> 
   <td> <p>Overgeboekt van een sjabloon naast de bestaande factureringstarieven voor het project. </p> <p>Als er een verschillend tarief voor de zelfde baanrol op zowel het project als het malplaatje is, blijft het tarief op het project onveranderd. </p> </td> 
   <td> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Factureringsgegevens</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Uitgaven</td> 
   <td>Van een sjabloon overgedragen naast de bestaande projectkosten</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Financiële informatie</td> 
   <td> <p>Wanneer dit in het gehechtheidsproces wordt geselecteerd, worden de volgende gebieden of overgebracht of toegevoegd aan het project: </p> 
    <ul> 
     <li> <p>Vaste kosten</p> <p>Wanneer de optie wordt geselecteerd, wordt de bijgewerkte Vaste Kosten van het project berekend gebruikend de volgende formule:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li> 
     <li> <p>Vaste inkomsten</p> <p>Wanneer de optie is geselecteerd, wordt de bijgewerkte vaste opbrengst van het project berekend aan de hand van de volgende formule:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li> 
     <li> <p>Type kosten voor taken</p> <p>Van sjabloon overgedragen</p> </li> 
     <li> <p>Inkomenssoort voor taken</p> <p>Van sjabloon overgedragen</p> </li> 
    </ul> <p>Als dit veld tijdens het bijlageproces niet is geselecteerd, gebeurt het volgende:</p> 
    <ul> 
     <li> <p>De vaste kosten en de vaste opbrengsten van het project blijven behouden.</p> </li> 
     <li> <p>De kosten en de Types van Inkomsten op de taken die van het malplaatje worden toegevoegd worden geplaatst aan Geen Kosten en niet Billable</p> </li> 
    </ul> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Uren</td> 
   <td>Projectinformatie blijft behouden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>De Details van de rij, de Groepen van het Onderwerp, de Onderwerpen van de Rij, die Regels verpletteren</td> 
   <td> <p>Van sjabloon overgedragen</p> <p>Als u de <strong> optie van de Eigenschappen van de Rij &amp; van de Opstelling van Kwesties </strong> tijdens het gehechtheidsproces selecteert, beschrijven de Details van de Rij van het malplaatje die van het project. In dit geval, worden de Verpletterende Regels, de Onderwerpen van de Rij, en de Groepen van het Onderwerp van het malplaatje toegevoegd aan die van het project. <br> als het project opstelling als verzoekrij is en het malplaatje u aan het project vastmaakt niet opstelling als verzoekrij, wordt de rijinformatie van het project verwijderd als u de <strong> gecontroleerde doos van de Eigenschappen &amp; van de Rij van de Rij </strong> verlaat. <br> als u de <strong> Eigenschappen van de Rij &amp; doos van de Opstelling van de Uitgave </strong> schrapt, worden alle montages van de Opstelling van de Rij van het project bewaard en geen montages van de Opstelling van de Rij van het malplaatje zijn in bijlage.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Taakbeperkingen</td> 
   <td> <p>Van sjabloon overgedragen </p> <p>Als deze optie tijdens het bijlageproces is uitgeschakeld, worden de taakbeperkingen zo snel mogelijk of zo laat mogelijk ingesteld, afhankelijk van het projectschema van het instellen. </p> </td> 
   <td> <p> </p> <p> </p> <p style="text-align: center;">✓</p> </td> 
  </tr> 
  <tr> 
   <td>Taakvoorgangers</td> 
   <td> <p>Van sjabloon overgedragen</p> <p>Als deze optie tijdens het bijlageproces is uitgeschakeld, worden alle eerdere verbindingen tussen de sjabloontaken verwijderd.</p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Opties voor delen</td> 
   <td> <p>Als deze optie niet is geselecteerd tijdens het bijlageproces, blijven de projectmachtigingen ongewijzigd.</p> <p>Als geselecteerd tijdens het gehechtheidsproces, worden de malplaatjetoestemmingen toegevoegd aan of die van het project beschrijven. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b> Voorbeeld: </b></span></span> als de Gebruiker A de toestemming van de Mening aan het project heeft, maar zij hebben leiden toestemmingen op het malplaatje, na het vastmaken van het malplaatjeGebruiker A zal toegang tot het project krijgen leiden.</p> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>



<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h2> </h2>
<h2>Understand changes to project fields when attaching a template</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and replaced with the table above, per Anna)</p>
-->
<!--
<p>Some template settings automatically transfer to the project, unless you specifically mark them to be excluded during the template attachment process. When you mark them to be excluded, the project field values are preserved. </p> <note type="important">
Not all project fields are available to manage in the process of attaching a template to a project. For information, see
<a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md" class="MCXref xref">Attach a template to a project</a>.
</note>
<p>The following scenarios exist when attaching a template to an existing project: </p>
<ul>
<li> <p><a href="#project-fields-that-are-empty-and-the-template-information-updates-them" class="MCXref xref">Project fields that are empty and the template information updates them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-the-template-information-overwrites-them" class="MCXref xref">Project fields that are populated and the template information overwrites them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-they-remain-unchanged-after-attaching-the-template" class="MCXref xref">Project fields that are populated and they remain unchanged after attaching the template</a> </p> </li>
</ul> <note type="important">
Attaching a template to a project is not the same as creating a project from a template. When you create a project from a template all template fields transfer to the new project. Attaching a template leaves some of the existing project's fields unchanged.
</note>
<p><strong>Project fields that are empty and the template information updates them</strong></p>
<p>Most project fields that are empty are populated with template information when attaching the template to an existing project. </p>
<p><strong>Project fields that are populated and the template information overwrites them</strong></p>
<p>The following fields always overwrite or update existing project information with template information when you attach a template to the project and they cannot be managed during attaching the template: </p>
<ul>
<li> <p><b>Resource manager</b>: The template Resource Managers are added to the list of existing resource managers on the project.</p> </li>
</ul>
<ul>
<li> <p><b>Financial Information</b>: You can indicate whether you want financial information to transfer from the template or to keep the existing financial information on the project in the process of attaching a template. However, when the Financial Information option is selected to indicate that you intend to keep the information from the template, the following fields are updated on the project: </p>
<ul>
<li> <p> The updated Fixed Cost of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li>
<li> <p>The updated Fixed Revenue of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li>
</ul> </li>
</ul>
<ul>
<li> <p><b>Filter Hour Types</b> </p> </li>
</ul>
<ul>
<li> <p><b>Access settings</b> </p> </li>
</ul>
<ul>
<li> <p><b>Custom Forms</b>: Template custom forms are added to the project, in addition to existing project custom forms. If the fields from the template custom forms already exist on the project and contain information, they preserve the information already on the project. You cannot edit them during attaching the template. </p> </li>
</ul>
<ul>
<li> <p><b>Start From</b> </p> </li>
</ul>
<p><strong>Project fields that are populated and they remain unchanged after attaching the template</strong></p>
<p>The following fields remain unchanged on the project, even if they are also populated on the template, and they cannot be managed during attaching the template: </p>
<ul>
<li> <p style="font-weight: bold;">URL</p> </li>
<li> <p style="font-weight: bold;">Project Owner</p> </li>
<li> <p style="font-weight: bold;">Project Sponsor</p> </li>
<li> <p style="font-weight: bold;">Group</p> </li>
<li> <p style="font-weight: bold;">Company</p> </li>
<li> <p style="font-weight: bold;">Currency</p> </li>
<li> <p style="font-weight: bold;">Milestone Path</p> </li>
<li> <p><b>Completion Mode</b> </p> </li>
<li> <p style="font-weight: bold;">Resource Pool</p> </li>
<li> <p style="font-weight: bold;">Tasks Settings fields</p> </li>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p style="font-weight: bold;">Issue Settings fields</p> </li>
</ul>
</div>
<p> </p>
</div>
-->


