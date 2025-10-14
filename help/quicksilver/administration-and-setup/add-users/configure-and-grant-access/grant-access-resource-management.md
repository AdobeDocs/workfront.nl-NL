---
title: Toegang verlenen tot beheer van hulpbronnen
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot het Beheer van het Middel in Workfront te bepalen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 0%

---

# Toegang verlenen tot beheer van hulpbronnen

Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot het Beheer van het Middel te bepalen, zoals die in [&#x200B; het overzicht van de Niveaus van de Toegang &#x200B;](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) wordt verklaard.

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

## Vorm gebruikerstoegang tot de hulpmiddelen van het Beheer van het Middel gebruikend een niveau van de douanetoegang

1. Beginnen creërend of het uitgeven van het toegangsniveau, zoals die in [&#x200B; wordt verklaard creeer of wijzig douanetoegangsniveaus &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klik het tandwielpictogram ![](assets/gear-icon-settings.png) op de **Mening** of **geef** knoop aan het recht van het Beheer van het Middel uit, dan selecteer de capaciteiten u onder **wilt verlenen - verbeter uw montages**.

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
      <td role="rowheader"><span> Update Gepland Uren in de Balancer van de Werkbelasting </span> </td> 
      <td> <p>Hiermee kunnen gebruikers met deze licentie de geplande uren aan werkitems bijwerken wanneer ze de gebruikerstoewijzingen in Workload Balancer bijwerken. Het totale aantal toegewezen uren wordt de Geplande Uren van de het werkpunten.</p> <p>Deze optie is standaard uitgeschakeld.</p> <p> Voor meer informatie, zie <a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref"> gebruikerstoewijzingen in de Balancer van de Werklast beheren </a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatief) om toegangsmontages voor andere voorwerpen en gebieden in het toegangsniveau te vormen u aan werkt, ga met één van de artikelen voort die in [&#x200B; worden vermeld toegang tot Adobe Workfront &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), zoals [&#x200B; toegang van de Verlening tot taken &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) en [&#x200B; toegang van de Verlening tot financiële gegevens &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wanneer u wordt gebeëindigd, klik **sparen**.

   Nadat het toegangsniveau wordt gecreeerd, kunt u het aan een gebruiker toewijzen. Voor meer informatie, zie [&#x200B; het profiel van een gebruiker &#x200B;](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

## Toegang tot hulpbronnenbeheer per licentietype

Voor informatie over welke gebruikers in elk toegangsniveau met het Beheer van het Middel kunnen doen, zie het sectie [&#x200B; Beheer van het Middel &#x200B;](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource) in de artikel [&#x200B; Functionaliteit beschikbaar voor elk objecten type &#x200B;](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Toegang tot gedeelde problemen

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Wanneer u een object deelt met een andere gebruiker, worden de rechten van de ontvanger op begrotings- of weergavetoewijzing voor het object bepaald door een combinatie van drie dingen:

* Het de toegangsniveau van de ontvanger plaatsen voor het Beheer van het Middel
* De toegang van de gebruiker tot financiële gegevens, zoals die in [&#x200B; wordt verklaard verleent toegang tot financiële gegevens &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* Eventuele machtigingen voor financiële gegevens die de deler heeft toegekend voor het object

Voor informatie over toestemmingengebruikers kunnen aan financiële gegevens op een voorwerp verlenen wanneer het delen van het voorwerp, zie [&#x200B; financiële toestemmingen van het Aandeel op een voorwerp &#x200B;](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).
