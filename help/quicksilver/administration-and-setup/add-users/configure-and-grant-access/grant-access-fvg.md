---
title: Toegang verlenen tot filters, weergaven en groepen
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot de filter, de mening, en het groeperen controles voor lijsten en rapporten te bepalen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4fb6eefd-74dd-4941-91d4-0e5f637febf3
source-git-commit: 09bb41e16da89edd2c2cbfb5a85213045e52394d
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# Toegang verlenen tot filters, weergaven en groepen

Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot de filter, de mening, en het groeperen controles voor lijsten en rapporten te bepalen, zoals die in [&#x200B; het overzicht van de Niveaus van de Toegang &#x200B;](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) wordt verklaard.

Voor informatie over de filter, de mening, en het groeperen controles, zie [&#x200B; Meldend elementen: filters, meningen, en groeperingen &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw beheerder van Workfront als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override=""> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Gebruikerstoegang tot filters, meningen, en groepen vormen gebruikend een niveau van de douanetoegang

1. Beginnen creërend of het uitgeven van het toegangsniveau, zoals die in [&#x200B; wordt verklaard creeer of wijzig douanetoegangsniveaus &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klik het tandwielpictogram ![](assets/gear-icon-settings.png) op de **Mening** of **geef** knoop aan het recht van Filters uit, dan selecteer de capaciteiten u onder **wilt verlenen - verbeter uw montages**.

   ![](assets/gear-icon-filters-dashboards-groupings.png)

   Standaard beschikken gebruikers met een licentie voor Overzicht, Werk, Reviewer of Aanvraag over de volledige weergave- en bewerkingsmogelijkheden. Gebruikers met een licentie voor externe gebruikers hebben geen toegang tot filters, weergaven en groepen.

   <!--If this changes, undraft section with table below
   -->

1. (Facultatief) om toegangsmontages voor andere voorwerpen en gebieden in het toegangsniveau te vormen u aan werkt, ga met één van de artikelen voort die in [&#x200B; worden vermeld toegang tot Adobe Workfront &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), zoals [&#x200B; toegang van de Verlening tot taken &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) en [&#x200B; toegang van de Verlening tot financiële gegevens &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wanneer u wordt gebeëindigd, klik **sparen**.

   Nadat het toegangsniveau wordt gecreeerd, kunt u het aan een gebruiker toewijzen. Voor meer informatie, zie [&#x200B; het profiel van een gebruiker &#x200B;](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

<!--## Access to filters, views, and groupings by license type

Drafting out this section for now because the table is redundant since all four license types can do everything.</span>-->

Deze lijst maakt een lijst van wat een beheerder van Workfront gebruikers met elk vergunningstype kan toestaan om met filter, meningen, en groeperingen te doen. Voor informatie over de de licentietypen van Workfront, zie [&#x200B; het vergunningsoverzicht van Adobe Workfront &#x200B;](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<thead>
<tr>
<th> Handeling </th>
<th> Planner </th>
<th> Worker </th>
<th> Revisor </th>
<th> Aanvragen </th>
</tr>
</thead>
<tbody>
<tr>
<td>Filters, weergaven en groepen bewerken</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Filters, weergaven en groepen maken</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Filters, weergaven en groepen weergeven</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Filters, weergaven en groepen verwijderen</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Filters, weergaven en groepen delen</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Filters, weergaven en groepen delen in het hele systeem</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
</tbody>
</table>
