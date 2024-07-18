---
title: Toegang verlenen tot programma's
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-beheerder kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot programma's in Workfront te definiëren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 169f6357-1fbb-43e0-83af-1c4be682ddbf
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Toegang verlenen tot programma&#39;s

Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot programma&#39;s te bepalen, zoals die in [ het overzicht van de Niveaus van de Toegang ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) wordt verklaard.

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

## Gebruikerstoegang tot programma&#39;s configureren met behulp van een aangepast toegangsniveau

1. Beginnen creërend of het uitgeven van het toegangsniveau, zoals die in [ wordt verklaard creeer of wijzig douanetoegangsniveaus ](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klik het tandwielpictogram ![](assets/gear-icon-settings.png) op de **Mening** of **geef** knoop aan het recht van Programma&#39;s uit, dan selecteer de capaciteiten u onder **wilt verlenen - verbeter uw montages**.

   Voor informatie over welke gebruikers in elk toegangsniveau met programma&#39;s kunnen doen, zie de sectie [ Programma&#39;s ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#programs) in de artikel [ Functionaliteit beschikbaar voor elk objecten type ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

   >[!NOTE]
   >
   >Wanneer u een toegangsniveau het plaatsen voor een bepaald type van voorwerp vormt, beïnvloedt die configuratie niet de toegang van de gebruikers tot voorwerpen met een lagere rang. Bijvoorbeeld, kunt u gebruikers van het schrappen van programma&#39;s in hun toegangsniveau beperken, maar dit beperkt hen niet van het schrappen van projecten, die lager-rangschikkend zijn dan programma&#39;s.Voor meer informatie over de hiërarchie van voorwerpen, zie de sectie [ Interdependentie en hiërarchie van voorwerpen ](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) in het artikel [ voorwerpen in Adobe Workfront ](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) begrijpen.

1. (Facultatief) om toegangsmontages voor andere voorwerpen en gebieden in het toegangsniveau te vormen u aan werkt, ga met één van de artikelen voort die in [ worden vermeld toegang tot Adobe Workfront ](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), zoals [ toegang van de Verlening tot taken ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) en [ toegang van de Verlening tot financiële gegevens ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wanneer u wordt gebeëindigd, klik **sparen**.

   Nadat het toegangsniveau wordt gecreeerd, kunt u het aan een gebruiker toewijzen. Voor meer informatie, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

## Toegang tot programma&#39;s per licentietype

Voor informatie over welke gebruikers in elk toegangsniveau met programma&#39;s kunnen doen, zie de sectie [ Programma&#39;s ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#programs) in de artikel [ Functionaliteit beschikbaar voor elk objecten type ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Toegang tot gedeelde programma&#39;s

Als eigenaar of schepper van een programma, kunt u met andere gebruikers delen door hen toestemmingen aan het te verlenen, zoals die in [ worden verklaard deel een programma ](../../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

Wanneer u een object met een andere gebruiker deelt, worden de rechten van de ontvanger op het object bepaald door een combinatie van twee dingen:

* De machtigingen die u aan de ontvanger toekent voor het object
* De instellingen van het toegangsniveau van de ontvanger voor het objecttype
