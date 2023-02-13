---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groeperen: uitsplitsing naar taakpercentage 1'
description: '''In deze aangepaste projectgroep kunt u projecten weergeven die zijn gegroepeerd op een bereik van hun volledige percentagewaarden. De onderverdelingen geven een percentage aan dat de volledige waarde van stappen van 25 procentpunten bevat: 0-25%, 25-50% enz."'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ddb9496c-9347-4dc9-a4ce-b9017abd0bb2
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 2%

---

# Groeperen: verdeling taakpercentage 1

In deze groepering van douaneproject, kunt u projecten tonen die door een waaier van hun percenten volledige waarden worden gegroepeerd. De onderverdelingen geven een percentage aan dat de volledige waarde van stappen van 25 procentpunten bevat: 0-25%, 25-50% enz. 

De volgende groepering organiseert taken door het percentage volledige waarde in 6 verschillende groepen:

* 0%
* 1-25%
* 26-50%
* 51-75%
* 76-99%
* 100%

![task_25_break_grouping.png](assets/task-25--breakdown-grouping-350x412.png)

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Uitsplitsing groep naar taakpercentage

Deze groep toepassen:

1. Ga naar een takenlijst.
1. Van de **Groepering** vervolgkeuzelijst, selecteert u **Nieuwe groepering**.

1. Klikken **Overschakelen naar tekstmodus**.
1. De tekst in het dialoogvenster verwijderen **Uw rapport groeperen** gebied.
1. Vervang de tekst door de volgende code:

   <pre>group.0.linkedname=direct<br>groep.0.name=Percent Break-down<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %", IF({percentComplete}&lt;=26,"0-25 %", IF({percentComplete}&lt;=51,"25-50 %", IF({percentComplete}&lt;=76,"50-75 %", IF({percentComplete} &lt;100,"75-99 %","100 %"))<br>group.0.valueFormat=string</pre>

1. Klikken **Groepering opslaan**.
