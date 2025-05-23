---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Verwijs een douaneformulier in een rapport
description: U kunt naar de aangepaste formulieren van een object verwijzen in de weergaven, filters en groepen van een rapport voor dat object.
author: Nolan
feature: Reports and Dashboards
exl-id: 8b0d2e7f-cc92-4f43-a91c-ab2b2d8a1c01
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 0%

---

# Verwijs een douaneformulier in een rapport

<!-- Audited: 11/2024 -->

U kunt naar de aangepaste formulieren van een object verwijzen in de weergaven, filters en groepen van een rapport voor dat object.

U kunt verwijzen naar de inhoud van aangepaste formulieren die u in een rapport wilt opnemen, of u kunt verwijzen naar informatie over de aangepaste formulieren die u zelf in een rapport wilt opnemen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
      <td> 
      <p>Nieuw:</p>
         <ul>
         <li><p>Standaard</p></li>
         </ul>
      <p>Huidige:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p></td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Het aangepaste formulier moet bestaan voordat u ernaar kunt verwijzen in een rapport.

Voor meer informatie bij het creëren van douaneformulieren, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

## Verwijzen naar de inhoud van aangepaste formulieren

U kunt verwijzen naar velden in aangepaste formulieren. Nadat een aangepast formulier op een object is toegepast, zijn alle velden die aan dat aangepaste formulier zijn gekoppeld, beschikbaar om in een rapport naar een ander veld in het object te worden verwezen, net als alle andere velden in het object.

>[!NOTE]
>
>Voor velden met meerdere opties zijn alle opties beschikbaar in de filters en vragen van het rapport, inclusief de opties die verborgen zijn.\
>Voor meer informatie over het verbergen van keuzen van een douanegebied met veelvoudige opties, zie het artikel [ een douanevorm ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

Wanneer u het rapport maakt, gebruikt u gewoon het objecttype van het formulier als de veldbron en gebruikt u de naam van het aangepaste veld als de veldnaam.

Bijvoorbeeld, zou u een douanevorm kunnen hebben die op alle projecten wordt toegepast die de adviseur van het douanegebied **&#x200B;**&#x200B;omvat. Om een rapport tot stand te brengen dat van alle projecten een lijst maakt waar Olivia Kim de consultant is, gebruik het **objecten van het 0&rbrace; Project &lbrace;als gebiedsbron, en gebruik** Consultant **als gebiedsnaam.** Plaats het filterbepaler aan **Gelijk**, toen type Olivia Kim.

![ Consultant filter ](assets/qs-consultant-filter-example-350x126.png)

Voor meer informatie over het creëren van een rapport, zie het artikel [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

## Referentiegegevens over aangepaste formulieren

U kunt verwijzen naar informatie over aangepaste formulieren, zoals de naam van aangepaste formulieren die aan een object zijn gekoppeld.

&#x200B; Afhankelijk van het element (Weergave, Filter of Groepering) kunt u naar een van de volgende opties verwijzen:

* Het primaire aangepaste formulier dat op een object wordt toegepast:

  Dit is het formulier dat het eerst wordt weergegeven op de pagina Details van het object.

* Alle aangepaste formulieren (als er meerdere aangepaste formulieren op een object zijn toegepast)

U kunt naar aangepaste formulieren verwijzen in Weergaven, Filters en Groepen:

* [ de douaneformulieren van de Verwijzing in een Mening van het rapport (Kolom) ](#reference-custom-forms-in-a-report-view-column)
* [ de douanevormen van de Verwijzing in een rapportfilter ](#reference-custom-forms-in-a-report-filter)
* [Verwijzing douaneformulieren in een rapport groeperen](#reference-custom-forms-in-a-report-grouping)

### Verwijzing douaneformulieren in een rapportmening (Kolom) {#reference-custom-forms-in-a-report-view-column}

Alle aangepaste formulieren weergeven die aan een object zijn gekoppeld:

1. Begin creërend een rapport zoals die in het artikel [ wordt beschreven creeer een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Op het **lusje van Kolommen**, breid het objecten type uit dat de douanevorm die u wilt van verwijzingen voorzien wordt toegepast op, dan klik **Naam van de Categorie**.\
   Bijvoorbeeld, om alle douaneformulieren te tonen verbonden aan een taak, breid de **het gebiedsbron van de Taak** &lbrace;uit, dan klik de **Naam van de Categorie** gebiedsnaam.\
   ![ de naamkolom van de Categorie ](assets/qs-category-name-column-350x267.png)

Alleen het primaire aangepaste formulier weergeven dat aan het object is gekoppeld:

1. Begin creërend een rapport zoals die in het artikel [ wordt beschreven creeer een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Op het **lusje van Kolommen**, breid de **bron van het Categorie** gebied uit, dan klik de **Naam** gebiedsnaam.\
   ![ Naam van de Categorie ](assets/qs-category-name-column-2-350x248.png)

### Verwijzing douaneformulieren in een rapportfilter {#reference-custom-forms-in-a-report-filter}

Filteren op alle aangepaste formulieren die aan het objecttype zijn gekoppeld:

1. Begin creërend een rapport zoals die in het artikel [ wordt beschreven creeer een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Op het **lusje van Filters**, breid **Categorieën** uit, dan klik **Naam**.\
   ![ de naamfilter van de Categorie ](assets/qs-categories-name-filter-350x311.png)

1. Selecteer de voorwaarde-aanduiding die u wilt gebruiken:

   * Is leeg
   * Is niet leeg
   * Bevat
   * Bevat niet
   * Gelijk
   * Niet gelijk

   Voor meer informatie over elke kwalificatie, zie de artikel [ Filter en voorwaardenbepalingen ](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Als het gebied u voor heeft veelvoudige opties filtert en u **niet Gelijk** gebruikt of **&#x200B;**&#x200B;geen bepalende eigenschappen bevat, bevat dit filters uit de resultaten die slechts de keus bevatten u specificeert. Als het veld aanvullende opties bevat, inclusief de opgegeven optie, worden die resultaten niet uit het rapport gefilterd. Dit omvat het filtreren voor veelvoudige Douane Forms als zij aan het zelfde voorwerp in bijlage zijn.

1. Typ de naam van het aangepaste formulier waarop u wilt filteren en klik vervolgens op de naam wanneer dit wordt weergegeven in de vervolgkeuzelijst.
1. (Facultatief) klik **voeg een andere Regel van de Filter toe**, dan herhaal stappen 2-4 om extra filterregels tot stand te brengen.
1. Klik **sparen+Sluiten**.

Alleen filteren op het primaire aangepaste formulier dat is gekoppeld aan het objecttype:

1. Begin creërend een rapport zoals die in het artikel [ wordt beschreven creeer een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Op het **lusje van Filters**, breid de **bron van het Categorie** gebied uit, dan klik de **Naam** gebiedsnaam.\
   ![ de naamfilter van de Categorie ](assets/qs-category-name-filter-350x437.png)

1. Selecteer de voorwaarde-aanduiding die u wilt gebruiken:

   * Is leeg
   * Is niet leeg
   * Bevat
   * Bevat niet
   * Gelijk
   * Niet gelijk

   Voor meer informatie over elke kwalificatie, zie de artikel [ Filter en voorwaardenbepalingen ](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. Typ de naam van het aangepaste formulier waarop u wilt filteren en klik vervolgens op de naam wanneer dit wordt weergegeven in de vervolgkeuzelijst.
1. (Facultatief) klik **voeg een andere Regel van de Filter toe**, dan herhaal stappen 2-4 om extra filterregels tot stand te brengen.
1. Klik **sparen+Sluiten**.

### Verwijzing douaneformulieren in een rapport groeperen {#reference-custom-forms-in-a-report-grouping}

>[!NOTE]
>
>U kunt items alleen groeperen op het primaire aangepaste formulier dat aan het object is gekoppeld. U kunt items niet groeperen door alle formulieren die aan het object zijn gekoppeld.

1. Begin creërend een rapport zoals die in het artikel [ wordt beschreven creeer een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Op het **lusje van Groepen**, breid **Categorie** uit, dan klik **Naam**.\
   ![ Naam groepering van de Categorie ](assets/qs-category-name-grouping-350x373.png)
