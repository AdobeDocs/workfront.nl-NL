---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Overzicht van de geplande afsluitdatum voor projecten, taken en problemen
description: De voorspelde Voltooiingsdatum is een real-time, berekende indicator van wanneer het project, de taak, of de kwestie zullen worden voltooid. Als het project, de taak of de uitgave is gemarkeerd als Voltooid, verandert de Geprojecteerde Voltooiingsdatum in de datum van de Werkelijke Voltooiingsdatum.
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# Overzicht van de geplande afsluitdatum voor projecten, taken en problemen

De voorspelde Voltooiingsdatum is een real-time, berekende indicator van wanneer het project, de taak, of de kwestie zullen worden voltooid. Als het project, de taak of de uitgave is gemarkeerd als Voltooid, verandert de Geprojecteerde Voltooiingsdatum in de datum van de Werkelijke Voltooiingsdatum.

In de volgende secties wordt beschreven hoe de Geprojecteerde Voltooiingsdatum wordt bepaald voor projecten, taken en problemen, en hoe u deze kunt vinden.

## Toegangsvereisten

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   <p>For current licenses: 
   <ul><li><p>Contributor or higher to view the Projected Completion Date in a report</p></li> <li><p>A Standard license to create a report</p></li> </ul>
   
   <p>For legacy licenses: 
   <ul><li><p>Review or higher to view the Projected Completion Date in a report</p></li> 
   <li><p>A Plan license to create a report</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>You must have Edit access to Reports, Dashboards, Calendars to create a report</p> <p>You must have Edit access to Filters, Views, Groupings to create a report or modify a list view</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Reviseren of hoger om de verwachte voltooiingsdatum in een rapport weer te geven</p> <p>Een licentie voor het maken van een rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten weergeven of vergroten</p> <p>U moet Edit toegang tot Rapporten, Dashboards, Kalenders hebben om een rapport tot stand te brengen</p> <p>U moet Edit toegang tot Filters, Weergaven, Groepen hebben om een rapport te cre??ren of een lijstmening te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening of hoger aan een project</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## De manier waarop Adobe Workfront de Geprojecteerde Voltooiingsdatum bepaalt

De voorspelde voltooiingsdatum is een berekend veld en kan niet handmatig worden gewijzigd.

De criteria die worden gebruikt om de Geprojecteerde Datum van Voltooiing te bepalen verschillen, afhankelijk van het voorwerp u bekijkt:

* **Projecten:** De geplande afsluitende datum voor projecten is gelijk aan de geplande afsluitende datum van de laatste projecttaak.
* **Taken:**??De verwachte afsluitende datum voor taken wordt bepaald op basis van de volgende criteria:

   * **Voortgangsgegevens over de taak die door de toegewezen taakontvanger is verricht:**??De updates van de vooruitgang omvatten veranderingen in volledig percentage en veranderingen van taakstatus.
   * **Vastlegdatum:** Als de toegewezen taak een Vastlegdatum opgeeft, wordt de Geprojecteerde Voltooiingsdatum gewijzigd en aangepast aan de Vastlegdatum.

      Raadpleeg het artikel voor meer informatie over Datums vastleggen [Overzicht van datum vastleggen](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **Voorgangers:** Als er geen vertragingen op de voorgangstaken zijn, zou de Verwachte Datum van Voltooiing de Geplande Datum van Voltooiing moeten aanpassen. Als er vertraging optreedt, geven afhankelijke taken een verwachte voltooiingsdatum groter aan dan de geplande voltooiingsdatum.

      Voor meer informatie over de Geplande Datum van Voltooiing van taken, zie [Overzicht van de geplande voltooiing van de taak](../../../manage-work/tasks/task-information/task-planned-completion-date.md).
   >[!IMPORTANT]
   >
   >Wanneer de voorganger van een taak een Werkelijke Datum van de Voltooiing heeft, ontvangen de afhankelijke taken een Geprojecteerde Datum van de Voltooiing zoals die in het volgende scenario wordt beschreven:
   >
   >
   >Als het project Taak A, Taak B, en Taak C heeft, en Taak B de opvolger van Taak A is, is Taak C de opvolger van Taak B en een Ware Voltooiingsdatum wordt toegevoegd aan Taak A, wordt de Geprojecteerde Datum van Voltooiing automatisch opnieuw berekend voor Taak B (op voorwaarde dat **Type update** van het project is ingesteld op Automatisch en Bij wijziging), maar het project wordt niet opnieuw berekend voor taak C. Workfront berekent momenteel de geplande voltooiingsdatum voor taken die ????n niveau hoger of lager zijn dan de bijgewerkte taak, om prestatieredenen.??

* **Problemen:**De naar verwachting afsluitende datum van uitgave is in eerste instantie zo ingesteld dat deze overeenkomt met de geplande afwerkingsdatum.

   Als de uitgiftebestemming een datum opgeeft die moet worden vastgelegd, veranderen zowel de Geprojecteerde Voltooiingsdatum als de Geplande Voltooiingsdatum zodat deze overeenkomt met de Vastleggingsdatum.

   Raadpleeg het artikel voor meer informatie over Datums vastleggen [Overzicht van datum vastleggen](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## De verwachte voltooiingsdatum weergeven

U kunt de Geprojecteerde Datum van Voltooiing van projecten, taken, en kwesties in rapporten bekijken. U kunt de Geprojecteerde Voltooiingsdatum van projecten en taken in andere gebieden van Workfront bekijken.??

* [De verwachte voltooiingsdatum van een project weergeven](#view-the-projected-completion-date-of-a-project)
* [De verwachte voltooiingsdatum van een taak weergeven](#view-the-projected-completion-date-of-a-task)
* [De verwachte voltooiingsdatum van een uitgave weergeven](#view-the-projected-completion-date-of-an-issue)

### De verwachte voltooiingsdatum van een project weergeven {#view-the-projected-completion-date-of-a-project}

1. Ga naar het project waar u de Geprojecteerde Datum van Voltooiing wilt bekijken.
1. Klikken **Projectdetails** in het linkerdeelvenster.
1. Zoek de **Geprojecteerde afsluitdatum** in het **Overzicht** sectie.

### De verwachte voltooiingsdatum van een taak weergeven {#view-the-projected-completion-date-of-a-task}

1. Ga naar de taak waar u de Geprojecteerde Voltooiingsdatum wilt bekijken.
1. Klikken **Taakdetails** in het linkerdeelvenster.
1. Zoek de **Geprojecteerde afsluitdatum** in het **Overzicht** sectie.

### De verwachte voltooiingsdatum van een uitgave weergeven {#view-the-projected-completion-date-of-an-issue}

U kunt de Geprojecteerde Voltooiingsdatum voor kwesties slechts in een uitgiftenrapport of lijstmening bekijken.??Het maken van een lijstmening is gelijkaardig aan het cre??ren van de mening in een rapport.

U kunt als volgt een uitgiftenrapport maken met de geplande afsluitdatum:

1. Een uitgiftenrapport maken, zoals beschreven in het artikel [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Selecteer **Kolommen (weergave)** tab.
1. Klikken **Kolom toevoegen** en begint te typen **Geprojecteerde afsluitdatum** in de **Tonen in deze kolom:** veld.

1. Selecteer deze optie wanneer deze in de lijst wordt weergegeven, onder de optie **Probleem** object.??
1. Klikken **Opslaan + Sluiten**.

   De **Geprojecteerde afsluitdatum**??kolom in het rapport is bevolkt.??

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
