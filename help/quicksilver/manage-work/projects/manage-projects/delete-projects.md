---
title: Projecten verwijderen
product-area: projects
navigation-topic: manage-projects
description: U kunt een project schrappen als het project en zijn gegevens niet meer nodig zijn.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Projecten verwijderen

U kunt een project schrappen als het project en zijn gegevens niet meer nodig zijn.

Als alternatief voor het schrappen van een project, adviseren wij het uitgeven van het project en het veranderen van de status in Voltooid of Dead. Dit verwijdert alle huidige taken met betrekking tot het project van de de taaklijst van een gebruiker, maar bewaart alle gegevens verbonden aan het project.

## Toegangsvereisten

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Delete</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>Edit access to Projects, Tasks,&nbsp;Issues with ability to Delete projects, tasks, and issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Bewerk toegang tot projecten, taken, problemen met de mogelijkheid projecten, taken en problemen te verwijderen</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>U kunt machtigingen voor het project, taken en problemen in het project beheren met de mogelijkheid het project, de taken en problemen te verwijderen. </p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.
U kunt een project in een projectlijst of op het projectniveau schrappen.

## Begrijp het proces om projecten te schrappen

* [Beperkingen voor het verwijderen van projecten](#limitations-for-deleting-projects)
* [Het effect van het schrappen van projecten](#the-impact-of-deleting-projects)

### Beperkingen voor het verwijderen van projecten  {#limitations-for-deleting-projects}

* Verwijderde items worden 30 dagen naar de prullenbak verplaatst en kunnen alleen door de Workfront-beheerder worden hersteld.

   Zie het artikel voor meer informatie over het herstellen van objecten [Verwijderde items herstellen](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Als het project taken of kwesties met geregistreerde uren heeft, moet de Workfront of groepsbeheerder de schrapping van deze taken toestaan door de Voorkeur van de Taak &amp; van de Uitgave in uw instantie van Workfront te vormen zodat u het project kunt schrappen dat de taken bevat.

   Voor meer informatie over het toelaten van de schrapping van taken, kwesties, of projecten waar de uren worden geregistreerd, zie de &quot;Schrapping&quot;sectie in [Taak- en probleemvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### Het effect van het schrappen van projecten {#the-impact-of-deleting-projects}

* Wanneer u een project schrapt, beïnvloedt u andere voorwerpen verbonden aan het project.

   De volgende voorwerpen in bijlage aan een project worden ook geschrapt wanneer u een project schrapt:

   * Documenten

      U kunt geen project verwijderen dat een bijgevoegd document heeft dat is uitgecheckt. Zie voor meer informatie over het uitchecken van documenten [Documenten uitchecken](../../../documents/managing-documents/check-out-documents.md).

   * Taken
   * Subtaken
   * Problemen
   * Notities
   * Goedkeuringen
   * Uitgaven

* Afhankelijk van hoe uw beheerder van Workfront het Project, de Taak, of de Voorkeur van de Schrapping van de Uitgave in de Voorkeur van de Tijdopname &amp; van het Uur van uw instantie van Workfront vormt, worden de uren geregistreerd voor de taken, de kwesties, of het project behandeld op één van de volgende manieren wanneer het schrappen van het project:

   * De uren blijven op timesheet als algemene tijd.
   * De uren worden verwijderd en worden hersteld als het project ooit wordt hersteld.

   Voor meer informatie over het vormen van de schrappingsvoorkeur voor uren het programma geopende kwesties, zie [Voorkeuren voor tijdpagina&#39;s en uren configureren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Als het project dat u verwijdert is gekoppeld aan een initiatief in het Workfront Scenario-abonnement:

   * Het initiatief blijft op het plan staan, maar het verband met het project wordt weggenomen.
   * Als het project u schrapt met het enige gepubliceerde initiatief van een plan verbonden is, wordt de aanwijzing dat het plan is gepubliceerd ook verwijderd.
   * Als u een geschrapt project terugkrijgt, wordt het project teruggekregen, maar zijn verbinding aan het initiatief wordt niet hersteld en het gebied van de Planner van het Scenario niet meer toont in de Details van het Project.

      De Scenario Planner is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring en vereist een aanvullende licentie. Voor informatie over de Workfront Scenario Planner raadpleegt u [Overzicht van de functie Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

      Voor informatie over projecten die verband houden met initiatieven in het Scenario Planner, zie [Werk of creeer projecten bij door initiatieven in de Planner van het Scenario te publiceren](../../../scenario-planner/publish-scenarios-update-projects.md).

* Als het project ook een activiteit voor een doel in de Doelen van Workfront is:

   * Het project wordt geschrapt van het doel. Ook de vooruitgang die door het project wordt aangegeven met betrekking tot het doel, wordt verwijderd.

   * Als u het geschrapte project terugkrijgt, wordt het project ook hersteld als activiteit van het doel.

      Hiervoor is een aanvullende licentie vereist. Voor informatie over Workfront Goals raadpleegt u [Overzicht van Adobe Workfront-doelen](../../../workfront-goals/goal-management/wf-goals-overview.md).

      Voor informatie over het associëren van projecten met doelstellingen, zie [Projecten toevoegen aan doelen in Adobe Workfront](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## Een project in een lijst verwijderen

U kunt projecten uit een lijst van projecten schrappen.

1. Ga naar een lijst van projecten of een projectrapport.
1. Selecteer het project u wilt schrappen, dan klik **Verwijderen** boven aan de lijst.

1. Klikken **Ja, verwijderen** om de schrapping te bevestigen.

   Het project wordt verwijderd en gedurende 30 dagen in de prullenbak opgeslagen. Uw Workfront-beheerder kan het product tijdens deze periode uit de prullenbak herstellen.

## Een project op projectniveau verwijderen

1. Ga naar het project u wilt schrappen.
1. Klik op de knop **Meer** pictogram ![](assets/qs-more-menu.png).

1. Klikken **Project verwijderen**.

1. Klikken **Ja, verwijderen**.

   Het project wordt verwijderd en gedurende 30 dagen in de prullenbak opgeslagen. Uw Workfront-beheerder kan het product tijdens deze periode uit de prullenbak herstellen.

## Verwijderde projecten herstellen

Een systeem- of groepsbeheerder kan projecten herstellen binnen 30 dagen nadat ze zijn verwijderd, zoals beschreven in het artikel [Verwijderde items herstellen](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
