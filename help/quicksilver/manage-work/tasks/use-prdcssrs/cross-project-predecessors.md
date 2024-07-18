---
product-area: projects
navigation-topic: use-predecessors
title: Predecessors voor meerdere projecten maken
description: Een voorganger voor meerdere projecten is een taak waarvan een andere taak (een opvolgertaak genoemd) in een ander project afhankelijk is. De voorganger is de taak die voorrang heeft op de afhankelijke (opvolger)taak. Bijvoorbeeld, kunt u tot een gebiedsdeel leiden dat vereist dat de voorgangertaak wordt duidelijk Voltooid alvorens de afhankelijke taak kan beginnen.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 0%

---

# Predecessors voor meerdere projecten maken

<!--Audited: 12/2023-->

Een voorganger voor meerdere projecten is een taak waarvan een andere taak (een opvolgertaak genoemd) in een ander project afhankelijk is. De voorganger is de taak die voorrang heeft op de afhankelijke (opvolger)taak. Bijvoorbeeld, kunt u tot een gebiedsdeel leiden dat vereist dat de voorgangertaak wordt duidelijk Voltooid alvorens de afhankelijke taak kan beginnen.

Adobe Workfront staat voor taken toe om van taken in andere projecten afhankelijk te zijn, enkel aangezien het predecessors binnen één enkel project toestaat.

>[!INFO]
>
>Een opgravingsbedrijf heeft bijvoorbeeld maar één hoes en twee projecten hebben taken die het gebruik van de hoes vereisen. De projectmanager kan van de taak in het eerste project een voorganger aan de taak in het tweede project maken. Dit toont aan dat het tweede project kan beginnen gebruikend de hoes wanneer het eerste project met het wordt gebeëindigd.

Wanneer het verbinden van projecten door dwars-project predecessors, zullen de data van het primaire project (die de voorgangertaak heeft) het secundaire project (die de opvolgertaak heeft) beïnvloeden.

>[!TIP]
>
>U moet chronologie voor de projecten opnieuw berekenen om data te zien die voor het secundaire project worden bijgewerkt. Voor meer informatie bij het opnieuw berekenen van chronologie, zie [ chronologieherberekeningen voor projecten ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md) vormen.

Voor meer informatie over voorgangersverhoudingen, zie [ Overzicht van taakvoorgangers ](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Nieuw: Standaard </p> 
   of
   <p>Huidig: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot taken en projecten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor de taken en projecten beheren</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Een voorganger voor meerdere projecten maken

1. Ga naar de taak die uw opvolger (afhankelijke taak) zal zijn.
1. Klik **Predecessors** in het linkerpaneel.
1. Klik **toevoegen Voorganger.**
1. Op het **gebied van het Project van de Ouder 0} {, begin typend de naam van het project dat de taak bevat die u voorganger aan uw huidige taak wilt zijn.**
1. Klik op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.
1. Op het **gebied van Taken**, begin typend de naam van de taak die u voorganger aan uw huidige taak wilt zijn.
1. Geef de volgende informatie op voor het definiëren van de relatie tussen de voorganger en de afhankelijke taak:

   * **Type van Afhankelijkheid:** selecteer de verhouding die u de voorgangertaak met de afhankelijke taak wilt hebben. De standaardverhouding is &quot;eind-Begin,&quot;betekenend dat de voorgangerstaak moet beëindigen alvorens de afhankelijke taak kan beginnen. Voor meer informatie over de diverse gebiedsdeeltypes, zie [ Overzicht van de types van taakgebiedsdeel ](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * **Lag:** specificeer de hoeveelheid tijd die na de voltooiing van afgedwongen voorganger moet overgaan tot de afhankelijke taak kan beginnen. Voor meer informatie over de diverse soorten vertraging, zie [ Overzicht van de Types van Markeringen ](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **gedwongen:** wanneer deze optie wordt geselecteerd, kan de gebiedsverhouding tussen de twee taken niet worden omzeild door gebruikers die taken beginnen vroeg. Bijvoorbeeld, als u een verband tussen Taak A en Taak B afdwingt, kan de Taak B niet worden begonnen tot Taak A volledig is. Voor meer informatie over het afdwingen van predecessors, zie [ predecessors ](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md) afdwingen.

     Als deze optie niet is geselecteerd, wordt de afhankelijkheid behandeld als een suggestie voor gebruikers. Bijvoorbeeld, kunnen de gebruikers Taak B beginnen alvorens Taak A volledig is.

1. Klik **sparen**.

   De taken die een dwars-projectvoorganger hebben tonen het verwijzingsaantal van het project predecessor tot behoort en het aantal van de taak, die door een dubbelpunt wordt gescheiden, in de kolom van Predecessors op een taaklijst.

   ![ dwars-project voorganger ](assets/cross-project-predecessor-in-list-view.png)

   Het voorgangspictogram wordt groen als de voorganger de markering Voltooid heeft. Dit wijst erop dat de afhankelijke taak klaar voor het werk is.

   Houd de muisaanwijzer boven deze waarde voor meer informatie over de voorganger, het project en de datums. Klik op de voorganger voor meerdere projecten in het vak Details om de taak te openen.

   Klik bij de bovenkant van het aanwijsvenster om meer informatie over het project van de voorganger te zien.

   Klik **zie Project** om het project van de voorganger te openen.

   ![ dwars-project voorgangersdetails ](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   **zie de optiesvertoningen van het Project** slechts wanneer het bekijken van een dwars-projectvoorganger.

