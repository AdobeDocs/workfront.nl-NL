---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Overzicht van de geplande afsluitdatum voor projecten, taken en problemen
description: De voorspelde Voltooiingsdatum is een real-time, berekende indicator van wanneer het project, de taak, of de kwestie zullen worden voltooid. Als het project, de taak of de uitgave is gemarkeerd als Voltooid, verandert de Geprojecteerde Voltooiingsdatum in de datum van de Werkelijke Voltooiingsdatum.
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: d71ee30378c39975366f4f257e3f7b17aba0c0ae
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# Overzicht van de geplande afsluitdatum voor projecten, taken en problemen

<!-- Audited: 1/2024 -->

De voorspelde Voltooiingsdatum is een real-time, berekende indicator van wanneer het project, de taak, of de kwestie zullen worden voltooid. Als het project, de taak of de uitgave is gemarkeerd als Voltooid, verandert de Geprojecteerde Voltooiingsdatum in de datum van de Werkelijke Voltooiingsdatum.

In de volgende secties wordt beschreven hoe de Geprojecteerde Voltooiingsdatum wordt bepaald voor projecten, taken en problemen, en hoe u deze kunt vinden.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Nieuw: 
   <ul><li><p>Medewerker of hoger om de voorspelde voltooiingsdatum in een rapport weer te geven</p></li> <li><p>Een standaardlicentie voor het maken van een rapport</p></li> </ul>

<p>Huidige: 
   <ul><li><p>Reviseren of hoger om de verwachte voltooiingsdatum in een rapport weer te geven</p></li> 
   <li><p>Een licentie voor het maken van een rapport</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten weergeven of vergroten</p> <p>U moet Edit toegang tot Rapporten, Dashboards, Kalenders hebben om een rapport tot stand te brengen</p> <p>U moet Edit toegang tot Filters, Weergaven, Groepen hebben om een rapport te creëren of een lijstmening te wijzigen</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening of hoger aan een project</p> </td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Hoe Adobe Workfront de verwachte voltooiingsdatum bepaalt

De verwachte Voltooiingsdatum is een berekend gebied en kan niet manueel worden veranderd.

De criteria die worden gebruikt om de Geprojecteerde Datum van Voltooiing te bepalen verschillen, afhankelijk van het voorwerp u bekijkt:

* **Projecten:** De geplande afsluitende datum voor projecten is gelijk aan de geplande afsluitende datum van de laatste projecttaak.

  Als u bijvoorbeeld een hoger percentage hebt bereikt, wordt de voorspelde voltooide datum van de taak dichter bij de huidige dag geplaatst. Als de status van de taak Nieuw is en de geplande voltooiingsdatum dichtbij is of is verstreken, gaat de geplande voltooiingsdatum verder naar de toekomst.

* **Taken:** De verwachte afsluitende datum voor taken wordt bepaald op basis van de volgende criteria:

   * **Voortgangsgegevens over de taak die door de toegewezen taakontvanger is verricht:** De updates van de vooruitgang omvatten veranderingen in volledig percentage en veranderingen van taakstatus.
   * **Vastlegdatum:** Als de toegewezen taak een Vastlegdatum opgeeft, wordt de Geprojecteerde Voltooiingsdatum gewijzigd en aangepast aan de Vastlegdatum.

     Raadpleeg het artikel voor meer informatie over Datums vastleggen [Overzicht van datum vastleggen](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **Voorgangers:** Als er geen vertragingen op de voorgangstaken zijn, zou de Verwachte Datum van Voltooiing de Geplande Datum van Voltooiing moeten aanpassen. Als er vertragingen optreden, geven afhankelijke taken een verwachte voltooiingsdatum groter weer dan de geplande voltooiingsdatum.

     Voor meer informatie over de Geplande Datum van Voltooiing van taken, zie [Overzicht van de geplande voltooiing van de taak](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

  >[!IMPORTANT]
  >
  >Wanneer de voorganger van een taak een Werkelijke Datum van de Voltooiing heeft, ontvangen de afhankelijke taken een Geprojecteerde Datum van de Voltooiing zoals die in het volgende scenario wordt beschreven:
  >
  >
  >Als het project Taak A, Taak B, en Taak C heeft, en Taak B de opvolger van Taak A is, is Taak C de opvolger van Taak B en een Ware Voltooiingsdatum wordt toegevoegd aan Taak A, wordt de Geprojecteerde Datum van Voltooiing automatisch opnieuw berekend voor Taak B (op voorwaarde dat **Type update** van het project is ingesteld op Automatisch en Bij wijziging), maar het project wordt niet opnieuw berekend voor taak C. Workfront berekent momenteel de geplande voltooiingsdatum voor taken die één niveau hoger of lager zijn dan de bijgewerkte taak, om prestatieredenen. 

* **Problemen:** De naar verwachting aangebrachte afsluitdatum van de uitgave komt in eerste instantie overeen met de geplande afwerkingsdatum van de uitgave.

  Als de uitgiftebestemming een datum opgeeft die moet worden vastgelegd, veranderen zowel de Geprojecteerde Voltooiingsdatum als de Geplande Voltooiingsdatum zodat deze overeenkomt met de Vastleggingsdatum.

  Raadpleeg het artikel voor meer informatie over Datums vastleggen [Overzicht van datum vastleggen](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## De verwachte voltooiingsdatum weergeven

U kunt de Geprojecteerde Datum van Voltooiing van projecten, taken, en kwesties in rapporten bekijken. U kunt de Geprojecteerde Voltooiingsdatum van projecten en taken in andere gebieden van Workfront bekijken.

### De verwachte voltooiingsdatum van een project weergeven {#view-the-projected-completion-date-of-a-project}

1. Ga naar het project waar u de Geprojecteerde Datum van Voltooiing wilt bekijken.
1. Klikken **Projectdetails** in het linkerdeelvenster.
1. Zoek de **Geprojecteerde afsluitdatum** in het veld **Overzicht** > **Projectdatums** sectie.

### De verwachte voltooiingsdatum van een taak weergeven {#view-the-projected-completion-date-of-a-task}

1. Ga naar de taak waar u de Geprojecteerde Voltooiingsdatum wilt bekijken.
1. Klikken **Taakdetails** in het linkerdeelvenster.
1. Zoek de **Geprojecteerde afsluitdatum** in het veld **Overzicht** > **Taken en beperkingen** sectie.

### De verwachte voltooiingsdatum van een uitgave weergeven {#view-the-projected-completion-date-of-an-issue}

U kunt de Geprojecteerde Voltooiingsdatum voor kwesties slechts in een uitgiftenrapport of lijstmening bekijken. Het maken van een lijstmening is gelijkaardig aan het creëren van de mening in een rapport.

U kunt als volgt een uitgiftenrapport maken met de geplande afsluitdatum:

1. Een uitgiftenrapport maken, zoals wordt beschreven in het artikel [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Selecteer de **Kolommen (weergave)** tab.
1. Klikken **Kolom toevoegen** en begint te typen **Geprojecteerde afsluitdatum** in de **Tonen in deze kolom:** veld.

1. Selecteer deze optie wanneer deze wordt weergegeven in de lijst onder de optie **Probleem** object. 
1. Klikken **Opslaan + Sluiten**.

   De **Geprojecteerde afsluitdatum** kolom in het rapport is bevolkt. 

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
