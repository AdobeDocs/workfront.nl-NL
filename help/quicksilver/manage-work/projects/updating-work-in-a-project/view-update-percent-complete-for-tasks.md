---
product-area: projects
navigation-topic: update-work-in-a-project
title: Percentage weergeven en bijwerken voltooid voor taken
description: U kunt het percentage van voltooiing van een taak bijwerken om de vooruitgang aan te geven die u op de taak hebt gemaakt om het te voltooien. Het bijwerken van het percentage voltooide uitgaven is vergelijkbaar met het bijwerken van het percentage voor een taak. In dit artikel wordt beschreven hoe u het percentage van een taak kunt bijwerken.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---

# Percentage van voltooiing weergeven en bijwerken voor taken

<!--Audited: 05/2025-->

U kunt het percentage van voltooiing van een taak bijwerken om de vooruitgang aan te geven die u op de taak hebt gemaakt om het te voltooien.

Het bijwerken van het percentage voltooide uitgaven is vergelijkbaar met het bijwerken van het percentage voor een taak. In dit artikel wordt beschreven hoe u het percentage van een taak kunt bijwerken.

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
   <td> <p>Standard</p> 
   <p>Werk of hoger</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot taken bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor de taak beheren</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New license: Standard</p> 
   Or
   <p>Current license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Gebieden waar u het percentage van voltooiing van een taak kunt bijwerken

U kunt het voltooide percentage voor een taak op een van de volgende gebieden bijwerken:

* **in een taaklijst**: U kunt het percentage bijwerken volledig van een taak wanneer de Percent Volledige kolomvertoningen.

  Voor meer informatie over gealigneerde het uitgeven, zie [&#x200B; gealigneerd punten in een lijst in Adobe Workfront &#x200B;](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md) uitgeven.

* **in de mening van de Mijlpaal**: U kunt de percenten bijwerken volledig van een taak wanneer het gebruiken van de mening van de Mijlpaal op een projectlijst of een projectrapport.

  >[!TIP]
  >
  >  U kunt het percentage van de voltooide problemen niet bijwerken in de milestone-weergave.


  Voor meer informatie, zie [&#x200B; Gebruik de mening van de Mijlpaal &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **in de taakkopbal**: U kunt het percentage bijwerken volledig van een taak in de taakkopbal.

  ![&#x200B; Percentage van de Update in kopbal &#x200B;](assets/nwe-updatetaskpercentinheader-350x54.png)

* **in het Summiere paneel van een taak**: U kunt het percentage van een taak bij de bovenkant van het Summiere paneel bijwerken wanneer het bekijken van de taak op de volgende gebieden:

   * Taaklijst of rapport
   * Tijdschema
   * Werklastverdeling

  ![&#x200B; benadrukte Percentage van de Update in taakSamenvatting &#x200B;](assets/update-percent-complete-in-task-summary-highlighted.png)

  Voor meer informatie, zie [&#x200B; Samenvatting &#x200B;](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)

* **Huis**: U kunt het percentage bijwerken volledig van een taak of kwestie van het Summiere paneel in het gebied van het Huis, of van Mijn Werk widget.

  Voor informatie, zie [&#x200B; Begonnen het worden met Huis &#x200B;](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

## Overwegingen bij het bijwerken van het percentage voltooide taken

* Wanneer u een taak markeert als 100% voltooid, wordt de taakstatus bijgewerkt naar Voltooid. De status van een uitgave wordt bijgewerkt naar Gesloten.
* Als u een taak voltooit, wordt ook het volledige percentage van het bovenliggende en het geselecteerde project bijgewerkt.
* De volgende scenario&#39;s bestaan voor oudertaken en projecten:
   * U kunt niet het percentage bijwerken volledig van een oudertaak aan 100% wanneer de Summiere Wijze van de Voltooiing van het project aan Automatisch wordt geplaatst en de subtaken niet worden voltooid.
   * U kunt het percentage bijwerken volledig van een oudertaak of van een project aan 100% wanneer de Summiere Wijze van de Voltooiing van het project aan Handboek wordt geplaatst en subtaken worden voltooid of onvolledig.

  Voor meer informatie, zie [&#x200B; projecten &#x200B;](../manage-projects/edit-projects.md) uitgeven.

## Het percentage van een taak bijwerken

1. Ga naar een van de gebieden waar u het percentage wilt bijwerken dat een taak is voltooid.

   Voor informatie, zie de sectie [&#x200B; Gebieden waar u het percent volledig van een taak &#x200B;](#areas-where-you-can-update-the-percent-complete-of-a-task) in dit artikel kunt bijwerken.

1. Bepaal de plaats van het **Volledige** gebied van de Percentage voor de taak waarvan percent voltooit u wilt bijwerken.

   >[!TIP]
   >
   >Het veld Percentage voltooid wordt altijd boven in het deelvenster Overzicht weergegeven.

1. Klik binnen het **Volledige 1&rbrace; gebied van de Percentage &lbrace;en typ een aantal tussen 0 en 100**

   of

   Klik en sleep de **Volledige** blauwe bel van de Procent aan het noodzakelijke aantal om erop te wijzen hoeveel van de taak u voltooide, wanneer beschikbaar.

   >[!NOTE]
   >
   >    * U kunt geen decimaal aantal ingaan wanneer u binnen de Percent Volledige bel klikt.
   >    * Wanneer u de blauwe ballon in het deelvenster Samenvatting sleept, wordt de optie Percentage voltooid in stappen van één punt bijgewerkt.
   >
   >    * Wanneer u de blauwe bel in de taakkopbal sleept en laat vallen, werkt Percentage volledig in 5 punttoename bij.

1. Druk op Enter op het toetsenbord om het volledige percentage op te slaan.

   De Percentage Voltooide van het project of om het even welke oudertaken zouden ook automatisch kunnen bijwerken.

   De status van de taak of van de uitgave wordt ook bijgewerkt.

