---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groeperen: uitsplitsing naar projectpercentage 2'
description: '''In deze aangepaste projectgroep kunt u projecten weergeven die zijn gegroepeerd op een bereik van hun volledige percentagewaarden. De onderverdelingen geven een percentage aan van de volledige waarde van stappen van 10 procentpunten: 0-10%, 11-20%, 21-30% enz."'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7845fd66-8304-4154-8630-e72482cd753f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 4%

---

# Groeperen: uitsplitsing naar projectpercentage 2

In deze groepering van douaneproject, kunt u projecten tonen die door een waaier van hun percenten volledige waarden worden gegroepeerd. De onderverdelingen geven een percentage aan van de volledige waarde van stappen van 10 procentpunten: 0-10%, 11-20%, 21-30% enz.

De volgende groepering organiseert projecten door het percentage volledige waarde in één van deze groepen:

* 0%
* 1-10%
* 11-20%
* 21-30%
* 31-40%
* 41-50%
* 51-60%
* 61-70%
* 71-80%
* 81-90%
* 91-99%
* 100%

![percent_complete_specificatie_for_projects_in_10__increment.png](assets/percent-complete-breakdown-350x94.png)

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

## Uitsplitsing naar projectpercentage per groep

Deze groep toepassen:

1. Ga naar een lijst met projecten.
1. Van de **Groepering** vervolgkeuzelijst, selecteert u **Nieuwe groepering**.

1. Klikken **Overschakelen naar tekstmodus**.
1. Verwijder de tekst in het vak en plak de volgende code in de beschikbare ruimte:
   <pre>group.0.linkedname=direct<br>groep.0.name=Percent Break-down<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %", IF({percentComplete}&lt;=11,"1-10 %", IF({percentComplete}&lt;=21,"11-20 %", IF({percentComplete}&lt;=31,"21-30 %", IF({percentComplete} &lt;41, "31-40 %", IF ({percentComplete}&lt;51, "41-50 %", IF ({percentComplete}&lt;61, "51-60 %", IF ({percentComplete}&lt;71, "61-70 %", IF ({percentComplete}&lt;81,"7 1-80 %", IF ({percentComplete}&lt;91, "81-90 %", IF ({percentComplete}&lt;100, "91-99 %", "100 %")))))<br>textmode=true</pre>

1. Klikken **Groepering opslaan**.
