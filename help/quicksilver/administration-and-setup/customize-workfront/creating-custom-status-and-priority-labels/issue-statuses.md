---
title: Toegang krijgen tot de lijst met systeemuitgiftestatussen
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Met de status van een uitgave kunt u gebruikers in het systeem laten zien in welk ontwikkelingsstadium een uitgave zich op een bepaald moment bevindt.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9bdaec2f-acdf-4cbf-a308-ebcc861dbb89
source-git-commit: 366043a786c94f1bc40ad3b20af175bb84c94742
workflow-type: tm+mt
source-wordcount: '1422'
ht-degree: 0%

---

# Toegang krijgen tot de lijst met systeemuitgiftestatussen

Met de status van een uitgave kunt u gebruikers in het systeem laten zien in welk ontwikkelingsstadium een uitgave zich op een bepaald moment bevindt.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>Systeembeheerder</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Status van toegangskwesties

U kunt tot systeem-vlakke uitgiftestatussen toegang hebben en wijzigen. U kunt bepaalde informatie over de standaardsysteemstatus bewerken of u kunt nieuwe aangepaste statussen maken. Voor meer informatie over het creëren van douanestatus of het uitgeven systeemstatussen, zie [ tot stand brengen of een status ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) uitgeven.

Toegang krijgen tot uitgiftestatussen op systeemniveau:

{{step-1-to-setup}}

1. Klik **Voorkeur van het Project** > **Statussen**.

1. Klik het **lusje van Kwesties** om de uitgevende statussen beschikbaar in Workfront te zien.

   ![ status van de Uitgave ](assets/issue-status.png)

## Statussen van systeemuitgiften

Workfront wordt geleverd met 10 oorspronkelijke uitgiftestatussen. De eerste 4 in de tabel hieronder zijn vereist. Dit betekent dat u de bestanden kunt ontgrendelen, hernoemen en opnieuw ordenen, maar dat u ze niet kunt verbergen of verwijderen.

U kunt aangepaste uitgiftestatussen toevoegen aan de behoeften van uw organisatie. Voor meer informatie, zie [ een status ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) creëren of uitgeven.

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
   <td> <p>U kunt een probleem in deze status plaatsen om aan te geven dat het werk aan dat probleem is begonnen.</p> <p>Als de oplossing van de kwestie met een ander voorwerp (een taak, een project, of een andere kwestie) wordt verbonden, wordt de status van de kwestie veranderd automatisch in Bezig, wanneer u de status van het het oplossen voorwerp in Bezig verandert. </p> <p>Voor meer informatie over het oplossen van voorwerpen, zie <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref"> Overzicht van het Oplossen van en Oplosbare Voorwerpen </a>.</p> </td> 
   <td> <p>Als de kwestie op een project in een status van Huidig is, toont de kwestie in het Werken aan lusje van de gebruikers die aan de kwestie worden toegewezen.</p> <p>Wanneer een probleem in uitvoering is, geeft de uitgave een waarde weer voor de werkelijke begindatum.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Gesloten (vereiste status)</td> 
   <td> <p>U kunt een kwestie manueel als Gesloten merken wanneer het werk aan het wordt voltooid. </p> <p>Als de oplossing van de kwestie met een ander voorwerp (een taak, een project, of een andere kwestie) wordt verbonden, wordt de uitgiftestatus automatisch veranderd in Gesloten, wanneer u de status van het het oplossen voorwerp in Gesloten verandert.</p> <p>Voor meer informatie over het oplossen van voorwerpen, zie <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref"> Overzicht van het Oplossen van en Oplosbare Voorwerpen </a>.</p> </td> 
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
   <td> <p>Deze status is belangrijk bij de rapportage, om onderscheid te maken tussen kwesties die met of zonder een oplossing zijn gesloten (gewoonlijk in de status Gesloten) en kwesties die zonder een daadwerkelijke resolutie zijn gesloten (gewoonlijk in de status van Geen oplossing).</p> <p>Wanneer een probleem wordt gemarkeerd als Geen oplossing, wordt het probleem verwijderd uit de lijst Werkgroep van de ontvanger. In dit geval geeft de uitgave een waarde weer voor de datum van feitelijke voltooiing.</p> <p>Als alle taken op een project worden voltooid, en minstens één kwestie in een Won is lost status niet op, kan het project worden voltooid.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Uitgiftestatussen aanpassen

Een Workfront-beheerder kan emissiestatussen op systeemniveau en op groepsniveau toevoegen aan Workfront en de volgorde wijzigen waarin gebruikers deze weergeven. Voor meer informatie, zie [ een status ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) creëren of uitgeven.

Een groepbeheerder kan een aangepaste status toevoegen die specifiek is voor één groep. Voor meer informatie, zie [ creeer of geef een groepsstatus ](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md) uit.
