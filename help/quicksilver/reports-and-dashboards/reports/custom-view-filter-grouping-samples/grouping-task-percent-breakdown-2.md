---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groepering: verdeling taakpercentage 2'
description: 'In deze aangepaste taakgroep kunt u taken weergeven die zijn gegroepeerd op een bereik van hun procentuele volledige waarden. De uitsplitsingen tonen een percentage complete waarde van 10 percentagestappen: 1-10%, 11-20%, enz.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d5a40dd-d451-48c7-9323-af52aa387709
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# Groepering: verdeling taakpercentage 2

In deze aangepaste taakgroep kunt u taken weergeven die zijn gegroepeerd op een bereik van hun procentuele volledige waarden. De uitsplitsingen geven het percentage aan dat de volledige waarde is in stappen van 10 procentpunten: 1-10%, 11-20% enzovoort.

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

![ task_10__break_grouping.png ](assets/task-10--breakdown-grouping-350x547.png)

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
   <pre>groep.0.linkedname=direct <br> group.0.name=Percent Breakdown <br> group.0.notime=false <br> group.0.valueexpression=IF ({percentComplete}=0, "0 %", IF ({percentComplete} &lt;=11, "1-10 %", IF ({percentComplete}&lt;=21, "11-20 %" IF ({percentComplete}&lt;=31, "21-30 %", IF ({percentComplete} &lt;41, "31-40 %", IF ({percentComplete}&lt;51, "41-50 %", IF ({percentComplete} &lt;61, "51-60 %", IF ({percentComplete}&lt;71, "6 1-70 %", IF ({percentComplete} &lt;81, "71-80 %", IF ({percentComplete} &lt;91, "81-90 %", IF ({percentComplete} &lt;100, "91-99 %", "100 %"))))) <br>  textmode=true</pre>

1. Klik **sparen Groepering**.
