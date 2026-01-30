---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Overzicht van het project Werkelijke Begindatum
description: Projecten, taken en problemen hebben een werkelijke begindatum in Adobe Workfront. Voor taken, en kwesties, is dit de datum wanneer zij zoals Lopend zijn gemerkt. Voor projecten is dit de datum waarop de eerste taak van het project wordt gemarkeerd als Bezig of voltooid.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Overzicht van het project Werkelijke Begindatum

Projecten, taken en problemen hebben een werkelijke begindatum in Adobe Workfront. Voor taken, en kwesties, is dit de datum wanneer zij zoals Lopend zijn gemerkt. Voor projecten is dit de datum waarop de eerste taak van het project wordt gemarkeerd als Bezig of voltooid.

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
   <td><p>Licht of hoger</p> 
   <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten weergeven of vergroten</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening of hoger aan een project</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Overwegingen over werkelijke begindatums in Workfront

* De daadwerkelijke Datum van het Begin wordt gevestigd in de sectie van Details van projecten, taken, en kwesties.
* De daadwerkelijke Datum van het Begin van een project, een taak, of een kwestie is niet bevolkt wanneer deze punten worden gecreeerd.
* De werkelijke begindatum wordt ingevuld wanneer het werk daadwerkelijk begint met het project, de taak of de uitgave.
* De daadwerkelijke Datum van het Begin toont niet op het lusje van de Details van het Project als het werk aan het project nog niet is begonnen.

  De daadwerkelijke Datum van het Begin toont leeg op de lusjes van de Details van de Taak en van de Uitgave als het werk nog niet op hen is begonnen.

* U kunt de Ware Datum van het Begin van een taak of een kwestie manueel wijzigen, maar u kunt niet de Ware Datum van het Begin van een project wijzigen.

## Overwegingen over werkelijke begindatums voor projecten

* Workfront stelt automatisch de werkelijke datum van een project in wanneer een van de volgende situaties zich voordoet:

   * Een taaktoegewezen persoon verandert het statuut van een taak van *Nieuw* in een andere status die *Nieuw* niet gelijkstelt.

   * Een toegewezen taak wijzigt het percentage voltooide taak.

     >[!IMPORTANT]
     >
     >De daadwerkelijke Datum van het Begin van het Project bevolkt niet wanneer het project als Huidig wordt gemerkt. De werkelijke werkzaamheden moeten beginnen met de taken van het project voordat de werkelijke begindatum van het project wordt ingevuld.

     In deze gevallen wordt de werkelijke begindatum van het project ingesteld op de datum en het tijdstip waarop deze handelingen voor de vroegste taak van het project zijn uitgevoerd. Dit wijst erop dat het project eigenlijk op deze datum en tijd begon.

## De werkelijke begindatum van een project zoeken

U kunt de werkelijke begindatum van een project vinden in de volgende gebieden:

* In de sectie Details van een Project.
* In een projectrapport of een mening, wanneer u de **Ware Datum van het Begin** voor het voorwerp van het Project in het rapport toevoegt.

  Voor informatie over het creëren van rapporten, zie het artikel [&#x200B; een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

U kunt als volgt de werkelijke begindatum vinden in de sectie Details van het project:

{{step1-to-projects}}

1. Klik op het project waarvoor u de werkelijke begindatum wilt weergeven.
1. Klik **Details van het Project** in het linkerpaneel, dan ga naar de **sectie van het Overzicht**.

   ![&#x200B; benadrukt de daadwerkelijke van het Project begindatum &#x200B;](assets/nwe-project-actual-start-date--highlighted-350x367.png)

   De **Ware Datum van het Begin** vertoningen langs andere projectdata.


