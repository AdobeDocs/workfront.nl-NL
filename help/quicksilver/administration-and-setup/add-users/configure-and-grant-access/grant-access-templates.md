---
title: Toegang tot sjablonen verlenen
user-type: administrator
product-area: system-administration;templates
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-beheerder kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot sjablonen in Workfront te definiëren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c8e6af1b-8cf3-4522-b0eb-7e5f2d34f5a9
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Toegang tot sjablonen verlenen

Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot malplaatjes te bepalen, zoals die in [ het overzicht van de Niveaus van de Toegang ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) wordt verklaard.

Alleen gebruikers met een licentie voor abonnementen kunnen volledige toegang tot sjablonen hebben.

Voor informatie over het gebruiken van de niveaus van de douanetoegang om gebruikers&#39; toegang tot andere objecten types in Workfront te beheren, zie [ tot douanetoegangsniveaus leiden of wijzigen ](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

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
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw beheerder van Workfront als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override=""> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Toegang van gebruikers tot sjablonen configureren met behulp van een aangepast toegangsniveau

1. Beginnen creërend of het uitgeven van het toegangsniveau, zoals die in [ wordt verklaard creeer of wijzig douanetoegangsniveaus ](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klik het tandwielpictogram ![](assets/gear-icon-settings.png) op de **Mening** of **geef** knoop aan het recht van Malplaatjes uit, dan selecteer de capaciteiten u onder **wilt verlenen - verbeter uw montages**.

   ![](assets/access-level-to-templates-with-edit-expanded-1.png)

1. (Facultatief) om toegangsmontages voor andere voorwerpen en gebieden in het toegangsniveau te vormen u aan werkt, ga met één van de artikelen voort die in [ worden vermeld toegang tot Adobe Workfront ](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), zoals [ toegang van de Verlening tot taken ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) en [ toegang van de Verlening tot financiële gegevens ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wanneer u wordt gebeëindigd, klik **sparen**.

   Nadat het toegangsniveau wordt gecreeerd, kunt u het aan een gebruiker toewijzen. Voor meer informatie, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

## Toegang tot sjablonen per licentietype

Voor informatie over welke gebruikers in elk toegangsniveau met malplaatjes kunnen doen, zie de sectie [ Malplaatjes ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#template) in de artikel [ Functionaliteit beschikbaar voor elk objecten type ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Toegang tot gedeelde sjablonen

Als eigenaar of schepper van een kwestie, kunt u met andere gebruikers delen door hen toestemmingen aan het te verlenen, zoals die in [ worden verklaard deel een malplaatje ](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Wanneer u een object met een andere gebruiker deelt, worden de rechten van de ontvanger op het object bepaald door een combinatie van twee dingen:

* De machtigingen die u aan de ontvanger toekent voor het object
* De instellingen van het toegangsniveau van de ontvanger voor het objecttype
