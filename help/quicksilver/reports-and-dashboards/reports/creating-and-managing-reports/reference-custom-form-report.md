---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Verwijs een douaneformulier in een rapport
description: U kunt naar de aangepaste formulieren van een object verwijzen in de weergaven, filters en groepen van een rapport voor dat object.
author: Nolan
feature: Reports and Dashboards
exl-id: 8b0d2e7f-cc92-4f43-a91c-ab2b2d8a1c01
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '998'
ht-degree: 0%

---

# Verwijs een douaneformulier in een rapport

U kunt naar de aangepaste formulieren van een object verwijzen in de weergaven, filters en groepen van een rapport voor dat object.

U kunt verwijzen naar de inhoud van aangepaste formulieren die u in een rapport wilt opnemen, of u kunt verwijzen naar informatie over de aangepaste formulieren die u zelf in een rapport wilt opnemen.

## Toegangsvereisten

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Vereisten

Het aangepaste formulier moet bestaan voordat u ernaar kunt verwijzen in een rapport.

Voor meer informatie bij het creëren van douaneformulieren, zie [ een douaneformulier ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) creëren of uitgeven.

## Verwijzen naar de inhoud van aangepaste formulieren

U kunt verwijzen naar velden in aangepaste formulieren. Nadat een aangepast formulier op een object is toegepast, zijn alle velden die aan dat aangepaste formulier zijn gekoppeld, beschikbaar om in een rapport naar een ander veld in het object te worden verwezen, net als alle andere velden in het object.

>[!NOTE]
>
>Voor velden met meerdere opties zijn alle opties beschikbaar in de filters en vragen van het rapport, inclusief de opties die verborgen zijn.\
>Voor meer informatie over het verbergen van keuzen van een douanegebied met veelvoudige opties, zie het artikel [ creeer of geef een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) uit.

Wanneer u het rapport maakt, gebruikt u gewoon het objecttype van het formulier als de veldbron en gebruikt u de naam van het aangepaste veld als de veldnaam.

Bijvoorbeeld, zou u een douanevorm kunnen hebben die op alle projecten wordt toegepast die de adviseur van het douanegebied **** omvat. Om een rapport tot stand te brengen dat van alle projecten een lijst maakt waar Olivia Kim de consultant is, gebruik het **objecten van het 0} Project {als gebiedsbron, en gebruik** Consultant **als gebiedsnaam.** Plaats het filterbepaler aan **Gelijk**, toen type Olivia Kim.

![](assets/qs-consultant-filter-example-350x126.png)

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
   Bijvoorbeeld, om alle douaneformulieren te tonen verbonden aan een taak, breid de **het gebiedsbron van de Taak** {uit, dan klik de **Naam van de Categorie** gebiedsnaam.\
   ![](assets/qs-category-name-column-350x267.png)

Alleen het primaire aangepaste formulier weergeven dat aan het object is gekoppeld:

1. Begin creërend een rapport zoals die in het artikel [ wordt beschreven creeer een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Op het **lusje van Kolommen**, breid de **bron van het Categorie** gebied uit, dan klik de **Naam** gebiedsnaam.\
   ![](assets/qs-category-name-column-2-350x248.png)

### Verwijzing douaneformulieren in een rapportfilter {#reference-custom-forms-in-a-report-filter}

Filteren op alle aangepaste formulieren die aan het objecttype zijn gekoppeld:

1. Begin creërend een rapport zoals die in het artikel [ wordt beschreven creeer een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Op het **lusje van Filters**, breid **Categorieën** uit, dan klik **Naam**.\
   ![](assets/qs-categories-name-filter-350x311.png)

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
   >Als het gebied u voor heeft veelvoudige opties filtert en u **niet Gelijk** gebruikt of **** geen bepalende eigenschappen bevat, bevat dit filters uit de resultaten die slechts de keus bevatten u specificeert. Als het veld aanvullende opties bevat, inclusief de opgegeven optie, worden die resultaten niet uit het rapport gefilterd. Dit omvat het filtreren voor veelvoudige Douane Forms als zij aan het zelfde voorwerp in bijlage zijn.

1. Typ de naam van het aangepaste formulier waarop u wilt filteren en klik vervolgens op de naam wanneer dit wordt weergegeven in de vervolgkeuzelijst.
1. (Facultatief) klik **voeg een andere Regel van de Filter toe**, dan herhaal stappen 2-4 om extra filterregels tot stand te brengen.
1. Klik **sparen+Sluiten**.

Alleen filteren op het primaire aangepaste formulier dat is gekoppeld aan het objecttype:

1. Begin creërend een rapport zoals die in het artikel [ wordt beschreven creeer een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Op het **lusje van Filters**, breid de **bron van het Categorie** gebied uit, dan klik de **Naam** gebiedsnaam.\
   ![](assets/qs-category-name-filter-350x437.png)

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
   ![](assets/qs-category-name-grouping-350x373.png)
