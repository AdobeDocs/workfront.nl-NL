---
title: Toegang krijgen tot de lijst met systeemuitgiftestatussen
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Met de status van een uitgave kunt u gebruikers in het systeem laten zien in welk ontwikkelingsstadium een uitgave zich op een bepaald moment bevindt.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9bdaec2f-acdf-4cbf-a308-ebcc861dbb89
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 0%

---

# Toegang krijgen tot de lijst met systeemuitgiftestatussen

Met de status van een uitgave kunt u gebruikers in het systeem laten zien in welk ontwikkelingsstadium een uitgave zich op een bepaald moment bevindt.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

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
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Status van toegangskwesties

U kunt tot systeem-vlakke uitgiftestatussen toegang hebben en wijzigen. U kunt bepaalde informatie over de standaardsysteemstatus bewerken of u kunt nieuwe aangepaste statussen maken. Ga voor meer informatie over het maken van aangepaste statussen of het bewerken van systeemstatussen naar [Een status maken of bewerken](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Toegang krijgen tot uitgiftestatussen op systeemniveau:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Projectvoorkeuren** > **Statussen**.

1. Klik op de knop **Problemen** om de uitgiftestatus te bekijken die beschikbaar is in Workfront.

   ![](assets/issue-status.png)

## Statussen van systeemuitgiften

Workfront wordt geleverd met 10 oorspronkelijke uitgiftestatussen. De eerste 4 in de tabel hieronder zijn vereist. Dit betekent dat u de bestanden kunt ontgrendelen, hernoemen en opnieuw ordenen, maar dat u ze niet kunt verbergen of verwijderen.

U kunt aangepaste uitgiftestatussen toevoegen aan de behoeften van uw organisatie. Zie voor meer informatie [Een status maken of bewerken](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Voor gebruikers is het wijzigen van de status van een uitgave doorgaans een handmatig proces. Er zijn echter situaties, die in de volgende lijst worden beschreven, waarin de status van een uitgave automatisch verandert, afhankelijk van andere factoren die zich in het systeem voordoen.

De volgende uitgavestatussen worden bij uw Workfront-exemplaar geleverd:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Status van systeemafgifte</th> 
   <th>Hoe u de status kunt gebruiken</th> 
   <th>Wat gebeurt er in de status</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nieuw (vereiste status)</td> 
   <td>Dit is de standaardstatus voor elke nieuwe uitgave.</td> 
   <td>Als de kwestie op een project in een status van Huidig is, toont de kwestie op het lusje van de Verzoeken van het Werk van de gebruikers die aan de kwestie worden toegewezen. Gebruikers kunnen nu aan dit probleem beginnen te werken.</td> 
  </tr> 
  <tr> 
   <td>Bezig (vereiste status)</td> 
   <td> <p>U kunt een probleem in deze status plaatsen om aan te geven dat het werk aan dat probleem is begonnen.</p> <p>Als de oplossing van de kwestie met een ander voorwerp (een taak, een project, of een andere kwestie) wordt verbonden, wordt de status van de kwestie veranderd automatisch in Bezig, wanneer u de status van het het oplossen voorwerp in Bezig verandert. </p> <p>Zie voor meer informatie over het omzetten van objecten <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overzicht van Oplossende en Oplosbare objecten </a>.</p> </td> 
   <td> <p>Als de kwestie op een project in een status van Huidig is, toont de kwestie in het Werken aan lusje van de gebruikers die aan de kwestie worden toegewezen.</p> <p>Wanneer een probleem in uitvoering is, geeft de uitgave een waarde weer voor de werkelijke begindatum.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Gesloten (vereiste status)</td> 
   <td> <p>U kunt een kwestie manueel als Gesloten merken wanneer het werk aan het wordt voltooid. </p> <p>Als de oplossing van de kwestie met een ander voorwerp (een taak, een project, of een andere kwestie) wordt verbonden, wordt de uitgiftestatus automatisch veranderd in Gesloten, wanneer u de status van het het oplossen voorwerp in Gesloten verandert.</p> <p>Zie voor meer informatie over het omzetten van objecten <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overzicht van Oplossende en Oplosbare objecten </a>.</p> </td> 
   <td> <p>Wanneer een kwestie wordt gesloten, wordt de kwestie verwijderd uit de Werkgroep van de ontvanger aan lijst. In dit geval geeft de uitgave een waarde weer voor de datum van feitelijke voltooiing. </p> <p>Wanneer alle taken worden voltooid en de kwesties op een project worden gesloten, kan het project worden voltooid.</p> </td> 
  </tr> 
  <tr> 
   <td>In de wachtstand (vereiste status)</td> 
   <td> <p>U kunt een probleem handmatig markeren als In wachtstand om aan te geven dat er een vertraging is opgetreden bij het voltooien van de uitgave. </p> </td> 
   <td> <p>Als de kwestie op een project in een status van Huidig is, toont de kwestie in het Werken aan lusje van de gebruikers die aan de kwestie worden toegewezen. </p> <p>Wanneer alle taken op een project worden voltooid, maar er minstens één kwestie van de Greep op het project is, kan het project niet worden voltooid. </p> </td> 
  </tr> 
  <tr> 
   <td>Heropend (komt overeen met Bezig)</td> 
   <td> <p>U kunt een kwestie in deze status plaatsen om erop te wijzen dat het werk aan die kwestie niet volledig was toen de kwestie eerder werd gesloten, en het moest worden heropend om het werk te voltooien.</p> </td> 
   <td> <p>Als de kwestie op een project in een status van Huidig is, toont de kwestie op het lusje van de Verzoeken van het Werk van de gebruikers die aan de kwestie worden toegewezen. Gebruikers kunnen nu aan dit probleem beginnen te werken.</p> <p>Deze status is belangrijk bij de rapportage, om onderscheid te maken tussen kwesties die voor het eerst open zijn (gewoonlijk in de Nieuwe status), en kwesties die worden geopend nadat ze eerder zijn gesloten (gewoonlijk in de Heropende status). </p> </td> 
  </tr> 
  <tr> 
   <td>Nog geen feedback (komt overeen met In wachtstand)</td> 
   <td>Je kunt een probleem in deze status plaatsen om aan te geven dat je wacht op feedback (doorgaans via de primaire contactpersoon) voordat je aan het probleem kunt blijven werken. </td> 
   <td> <p>Als de kwestie op een project in een status van Huidig is, toont de kwestie in het Werken aan lusje van de gebruikers die aan de kwestie worden toegewezen.</p> <p>Als er een probleem is dat nog geen feedback heeft, kan een project niet worden voltooid.</p> <p>Deze status is belangrijk in rapportage, om onderscheid te maken tussen kwesties die momenteel open zijn maar waaraan wordt gewerkt (gewoonlijk in de status In uitvoering) en kwesties die momenteel open zijn maar waaraan niet wordt gewerkt omdat meer feedback nodig is om deze te voltooien (meestal in de status Wachtende feedback).</p> </td> 
  </tr> 
  <tr> 
   <td>Kan niet dupliceren (komt overeen met gesloten)</td> 
   <td>U kunt een probleem in deze status plaatsen om aan te geven dat u het probleem sluit, maar u kunt het probleem dat het openen van het probleem heeft veroorzaakt, niet zien. Het probleem bestaat misschien nog, maar het kan niet op een bepaald moment worden herhaald. </td> 
   <td> <p>Deze status is belangrijk bij de rapportage, om onderscheid te maken tussen problemen die zijn voltooid en waarvan het probleem is opgelost (meestal in de status Gesloten) en problemen waarvan het probleem op een bepaald moment niet zichtbaar is (meestal in de status Kan niet dupliceren).</p> <p>Wanneer een probleem is gemarkeerd als Kan niet dupliceren, wordt het probleem verwijderd uit de lijst Werkgroep van de ontvanger. In dit geval geeft de uitgave een waarde weer voor Actual CompletionDate.</p> <p>Als alle taken op een project worden voltooid, en sommige kwesties in niet kunnen status dupliceren zijn, kan het project worden voltooid.</p> </td> 
  </tr> 
  <tr> 
   <td>Opgelost (komt overeen met Gesloten)</td> 
   <td>U kunt een probleem in deze status plaatsen om aan te geven dat u het probleem sluit en dat het probleem waardoor het is ontstaan, is opgelost.</td> 
   <td> <p>Deze status is belangrijk bij de rapportage, om onderscheid te maken tussen kwesties die met of zonder een oplossing zijn gesloten (gewoonlijk in de status Gesloten) en kwesties die met een werkelijke resolutie zijn afgesloten (gewoonlijk in de status van Opgelost).</p> <p>Wanneer een probleem is gemarkeerd als Opgelost, wordt het probleem verwijderd uit de lijst Werkgroep van de ontvanger. In dit geval geeft de uitgave een waarde weer voor de datum van feitelijke voltooiing.</p> <p>Als alle taken op een project worden voltooid, en minstens één kwestie in een Resolved status is, kan het project worden voltooid. </p> </td> 
  </tr> 
  <tr> 
   <td>Geverifieerd voltooid (komt overeen met gesloten)</td> 
   <td>U kunt een probleem in deze status plaatsen om aan te geven dat u het probleem sluit en dat u hebt gecontroleerd of het probleem dat het probleem heeft veroorzaakt, is opgelost.</td> 
   <td> <p>Wanneer een probleem is gemarkeerd als Geverifieerd voltooid, wordt het probleem verwijderd uit de lijst Werkgroep van de ontvanger. In dit geval geeft de uitgave een waarde weer voor de datum van feitelijke voltooiing.</p> <p>Als alle taken op een project worden voltooid, en sommige kwesties in een Verified Volledige status zijn, kan het project worden voltooid.</p> </td> 
  </tr> 
  <tr> 
   <td>Geen oplossing (komt overeen met gesloten)</td> 
   <td>U kunt een probleem in deze status plaatsen om aan te geven dat u het probleem sluit, maar het probleem dat het heeft veroorzaakt, kan niet worden opgelost.</td> 
   <td> <p>Deze status is belangrijk bij de rapportage, om onderscheid te maken tussen kwesties die met of zonder een oplossing zijn gesloten (gewoonlijk in de status Gesloten) en kwesties die zonder een daadwerkelijke resolutie zijn gesloten (gewoonlijk in de status van Won't Resolve).</p> <p>Wanneer een probleem wordt gemarkeerd als Geen oplossing, wordt het probleem verwijderd uit de lijst Werkgroep van de ontvanger. In dit geval geeft de uitgave een waarde weer voor de datum van feitelijke voltooiing.</p> <p>Als alle taken op een project worden voltooid, en minstens één kwestie in een Won is lost status niet op, kan het project worden voltooid.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Uitgiftestatussen aanpassen

Een Workfront-beheerder kan emissiestatussen op systeemniveau en op groepsniveau toevoegen aan Workfront en de volgorde wijzigen waarin gebruikers deze weergeven. Zie voor meer informatie [Een status maken of bewerken](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Een groepbeheerder kan een aangepaste status toevoegen die specifiek is voor één groep. Zie voor meer informatie [Een groepsstatus maken of bewerken](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
