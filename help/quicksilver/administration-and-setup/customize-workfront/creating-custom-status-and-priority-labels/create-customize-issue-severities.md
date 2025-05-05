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
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# Uitgiftecontroles maken of aanpassen

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

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
     <p>Nieuw: Standaard</p>
     <p>of</p>
     <p>Huidig: Plan</p>
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

## Ingebouwde uitgavendeclaraties

Workfront beschikt over vijf ingebouwde uitgavesecties:

* Cosmetisch
* Verwardheid
* Fout met tijdelijke oplossing
* Fout zonder tijdelijke oplossing
* Fatale fout

<p>U kunt het volgende bewerken voor deze controles:</p>

* Naam
* Kleur

  De kleur van een ernst blijft behouden in een diagramrapport als u de resultaten groepeert op Issue Severity. Voor informatie over grafiekrapporten, zie [ een grafiek aan een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md) toevoegen.

* Welke strengheid is het gebrek

  Voor meer informatie over standaardcontroles, zie [ creeer of geef een kwestie strengheid ](#create-or-edit-an-issue-severity) in dit artikel uit.
* Beschrijving
* Of een ernst verborgen is in Workfront

  Voor meer informatie over het verbergen van een strengheid, zie [ creeer of geef een kwestie strengheid ](#create-or-edit-an-issue-severity") uit

* Ernst verwijderen

  Wanneer u dit doet, moet u een vervangingsstrengheid selecteren.

## Ernst van uitgaven maken of bewerken {#create-or-edit-an-issue-severity}

Als Workfront-beheerder kunt u uitgiftesetters maken en bewerken die zijn afgestemd op de behoeften van uw gebruikers.

{{step-1-to-setup}}

1. In het linkerpaneel, klik **>** de Voorkeur van het Project **&#x200B;**.

1. Als u een nieuwe strengheid creeert, voegt de klik **een Nieuwe Ernst** toe.
1. Vorm de volgende opties voor de nieuwe strengheid of geef hen voor bestaande uit:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ernstnaam</td> 
      <td>Typ een naam voor de ernst</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Belang</td> 
      <td>Verhoog of verlaag de ernst die oorspronkelijk door Workfront is toegewezen.
      <p>Het belangrijke aantal voor elke strengheid moet uniek zijn. Het hoogste getal komt overeen met het hoogste niveau van ernst.</p> <p>U kunt dit nummer niet bewerken nadat u de ernst hebt opgeslagen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kleur</td> 
      <td> <p>Kies een kleur voor de ernst.</p> 
      <p>De kleur van de ernst wordt gebruikt in grafiekrapporten wanneer u uw resultaten groepeert door de Ernst van de Uitgave. Voor informatie over grafiekrapporten, zie <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref"> een grafiek aan een rapport </a> toevoegen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standaardernst</td> 
      <td>Selecteer de ernst die Workfront automatisch moet selecteren voor alle nieuwe uitgaven.</p>
      <p>Cosmetisch is de standaardernst voor problemen in Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschrijving</td> 
      <td>Typ een beschrijving voor de ernst om de functie uit te leggen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verbergen</td> 
      <td> Verberg een ernst die u niet meer nodig hebt. 
      <p>Een verborgen ernst wordt nergens in Workfront weergegeven, dus gebruikers kunnen deze optie niet kiezen voor hun uitgaven.</p> 
      <p><b> BELANGRIJK </b>: In plaats van het schrappen van controles die u niet meer wilt gebruiken, stellen wij voor dat u hen verbergt. Op deze manier houdt u al uw historische gegevens over objecten die al met de ernst zijn voltooid, en voorkomt u dat mensen in de toekomst de ernst van de zaak zullen gebruiken.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Wijzig de volgorde van de aanbiedingen door deze in de gewenste volgorde te slepen.

   Dit verandert de orde waarin zij voor kwesties tonen. Het verandert niet het **Aantal van het Belang**.

1. Klik **sparen**.

Voor meer informatie over hoe te om servers te gebruiken terwijl het werken met kwesties, zie [ de vraagstrengheid van de Update ](../../../manage-work/issues/issue-information/update-issue-severity.md).
