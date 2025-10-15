---
title: Toegang verlenen tot de functie Scenario Planner
description: Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot de Planner van het Scenario te bepalen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---

# Toegang verlenen tot Scenario Planner

Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot de Planner van het Scenario te bepalen, zoals verklaard in [&#x200B; overzicht van de Niveaus van de Toegang &#x200B;](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Naast toegang tot Scenario Planner, moet een gebruiker met een niet-Systeem toegangsniveau van de Beheerder ook toegang tot financiële gegevens hebben om om het even welke financiële informatie te zien in een plan, zoals begrotingen, kosten, en baanroltarieven. Voor meer informatie, zie [&#x200B; toegang van de Verlening tot financiële gegevens &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-pakket</p> </td> 
   <td>Zakelijk of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Licht of hoger</p>
   <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>U moet een extra licentie aanschaffen voor de Adobe Workfront Scenario Planner.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot of hoger weergeven voor de functie Scenario Planner</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Objectmachtigingen</p> </td> 
   <td> <p>Machtigingen of hoger weergeven voor een abonnement</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vorm gebruikerstoegang tot de Planner van het Scenario gebruikend een niveau van de douanetoegang

1. Beginnen creërend of het uitgeven van het toegangsniveau, zoals die in [&#x200B; wordt verklaard creeer of wijzig douanetoegangsniveaus &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klik de optie aan het recht van **Planner van het Scenario** die u voor dit toegangsniveau wilt gebruiken.

   >[!NOTE]
   >
   >Het verzoektype of het Externe vergunningstype verleent geen Mening of geeft toegang tot de Planner van het Scenario uit.

1. (Facultatief) om toegangsmontages voor andere voorwerpen en gebieden in het toegangsniveau te vormen u aan werkt, ga met één van de artikelen voort die in [&#x200B; worden vermeld toegang tot Adobe Workfront &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), zoals [&#x200B; toegang van de Verlening tot taken &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) en [&#x200B; toegang van de Verlening tot financiële gegevens &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wanneer u wordt gebeëindigd, klik **sparen**.

## Toegang tot de functie Scenario Planner per licentietype

Voor informatie over welke gebruikers in elk toegangsniveau met de Planner van het Scenario kunnen doen, zie het sectie [&#x200B; gebied van de Planner van het Scenario &#x200B;](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) in de artikel [&#x200B; Functionaliteit beschikbaar voor elk objecten type &#x200B;](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Toegang tot Scenario Planner via toegangsniveau instellen

De volgende informatie kan u helpen begrijpen hoe te om de het niveaumontages van de Toegang te gebruiken om de toegang van gebruikers tot informatie in de Planner van het Scenario van Workfront te controleren.

* [&#x200B; Geen toegang &#x200B;](#no-access)
* [&#x200B; toegang van de Mening &#x200B;](#view-access)
* [Toegang bewerken](#edit-access)

### Geen toegang {#no-access}

Een gebruiker zonder toegang tot de Planner van het Scenario kan niet het pictogram Scenario&#39;s in het Belangrijkste Menu zien wanneer het aan hun lay-outmalplaatje wordt toegevoegd, noch plannen en initiatieven bekijken die met hen worden gedeeld. Als de verbinding aan een plan met een gebruiker wordt gedeeld die geen toegang tot Planner Scenario heeft, kan de gebruiker niet het plan bekijken of uitgeven.

### Toegang weergeven {#view-access}

De gebruikers met de toegang van de Mening tot de Planner van het Scenario kunnen het volgende doen:

* Zie het pictogram Scenario&#39;s in het Hoofdmenu ![](assets/esp-icon-in-main-menu.png) , hoewel het gebied van Abonnementen leeg is tenzij de gebruiker op een planverbinding klikt die door een andere gebruiker wordt gedeeld.
* Een abonnement weergeven wanneer een andere gebruiker de koppeling deelt.

  Dit omvat alle informatie over de rol van de baan in het plan.

  Het omvat ook baanroltarieven en kosteninformatie over het plan als de ontvangende gebruiker ook toegang tot financiële gegevens heeft. Voor meer informatie, zie [&#x200B; toegang van de Verlening tot financiële gegevens &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### Toegang bewerken {#edit-access}

Gebruikers met toegang tot Scenario-planner bewerken kunnen het volgende doen:

* Zie het pictogram Scenario&#39;s in het Hoofdmenu ![](assets/esp-icon-in-main-menu.png) en gebruik het om tot plangegevens toegang te hebben.
* Plan maken.
* De mening, geeft, en schrapt plannen uit die zij creëren.
* De plannen van andere gebruikers bekijken, uitgeven en schrappen die zij tot het gebruiken van een gedeelde verbinding toegang hebben.

  Dit omvat alle informatie over de rol van de baan in een plan.

  Het omvat ook baanroltarieven en kosteninformatie over het plan als de ontvankelijke gebruiker toegang tot financiële gegevens heeft. Voor meer informatie, zie [&#x200B; toegang van de Verlening tot financiële gegevens &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
