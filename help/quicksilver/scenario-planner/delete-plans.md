---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Plannen verwijderen in het deelvenster Scenario
description: U kunt plannen schrappen die u creeerde. U kunt geen plannen schrappen die met u worden gedeeld.
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---

# Plannen verwijderen in het dialoogvenster [!DNL Scenario Planner]

U kunt plannen schrappen die u creeerde. U kunt geen plannen schrappen die met u worden gedeeld.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] of hoger</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licentie*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td><b>Product</b> </td> 
   <td> <p>U moet een extra licentie aanschaffen voor de [!DNL Adobe Workfront Scenario Planner] voor toegang tot de functionaliteit die in dit artikel wordt beschreven.</p> <p>Voor informatie over het verkrijgen van de [!DNL Workfront Scenario Planner], zie <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Toegang nodig om de [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraties op toegangsniveau*</strong> </td> 
   <td> <p>[!UICONTROL Edit] toegang tot [!DNL Scenario Planner]</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objectmachtigingen</strong> </p> </td> 
   <td> <p>[!UICONTROL Manage] machtigingen voor een abonnement</p> <p>Voor informatie over het vragen van om extra toegang tot een plan, zie <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Toegang aanvragen tot een abonnement in de [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Abonnementen verwijderen

>[!IMPORTANT]
>
>U kunt verwijderde plannen niet herstellen.

U kunt een plan schrappen of u kunt één scenario in een plan schrappen.

* [Abonnementen verwijderen](#delete-plans)
* [Scènes verwijderen](#delete-scenarios)

### Abonnementen verwijderen

>[!IMPORTANT]
>
>Overweeg het volgende wanneer het schrappen van plannen:
>
>* Alle informatie met betrekking tot het plan wordt eveneens geschrapt. Hieronder vallen alle scenario&#39;s en initiatieven die verband houden met het plan, met inbegrip van informatie over functies en kosten. Deze informatie kan niet worden hersteld.
>* Als het plan een gepubliceerd scenario bevat, blijven de projecten die verband houden met de geschrapte initiatieven behouden en [!DNL Scenario Planner] het gebied blijft in [!UICONTROL Project Details] sectie.
>
>  Voor informatie over het publiceren van initiatieven aan projecten, zie [Werk of creeer projecten bij door initiatieven in te publiceren [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Een abonnement verwijderen:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png)en klik vervolgens op [!UICONTROL Scenarios].

   Een lijst met plannen wordt weergegeven.

1. Klik op de naam van een abonnement om het te openen.
1. Klik op de knop **[!UICONTROL More menu]** ![](assets/more-menu.png) rechts van de naam van het abonnement klikt u op **[!UICONTROL Delete]** > **[!UICONTROL Yes, delete it]**.

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
>  Voor informatie over het publiceren van initiatieven aan projecten, zie [Werk of creeer projecten bij door initiatieven in te publiceren [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Een scenario verwijderen:

1. Ga naar het plan waarvoor u een scenario wilt schrappen.

   Standaard wordt het Eerste scenario weergegeven.

1. Klik op **[!UICONTROL Compare scenarios]**.
1. Klik in de rechterbovenhoek van de scenario-kaart op de knop **[!UICONTROL More]** menu ![](assets/more-menu.png)en klik vervolgens op **[!UICONTROL Delete]**.

   Het scenario wordt verwijderd.

1. Klikken **[!UICONTROL Save plan]** om uw wijzigingen op te slaan.

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


