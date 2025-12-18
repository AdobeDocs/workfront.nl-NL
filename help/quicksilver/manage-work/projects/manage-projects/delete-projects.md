---
title: Projecten verwijderen
product-area: projects
navigation-topic: manage-projects
description: U kunt een project schrappen als het project en zijn gegevens niet meer nodig zijn. Als alternatief voor het schrappen van een project, adviseren wij het uitgeven van het project en het veranderen van de status in Voltooid of Dead. Dit verwijdert alle huidige taken met betrekking tot het project van de de taaklijst van een gebruiker, maar bewaart alle gegevens verbonden aan het project.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
recommendations: noDisplay, noCatalog
source-git-commit: ba5089fd02ca099d25ce0d3c2c2c039c2c6e2fe2
workflow-type: tm+mt
source-wordcount: '1067'
ht-degree: 0%

---

# Projecten verwijderen

<!--Audited: 07/2024-->

U kunt een project schrappen als het project en zijn gegevens niet meer nodig zijn.

Als alternatief voor het schrappen van een project, adviseren wij het uitgeven van het project en het veranderen van de status in Voltooid of Dead. Dit verwijdert alle huidige taken met betrekking tot het project van de de taaklijst van een gebruiker, maar bewaart alle gegevens verbonden aan het project.

U kunt een project in een projectlijst of op het projectniveau schrappen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-pakket</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-licentie</p> </td> 
   <td> <p>Standard</p>
   <p>Plan</p> 
   </td> 
  </tr> 
    <td>Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten bewerken met de mogelijkheid projecten te maken en te verwijderen</p> </td> 
  </tr> 
    <td> <p>Objectmachtigingen</p> </td> 
   <td> <p>Bewerk toegang tot projecten, taken, problemen met de mogelijkheid projecten, taken en problemen te verwijderen</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>New license: Standard </p>
   <p>Current license: Plan </p> 
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level configuration</td> 
   <td> <p>Edit access to Projects with ability to Create and Delete projects</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>Edit access to Projects, Tasks, Issues with ability to Delete projects, tasks, and issues</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Begrijp het proces om projecten te schrappen

* [ Beperkingen voor het schrappen van projecten ](#limitations-for-deleting-projects)
* [Het effect van het schrappen van projecten](#the-impact-of-deleting-projects)

### Beperkingen voor het verwijderen van projecten  {#limitations-for-deleting-projects}

* Verwijderde items worden 30 dagen naar de prullenbak verplaatst en kunnen alleen door de Workfront-beheerder worden hersteld.

  Voor meer informatie over het herstellen van voorwerpen, zie het artikel [ schrapte punten ](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md) herstellen.

* Als het project taken of kwesties met geregistreerde uren heeft, moet de Workfront of groepsbeheerder de schrapping van deze taken toestaan door de Voorkeur van de Taak &amp; van de Uitgave in uw instantie van Workfront te vormen zodat u het project kunt schrappen dat de taken bevat.

  Voor meer informatie over het toelaten van de schrapping van taken, kwesties, of projecten waar de uren worden geregistreerd, zie de &quot;Schrapping&quot;sectie in [ de taak van het hele systeem vormen en voorkeur uitgeven ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### Het effect van het schrappen van projecten {#the-impact-of-deleting-projects}

* Wanneer u een project schrapt, beïnvloedt u andere voorwerpen verbonden aan het project.

  De volgende voorwerpen in bijlage aan een project worden ook geschrapt wanneer u een project schrapt:

   * Documenten

     U kunt geen project verwijderen dat een bijgevoegd document heeft dat is uitgecheckt. Voor meer informatie over het controleren van documenten, zie [ Controle uit documenten ](../../../documents/managing-documents/check-out-documents.md).

   * Taken
   * Subtaken
   * Problemen
   * Updates
   * Goedkeuringen
   * Uitgaven
   * Risico&#39;s
   * Basislijnen
   * Informatie over bedrijfscase
   * Gegevens over wachtrij
   * Factureringstarieven
   * Factureringsgegevens

     U kunt geen project schrappen dat de Verslagen van het Factureren met een status van Gevonden heeft. Voor meer informatie, zie [ het factureren verslagen ](../../projects/project-finances/create-billing-records.md) creëren.

* Afhankelijk van hoe uw beheerder van Workfront de Voorkeur van het Project, van de Taak, of van de Schrapping van de Uitgave in de Voorkeur van de Tijdopname &amp; van Uren van uw instantie van Workfront vormt, worden de uren geregistreerd voor de taken, de kwesties, of het project behandeld op één van de volgende manieren wanneer het schrappen van het project:

   * De uren blijven op timesheet als algemene tijd.
   * De uren worden verwijderd en worden hersteld als het project ooit wordt hersteld.

  Voor meer informatie over het vormen van de schrappingsvoorkeur voor uren het programma geopende kwesties, zie [ timesheet en uurvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) vormen.

* Als het project dat u verwijdert is gekoppeld aan een initiatief in het Workfront Scenario-abonnement:

   * Het initiatief blijft op het plan staan, maar het verband met het project wordt weggenomen.
   * Als het project u schrapt met het enige gepubliceerde initiatief van een plan verbonden is, wordt de aanwijzing dat het plan is gepubliceerd ook verwijderd.
   * Als u een geschrapt project terugkrijgt, wordt het project teruggekregen, maar zijn verbinding aan het initiatief wordt niet hersteld en het gebied van de Planner van het Scenario niet meer toont in de Details van het Project.

     Voor de Scenario Planner is een aanvullende licentie vereist. Voor informatie over de Planner van het Scenario van Workfront, zie [ het overzicht van de Planner van het Scenario ](../../../scenario-planner/scenario-planner-overview.md).

     Voor informatie over projecten verbonden aan initiatieven in de Planner van het Scenario, zie [ Update of creeer projecten door initiatieven in de Planner van het Scenario te publiceren ](../../../scenario-planner/publish-scenarios-update-projects.md).

* Als het project ook een activiteit voor een doel in de Doelen van Workfront is:

   * Het project wordt geschrapt van het doel. Ook de vooruitgang die door het project wordt aangegeven met betrekking tot het doel, wordt verwijderd.

   * Als u het geschrapte project terugkrijgt, wordt het project ook hersteld als activiteit van het doel.

     Hiervoor is een aanvullende licentie vereist. Voor informatie over de Doelen van Workfront, zie [ overzicht van de Doelen van Adobe Workfront ](../../../workfront-goals/goal-management/wf-goals-overview.md).

     Voor informatie over het associëren van projecten met doelstellingen, zie [ projecten aan doelstellingen in de Doelen van Adobe Workfront ](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md) toevoegen.

## Een project in een lijst verwijderen

U kunt projecten uit een lijst van projecten schrappen.

1. Ga naar een lijst van projecten of een projectrapport.
1. Selecteer het project of de projecten die u wilt schrappen, dan klik het **pictogram van de Schrapping** pictogram van de Schrapping ![ bij de bovenkant van de lijst.](assets/delete-icon.png)

1. Klik **ja, schrap het** om de schrapping te bevestigen.

   De projecten worden verwijderd en gedurende 30 dagen in de prullenbak opgeslagen. Uw Workfront-beheerder kan tijdens deze periode verwijderde projecten uit de prullenbak herstellen.

## Een project op projectniveau verwijderen

1. Ga naar het project u wilt schrappen.
1. Klik het **Meer** pictogram ![ Meer menu ](assets/qs-more-menu.png) aan het recht van de projectnaam, dan klik **Project van de Schrapping**.

   ![ Meer uitgevouwen menu ](assets/more-icon-expanded-delete-project-highlighted.png)

1. Klik **ja, schrap het**.

   Het project wordt verwijderd en gedurende 30 dagen in de prullenbak opgeslagen. Uw Workfront-beheerder kan het product tijdens deze periode uit de prullenbak herstellen.

## Een project verwijderen uit de pagina met verbonden records van een Workfront-planningsrecord

>[!NOTE]
>
>De informatie in deze sectie verwijst naar Adobe Workfront Planning, een extra mogelijkheid van Adobe Workfront.
>
>Voor een lijst van vereisten om tot de Planning van Workfront toegang te hebben, zie [ het toegangsoverzicht van de Planning van Adobe Workfront ](/help/quicksilver/planning/access/access-overview.md).
> 
>Voor algemene informatie over de Planning van Workfront, zie [ begonnen worden met de Planning van Adobe Workfront ](/help/quicksilver/planning/general/planning-overview.md).

U moet het volgende hebben alvorens u tot projecten van een Planning van Workfront toegang hebt en kunt schrappen verbonden verslagenpagina:

* Planning recordtypen die met Workfront-projecten zijn verbonden. Voor informatie, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).
* Planningsrecords. Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/create-records.md) creëren.
* Een verbonden verslagenpagina die projecten toont die met een verslag van de Planning worden verbonden. Voor informatie, zie [ een Verbonden verslagenpagina aan een verslag ](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md) toevoegen.

Een record verwijderen uit een pagina met verbonden records:

1. Van de verbonden verslagenpagina die projecten toont die met een verslag worden verbonden, houd over de naam van een project en klik **Meer** pictogram ![ Meer pictogram ](assets/more-icon.png)

   of

   Selecteer een of meerdere projecten in de lijst. Let op de blauwe balk onder aan de projectlijst.

1. Klik **Schrapping**, dan **Schrapping** om te bevestigen.

   De projecten worden verwijderd en in de prullenbak van Workfront geplaatst.

## Verwijderde projecten herstellen

Een systeem of groepsbeheerder kan projecten herstellen binnen 30 dagen nadat zij worden geschrapt, zoals die in artikel [ worden beschreven herstelt geschrapte punten ](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
