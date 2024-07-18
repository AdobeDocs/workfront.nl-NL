---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groepering: taakgroep op vier niveaus voor eigenaar Portfolio, eigenaar programma, eigenaar project en status project'
description: Deze taakgroepering verstrekt 4 niveaus van Groepering. In dit geval worden de taken gegroepeerd door de eigenaar van het Portfolio, de programmaeigenaar, de eigenaar van het project en de projectstatus. U kunt slechts tot 3 niveaus van Groepering hebben gebruikend de standaardinterface. Als u een vierde niveau wilt toevoegen, moet u Tekstmodus gebruiken. U kunt rapporten niet groeperen met meer dan 4 criteria tezelfdertijd.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Groepering: taakgroepering op vier niveaus voor eigenaar van Portfolio, eigenaar van programma, eigenaar van project en status van project

Deze taakgroepering verstrekt 4 niveaus van Groepering. In dit geval worden de taken gegroepeerd door de eigenaar van het Portfolio, de programmaeigenaar, de eigenaar van het project en de projectstatus. U kunt slechts tot 3 niveaus van Groepering hebben gebruikend de standaardinterface. Als u een vierde niveau wilt toevoegen, moet u Tekstmodus gebruiken. U kunt rapporten niet groeperen met meer dan 4 criteria tezelfdertijd.

![ four_tier_grouping_for_tasks.png ](assets/four-tier-grouping-for-tasks-350x239.png)

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
   <td> <p>Verzoek om een groepering te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een groep te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Creeer een 4 vlakke taakgroepering voor de Eigenaar van het Portfolio, de Eigenaar van het Programma, de Eigenaar van het Project, en de Status van het Project

Deze groep toepassen:

1. Ga naar een takenlijst.
1. Van **het Groeperen** drop-down menu, uitgezochte **Nieuwe Groepering**.

1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. Verwijder de tekst in de **Groep uw gebied van het Rapport**.
1. Vervang de tekst door de volgende code:
   <pre>groep.0.linkedname=project <br> group.0.name=Portfolio Eigenaar <br> group.0.notime=false <br> group.0.valueField=project :portfolio: eigenaar:name <br> group.0.valueformat=string <br> group.1.linkedname=project <br> group.1.name=Program Eigenaar <br> group.1.notime=false <br> group.1.valueField=project :program: eigenaar:name <br> group.1.valueformat=string <br> group.2.linkedname=projectOwnerMM <br> group.2.listgrouingparsedmethod=nested (project).nested (eigenaar).string(naam) <br> group.2.namekey projectownermm <br> group.2.notime=false <br> group.2.valuefield=projectOwnerMM:name <br> group.2.valueformat=string <br> group.3.enumclass=com.attask.common.constants.ProjectStatusEnum <br> group.3.linkedname=project <br> 9} group.3.namekey=view.relatedcolumn <br> group.3.namekeyargkey.0=project <br> group.3.namekeyargkey.1=status <br> group.3.notime=false <br> group.3.valuefield=project:status <br> group.3.valueformat=val</pre>

1. Klik **sparen Groepering**.
