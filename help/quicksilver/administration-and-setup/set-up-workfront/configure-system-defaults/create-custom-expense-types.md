---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Aangepaste kostentypen maken
description: Als  [!DNL Adobe Workfront]  beheerder, kunt u de types van douanefoto tot stand brengen om de uitgaven te bepalen en te volgen verbonden aan uw taken en projecten. De kosten zijn niet-arbeidskosten die met taken of projecten kunnen worden geassocieerd.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 7f95df7acfb1afd0974c0138152a68326631d265
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 1%

---

# Aangepaste uitgaventypen maken

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Als [!DNL Adobe Workfront] beheerder, kunt u de types van douaneuitgave tot stand brengen om de uitgaven te bepalen en te volgen verbonden aan uw taken en projecten. De kosten zijn niet-arbeidskosten die met taken of projecten kunnen worden geassocieerd.

U kunt alle onkostentypen die u maakt, bewerken of verwijderen. U kunt de ingebouwde uitgaventypen van [!DNL Workfront] niet verwijderen of bewerken.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td><p>Nieuw: [!UICONTROL Standard]</p>
   of
   <p>Huidige: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr>
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Standaarduitgaventypen

De standaarduitgaventypen in [!DNL Workfront] die niet kunnen worden verwijderd of bewerkt, zijn onder andere:

* [!UICONTROL Advertising]
* [!UICONTROL Consulting]
* [!UICONTROL Entertainment]
* [!UICONTROL General]
* [!UICONTROL Materials]
* [!UICONTROL Travel]

## Aangepaste uitgaventypen maken

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Expense Types]**.
1. Klik op **[!UICONTROL New expense type]**.
1. Voer in het dialoogvenster **[!UICONTROL New Expense Type]** de volgende gegevens in:

   * **Naam** - een naam voor de uitgave.
   * **Beschrijving** - een beschrijving van de uitgave.
   * **Berekende Eenheid** - selecteer de eenheid van meting voor uw uitgaventype van de drop-down lijst. De volgende maateenheden zijn beschikbaar:

      * Mile
      * Kilometer
      * Kilogram
      * Dollar
      * Uur
      * Dag
      * Anders - Als u deze optie selecteert, wordt u gevraagd de maateenheid een naam te geven en de maateenheid te definiëren als iets dat uw organisatie kent.

   * **Tarief** - de prijs per eenheid. Dit is een munt geformatteerd gebied en het vertegenwoordigt de kosten van elke eenheid die op het **Berekende gebied van de Eenheid** wordt gevestigd. De snelheid kan een numerieke waarde met maximaal 4 cijfers achter de komma bevatten. Bijvoorbeeld 1,0375.

1. Klik op **[!UICONTROL Save]**.

   Het uitgaventype is nu beschikbaar voor gebruikers om het met hun uitgaven op projecten en taken te associëren.

## Aangepaste uitgaventypen wijzigen

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Expense Types]**.
1. Selecteer het onkostentype dat u wilt wijzigen, dan klik het **[!UICONTROL Edit]** pictogram ![ uitgeven pictogram ](assets/edit-icon.png).

   Het dialoogvenster **[!UICONTROL Edit Expense Type]** wordt weergegeven.

1. Breng de gewenste wijzigingen aan en klik op **[!UICONTROL Save]** .

   Het uitgaventype is nu beschikbaar voor gebruikers om het met hun uitgaven op projecten en taken te associëren.

Voor meer informatie over hoe te om kosten te gebruiken en hoe zij de kosten van een project kunnen beïnvloeden, zie artikel [ projectuitgaven beheren ](../../../manage-work/projects/project-finances/manage-project-expenses.md).
