---
title: Toegang verlenen tot projecten
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot projecten in Workfront te bepalen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: ba6a9e68-68a1-4152-b024-cd39e06d556f
source-git-commit: 97f5adc8811a3be7be23137a82d10d45b76ec605
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Toegang verlenen tot projecten

<!-- Audited: 12/2023 -->

Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot projecten te bepalen, zoals die in de volgende artikelen wordt verklaard:

* [Overzicht van toegangsniveaus](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)
* [Overzicht van nieuwe toegangsniveaus](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)

Voor informatie over het gebruiken van de niveaus van de douanetoegang om gebruikers&#39; toegang tot andere objecten types in Workfront te beheren, zie [ tot douanetoegangsniveaus leiden of wijzigen ](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td>Alle</td> 
  </tr> 
    <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p>
   <p>Plan</p>
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vorm gebruikerstoegang tot projecten gebruikend een niveau van de douanetoegang

1. Beginnen creërend of het uitgeven van het toegangsniveau, zoals die in [ wordt verklaard creeer of wijzig douanetoegangsniveaus ](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klik het de montagespictogram van het tandwielpictogram ![ Gear ](assets/gear-icon-settings.png) op de **Mening** of **geef** knoop rechts van Projecten uit, dan selecteer de capaciteiten u onder **wilt verlenen fijn-stemt uw montages**.

   ![ Eet montages voor het kopiëren projecten ](assets/planner-fine-tune-your-settings-with-copy-projects.png)

   >[!NOTE]
   >
   >* Gebruikers met een werkvergunning hebben beperkte projectrechten. Ze kunnen wel bijdragen aan een project, maar niet beheren.
   >* Gebruikers met een Revisielicentie hebben weergaverechten voor projecten van omgezette uitgaven, maar hun weergaverechten zijn beperkt.
   >* Voor informatie over toestemmingengebruikers kunnen verlenen wanneer het delen van projecten met anderen, zie [ een project in Adobe Workfront ](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md) delen.
   >* Wanneer u een toegangsniveau het plaatsen voor een bepaald type van voorwerp vormt, beïnvloedt die configuratie niet de toegang van de gebruikers tot voorwerpen met een lagere rang. Bijvoorbeeld, kunt u gebruikers van het schrappen van projecten in hun toegangsniveau beperken, maar dit beperkt hen niet van het schrappen van taken, die lager-rangschikkend zijn dan projecten.Voor meer informatie over de hiërarchie van voorwerpen, zie de sectie [ Interdependentie en hiërarchie van voorwerpen ](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) in het artikel [ voorwerpen in Adobe Workfront ](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) begrijpen.
   * Een gebruiker wiens toegangsniveau toegang tot financiële gegevens niet toestaat kan geen toegang verlenen die anderen zou toestaan om financiële gegevens te bekijken. Dit omvat het verlenen van toegang tot projecten die financiële gegevens tonen, of het wijzigen van een toegangsniveau om het bekijken van financiële gegevens toe te staan.


1. (Facultatief) klik **plaats delend gebreken** rechts van de Create optie, dan **voeg Regel** toe om een het delen regel voor nieuwe projecten toe te voegen.

   Wanneer de gebruiker met dit toegangsniveau tot een project leidt, wordt het project gedeeld automatisch met de gebruikers u in het menu op de linkerzijde selecteert.

   ![](assets/project-sharing-menu.png)

   In het menu aan de rechterkant geeft u op hoe u het project wilt delen met die gebruikers:

   ![](assets/project-sharing-right-menu.png)

   >[!NOTE]
   >
   >Als een gebruiker met dit toegangsniveau een malplaatje van de projecttoegang gebruikt, treedt het malplaatje de het delen montages op het toegangsniveau met voeten. Voor informatie over de malplaatjes van de projecttoegang, zie [ een project in Adobe Workfront ](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md) delen.

   U kunt deze stap herhalen om zo vele project toe te voegen delend regels aangezien u voor het toegangsniveau nodig hebt.

1. Klik X om **te sluiten verbeter uw montages** doos.
1. (Facultatief) om toegangsmontages voor andere voorwerpen en gebieden in het toegangsniveau te vormen u aan werkt, ga met één van de artikelen voort die in [ worden vermeld toegang tot Adobe Workfront ](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), zoals [ toegang van de Verlening tot taken ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) en [ toegang van de Verlening tot financiële gegevens ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wanneer u wordt gebeëindigd, klik **sparen**.

   Nadat het toegangsniveau wordt gecreeerd, kunt u het aan een gebruiker toewijzen. Voor meer informatie, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

## Toegang tot rapporten, dashboards en kalenders per licentietype

Voor informatie over welke gebruikers in elk toegangsniveau met kwesties kunnen doen, zie de sectie [ Projecten ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects) in de artikel [ Functionaliteit beschikbaar voor elk objecten type ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Toegang tot gedeelde projecten

Als eigenaar of schepper van een kwestie, kunt u met andere gebruikers delen door hen toestemmingen aan het toe te kennen, zoals die in [ wordt verklaard een project in Adobe Workfront ](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md) delen.

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Wanneer u een object met een andere gebruiker deelt, worden de rechten van de ontvanger op het object bepaald door een combinatie van twee dingen:

* De machtigingen die u aan de ontvanger toekent voor het object
* De instellingen van het toegangsniveau van de ontvanger voor het objecttype
