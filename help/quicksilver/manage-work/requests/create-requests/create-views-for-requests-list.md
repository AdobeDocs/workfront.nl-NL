---
product-area: requests
navigation-topic: create-requests
title: Weergaven maken en beheren in het gebied Verzoeken
description: Als u gebruikmaakt van de nieuwe ervaring voor aanvragen, kunt u weergaven maken en opslaan voor het gebied Verzoeken.
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
source-git-commit: e4d57d0b5042dc4889d5b676396b56c05ab1515d
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 0%

---


# Weergaven maken en beheren in het gebied Verzoeken

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>





Als u de nieuwe verzoekervaring in Adobe Workfront gebruikt, kunt u meningen voor het gebied van Verzoeken tot stand brengen en bewaren. Deze weergaven omvatten filters en kolomschikkingen.

<!--<span class="preview"> and groupings.</span>-->


>[!IMPORTANT]
>
>* Deze functionaliteit is alleen beschikbaar in de nieuwe ervaring die u opvraagt op het gebied Verzoeken.
>* De weergave-instellingen zijn ook beschikbaar in de widget Mijn verzoeken in Home. De weergaven in het gebied Verzoeken zijn echter gescheiden van die in de widget Mijn verzoeken.
>* De lijst met verzoeken in het gebied Verzoeken gebruikt de uitgebreide lijst in Workfront. Voor meer informatie, zie [ Gebruik verbeterde lijsten ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Medewerker of hoger</p>
   <p>Aanvraag of hoger</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot problemen bewerken</p>  <p>U moet een Workfront-beheerder zijn om weergaven toe te voegen aan lay-outsjablonen</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>U moet Adobe Workfront Planning hebben om de verzoeken van de Planning te bekijken of om formulieren te verzoeken</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een weergave voor aanvragen maken

U kunt een weergave maken in het gebied Verzoeken van Workfront wanneer u de nieuwe aanvraagervaring gebruikt.

1. U kunt als volgt de lijst met verzoeken openen:

   {{step1-to-requests}}

1. Verzeker het **gebruik nieuwe ervaring** het plaatsen wordt aangezet.

1. In de **lijst van Verzoeken**, klik de **3} dropdown menu van Meningen** dropdown ![ en klik ](assets/view-icon-requests.png) Nieuwe mening **.**

   ![ Nieuwe mening ](assets/create-new-view.png)

1. Ga een naam voor de nieuwe mening in, en klik **creeer**.
1. Ga aan [ uit uitgeven een mening op het gebied van Verzoeken ](#edit-a-view-in-the-requests-area).

## Een weergave voor aanvragen bewerken

U kunt bestaande weergaven bewerken, inclusief de weergaven die u zojuist hebt gemaakt in het gedeelte Aanvragen van Workfront.

Door een weergave te bewerken in het gebied Verzoeken kunt u de volgende elementen van de weergave wijzigen:

* Naam
* Filters
* Kolommen

De wijzigingen die u aanbrengt in een weergave, zijn zichtbaar voor alle gebruikers met wie u de weergave deelt.

1. Een lijst met verzoeken in de verzoeken kan als volgt worden geopend:

   {{step1-to-requests}}

1. Verzeker het **gebruik nieuwe ervaring** het plaatsen wordt aangezet.
1. In de **lijst van Verzoeken**, bepaal de plaats van de mening die u van het **** dropdown menu van Meningen ![ dropdown ](assets/view-icon-requests.png) wilt uitgeven Meningen.

1. Klik de **dropdown** Meningen 1} van Meningen ![ en klik het drie-punt menu naast de mening, uitgezocht ](assets/view-icon-requests.png) anders noemen **, dan type in de nieuwe naam voor de mening.**
1. Druk op Enter om de nieuwe naam op te slaan.
1. Klik de **dropdown** drop-down Meningen ![ en selecteer de mening u wilt uitgeven.](assets/view-icon-requests.png)
1. Om een gebied als kolom toe te voegen, klik **kolom** pictogram ![ toevoegen kolom ](assets/add-column.png) in de hoger-juiste hoek van de lijst.

   De **manager van de Kolom** opent.
1. Klik het plusteken naast het gebied dat u als kolom aan de mening wilt toevoegen, dan klik **sparen**.

   Velden die aan de objecten in de lijst zijn gekoppeld, kunnen als kolommen worden toegevoegd. <!--keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future-->

   >[!TIP]
   >
   >De gebieden u aan de kolommen toevoegt moeten bestaan alvorens zij in de **manager van de Kolom** beschikbaar zijn.


1. (Facultatief) klik **Kolommen** om F **het zicht en de orde van het gebiedsdeel te openen** doos.
1. Schakel de instelling in voor elk veld dat u in de lijst wilt weergeven, schakel deze uit om het te verbergen of sleep de velden in een andere volgorde.

1. (Facultatief) klik **Filters** en begin voorwaarden toe te voegen voor welke verzoeken u wilt bekijken.

   U kunt filteren op de volgende aanvraagvelden:

   * **Workspace**: De werkruimte de verzoekvorm wordt geassocieerd met.
   * **Type van Objecten**: Het verslagtype het verzoekvorm wordt geassocieerd met.
   * **Datum van de Ingang**: De datum toen het verzoek werd voorgelegd.
   * **vorm van het Verzoek**: De naam van de verzoekvorm die wordt gebruikt om het verzoek voor te leggen.
   * **Status**: De status van het verzoek.
   * **ingegaan door**: De naam van de gebruiker die het verzoek toevoegde. Als het verzoek door iemand buiten Workfront werd toegevoegd, **ingegaan door** gebied toont `N/A`.

   U kunt ook filteren door alle velden die aan de weergave zijn toegevoegd voor elk object dat zichtbaar is in de weergave.

   U kunt veelvoudige filters hebben die door of **worden aangesloten en** of **of**.
De aanvraaglijst wordt automatisch gefilterd, aangezien u de filtervoorwaarden toevoegt.


<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * Wijzigingen in weergaven worden automatisch opgeslagen.
> * Wijzigingen in weergaven zijn zichtbaar voor iedereen die de weergave gebruikt.
> * Gebruik **me (het programma geopende gebruiker)** filtervervanging op om het even welk gebied dat gebruikers als waarde heeft.

## Voeg de verzoekmening aan een lay-outmalplaatje toe.

Een Workfront-beheerder kan de nieuwe weergave toevoegen aan lay-outsjablonen.

Voor instructies, zie [ Filters, Mening, en Groepen aanpassen gebruikend een lay-outmalplaatje ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Een weergave delen

U kunt weergaven delen die u maakt met andere gebruikers, teams of groepen.

1. Een lijst met verzoeken in de verzoeken kan als volgt worden geopend:

   {{step1-to-requests}}

1. Verzeker het **gebruik nieuwe ervaring** het plaatsen wordt aangezet.
1. In de **lijst van Verzoeken**, bepaal de plaats van de mening die u wilt delen.
1. Beweeg over de mening die u wilt delen, dan klik op het drie-punt menu rechts van de meningsnaam, dan klik **Aandeel**.
1. In het **vakje van het Aandeel**, ga de mensen, de teams, de rollen, de groepen, of de bedrijven in die u de mening met wilt delen, dan hen van de lijst selecteren wanneer zij verschijnen.
1. Klik **sparen**.

   De weergave wordt gedeeld met de entiteiten die u aangeeft. Ze kunnen de bijgewerkte weergave-elementen die u voor de weergave hebt bewerkt, bekijken voordat ze deze delen. <span class="preview"> als zij de mening bijwerken, zullen hun veranderingen niet zichtbaar aan anderen, tenzij zij een exemplaar van de zelfde mening maken en hun veranderingen bewaren alvorens zij het exemplaar delen. Voor meer informatie, zie [ Gebruik verbeterde lijsten ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>
