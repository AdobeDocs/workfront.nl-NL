---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Plannen verwijderen in het deelvenster Scenario
description: U kunt plannen schrappen die u creeerde. U kunt geen plannen schrappen die met u worden gedeeld.
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# Plannen verwijderen in de [!DNL Scenario Planner]

U kunt plannen schrappen die u creeerde. U kunt geen plannen schrappen die met u worden gedeeld.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>Nieuw: Ultimate </p></li>
   <p>De Scenario Planner is niet beschikbaar voor de nieuwe Workfront Select- of Workfront Prime-plannen. </p>
   <li><p>Huidig: [!UICONTROL Business] of hoger</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licentie*</p> </td> 
   <td> <p>Nieuw: Licht of hoger</p> 
   <p>Huidig: [!UICONTROL Review] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>Voor de nieuwe plannen van Workfront:</p><p> Adobe Workfront</li></p>
   <li><p>Voor de huidige plannen van Workfront: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>

<p>Voor meer informatie, zie <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref"> Toegang nodig om [!DNL Scenario Planner]</a> te gebruiken. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Toegangsniveau </td> 
   <td> <p>[!UICONTROL Edit] toegang tot de [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objectmachtigingen </p> </td> 
   <td> <p>[!UICONTROL Manage] machtigingen voor een abonnement</p> <p>Voor informatie bij het vragen van om extra toegang tot een plan, zie <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref"> de toegang van het Verzoek tot een plan in [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang tot de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Abonnementen verwijderen

>[!IMPORTANT]
>
>U kunt verwijderde plannen niet herstellen.

U kunt een plan schrappen of u kunt één scenario in een plan schrappen.

* [ Schrap plannen ](#delete-plans)
* [Scènes verwijderen](#delete-scenarios)

### Abonnementen verwijderen

>[!IMPORTANT]
>
>Overweeg het volgende wanneer het schrappen van plannen:
>
>* Alle informatie met betrekking tot het plan wordt eveneens geschrapt. Hieronder vallen alle scenario&#39;s en initiatieven die verband houden met het plan, met inbegrip van informatie over functies en kosten. Deze informatie kan niet worden hersteld.
>* Als het plan een gepubliceerd scenario bevat, blijven de projecten met betrekking tot de verwijderde initiatieven behouden en blijft het [!DNL Scenario Planner] -gebied in de [!UICONTROL Project Details] -sectie.
>
>  Voor informatie over het publiceren van initiatieven aan projecten, zie [ Update of creeer projecten door initiatieven in  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) te publiceren.

Een abonnement verwijderen:

{{step1-to-scenario-planner}}

Een lijst met plannen wordt weergegeven.

1. Klik op de naam van een abonnement om het te openen.
1. Klik **[!UICONTROL More menu]** ![ Meer menu ](assets/more-menu.png) aan het recht van de plannaam, dan klik **[!UICONTROL Delete]** > **[!UICONTROL Yes, delete it]**.

   Het plan wordt geschrapt en u keert aan de lijst van plannen terug.

### Scènes verwijderen {#delete-scenarios}

>[!IMPORTANT]
>
>Overweeg het volgende wanneer het schrappen van een scenario:
>
>* Als u een scenario verwijdert, worden alle initiatieven en de bijbehorende informatie uit het scenario verwijderd. Als ze naar andere scenario&#39;s worden gekopieerd, blijven de initiatieven op de andere scenario&#39;s.
>* Wanneer het schrappen van een scenario, neemt het verdere scenario het aantal van het geschrapte scenario en de telorde wordt bewaard. Als u bijvoorbeeld Scenario 4 verwijdert, wordt Scenario 5 Scenario 4.
>* Als bepaalde initiatieven over het scenario worden gepubliceerd, blijft het project dat met het initiatief verband houdt, behouden en blijft het gebied Scenario Planner op de gekoppelde projecten
>* Als de gepubliceerde initiatieven op een ander scenario bestaan, blijven zij op dat scenario, met inbegrip van hun verband met het project. Als u deze initiatieven publiceert vanuit de andere scenario&#39;s, worden de gekoppelde projecten bijgewerkt met nieuwe informatie uit die scenario&#39;s.
>
>  Voor informatie over het publiceren van initiatieven aan projecten, zie [ Update of creeer projecten door initiatieven in  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) te publiceren.

Een scenario verwijderen:

1. Ga naar het plan waarvoor u een scenario wilt schrappen.

   Standaard wordt het Eerste scenario weergegeven.

1. Klik op **[!UICONTROL Compare scenarios]**.
1. Van de hoger-juiste hoek van de scenario kaart, klik het **[!UICONTROL More]** menu ![ Meer menu ](assets/more-menu.png), dan klik **[!UICONTROL Delete]**.

   Het scenario wordt verwijderd.

1. Klik op **[!UICONTROL Save plan]** om de wijzigingen op te slaan.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete initiatives</h2>
<p>(NOTE: moved this section to its own article about deleting initiatives) </p> <note type="important">
<p>Consider the following when deleting initiatives:</p>
<ul>
<li>Deleting an initiative deletes the job roles and cost information from the initiative.</li>
<li><span>When you delete an initiative that is published to a project, the initiative is removed from the scenario but the Scenario Planner area remains in the Project Details section.</span> </li>
<li> <p>If the initiative you delete is the only published initiative on the scenario, the indicator that the plan has been published is also removed. </p> <p>For information about publishing initiatives to projects, see <a href="../scenario-planner/publish-scenarios-update-projects.md" class="MCXref xref">Update or create projects by publishing initiatives in the Scenario Planner</a>.</p> </li>
</ul>
</note>
<p>To delete an initiative:</p>
<ol>
<li value="1"> <p> <p>Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png">, then click Scenarios.</p> </p> <p>A list of plans displays. </p> </li>
<li value="2">Click the name of a plan to open it, then locate the initiative you want to delete.</li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/more-menu.png"> to the right of the initiative name, then click <strong>Delete</strong> > <strong>Yes, delete it</strong>. </p> <p>The initiative is deleted. </p> </li>
<li value="4">Click <strong>Save Plan</strong> to save your changes. </li>
</ol>
</div>
-->


