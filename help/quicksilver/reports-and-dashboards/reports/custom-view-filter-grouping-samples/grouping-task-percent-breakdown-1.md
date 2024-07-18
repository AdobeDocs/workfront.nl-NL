---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groepering: verdeling taakpercentage 1'
description: 'In deze aangepaste projectgroep kunt u projecten weergeven die zijn gegroepeerd op een bereik van hun volledige percentagewaarden. De uitsplitsingen tonen een percentage complete waarde van 25 percentagestappen: 0-25%, 25-50%, enz.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ddb9496c-9347-4dc9-a4ce-b9017abd0bb2
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

# Groepering: verdeling taakpercentage 1

In deze groepering van douaneproject, kunt u projecten tonen die door een waaier van hun percenten volledige waarden worden gegroepeerd. De uitsplitsingen geven het percentage aan dat de volledige waarde is in stappen van 25 procentpunten: 0-25%, 25-50% enzovoort. 

De volgende groepering organiseert taken door het percentage volledige waarde in 6 verschillende groepen:

* 0%
* 1-25%
* 26-50%
* 51-75%
* 76-99%
* 100%

![ task_25__break_grouping.png ](assets/task-25--breakdown-grouping-350x412.png)

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

## Uitsplitsing groep naar taakpercentage

Deze groep toepassen:

1. Ga naar een takenlijst.
1. Van **het Groeperen** drop-down menu, uitgezochte **Nieuwe Groepering**.

1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. Verwijder de tekst in de **Groep uw gebied van het Rapport**.
1. Vervang de tekst door de volgende code:
   <pre>groep.0.linkedname=direct <br> group.0.name=Percent Breakdown <br> group.0.notime=false <br> group.0.valueexpression=IF ({percentComplete}=0, "0 %", IF ({percentComplete} &lt;=26, "0-25 %", IF ({percentComplete}&lt;=51, "25-50 %" IF ({percentComplete}&lt;=76, "50-75 %", IF ({percentComplete} &lt;100, "75-99 %", "100 %")) <br> group.0.valueformat=string</pre>

1. Klik **sparen Groepering**.
