---
title: Projecten verwijderen
product-area: projects
navigation-topic: manage-projects
description: U kunt een project schrappen als het project en zijn gegevens niet meer nodig zijn. Als alternatief voor het schrappen van een project, adviseren wij het uitgeven van het project en het veranderen van de status in Voltooid of Dead. Dit verwijdert alle huidige taken met betrekking tot het project van de de taaklijst van een gebruiker, maar bewaart alle gegevens verbonden aan het project.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
recommendations: noDisplay, noCatalog
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 0%

---

# Projecten verwijderen

<!--Audited: 07/2024-->

U kunt een project schrappen als het project en zijn gegevens niet meer nodig zijn.

Als alternatief voor het schrappen van een project, adviseren wij het uitgeven van het project en het veranderen van de status in Voltooid of Dead. Dit verwijdert alle huidige taken met betrekking tot het project van de de taaklijst van een gebruiker, maar bewaart alle gegevens verbonden aan het project.

U kunt een project in een projectlijst of op het projectniveau schrappen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-plan</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-licentie*</p> </td> 
   <td> <p>Nieuwe licentie: standaard </p>
   <p>Huidige licentie: abonnement </p> 
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configuratie op toegangsniveau</td> 
   <td> <p>Toegang tot projecten bewerken met de mogelijkheid projecten te maken en te verwijderen</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objectmachtigingen </p> </td> 
   <td> <p>Bewerk toegang tot projecten, taken, problemen met de mogelijkheid projecten, taken en problemen te verwijderen</p> </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Begrijp het proces om projecten te schrappen

* [&#x200B; Beperkingen voor het schrappen van projecten &#x200B;](#limitations-for-deleting-projects)
* [Het effect van het schrappen van projecten](#the-impact-of-deleting-projects)

### Beperkingen voor het verwijderen van projecten  {#limitations-for-deleting-projects}

* Verwijderde items worden 30 dagen naar de prullenbak verplaatst en kunnen alleen door de Workfront-beheerder worden hersteld.

  Voor meer informatie over het herstellen van voorwerpen, zie het artikel [&#x200B; schrapte punten &#x200B;](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md) herstellen.

* Als het project taken of kwesties met geregistreerde uren heeft, moet de Workfront of groepsbeheerder de schrapping van deze taken toestaan door de Voorkeur van de Taak &amp; van de Uitgave in uw instantie van Workfront te vormen zodat u het project kunt schrappen dat de taken bevat.

  Voor meer informatie over het toelaten van de schrapping van taken, kwesties, of projecten waar de uren worden geregistreerd, zie de &quot;Schrapping&quot;sectie in [&#x200B; de taak van het hele systeem vormen en voorkeur uitgeven &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### Het effect van het schrappen van projecten {#the-impact-of-deleting-projects}

* Wanneer u een project schrapt, beïnvloedt u andere voorwerpen verbonden aan het project.

  De volgende voorwerpen in bijlage aan een project worden ook geschrapt wanneer u een project schrapt:

   * Documenten

     U kunt geen project verwijderen dat een bijgevoegd document heeft dat is uitgecheckt. Voor meer informatie over het controleren van documenten, zie [&#x200B; Controle uit documenten &#x200B;](../../../documents/managing-documents/check-out-documents.md).

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

     U kunt geen project schrappen dat de Verslagen van het Factureren met een status van Gevonden heeft. Voor meer informatie, zie [&#x200B; het factureren verslagen &#x200B;](../../projects/project-finances/create-billing-records.md) creëren.

* Afhankelijk van hoe uw beheerder van Workfront de Voorkeur van het Project, van de Taak, of van de Schrapping van de Uitgave in de Voorkeur van de Tijdopname &amp; van Uren van uw instantie van Workfront vormt, worden de uren geregistreerd voor de taken, de kwesties, of het project behandeld op één van de volgende manieren wanneer het schrappen van het project:

   * De uren blijven op timesheet als algemene tijd.
   * De uren worden verwijderd en worden hersteld als het project ooit wordt hersteld.

  Voor meer informatie over het vormen van de schrappingsvoorkeur voor uren het programma geopende kwesties, zie [&#x200B; timesheet en uurvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) vormen.

* Als het project dat u verwijdert is gekoppeld aan een initiatief in het Workfront Scenario-abonnement:

   * Het initiatief blijft op het plan staan, maar het verband met het project wordt weggenomen.
   * Als het project u schrapt met het enige gepubliceerde initiatief van een plan verbonden is, wordt de aanwijzing dat het plan is gepubliceerd ook verwijderd.
   * Als u een geschrapt project terugkrijgt, wordt het project teruggekregen, maar zijn verbinding aan het initiatief wordt niet hersteld en het gebied van de Planner van het Scenario niet meer toont in de Details van het Project.

     Voor de Scenario Planner is een aanvullende licentie vereist. Voor informatie over de Planner van het Scenario van Workfront, zie [&#x200B; het overzicht van de Planner van het Scenario &#x200B;](../../../scenario-planner/scenario-planner-overview.md).

     Voor informatie over projecten verbonden aan initiatieven in de Planner van het Scenario, zie [&#x200B; Update of creeer projecten door initiatieven in de Planner van het Scenario te publiceren &#x200B;](../../../scenario-planner/publish-scenarios-update-projects.md).

* Als het project ook een activiteit voor een doel in de Doelen van Workfront is:

   * Het project wordt geschrapt van het doel. Ook de vooruitgang die door het project wordt aangegeven met betrekking tot het doel, wordt verwijderd.

   * Als u het geschrapte project terugkrijgt, wordt het project ook hersteld als activiteit van het doel.

     Hiervoor is een aanvullende licentie vereist. Voor informatie over de Doelen van Workfront, zie [&#x200B; overzicht van de Doelen van Adobe Workfront &#x200B;](../../../workfront-goals/goal-management/wf-goals-overview.md).

     Voor informatie over het associëren van projecten met doelstellingen, zie [&#x200B; projecten aan doelstellingen in de Doelen van Adobe Workfront &#x200B;](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md) toevoegen.

## Een project in een lijst verwijderen

U kunt projecten uit een lijst van projecten schrappen.

1. Ga naar een lijst van projecten of een projectrapport.
1. Selecteer het project of de projecten die u wilt schrappen, dan klik het **pictogram van de Schrapping ![&#x200B; pictogram van de Schrapping &#x200B;](assets/delete-icon.png) bij de bovenkant van de lijst.**

1. Klik **ja, schrap het** om de schrapping te bevestigen.

   De projecten worden verwijderd en gedurende 30 dagen in de prullenbak opgeslagen. Uw Workfront-beheerder kan tijdens deze periode verwijderde projecten uit de prullenbak herstellen.

## Een project op projectniveau verwijderen

1. Ga naar het project u wilt schrappen.
1. Klik het **Meer** pictogram ![&#x200B; Meer menu &#x200B;](assets/qs-more-menu.png) aan het recht van de projectnaam, dan klik **Project van de Schrapping**.

   ![&#x200B; Meer uitgevouwen menu &#x200B;](assets/more-icon-expanded-delete-project-highlighted.png)

1. Klik **ja, schrap het**.

   Het project wordt verwijderd en gedurende 30 dagen in de prullenbak opgeslagen. Uw Workfront-beheerder kan het product tijdens deze periode uit de prullenbak herstellen.

## Verwijderde projecten herstellen

Een systeem of groepsbeheerder kan projecten herstellen binnen 30 dagen nadat zij worden geschrapt, zoals die in artikel [&#x200B; worden beschreven herstelt geschrapte punten &#x200B;](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
