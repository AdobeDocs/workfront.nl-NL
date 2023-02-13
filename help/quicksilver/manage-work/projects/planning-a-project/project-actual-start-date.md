---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Overzicht van het project Werkelijke Begindatum
description: Projecten, taken en problemen hebben een werkelijke begindatum in Adobe Workfront. Voor taken, en kwesties, is dit de datum wanneer zij zoals Lopend zijn gemerkt. Voor projecten is dit de datum waarop de eerste taak van het project wordt gemarkeerd als Bezig of voltooid.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Overzicht van het project Werkelijke Begindatum

Projecten, taken en problemen hebben een werkelijke begindatum in Adobe Workfront. Voor taken, en kwesties, is dit de datum wanneer zij zoals Lopend zijn gemerkt. Voor projecten is dit de datum waarop de eerste taak van het project wordt gemarkeerd als Bezig of voltooid.

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
   <td> <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten weergeven of vergroten</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening of hoger aan een project</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Overwegingen over werkelijke begindatums in Workfront

* De daadwerkelijke Datum van het Begin wordt gevestigd in de sectie van Details van projecten, taken, en kwesties. 
* De daadwerkelijke Datum van het Begin van een project, een taak, of een kwestie is niet bevolkt wanneer deze punten worden gecreeerd.
* De daadwerkelijke Datum van het Begin wordt bevolkt wanneer het werk eigenlijk op het project, de taak, of de kwestie begint.
* De daadwerkelijke Datum van het Begin toont niet op het lusje van de Details van het Project als het werk aan het project nog niet is begonnen.

   De daadwerkelijke Datum van het Begin toont leeg op de lusjes van de Details van de Taak en van de Uitgave als het werk nog niet op hen is begonnen.

* U kunt de Ware Datum van het Begin van een taak of een kwestie manueel wijzigen, maar u kunt niet de Ware Datum van het Begin van een project wijzigen.

## Overwegingen over werkelijke begindatums voor projecten

* Workfront stelt automatisch de werkelijke datum van een project in wanneer een van de volgende situaties zich voordoet:

   * Een toegewezen taak wijzigt de status van een taak van *Nieuw* aan elke andere status die niet gelijk is aan *Nieuw*.

   * Een toegewezen taak wijzigt het percentage voltooide taak.

      >[!IMPORTANT]
      >
      >De daadwerkelijke Datum van het Begin van het Project bevolkt niet wanneer het project als Huidig wordt gemerkt. De werkelijke werkzaamheden moeten beginnen met de taken van het project voordat de werkelijke begindatum van het project wordt ingevuld.

      In deze gevallen wordt de werkelijke begindatum van het project ingesteld op de datum en het tijdstip waarop deze handelingen voor de vroegste taak van het project zijn uitgevoerd. Dit wijst erop dat het project eigenlijk op deze datum en tijd begon.

## De werkelijke begindatum van een project zoeken

U kunt de Werkelijke Datum van het Begin van een project op de volgende gebieden de plaats bepalen:

* In de sectie Details van een Project.
* In een projectrapport of een mening, wanneer u de Ware Datum van het Begin voor het objectenProject in het rapport toevoegt.

   Zie het artikel voor informatie over het maken van rapporten [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

U kunt als volgt de werkelijke begindatum vinden in de sectie Details van het project:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Projecten**.
1. Klik op het project waarvoor u de werkelijke begindatum wilt weergeven.
1. Klikken **Projectdetails** in het linkerpaneel, dan ga naar **Overzicht** sectie.

   De daadwerkelijke Datum van het Begin toont langs andere projectdata.

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)

 
