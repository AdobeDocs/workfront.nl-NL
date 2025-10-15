---
title: Probleemernst maken of aanpassen
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Uw gebruikers kunnen serienummers gebruiken om te bepalen hoe ernstig een probleem is. U kunt een van de vijf standaardserienummers in Adobe Workfront aanpassen of een nieuwe ernst maken voor uw gebruikers.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: b0b9b80b4eb718e3e131ee0cd022f54cb906f187
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---

# Uitgiftecontroles maken of aanpassen

{{highlighted-preview}}

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

Uw gebruikers kunnen serienummers gebruiken om te bepalen hoe ernstig een probleem is. U kunt een van de vijf standaardserienummers in Adobe Workfront aanpassen of een nieuwe ernst maken voor uw gebruikers.

>[!NOTE]
>
>Taken en projecten hebben geen verificaties.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>Systeembeheerder</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

## Ingebouwde uitgavendeclaraties

Workfront beschikt over vijf ingebouwde uitgavesecties:

* Cosmetisch
* Verwardheid
* Fout met tijdelijke oplossing
* Fout zonder tijdelijke oplossing
* Fatale fout

U kunt het volgende bewerken voor deze controles:

* Naam
* Kleur

  De kleur van een ernst blijft behouden in een diagramrapport als u de resultaten groepeert op Issue Severity. Voor informatie over grafiekrapporten, zie [ een grafiek aan een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md) toevoegen.

* Welke strengheid is het gebrek

  Voor meer informatie over standaardcontroles, zie [ creeer of geef een kwestie strengheid ](#create-or-edit-an-issue-severity) in dit artikel uit.

* Beschrijving
* Of een ernst verborgen is in Workfront

  Voor meer informatie over het verbergen van een strengheid, zie [ creeer of geef een kwestie strengheid ](#create-or-edit-an-issue-severity) in dit artikel uit.

* Ernst verwijderen

  Wanneer u dit doet, moet u een vervangingsstrengheid selecteren.

## Ernst van uitgaven maken of bewerken {#create-or-edit-an-issue-severity}

Als Workfront-beheerder kunt u uitgiftesetters maken en bewerken die zijn afgestemd op de behoeften van uw gebruikers.

{{step-1-to-setup}}

1. In het linkerpaneel, klik **>** de Voorkeur van het Project ****.

1. Als u een nieuwe strengheid creeert, klik <span class="preview">**Nieuwe rij** bij de bodem van de lijst </span>, of **voeg een Nieuwe Ernst** toe.
1. Vorm de volgende opties voor de nieuwe strengheid of geef hen voor bestaande uit:

   * **Naam van de Ernst**: Type een naam voor de strengheid.
   * **Belangrijk**: Verhoog of verklein het niveau van ernst, oorspronkelijk toegewezen door Workfront, voor de strengheid.

     Het belangrijke aantal voor elke strengheid moet uniek zijn. Het hoogste getal komt overeen met het hoogste niveau van ernst.

     U kunt dit nummer niet bewerken nadat u de ernst hebt opgeslagen.

   * **Kleur**: Kies een kleur voor de strengheid.

     De kleur van de ernst wordt gebruikt in grafiekrapporten wanneer u uw resultaten groepeert door de Ernst van de Uitgave. Voor informatie over grafiekrapporten, zie [ een grafiek aan een rapport ](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md) toevoegen.

   * **StandaardErnst van de Ernst**: Selecteer de strengheid u Workfront automatisch op alle pas gecreëerde kwesties wilt toepassen.

     **Cosmetic** is de standaardstrengheid voor kwesties in Workfront.

     U kunt een verborgen ernst niet als standaard instellen.

     <div class="preview">

     De standaardstrengheid wordt vermeld met een pictogram ![ Standaard strengheidspictogram ](assets/default-icon.png). Voer een van de volgende handelingen uit om een nieuwe standaardinstelling te kiezen:

      * Selecteer de controledoos naast de ernstnaam en selecteer **maak Gebrek** in de actiebar bij de bodem van het scherm.
      * Beweeg over de ernstnaam en klik **Meer** menu dat verschijnt. Dan, uitgezochte **maak Gebrek**.

        De nieuwe standaardernst wordt geëtiketteerd met het pictogram.

     </div>

   * **Beschrijving**: Typ een beschrijving voor de strengheid om zijn functie te verklaren.
   * <span class="preview">**Keuze van de Huid**</span> of **Verbergen**: <span class="preview"> Uitgezochte **ja**</span> of selecteer de controledoos om een strengheid te verbergen die niet meer nodig is.

     Een verborgen ernst wordt nergens in Workfront weergegeven, dus gebruikers kunnen deze optie niet kiezen voor hun uitgaven.

     >[!IMPORTANT]
     >
     >In plaats van de controles te verwijderen die u niet meer wilt gebruiken, raden we u aan ze te verbergen. Op deze manier houdt u al uw historische gegevens over objecten die al met de ernst zijn voltooid, en voorkomt u dat mensen in de toekomst de ernst van de zaak zullen gebruiken.

1. (Optioneel) Wijzig de volgorde van de aanbiedingen door deze in de gewenste volgorde te slepen.

   Dit verandert de orde waarin zij voor kwesties tonen. Het verandert niet het **Aantal van het Belang**.

1. Klik **sparen**.

Voor meer informatie over hoe te om servers te gebruiken terwijl het werken met kwesties, zie [ de vraagstrengheid van de Update ](../../../manage-work/issues/issue-information/update-issue-severity.md).
