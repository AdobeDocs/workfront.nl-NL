---
product-area: requests
navigation-topic: create-requests
title: Weergaven maken en beheren in het gebied Verzoeken
description: Als u gebruikmaakt van de nieuwe ervaring voor aanvragen, kunt u weergaven maken en opslaan voor het gebied Verzoeken.
author: Becky
feature: Work Management
source-git-commit: d8e5e6d313eb39c9ac26e7cb60113beac5637890
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---

# Weergaven maken en beheren in het gebied Verzoeken

Als u gebruikmaakt van de nieuwe ervaring voor aanvragen, kunt u weergaven maken en opslaan voor het gebied Verzoeken. Deze weergaven omvatten filters en kolomschikkingen.

Weergaven kunnen worden gemaakt en beheerd op het gebied Verzoeken in Workfront.

>[!IMPORTANT]
>
>* Deze functionaliteit is alleen beschikbaar in de nieuwe ervaring die u opvraagt.
>* De weergave-instellingen zijn niet beschikbaar in de widget Mijn verzoeken in Home.

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

## Een weergave maken in het gebied Verzoeken

U kunt een weergave maken in het gebied Verzoeken van Workfront.

1. U kunt als volgt de lijst met verzoeken openen:

   {{step1-to-requests}}

1. In de lijst van Verzoeken, klik de **drop-down** Meningen van de Mening ![ en selecteer ](assets/view-icon-requests.png) Nieuwe mening **.**

   ![ Nieuwe mening ](assets/create-new-view.png)

1. Ga een naam voor de nieuwe mening in, en klik **creeer**.
1. Ga aan [ uit uitgeven een mening op het gebied van Verzoeken ](#edit-a-view-in-the-requests-area).

## Een weergave bewerken in het gebied Verzoeken

U kunt bestaande weergaven bewerken, inclusief de weergaven die u zojuist hebt gemaakt.

1. U kunt als volgt de lijst met verzoeken openen:

   {{step1-to-requests}}
1. Zoek in de lijst Verzoeken de weergave die u wilt bewerken.

1. (Facultatief) om een mening anders te noemen, klik **dropdown** Meningen ![ en klik het drie-punt menu naast de mening, ](assets/view-icon-requests.png) anders noemen **, dan type in de nieuwe naam voor de mening.**
1. Klik de **dropdown** drop-down Meningen ![ en selecteer de mening u wilt uitgeven.](assets/view-icon-requests.png)
1. Om een douanegebied als kolom toe te voegen, klik **kolom** pictogram ![ toevoegen kolom ](assets/add-column.png) dichtbij het recht van het scherm, en klik het plusteken naast het gebied van de douanevorm dat u als kolom aan de mening wilt toevoegen.

   >U kunt aangepaste velden op formulieren die aan het object in de lijst zijn gekoppeld, toevoegen als kolommen.

   >[!TIP]
   >
   >U kunt momenteel geen kolommen toevoegen in de productieomgeving.
1. (Facultatief) klik **Kolommen** en verberg, toon, of herschik de kolommen in de verzoeklijst.

   ![ doos van Kolommen ](assets/columns-editing-box-in-requests-planning-tab.png)

   >[!TIP]
   >
   >U kunt momenteel geen kolom meer toevoegen in de productieomgeving.

1. (Facultatief) klik **Filters** en begin voorwaarden toe te voegen voor welke verzoeken u in de Planning tabel wilt bekijken.

   ![ het Uitgeven filters in de Verzoeken tabel van de Planning ](assets/filters-editing-box-in-requests-planning-tab.png)

   U kunt filteren op de volgende velden:

   * **Workspace**: De werkruimte de verzoekvorm wordt geassocieerd met.
   * **Type van Verslag**: Het verslagtype het verzoekvorm wordt geassocieerd met.
   * **Datum van de Ingang**: De datum toen het verzoek werd voorgelegd.
   * **vorm van het Verzoek**: De naam van de verzoekvorm die wordt gebruikt om het verzoek voor te leggen.
   * **Status**: De status van het verzoek.
   * **ingegaan door**: De naam van de gebruiker die het verzoek toevoegde. Als het verzoek door iemand buiten Workfront werd toegevoegd, **ingegaan door** gebied toont `N/A`.

   U kunt ook filteren door aangepaste velden die aan de weergave zijn toegevoegd.

   U kunt veelvoudige filters hebben die door of **worden aangesloten en** of **of**.
De aanvraaglijst wordt automatisch gefilterd, aangezien u de filtervoorwaarden toevoegt.



>[!IMPORTANT]
>
> * Wijzigingen in weergaven worden automatisch opgeslagen.
> * Wijzigingen in weergaven zijn zichtbaar voor iedereen die de weergave gebruikt.
> * Om ervoor te zorgen dat de mening op de persoon van toepassing is die de mening, ongeacht gebruikt wie het creeerde, kunt u het &quot;me (het programma geopende gebruiker)&quot;filtervervanging op om het even welk gebied gebruiken dat gebruikers als waarde heeft.

## Voeg de weergave toe aan een lay-outsjabloon.

Een Workfront-beheerder kan de nieuwe weergave toevoegen aan lay-outsjablonen.

Voor instructies, zie [ Filters, Mening, en Groepen aanpassen gebruikend een lay-outmalplaatje ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Een weergave delen

U kunt weergaven delen die u maakt met andere gebruikers, teams of groepen.

1. U kunt als volgt de lijst met verzoeken openen:

   {{step1-to-requests}}

1. Zoek in de lijst Verzoeken de weergave die u wilt delen.
1. Houd de muisaanwijzer boven de weergave die u wilt delen en klik vervolgens op het menu met drie punten wanneer deze wordt weergegeven.
1. Selecteer **Aandeel**.
1. Voer in het dialoogvenster dat wordt geopend de namen in van de gebruikers, teams of groepen waarmee u de weergave wilt delen en selecteer ze in de lijst wanneer ze worden weergegeven.
1. Klik **sparen**.

