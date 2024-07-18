---
title: Prioriteiten maken en aanpassen
description: U kunt de prioriteiten voor projecten, taken, en kwesties in het gebied van de Opstelling van Workfront controleren. Prioriteiten geven belang aan uw projecten, taken of problemen in Adobe Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# Prioriteiten maken en aanpassen

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

U kunt de prioriteiten voor projecten, taken, en kwesties in het gebied van de Opstelling van Workfront controleren. Prioriteiten geven belang aan uw projecten, taken of problemen in Adobe Workfront.

## Toegangsvereisten

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw beheerder van Workfront als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Bestaande prioriteiten aanpassen

Als beheerder van Workfront, kunt u de volgende wijzigingen in de standaardprioriteiten aanbrengen die in Workfront worden verstrekt:

* Wijzig de naam van prioriteiten.
* Herstel de prioriteiten.

  Voor meer informatie over hoe te om prioriteiten te herschikken, zie [ een prioriteit voor een projecttaak, of uitgeven ](#create-a-priority-for-a-project-task-or-issue) creëren.

* Wijzig de standaardprioriteit.

  Voor meer informatie over de functionaliteit om de standaardprioriteit te veranderen, zie [ een prioriteit voor een projecttaak, of kwestie ](#create-a-priority-for-a-project-task-or-issue) creëren.

* Bewerk de beschrijving van de prioriteiten.
* Stel een kleur in voor elke prioriteit.

  De kleur van de prioriteit wordt gebruikt in grafiekrapporten, wanneer u uw resultaten door **Prioriteit** groepeert.

  Voor meer informatie over grafiekrapporten, zie [ een grafiek aan een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md) toevoegen.

* Prioriteiten verwijderen.

  Wanneer u een bestaande prioriteit verwijdert, moet u een vervangende prioriteit selecteren.

* Prioriteiten verbergen.

  Voor meer informatie over de functionaliteit om prioriteiten te verbergen, zie [ een prioriteit voor een projecttaak, of uitgeven ](#create-a-priority-for-a-project-task-or-issue) creëren.

  >[!NOTE]
  >
  >U moet voor elk object ten minste één prioriteit in uw Workfront-account hebben.

De prioriteiten die standaard worden opgegeven voor elk objecttype (project, taak en uitgave) zijn identiek:

* Geen
* Laag
* Normaal
* Hoog
* Dringend

## Een prioriteit maken voor een projecttaak of uitgave {#create-a-priority-for-a-project-task-or-issue}

Naast de standaardprioriteiten in Workfront kunt u ook uw eigen prioriteiten toevoegen om aan de behoeften van uw organisatie te voldoen.

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Opstelling** ![](assets/gear-icon-settings.png).

1. In het linkerpaneel, klik **Voorkeur van het Project** > **Prioriteiten**.

1. Klik het lusje voor het objecten type u een prioriteit voor (**Project**, **Taak**, of **Kwestie**) wilt tot stand brengen.
1. Klik **toevoegen een Nieuwe Prioriteit**.
1. Geef de volgende informatie op voor de nieuwe prioriteit:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Prioriteitsnaam</td> 
      <td>Typ een naam voor uw prioriteit.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Belang</td> 
      <td> <p>Wanneer het toevoegen van een nieuwe prioriteit, wordt een aantal toegewezen aan het door gebrek. Bewerk dit nummer als het niet aan uw wensen voldoet.</p> <p>Het </strong> aantal van het belang <strong> {voor elke prioriteit moet voor het voorwerp uniek zijn u selecteerde.<br> het aantal van de prioriteit wijst op het belang van het project, de taak of de kwestie: het hoogste aantal beantwoordt aan de hoogste prioriteit.</p> <p><b> NOTA </b>: U kunt niet het aantal van de Belangrijkheid uitgeven, nadat u sparen de prioriteit. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kleur</td> 
      <td> <p>Kies een kleur voor uw prioriteit.</p> <p>De kleur van de prioriteit wordt gebruikt in grafiekrapporten en de Montages van het Team van de Gelijkheid. Voor meer informatie over grafiekrapporten, zie <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref"> een grafiek aan een rapport </a> toevoegen.</p> <p>Voor meer informatie over de Montages van het Team van de Geldige, zie in.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standaardprioriteit</td> 
      <td> <p>Bepaal of dit een standaardprioriteit moet zijn of niet door het keuzerondje te selecteren.</p> <p>Als een prioriteit als <strong> StandaardPrioriteit </strong> wordt aangewezen, wordt het automatisch gekozen voor alle projecten, taken, of kwesties in Workfront. <strong> Normaal </strong> is de standaardprioriteit voor alle voorwerpen in Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschrijving</td> 
      <td>Voeg een beschrijving voor uw prioriteit toe om zijn functie te verklaren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verbergen</td> 
      <td> <p>Selecteer dit vakje als u de prioriteit wilt verbergen.</p><p>Wanneer u de <b> optie van de Verbergen </b> selecteert, toont de prioriteit nergens in Workfront en de gebruikers kunnen niet het voor hun projecten, taken, en kwesties kiezen.</p> 
      <p><b> BELANGRIJK </b>: Wij adviseren dat u de prioriteiten verbergt die u niet meer wilt gebruiken, eerder dan hen te schrappen. Door ze te verbergen, houdt u nog steeds al uw historische gegevens bij, van objecten die met deze prioriteit zijn voltooid, en voorkomt u dat mensen in de toekomst deze prioriteit kiezen. </p>
      <p>U kunt desgewenst de volgorde van uw prioriteiten wijzigen door deze in de gewenste volgorde te slepen. Dit verandert de orde waarin zij voor projecten, taken, en kwesties tonen. Dit verandert niet het <b> Aantal van het Belang </b>. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **sparen**.

Zie de volgende artikelen voor instructies over het toepassen van prioriteiten op projecten, taken en kwesties:

* [ Begrijp en werk projectprioriteiten bij ](../../../manage-work/projects/planning-a-project/project-priority.md)
* [ Prioriteit van de Taak van de Update ](../../../manage-work/tasks/task-information/task-priority.md)
* [Prioriteit van probleem bijwerken](../../../manage-work/issues/issue-information/update-issue-priority.md)
