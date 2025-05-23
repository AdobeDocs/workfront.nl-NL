---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Toegang tot objecten aanvragen
description: De zichtbaarheid van objecten in Adobe Workfront is afhankelijk van de toegang tot dat type object en van de machtigingen die u voor een afzonderlijk object hebt.
author: Becky
feature: Get Started with Workfront
exl-id: ad1c525c-42a8-4fb7-a2cd-7792e1c280ab
source-git-commit: 18b96a6d57dc358bfe52e813bc98d8eb19f37dba
workflow-type: tm+mt
source-wordcount: '1338'
ht-degree: 0%

---

# Toegang tot objecten aanvragen

<!-- Audited: 4/2025 -->

De zichtbaarheid van objecten in Adobe Workfront is afhankelijk van de toegang tot dat type object en van de machtigingen die u voor een afzonderlijk object hebt.

>[!NOTE]
>
>In dit artikel wordt beschreven hoe u machtigingen kunt aanvragen voor alle objecten, behalve voor het volgende:
>
>* Scenario Planner is van plan in het Adobe Workfront Scenario Planner. Voor meer informatie, zie [ toegang van het Verzoek tot een plan in de Planner van het Scenario ](../../scenario-planner/request-access-to-plan.md). Hiervoor is een aanvullende licentie vereist.
>
>* Weergaven en werkruimten in Workfront Planning. Voor meer informatie, zie [ Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront ](/help/quicksilver/planning/access/sharing-permissions-overview.md). Hiervoor is een aanvullende licentie vereist.


Uw Workfront-beheerder configureert uw toegang tot een type object op uw toegangsniveau. Voor meer informatie, zie [ hoe de toegangsniveaus en de toestemmingen samen ](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) werken.

Als u machtigingen nodig hebt voor specifieke objecten in Workfront, kunt u deze objecten aanvragen. In plaats van een e-mail naar de Workfront-beheerder of objecteigenaar te verzenden om uw behoeften uit te leggen, kunt u aanvullende toegang (of machtigingen) aanvragen in Workfront.

U kunt een eerste toegang tot objecten aanvragen als iemand een koppeling naar het object met u deelt, of als u aanvullende toegang tot objecten wilt aanvragen waarvoor u al weergavemachtigingen hebt. Bijvoorbeeld, zou u de toestemmingen van de Mening aan een project kunnen hebben, maar u moet taken aan het toevoegen. In dit geval kunt u Contribute-machtigingen voor het project aanvragen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben om objecten te delen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Nieuw: Standaard</p> 
   <p>of</p>
   <p>Huidig: Werk of hoger</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot of hoger weergeven voor objecten waarvoor u machtigingen aanvraagt</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer details over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Standaarden voor delen begrijpen

De volgende standaard regels voor delen zijn standaardopties in uw Workfront-systeem en worden automatisch van kracht:

* Gebruikers die zijn toegewezen aan een taak of een uitgave, hebben Contribute-toegang hierop.
* Project-, Portfolio- en Program-managers hebben toegang tot de objecten die ze bezitten.
* De gebruikers inbegrepen in een gesprek hebben de toegang van de Mening over het voorwerp waar het gesprek gebeurt.
* Gebruikers die als fiatteurs zijn toegewezen, hebben toegang tot de weergave op het object dat wacht op goedkeuring.
* Wanneer u een dashboard deelt, worden alle rapporten op het dashboard ook gedeeld met dezelfde toegang tot dezelfde gebruikers.
* Objecteigenaars kunnen de toegang tot een object niet uitbreiden tot buiten hun toegang tot dat object, zoals gedefinieerd door de beheerder.

## Toegang aanvragen

U kunt een eerste toegang aanvragen tot objecten waartoe u momenteel geen toegang hebt, of u kunt aanvullende toegang aanvragen tot objecten waartoe u slechts beperkte toegang hebt.

* [ Verzoek eerste toegang ](#request-initial-access)
* [Aanvullende toegang aanvragen](#request-additional-access)

### Aanvankelijke toegang aanvragen  {#request-initial-access}

Als u nog geen toegang hebt tot een object en u vanuit een koppeling naar dat object navigeert, wordt een scherm weergegeven met de mededeling dat u geen toegang hebt om de informatie te bekijken.

Aanvankelijke toegang tot een object aanvragen:

1. Klik **Toegang van het Verzoek**. De **vertoningen van het de toegangsvakje van het Verzoek**.

1. (Voorwaardelijk) als meer dan één gebruiker de aangewezen toegang heeft om u extra toegang te verlenen, toont een drop-down pijl naast de naam van de gebruiker. Selecteer de gebruiker die uw toegangsverzoek van de drop-down lijst zal ontvangen.

   Slechts tien gebruikers worden getoond in de drop-down lijst, die alfabetisch wordt gesorteerd. Voor meer informatie over de orde van de gebruikers die in dit drop-down menu worden vermeld, zie [ Hiërarchie van de &quot;Toegang van het Verzoek&quot;en &quot;Vraag Meer Toegang&quot;drop-down menu&#39;s ](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Selecteer in de vervolgkeuzelijst het type toegang dat u aanvraagt.
1. (Facultatief) op het **P.S.** gebied, ga een nota betreffende in waarom u extra toegang nodig hebt.

   ![ de dialoogdoos van de Toegang van het Verzoek ](assets/request-access-to-project.png)

1. Klik **Toegang van het Verzoek**.

<!--
If you do not have access level rights to an object and you try to access that object from a link, a screen is displayed informing you to contact the Workfront administrator.

For example, if you do not have portfolio access, but you were given a link to a portfolio, you would see the following message:  
![](assets/permission-request-initial2-350x96.png)
-->

### Aanvullende toegang aanvragen {#request-additional-access}

Aanvullende toegang aanvragen tot een object waartoe u al beperkte toegang hebt:

1. Ga naar het object waartoe u aanvullende toegang wilt aanvragen.

1. Klik het **Meer** menu rechts van de projectnaam, dan klik **Verzoek Meer Toegang**.

   ![ Verzoek meer Toegang ](assets/more-menu-request-more-access.png)

1. (Voorwaardelijk) als meer dan één gebruiker de aangewezen toegang heeft om u extra toegang te verlenen, toont een drop-down pijl naast de naam van de gebruiker. Selecteer de gebruiker die uw toegangsverzoek van de drop-down lijst zal ontvangen.

   Slechts tien gebruikers worden getoond in de drop-down lijst, die alfabetisch wordt gesorteerd. Voor meer informatie over de orde van de gebruikers die in dit drop-down menu worden vermeld, zie [ Hiërarchie van de &quot;Toegang van het Verzoek&quot;en &quot;Vraag Meer Toegang&quot;drop-down menu&#39;s ](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Selecteer in de vervolgkeuzelijst het toegangsniveau dat u aanvraagt.
1. (Facultatief) op het **P.S.** gebied, ga een nota betreffende in waarom u extra toegang nodig hebt.

   ![ de dialoogdoos van de Toegang van het Verzoek ](assets/request-access-to-project.png)

1. Klik **Toegang van het Verzoek**.

## Hiërarchie van de keuzemenu&#39;s Toegang aanvragen en Meer toegang aanvragen {#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus}

* [ begrijp de hiërarchie van gebruikers die in de Toegang van het Verzoek en het Verzoek Meer drop-down menu&#39;s van de Toegang worden vermeld ](#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus)
* [De eigenaar van een object begrijpen](#understand-the-owner-of-an-object)

### Begrijp de hiërarchie van gebruikers die in de drop-down menu&#39;s van de Toegang van het Verzoek en van het Verzoek Meer Toegang worden vermeld {#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus}

Wanneer het bevolken van de lijsten van de Toegang van het Verzoek of van het Verzoek Meer van de Toegang op voorwerpen, selecteert Workfront een lijst van maximaal 10 gebruikers die diverse rollen vervullen die objecten toegang tot de gebruiker kunnen verlenen die het verzoekt. De resulterende lijst wordt dan gesorteerd op hun naam in oplopende alfabetische volgorde.

De orde van de gebruikers in de Toegang van het Verzoek of het Verzoek Meer drop-down van de Toegang wordt gedicteerd door de volgende regels:

* De eerste gebruiker in de lijst is de objecten &quot;eigenaar&quot;, zoals die in [ wordt beschreven Begrijp de eigenaar van een voorwerp ](#understand-the-owner-of-an-object).
* De lijst wordt vervolgens gevuld met gebruikers met wie het object afzonderlijk wordt gedeeld. Ze worden in alfabetische volgorde weergegeven.
* De lijst wordt dan verder bevolkt met gebruikers die de vereiste toegang door het delen met hun teams, groepen, of bedrijven krijgen. Ze worden in alfabetische volgorde weergegeven.
* Als de lijst leeg is, worden de beheerders van Workfront toegevoegd zodat er altijd iemand is om toegang van te vragen. Ze worden in alfabetische volgorde weergegeven.
* Elk van de gebruikers in de lijst moet de gevraagde toegang tot het voorwerp en de toegang hebben om het voorwerp te delen.

### De eigenaar van een object begrijpen {#understand-the-owner-of-an-object}

De eigenaar van een object wordt als volgt gedefinieerd:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong> Voorwerp </strong> </th> 
   <th><strong> Definitie van de Eigenaar van het Voorwerp </strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projecten</td> 
   <td>De eigenaar is de eigenaar van het project of, als deze ontbreekt of niet over de benodigde toegang beschikt, de eigenaar van het bovenliggende portfolio. <p>Zij zouden niet de zelfde persoon kunnen zijn zoals de projectschepper. </p></td> 
  </tr> 
  <tr> 
   <td>Taken</td> 
   <td>De eigenaar is de Primaire Ontvanger of, als het ontbreekt of zij hebben niet de noodzakelijke toegang, de eigenaar van project waarop de taak, zoals hierboven bepaald verblijft. <p>Zij zouden niet de zelfde persoon kunnen zijn zoals de taakschepper. </p></td> 
  </tr> 
  <tr> 
   <td>Problemen</td> 
   <td> <p>De eigenaar is de primaire contactpersoon van de uitgave of, als deze ontbreekt of niet over de benodigde toegang beschikt, de eigenaar van het project waarop de uitgave zich bevindt, zoals hierboven gedefinieerd. </p> <p>Ze zijn mogelijk niet dezelfde persoon als de maker van de uitgave. </p> </td> 
  </tr> 
  <tr> 
   <td>Portfolio's</td> 
   <td>De eigenaar is de eigenaar van Portfolio. <p>Ze zijn mogelijk niet dezelfde persoon als de maker van de portefeuille. </p></td> 
  </tr> 
  <tr> 
   <td>Documenten</td> 
   <td>De eigenaar is de eigenaar van het document (de gebruiker die het document heeft geüpload) of, als het document ontbreekt of niet de benodigde toegang heeft, de eigenaar van het object waarop het document zich bevindt.</td> 
  </tr> 
  <tr> 
   <td>Rapporten en dashboards</td> 
   <td>De eigenaar is de maker van het rapport of het dashboard. </td> 
  </tr> 
  <tr> 
   <td>Kalenders</td> 
   <td>De eigenaar is de maker van de kalender. Aan alle gebruikers is standaard een kalender toegewezen. Zij worden beschouwd als de eigenaar van die kalender. </td> 
  </tr> 
  <tr> 
   <td>Filters, weergaven en groepen</td> 
   <td>De eigenaar van een filter, weergave of groep is de maker. </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span> Abonnementen </span> </td> 
   <td> <p><span> de eigenaar is de schepper van het plan.</span> </p> <p>Hiervoor is een aanvullende licentie vereist. </p> <p><span> voor informatie over de Planner van het Scenario van Workfront, zie </span> <a href="../../scenario-planner/scenario-planner-overview.md" class="MCXref xref"> het overzicht van de Planner van het Scenario </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Doelen</td> 
   <td> <p>De eigenaar is de gebruiker die als eigenaar is aangewezen. Ze zijn misschien niet dezelfde persoon als de maker van het doel. </p> <p>Hiervoor is een aanvullende licentie vereist. </p> <p>Voor informatie over de Doelen van Workfront, zie <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref"> overzicht van de Doelen van Adobe Workfront </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


