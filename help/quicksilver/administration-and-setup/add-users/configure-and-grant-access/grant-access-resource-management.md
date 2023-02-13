---
title: Toegang verlenen tot beheer van hulpbronnen
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot het Beheer van het Middel in Workfront te bepalen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Toegang verlenen tot beheer van hulpbronnen

Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot het Beheer van het Middel te bepalen, zoals die in wordt verklaard [Overzicht van toegangsniveaus](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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

## Vorm gebruikerstoegang tot de hulpmiddelen van het Beheer van het Middel gebruikend een niveau van de douanetoegang

1. Beginnen met het maken of bewerken van het toegangsniveau, zoals wordt uitgelegd in [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klik op het tandwielpictogram ![](assets/gear-icon-settings.png) op de **Weergave** of **Bewerken** knoop rechts van het Beheer van het Middel, dan selecteer de capaciteiten u onder wilt verlenen **Uw instellingen nauwkeurig afstellen**.

   ![](assets/resource-management-details-of-edit-in-the-access-level.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Prioriteiten en begrotingstijden bewerken in de Planner</td> 
      <td> <p>Hiermee kunnen gebruikers met deze licentie het volgende doen:</p> <p>Prioriteit geven aan projecten in de Planner van het Middel.</p> <p>De toewijzing van de begroting voor middelen in de hulpmiddelen van de Planning van het Middel (de Planner van het Middel en de sectie van de Begroting van het Middel in het BedrijfsGeval van een project.)</p> <p>Deze optie is standaard ingeschakeld.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bronnenpools beheren</td> 
      <td> <p>Hiermee kunnen gebruikers met deze licentie bronnenpools maken, bewerken en verwijderen. Deze optie is standaard uitgeschakeld.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>Geplande uren bijwerken in werklastbalans</span> </td> 
      <td> <p>Hiermee kunnen gebruikers met deze licentie de geplande uren aan werkitems bijwerken wanneer ze de gebruikerstoewijzingen in Workload Balancer bijwerken. Het totale aantal toegewezen uren wordt de Geplande Uren van de het werkpunten.</p> <p>Deze optie is standaard uitgeschakeld.</p> <p> Zie voor meer informatie <a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Toewijzingen van gebruikers beheren in Workload Balancer</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Als u de toegangsinstellingen wilt configureren voor andere objecten en gebieden in het toegangsniveau waaraan u werkt, gaat u verder met een van de artikelen in [Toegang tot Adobe Workfront configureren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), zoals [Toegang verlenen tot taken](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) en [Toegang tot financiële gegevens verlenen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Als u klaar bent, klikt u op **Opslaan**.

   Nadat het toegangsniveau wordt gecreeerd, kunt u het aan een gebruiker toewijzen. Zie voor meer informatie [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Toegang tot hulpbronnenbeheer per licentietype

Voor informatie over wat de gebruikers in elk toegangsniveau met het Beheer van het Middel kunnen doen, zie de sectie [Bronbeheer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource) in het artikel [Beschikbare functionaliteit voor elk objecttype](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Toegang tot gedeelde problemen

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Wanneer u een object deelt met een andere gebruiker, worden de rechten van de ontvanger op begrotings- of weergavetoewijzing voor het object bepaald door een combinatie van drie dingen:

* De het toegangsniveau van de ontvanger het plaatsen voor het Beheer van het Middel
* De toegang van de gebruiker tot financiële gegevens, zoals uitgelegd in [Toegang tot financiële gegevens verlenen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* Eventuele machtigingen voor financiële gegevens die de deler heeft toegekend voor het object

Voor informatie over toestemmingen kunnen de gebruikers aan financiële gegevens op een voorwerp verlenen wanneer het delen van het voorwerp, zie [Financiële machtigingen delen op een object](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).
