---
title: Toegang verlenen tot filters, weergaven en groepen
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot de filter, de mening, en het groeperen controles voor lijsten en rapporten te bepalen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4fb6eefd-74dd-4941-91d4-0e5f637febf3
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# Toegang verlenen tot filters, weergaven en groepen

Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot de filter, de mening, en het groeperen controles voor lijsten en rapporten te bepalen, zoals die in [Overzicht van toegangsniveaus](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Voor informatie over de filter, mening, en groeperingscontroles, zie [Elementen rapporteren: filters, weergaven en groepen](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Toegangsvereisten

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
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Gebruikerstoegang tot filters, meningen, en groepen vormen gebruikend een niveau van de douanetoegang

1. Beginnen met het maken of bewerken van het toegangsniveau, zoals wordt uitgelegd in [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klik op het tandwielpictogram ![](assets/gear-icon-settings.png) op de **Weergave** of **Bewerken** rechts van Filters en selecteer vervolgens de mogelijkheden die u onder **Uw instellingen nauwkeurig afstellen**.

   ![](assets/gear-icon-filters-dashboards-groupings.jpg)

   Standaard beschikken gebruikers met een licentie voor Overzicht, Werk, Reviewer of Aanvraag over de volledige weergave- en bewerkingsmogelijkheden. Gebruikers met een licentie voor externe gebruikers hebben geen toegang tot filters, weergaven en groepen.

   <!--If this changes, undraft section with table below
   -->

1. (Optioneel) Als u de toegangsinstellingen wilt configureren voor andere objecten en gebieden in het toegangsniveau waaraan u werkt, gaat u verder met een van de artikelen in [Toegang tot Adobe Workfront configureren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), zoals [Toegang verlenen tot taken](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) en [Toegang tot financiële gegevens verlenen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Als u klaar bent, klikt u op **Opslaan**.

   Nadat het toegangsniveau wordt gecreeerd, kunt u het aan een gebruiker toewijzen. Zie voor meer informatie [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

<!--## Access to filters, views, and groupings by license type

Drafting out this section for now because the table is redundant since all four license types can do everything.</span>-->

Deze lijst maakt een lijst van wat een beheerder van Workfront gebruikers met elk vergunningstype kan toestaan om met filter, meningen, en groeperingen te doen. Voor informatie over de Workfront-licentietypen raadpleegt u [Overzicht van Adobe Workfront-licenties](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

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
