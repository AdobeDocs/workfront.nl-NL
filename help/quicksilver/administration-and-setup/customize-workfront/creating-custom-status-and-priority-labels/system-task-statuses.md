---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Status van systeemtaken
description: De drie geïntegreerde taakstatussen van het systeem in Workfront zijn vereist, wat betekent dat u ze kunt ontgrendelen, hernoemen en opnieuw rangschikken, maar u kunt ze niet verbergen of verwijderen. U kunt ook nieuwe taakstatussen van het systeem toevoegen om aan de behoeften in uw organisatie te voldoen. Het wijzigen van de status van een taak is doorgaans een handmatig proces, maar soms wordt de status van een taak automatisch gewijzigd, afhankelijk van andere factoren die zich in het systeem voordoen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Status van systeemtaken

De drie geïntegreerde taakstatussen van het systeem in Workfront zijn vereist, wat betekent dat u ze kunt ontgrendelen, hernoemen en opnieuw rangschikken, maar u kunt ze niet verbergen of verwijderen.

U kunt ook nieuwe taakstatussen van het systeem toevoegen om aan de behoeften in uw organisatie te voldoen.

Het wijzigen van de status van een taak is doorgaans een handmatig proces. Nochtans, zijn er tijden die in de volgende lijst worden geschetst wanneer de status van een taak automatisch wordt veranderd, afhankelijk van andere factoren die in het systeem gebeuren.

De volgende taakstatussen worden geleverd bij uw Workfront-exemplaar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Status van systeemtaak</th> 
   <th>Wanneer deze status optreedt</th> 
   <th>Handelingen die plaatsvinden wanneer een taak zich in deze status bevindt</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nieuw (vereiste status)</td> 
   <td>Dit is de standaardstatus voor elke nieuwe taak.</td> 
   <td>Als de taak op een project in een status van Huidig is, toont de taak op het lusje van de Verzoeken van het Werk van de gebruikers die aan de taken worden toegewezen. Gebruikers kunnen nu aan de taak beginnen te werken.</td> 
  </tr> 
  <tr> 
   <td>Bezig (vereiste status)</td> 
   <td>U kunt een taak in deze status plaatsen om erop te wijzen dat het werk aan die taak is begonnen.</td> 
   <td> <p>Wanneer u een taak markeert zoals Bezig, toont de taak een waarde voor de Ware Datum van het Begin.</p> <p>De vooruitgang op de taak wordt niet geregistreerd tot u manueel het percentage bijwerkt voltooit van de taak.</p> </td> 
  </tr> 
  <tr> 
   <td>Voltooid (vereiste status)</td> 
   <td> <p>U kunt een taak handmatig markeren als deze is voltooid.</p> <p>Als de modus Tekstspatiëring van een taak is ingesteld op Automatisch aanvullen, wordt de taak automatisch gemarkeerd als Voltooid wanneer de geplande datum van voltooiing is bereikt.</p> </td> 
   <td> <p>Wanneer een taak wordt voltooid, is het percentage voltooide van de taak duidelijk als 100%. De taak wordt verwijderd uit de werklijst van de ontvanger in het gebied van het Huis wanneer het wordt voltooid.</p> <p>Wanneer u een taak markeert als Voltooid, toont de taak een waarde voor de Ware Datum van Voltooiing.</p> <p><b> NOTA </b>: Als de taak onvolledige kwesties heeft en u de taakstatus in Voltooid verandert, verandert de status automatisch in Volledig - In afwachting van Kwesties.</p> </td> 
  </tr> 
 </tbody> 
</table>
