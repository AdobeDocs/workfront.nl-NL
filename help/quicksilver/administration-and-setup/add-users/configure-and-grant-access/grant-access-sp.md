---
title: Toegang verlenen tot Scenario Planner
description: Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot de Planner van het Scenario te bepalen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# Toegang verlenen tot Scenario Planner

Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot de Planner van het Scenario te bepalen, zoals verklaard in [ overzicht van de Niveaus van de Toegang ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Naast toegang tot Scenario Planner, moet een gebruiker met een niet-Systeem toegangsniveau van de Beheerder ook toegang tot financiële gegevens hebben om om het even welke financiële informatie te zien in een plan, zoals begrotingen, kosten, en baanroltarieven. Voor meer informatie, zie [ toegang van de Verlening tot financiële gegevens ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-abonnement*</p> </td> 
   <td>Zakelijk of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Reviseren of hoger. Voor meer informatie, zie <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref" data-mc-variable-override=""> overzicht van Vergunningen </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>U moet een extra licentie voor de Adobe Workfront Scenario Planner aanschaffen om toegang te krijgen tot de functionaliteit die in dit artikel wordt beschreven.</p> <p>Voor informatie over het verkrijgen van de Planner van het Scenario van Workfront, zie <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref" data-mc-variable-override=""> Toegang nodig om de Planner van het Scenario te gebruiken </a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau*</td> 
   <td> <p>Toegang tot of hoger weergeven voor de functie Scenario Planner</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw beheerder van Workfront als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override=""> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Objectmachtigingen</p> </td> 
   <td> <p>Machtigingen of hoger weergeven voor een abonnement</p> <p>Voor informatie bij het verzoeken van extra toegang tot een plan, zie <a href="../../../scenario-planner/request-access-to-plan.md" class="MCXref xref" data-mc-variable-override=""> toegang van het Verzoek tot een plan in de Planner van het Scenario </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Vorm gebruikerstoegang tot de Planner van het Scenario gebruikend een niveau van de douanetoegang

1. Beginnen creërend of het uitgeven van het toegangsniveau, zoals die in [ wordt verklaard creeer of wijzig douanetoegangsniveaus ](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klik de optie aan het recht van **Planner van het Scenario** die u voor dit toegangsniveau wilt gebruiken.

   >[!NOTE]
   >
   >Het verzoektype of het Externe vergunningstype verleent geen Mening of geeft toegang tot de Planner van het Scenario uit.

1. (Facultatief) om toegangsmontages voor andere voorwerpen en gebieden in het toegangsniveau te vormen u aan werkt, ga met één van de artikelen voort die in [ worden vermeld toegang tot Adobe Workfront ](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), zoals [ toegang van de Verlening tot taken ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) en [ toegang van de Verlening tot financiële gegevens ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wanneer u wordt gebeëindigd, klik **sparen**.

## Toegang tot de functie Scenario Planner per licentietype

Voor informatie over welke gebruikers in elk toegangsniveau met de Planner van het Scenario kunnen doen, zie het sectie [ gebied van de Planner van het Scenario ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) in de artikel [ Functionaliteit beschikbaar voor elk objecten type ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Toegang tot Scenario Planner via toegangsniveau instellen

De volgende informatie kan u helpen begrijpen hoe te om de het niveaumontages van de Toegang te gebruiken om de toegang van gebruikers tot informatie in de Planner van het Scenario van Workfront te controleren.

* [ Geen toegang ](#no-access)
* [ toegang van de Mening ](#view-access)
* [Toegang bewerken](#edit-access)

### Geen toegang {#no-access}

Een gebruiker zonder toegang tot de Planner van het Scenario kan niet het pictogram Scenario&#39;s in het Belangrijkste Menu zien wanneer het aan hun lay-outmalplaatje wordt toegevoegd, noch plannen en initiatieven bekijken die met hen worden gedeeld. Als de verbinding aan een plan met een gebruiker wordt gedeeld die geen toegang tot Planner Scenario heeft, kan de gebruiker niet het plan bekijken of uitgeven.

### Toegang weergeven {#view-access}

De gebruikers met de toegang van de Mening tot de Planner van het Scenario kunnen het volgende doen:

* Zie het pictogram Scenario&#39;s in het Hoofdmenu ![](assets/esp-icon-in-main-menu.png) , hoewel het gebied van Abonnementen leeg is tenzij de gebruiker op een planverbinding klikt die door een andere gebruiker wordt gedeeld.
* Een abonnement weergeven wanneer een andere gebruiker de koppeling deelt.

  Dit omvat alle informatie over de rol van de baan in het plan.

  Het omvat ook baanroltarieven en kosteninformatie over het plan als de ontvangende gebruiker ook toegang tot financiële gegevens heeft. Voor meer informatie, zie [ toegang van de Verlening tot financiële gegevens ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### Toegang bewerken {#edit-access}

Gebruikers met toegang tot Scenario-planner bewerken kunnen het volgende doen:

* Zie het pictogram Scenario&#39;s in het Hoofdmenu ![](assets/esp-icon-in-main-menu.png) en gebruik het om tot plangegevens toegang te hebben.
* Plan maken.
* De mening, geeft, en schrapt plannen uit die zij creëren.
* De plannen van andere gebruikers bekijken, uitgeven en schrappen die zij tot het gebruiken van een gedeelde verbinding toegang hebben.

  Dit omvat alle informatie over de rol van de baan in een plan.

  Het omvat ook baanroltarieven en kosteninformatie over het plan als de ontvankelijke gebruiker toegang tot financiële gegevens heeft. Voor meer informatie, zie [ toegang van de Verlening tot financiële gegevens ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
