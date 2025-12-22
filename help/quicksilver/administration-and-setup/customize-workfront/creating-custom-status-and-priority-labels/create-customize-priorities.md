---
title: Prioriteiten maken en aanpassen
description: U kunt de prioriteiten voor projecten, taken, en kwesties in het gebied van de Opstelling van Workfront controleren. Prioriteiten geven belang aan uw projecten, taken of problemen in Adobe Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# Prioriteiten maken en aanpassen

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

U kunt de prioriteiten voor projecten, taken, en kwesties in het gebied van de Opstelling van Workfront controleren. Prioriteiten geven belang aan uw projecten, taken of problemen in Adobe Workfront.

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

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bestaande prioriteiten aanpassen

Als beheerder van Workfront, kunt u de volgende wijzigingen in de standaardprioriteiten aanbrengen die in Workfront worden verstrekt:

* Wijzig de naam van prioriteiten.
* Herstel de prioriteiten.

  Voor meer informatie over hoe te om prioriteiten te herschikken, zie [&#x200B; een prioriteit voor een project, een taak, of een kwestie &#x200B;](#create-a-priority-for-a-project-task-or-issue) creëren.

* Wijzig de standaardprioriteit.

  Voor meer informatie over de functionaliteit om de standaardprioriteit te veranderen, zie [&#x200B; een prioriteit voor een project, een taak, of een kwestie &#x200B;](#create-a-priority-for-a-project-task-or-issue) creëren.

* Bewerk de beschrijving van de prioriteiten.
* Stel een kleur in voor elke prioriteit.

  De kleur van de prioriteit wordt gebruikt in grafiekrapporten, wanneer u uw resultaten door **Prioriteit** groepeert.

  Voor meer informatie over grafiekrapporten, zie [&#x200B; een grafiek aan een rapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md) toevoegen.

* Prioriteiten verwijderen.

  Wanneer u een bestaande prioriteit verwijdert, moet u een vervangende prioriteit selecteren.

* Prioriteiten verbergen.

  Voor meer informatie over de functionaliteit om prioriteiten te verbergen, zie [&#x200B; een prioriteit voor een project, een taak, of een kwestie &#x200B;](#create-a-priority-for-a-project-task-or-issue) creëren.

  >[!NOTE]
  >
  >U moet voor elk object ten minste één prioriteit in uw Workfront-account hebben.

De prioriteiten die standaard worden opgegeven voor elk objecttype (project, taak en uitgave) zijn identiek:

* Geen
* Laag
* Normaal
* Hoog
* Dringend

## Een prioriteit maken voor een project, taak of uitgave {#create-a-priority-for-a-project-task-or-issue}

Naast de standaardprioriteiten in Workfront kunt u ook uw eigen prioriteiten toevoegen om aan de behoeften van uw organisatie te voldoen.

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Voorkeur van het Project** > **Prioriteiten**.

1. Klik het lusje voor het objecten type u een prioriteit voor (**Project**, **Taak**, of **Kwestie**) wilt tot stand brengen.
1. Klik **Nieuwe rij** bij de bodem van de lijst.
1. Configureer de volgende opties voor de prioriteit:

   * **Prioriteitsnaam**: Type een naam voor de prioriteit.
   * **Belangrijk**: Wanneer het toevoegen van een nieuwe prioriteit, wordt een aantal toegewezen aan het door gebrek. Bewerk dit nummer als het niet aan uw wensen voldoet.

     Het belangrijke nummer voor elke prioriteit moet uniek zijn. Het nummer van de prioriteit weerspiegelt het belang van het project, de taak of de kwestie: het hoogste aantal komt overeen met de hoogste prioriteit.

     U kunt dit nummer niet meer bewerken nadat u de prioriteit hebt opgeslagen.

   * **Kleur**: Kies een kleur voor de prioriteit.

     De kleur van de prioriteit wordt gebruikt in grafiekrapporten en de Montages van het Team van de Gelijkheid. Voor informatie over grafiekrapporten, zie [&#x200B; een grafiek aan een rapport &#x200B;](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md) toevoegen. Voor informatie over de Montages van het Team van de Gelijke, zie [&#x200B; een team van de Gelijkheid &#x200B;](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md) creëren.

   * **Standaard Prioriteit**: Selecteer de prioriteit u Workfront automatisch op alle pas gecreëerde projecten, taken, of kwesties wilt toepassen.

     **Normaal** is de standaardprioriteit voor alle voorwerpen in Workfront.

     U kunt een verborgen prioriteit niet als standaard instellen.

     De standaardprioriteit wordt vermeld met een pictogram ![&#x200B; Standaard prioritaire pictogram &#x200B;](assets/default-icon.png). Voer een van de volgende handelingen uit om een nieuwe standaardinstelling te kiezen:

      * Selecteer de controledoos naast de prioritaire naam en selecteer **maak Gebrek** in de actiebar bij de bodem van het scherm.
      * Beweeg over de prioritaire naam en klik **Meer** menu dat verschijnt. Dan, uitgezochte **maak Gebrek**.

        De nieuwe standaardprioriteit wordt geëtiketteerd met het pictogram.

   * **Beschrijving**: Type een beschrijving voor de prioriteit om zijn functie te verklaren.
   * **Keuze van de Huid**: Selecteer **ja** om een prioriteit te verbergen die niet meer nodig is.

     Een verborgen prioriteit wordt nergens in Workfront weergegeven, zodat gebruikers deze niet kunnen kiezen voor hun projecten, taken of problemen.

     >[!IMPORTANT]
     >
     >In plaats van prioriteiten te schrappen die u niet meer wilt gebruiken, stellen wij voor dat u ze verbergt. Op deze manier houdt u al uw historische gegevens bij over objecten die al met de prioriteit zijn voltooid, en voorkomt u dat mensen in de toekomst de prioriteit gebruiken.

1. (Optioneel) Wijzig de volgorde van uw prioriteiten door deze in de gewenste volgorde te slepen.

   Dit verandert de orde waarin zij voor projecten, taken, of kwesties tonen. Het verandert niet het **Aantal van het Belang**.

1. Klik **sparen**.

Zie de volgende artikelen voor instructies over het toepassen van prioriteiten op projecten, taken en kwesties:

* [&#x200B; Begrijp en werk projectprioriteiten bij &#x200B;](../../../manage-work/projects/planning-a-project/project-priority.md)
* [&#x200B; Prioriteit van de Taak van de Update &#x200B;](../../../manage-work/tasks/task-information/task-priority.md)
* [Prioriteit van probleem bijwerken](../../../manage-work/issues/issue-information/update-issue-priority.md)
