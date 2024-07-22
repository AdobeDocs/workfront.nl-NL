---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Overzicht van de geplande afsluitdatum voor projecten, taken en problemen
description: De voorspelde Voltooiingsdatum is een real-time, berekende indicator van wanneer het project, de taak, of de kwestie zullen worden voltooid. Als het project, de taak of de uitgave is gemarkeerd als Voltooid, verandert de Geprojecteerde Voltooiingsdatum in de datum van de Werkelijke Voltooiingsdatum.
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# Overzicht van de geplande afsluitdatum voor projecten, taken en problemen

<!-- Audited: 1/2024 -->

De voorspelde Voltooiingsdatum is een real-time, berekende indicator van wanneer het project, de taak, of de kwestie zullen worden voltooid. Als het project, de taak of de uitgave is gemarkeerd als Voltooid, verandert de Geprojecteerde Voltooiingsdatum in de datum van de Werkelijke Voltooiingsdatum.

In de volgende secties wordt beschreven hoe de Geprojecteerde Voltooiingsdatum wordt bepaald voor projecten, taken en problemen, en hoe u deze kunt vinden.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> 
   <p>Nieuw: 
   <ul><li><p>Medewerker of hoger om de voorspelde voltooiingsdatum in een rapport weer te geven</p></li> <li><p>Een standaardlicentie voor het maken van een rapport</p></li> </ul>

<p>Huidige: 
   <ul><li><p>Reviseren of hoger om de verwachte voltooiingsdatum in een rapport weer te geven</p></li> 
   <li><p>Een licentie voor het maken van een rapport</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau</td> 
   <td> <p>Toegang tot projecten weergeven of vergroten</p> <p>U moet Edit toegang tot Rapporten, Dashboards, Kalenders hebben om een rapport tot stand te brengen</p> <p>U moet Edit toegang tot Filters, Weergaven, Groepen hebben om een rapport te creëren of een lijstmening te wijzigen</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening of hoger aan een project</p> </td> 
  </tr> 
 </tbody> 
</table>

*For meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hoe Adobe Workfront de verwachte voltooiingsdatum bepaalt

De verwachte Voltooiingsdatum is een berekend gebied en kan niet manueel worden veranderd.

De criteria die worden gebruikt om de Geprojecteerde Datum van Voltooiing te bepalen verschillen, afhankelijk van het voorwerp u bekijkt:

* **Projecten:** de Geprojecteerde Datum van de Voltooiing voor projecten is met de Geprojecteerde Datum van de Voltooiing van de recentste taak op het project gelijk.

  Als u bijvoorbeeld een hoger percentage hebt bereikt, wordt de voorspelde voltooide datum van de taak dichter bij de huidige dag geplaatst. Als de status van de taak Nieuw is en de geplande voltooiingsdatum dichtbij is of is verstreken, gaat de geplande voltooiingsdatum verder naar de toekomst.

* **Taken:** de Verwachte Datum van de Voltooiing voor taken wordt bepaald gebaseerd op de volgende criteria:

   * **de updates van de Voortgang die op de taak door de taaktoegewezen persoon worden aangebracht:** de updates van de Voortgang omvatten veranderingen in percenten volledig en veranderingen van taakstatus.
   * **VastleggingsDatum:** als de taaktoegewezen persoon een VastleggingsDatum specificeert, verandert de Geprojecteerde Datum van de Voltooiing om de VastleggingsDatum aan te passen.

     Voor meer informatie over Commit Dates, zie het artikel [ overzicht van de Datum van het Vastleggen ](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **predecessors:** als er geen vertragingen op de voorgangerstaken zijn, zou de Geprojecteerde Datum van de Voltooiing de Geplande Datum van de Voltooiing moeten aanpassen. Als er vertragingen optreden, geven afhankelijke taken een verwachte voltooiingsdatum groter weer dan de geplande voltooiingsdatum.

     Voor meer informatie over de Geplande Datum van de Voltooiing van taken, zie [ Overzicht van de taak Geplande Datum van de Voltooiing ](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

  >[!IMPORTANT]
  >
  >Wanneer de voorganger van een taak een Werkelijke Datum van de Voltooiing heeft, ontvangen de afhankelijke taken een Geprojecteerde Datum van de Voltooiing zoals die in het volgende scenario wordt beschreven:
  >
  >
  >Als het project Taak A, Taak B, en Taak C heeft, en Taak B de opvolger van Taak A is, is Taak C de opvolger van Taak B en een Ware Voltooiingsdatum wordt toegevoegd aan Taak A, wordt de Geprojecteerde Datum van de Voltooiing automatisch opnieuw berekend voor Taak B (op voorwaarde dat het **Type van Update** van het project aan Automatisch en op Verandering wordt geplaatst), maar het zal niet opnieuw worden berekend voor Taak C. Workfront berekent momenteel de geplande voltooiingsdatum voor taken die één niveau hoger of lager zijn dan de bijgewerkte taak, om prestatieredenen.

* **Kwesties:** de kwestie Geprojecteerde Datum van de Voltooiing is aanvankelijk geplaatst om de kwestie Geplande Datum van de Voltooiing aan te passen.

  Als de uitgiftebestemming een datum opgeeft die moet worden vastgelegd, veranderen zowel de Geprojecteerde Voltooiingsdatum als de Geplande Voltooiingsdatum zodat deze overeenkomt met de Vastleggingsdatum.

  Voor meer informatie over Commit Dates, zie het artikel [ overzicht van de Datum van het Vastleggen ](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## De verwachte voltooiingsdatum weergeven

U kunt de Geprojecteerde Datum van Voltooiing van projecten, taken, en kwesties in rapporten bekijken. U kunt de Geprojecteerde Voltooiingsdatum van projecten en taken in andere gebieden van Workfront bekijken.

### De verwachte voltooiingsdatum van een project weergeven {#view-the-projected-completion-date-of-a-project}

1. Ga naar het project waar u de Geprojecteerde Datum van Voltooiing wilt bekijken.
1. Klik **Details van het Project** in het linkerpaneel.
1. Bepaal de plaats van het **Geprojecteerde gebied van de Datum van de Voltooiing** op het **Overzicht** > **de data van het Project** sectie.

### De verwachte voltooiingsdatum van een taak weergeven {#view-the-projected-completion-date-of-a-task}

1. Ga naar de taak waar u de Geprojecteerde Voltooiingsdatum wilt bekijken.
1. Klik **Details van de Taak** in het linkerpaneel.
1. Bepaal de plaats van het **Geprojecteerde gebied van de Datum van de Voltooiing** op het **Overzicht** > **de datums van de Taak en beperkingssectie**.

### De verwachte voltooiingsdatum van een uitgave weergeven {#view-the-projected-completion-date-of-an-issue}

U kunt de Geprojecteerde Voltooiingsdatum voor kwesties slechts in een uitgiftenrapport of lijstmening bekijken. Het maken van een lijstmening is gelijkaardig aan het creëren van de mening in een rapport.

U kunt als volgt een uitgiftenrapport maken met de geplande afsluitdatum:

1. Creeer een uitgifterapport, zoals die in artikel [ wordt beschreven een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.
1. Selecteer de **Kolommen (Mening)** tabel.
1. Klik **toevoegen Kolom**, en beginnen **Geprojecteerde Datum van de Voltooiing** in **tonen in deze kolom te typen:** gebied.

1. Selecteer het wanneer het in de lijst, onder het **voorwerp van de Uitgave** verschijnt.
1. Klik **sparen + Sluiten**.

   De **Geprojecteerde kolom van de Datum van de Voltooiing** in het rapport is bevolkt.

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
