---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Groeperen: taken per portfolio, programma en project"'
description: Gebruik deze taakgroep om taken te groeperen door de portefeuille, door programma, en dan door het project zij met worden geassocieerd.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8fdad6a1-54b3-4d3e-8f21-4f2efc2dc27a
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Groeperen: taken per portfolio, programma en project

Gebruik deze taakgroep om taken te groeperen door de portefeuille, door programma, en dan door het project zij met worden geassocieerd.

![](assets/portfolio-program-project-grouping-for-tasks-350x120.png)

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

## Taken groeperen per portfolio, programma en project

Deze groep toepassen:

1. Ga naar een takenlijst.
1. Van de **Groepering** vervolgkeuzelijst, selecteert u **Nieuwe groepering**.

1. Klikken **Overschakelen naar tekstmodus**.
1. De tekst in het dialoogvenster verwijderen **Uw rapport groeperen** gebied.
1. Vervang de tekst door de volgende code:

   <pre>group.0.linkedname=project<br>group.0.namekey=portfolio<br>group.0.notime=false<br>group.0.valueField=project:portfolio:name<br>group.0.valueFormat=string<br>group.1.linkedname=project<br>group.1.namekey=program<br>group.1.notime=false<br>group.1.valueField=project:program:name<br>group.1.valueFormat=string<br>group.2.name=Project<br>group.2.valueField=project:name<br>groep.2.valueFormat=HTML<br>textmode=true<br></pre>

1. Klikken **Groepering opslaan**.
