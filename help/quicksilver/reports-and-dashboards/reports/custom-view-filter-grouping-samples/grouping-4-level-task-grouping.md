---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Grouping: Taakgroepering op vier niveaus voor eigenaar van Portfolio, eigenaar van programma, eigenaar van project en status project'
description: Deze taakgroepering verstrekt 4 niveaus van Groepering. In dit geval worden de taken gegroepeerd door de eigenaar van het Portfolio, de programmaeigenaar, de eigenaar van het project en de projectstatus. U kunt slechts tot 3 niveaus van Groepering hebben gebruikend de standaardinterface. Als u een vierde niveau wilt toevoegen, moet u Tekstmodus gebruiken. U kunt rapporten niet groeperen met meer dan 4 criteria tezelfdertijd.
author: Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# Groepering: taakgroepering op vier niveaus voor eigenaar van Portfolio, eigenaar van programma, eigenaar van project en status van project

<!--Audited: 10/2024-->

Deze taakgroepering verstrekt 4 niveaus van Groepering. In dit geval worden de taken gegroepeerd door de eigenaar van het Portfolio, de programmaeigenaar, de eigenaar van het project en de projectstatus. U kunt slechts tot 3 niveaus van Groepering hebben gebruikend de standaardinterface. Als u een vierde niveau wilt toevoegen, moet u Tekstmodus gebruiken. U kunt rapporten niet groeperen met meer dan 4 criteria tezelfdertijd.

![ four_tier_grouping_for_tasks.png ](assets/four-tier-grouping-for-tasks-350x239.png)

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
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> 
    <p>Nieuw:</p>
   <ul><li><p>Medewerker om een filter te wijzigen </p></li>
   <li><p>Standaard voor het wijzigen van een rapport</p></li> </ul>

<p>Huidige:</p>
   <ul><li><p>Verzoek om een filter te wijzigen </p></li>
   <li><p>Plan om een rapport te wijzigen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creeer een 4 vlakke taakgroepering voor de Eigenaar van het Portfolio, de Eigenaar van het Programma, de Eigenaar van het Project, en de Status van het Project

Deze groep toepassen:

1. Ga naar een takenlijst.
1. Van **het Groeperen** drop-down menu, uitgezochte **Nieuwe Groepering**.

1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. Verwijder de tekst in de **Groep uw gebied van het Rapport**.
1. Vervang de tekst in het vak dat wordt weergegeven door de volgende code:
   <pre>groep.0.linkedname=project <br> group.0.name=Portfolio Eigenaar <br> group.0.notime=false <br> group.0.valueField=project :portfolio: eigenaar:name <br> group.0.valueformat=string <br> group.1.linkedname=project <br> group.1.name=Program Eigenaar <br> group.1.notime=false <br> group.1.valueField=project :program: eigenaar:name <br> group.1.valueformat=string <br> group.2.linkedname=projectOwnerMM <br> group.2.listgrouingparsedmethod=nested (project).nested (eigenaar).string(naam) <br> group.2.namekey projectownermm <br> group.2.notime=false <br> group.2.valuefield=projectOwnerMM:name <br> group.2.valueformat=string <br> group.3.enumclass=com.attask.common.constants.ProjectStatusEnum <br> group.3.linkedname=project <br> 9} group.3.namekey=view.relatedcolumn <br> group.3.namekeyargkey.0=project <br> group.3.namekeyargkey.1=status <br> group.3.notime=false <br> group.3.valuefield=project:status <br> group.3.valueformat=val</pre>

1. Klik **Gedaan**, dan **sparen Groepering**.
1. (Facultatief) werk de naam voor de groepering bij, dan klik **sparen Groepering**.
