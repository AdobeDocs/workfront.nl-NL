---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Groeperen: Taakgroep op vier niveaus voor Portfolio-eigenaar, programmaeigenaar, projecteigenaar en projectstatus'
description: Deze taakgroepering verstrekt 4 niveaus van Groepering. In dit geval worden de taken gegroepeerd door Portfolio-eigenaar, programmaeigenaar, projecteigenaar en projectstatus. U kunt slechts tot 3 niveaus van Groepering hebben gebruikend de standaardinterface. Als u een vierde niveau wilt toevoegen, moet u Tekstmodus gebruiken. U kunt rapporten niet groeperen met meer dan 4 criteria tezelfdertijd.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Groeperen: Taakgroep op vier niveaus voor Portfolio-eigenaar, programmaeigenaar, projecteigenaar en projectstatus

Deze taakgroepering verstrekt 4 niveaus van Groepering. In dit geval worden de taken gegroepeerd door Portfolio-eigenaar, programmaeigenaar, projecteigenaar en projectstatus. U kunt slechts tot 3 niveaus van Groepering hebben gebruikend de standaardinterface. Als u een vierde niveau wilt toevoegen, moet u Tekstmodus gebruiken. U kunt rapporten niet groeperen met meer dan 4 criteria tezelfdertijd.

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

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

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Creeer een 4 vlakke taakgroepering voor de Eigenaar van de Portfolio, de Eigenaar van het Programma, de Eigenaar van het Project, en de Status van het Project

Deze groep toepassen:

1. Ga naar een takenlijst.
1. Van de **Groepering** vervolgkeuzelijst, selecteert u **Nieuwe groepering**.

1. Klikken **Overschakelen naar tekstmodus**.
1. De tekst in het dialoogvenster verwijderen **Uw rapport groeperen** gebied.
1. Vervang de tekst door de volgende code:

   <pre>group.0.linkedname=project<br>group.0.name=Portfolio Eigenaar<br>group.0.notime=false<br>group.0.valueField=project:portfolio:owner:name<br>group.0.valueFormat=string<br>group.1.linkedname=project<br>group.1.name=Program Owner<br>group.1.notime=false<br>group.1.valueField=project:program:owner:name<br>group.1.valueFormat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>group.2.valueField=projectOwnerMM:name<br>group.2.valueFormat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.namekey=view.related column<br>group.3.namekeyargkey.0=project<br>groep.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valueField=project:status<br>groep.3.valueFormat=val</pre>

1. Klikken **Groepering opslaan**.
