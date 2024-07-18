---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Groepering: verdeling van de projectpercentages 1"
description: In deze groepering van douaneproject, kunt u projecten tonen die door een waaier van hun percenten volledige waarden worden gegroepeerd.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7cdc8e56-3486-4e78-b494-b2ba9389c1f7
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Groepering: uitsplitsing projectpercentages 1

In deze groepering van douaneproject, kunt u projecten tonen die door een waaier van hun percenten volledige waarden worden gegroepeerd.

De volgende groepering organiseert projecten door het percentage volledige waarde in één van deze groepen:

* 0%
* 1-25%
* 26-50%
* 51-75%
* 76-99%
* 100%

![ percent_complete_break_custom_project_grouping_25__increment.png ](assets/percent-complete-breakdown-custom-350x56.png)

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

## Uitsplitsing naar projectpercentage per groep

Deze groep toepassen:

1. Ga naar een lijst met projecten.
1. Van **het Groeperen** drop-down menu, uitgezochte **Nieuwe Groepering**.

1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. Verwijder de tekst in het vak en plak de volgende code in de beschikbare ruimte:
   <pre>groep.0.linkedname=direct <br> group.0.name=Percent Breakdown <br> group.0.notime=false <br> group.0.valueexpression=IF ({percentComplete}=0, "0 %", IF ({percentComplete} &lt;=26, "0-25 %", IF ({percentComplete}&lt;=51, "25-50 %" IF ({percentComplete}&lt;=76, "50-75 %", IF ({percentComplete} &lt;100, "75-99 %", "100 %")) <br> group.0.valueformat=string</pre>

1. Klik **sparen Groepering**.
