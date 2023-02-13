---
product-previous: workfront-goals
navigation-topic: goal-management
title: Doelen sluiten en opnieuw openen in Adobe Workfront-doelen
description: U kunt een doel sluiten wanneer u wilt aangeven dat u het hebt voltooid of dat u er niet meer aan werkt omdat het verouderd is.
author: Alina
feature: Workfront Goals
exl-id: bbb549c1-aea6-4f5e-8a6b-01fc04cf06ef
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Doelen sluiten en opnieuw openen in Adobe Workfront-doelen

U kunt een doel sluiten wanneer u het volgende wilt aangeven:

* Het doel wordt bereikt, omdat u het hebt bereikt of omdat de periode is verstreken.
* U werkt er niet meer aan en u bent ook niet van plan dit in de nabije toekomst te doen.

U kunt doelstellingen opnieuw openen die zijn gesloten wanneer zij opnieuw relevant worden.

## Toegangsvereisten

<!--drafted for P&P release: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>

-->

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Pro of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Aanvraag of hoger</p> <p>Zie voor meer informatie <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Overzicht van Adobe Workfront-licenties</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>U moet een extra licentie voor de Adobe Workfront Goals aanschaffen om toegang te krijgen tot de functionaliteit die in dit artikel wordt beschreven. </p> <p>Zie voor meer informatie <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Vereisten voor het gebruik van Workfront-doelen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot doelen of hoger bewerken</p> <p><b>OPMERKING</b><p>Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Toegang tot Adobe Workfront-doelen verlenen</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> 
    <div> 
     <p>Rechten voor het doel beheren</p> 
     <p>Voor informatie over het delen van doelstellingen, zie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Een doel delen in Workfront-doelen</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

U moet het volgende hebben voordat u kunt beginnen:

* Een lay-outsjabloon die het gebied Doelen in het hoofdmenu bevat.

## Overwegingen bij het sluiten of opnieuw openen van doelen

* U moet toegang tot Edit Doelstellingen in uw toegangsniveau hebben alvorens u doelstellingen kunt sluiten en heropenen. Voor informatie over het verlenen van toegang tot Doelen, zie [Toegang tot Adobe Workfront-doelen verlenen](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).
* U kunt alleen actieve doelen sluiten. U kunt geen doelstellingen sluiten die in het statuut van Ontwerp zijn.

   Voor informatie over doelstatussen raadpleegt u [Overzicht van de status van objecten in Adobe Workfront Goals](../../workfront-goals/goal-management/goal-status-overview.md).

* Het sluiten van doelstellingen sluit in zijn vooruitgang en staat u toe om te schatten hoe goed u in het verwezenlijken van het deed.

   >[!CAUTION]
   >
   >Wanneer het sluiten van een doel dat actieve bijdragende doelstellingen heeft, verandert zijn vooruitgang na het sluiten om de vooruitgang van de bijdragende actieve doelstellingen te wijzen. Voor informatie over het richten van doelstellingen, zie [Richt doelstellingen door hen in de Doelen van Adobe Workfront te verbinden](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

* Werk de voortgangsindicatoren van het doel bij voordat u het doel sluit om ervoor te zorgen dat het doel wordt gesloten met een nauwkeurige voortgangswaarde. Als alle voortgangsindicatoren zijn bereikt, moet het streefpercentage voltooid 100% zijn en is uw doel bereikt. Voor informatie over het bijwerken van uw doelstellingen, zie [Voortgang van Adobe Workfront-doelen bijwerken](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).
* Laat eventuele laatste opmerkingen staan als een update van de doelen die u sluit. Voor informatie over het toevoegen van commentaren aan doelstellingen, zie [Doelopmerkingen beheren in Adobe Workfront-doelen](../../workfront-goals/goal-management/manage-goal-comments.md).
* U kunt de voortgang van resultaten en activiteiten niet meer bijwerken voor een doel dat u sluit.
* U kunt een gesloten doel opnieuw openen als u aan het wilt blijven werken.
* Als het doel niet is bereikt, kunt u overwegen de meeste informatie naar de volgende periode (kwartaal of jaar) te kopiëren. Dit is een grote optie voor doelstellingen die van één tijdspanne aan volgende of doelstellingen hetzelfde zijn die u misschien nog moet proberen te bereiken in het volgende tijdsbestek. Voor informatie over het kopiëren van doelstellingen, zie [Doelstellingen kopiëren in Adobe Workfront-doelen](../../workfront-goals/goal-management/copy-goals.md). U kunt ook de tijdsperiode voor het doel bijwerken in plaats van deze naar een andere periode te kopiëren.
* Workfront verwijdert de opmerkingen van een gesloten doel wanneer u het opnieuw opent. Als u de commentaren moet houden, adviseren wij kopiëren het gesloten doel met inbegrip van om het even welke resultaten verbonden aan het, eerder dan het heropenen van het.


## Doelstellingen sluiten

<!--
Closing goals differs depending on what environment you use. 

### Close goals in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are active.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md). 

1. Click an active goal.

   The Goal Details panel displays on the right. 

1. (Optional and recommended) Click the **Updates** tab and add an update in the **Comment here** field about the reason you are closing the goal, then click **Post**. 

1. Click the **More icon** ![](assets/more-icon.png) to the right of the goal name, then click **Close** > **Close Goal**.

   This closes the goal and saves the current progress on the goal and its results and activities.

   >[!IMPORTANT]
   >
   >If the goal has contributing goals that are still active, the progress of the goal continues to update based on the progress of the aligned goals.
   >
   >
   >![](assets/closing-goals-with-active-aligned-goals-warning-350x71.png)   >
   >

1. (Optional) Modify your filters again to display only closed goals. The goals you closed display on the screen.
-->

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) > **Doelen** in de rechterbovenhoek.

   De lijst met doelstellingen wordt geopend.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Optioneel) Wijzig de filters om alleen actieve doelen weer te geven.

   Voor informatie over het filtreren van informatie in de Doelen van Workfront, zie [Gegevens filteren in Adobe Workfront Goals](../goal-management/filter-information-wf-goals.md).
1. Klik op een actief doel.

   De doelpagina wordt geopend.

   ![](assets/goal-page-unshimmed.png)
1. Klik op de knop **Meer** menu ![](assets/more-icon.png) rechts van de doelnaam klikt u op **Sluiten**.

   Het doel wordt gesloten en u ontvangt een bevestiging in de hoger-juiste hoek van het scherm.

   ![](assets/goal-close-confirmation-with-add-closing-notes-link.png)

1. (Optioneel) Klik in het bevestigingsvak op **Afsluitende notities toevoegen** om opmerkingen toe te voegen over dit doel en waarom u het moet sluiten.
1. Voeg afsluitende notities toe en klik vervolgens op **Notities toevoegen**.

   ![](assets/add-closing-notes-box-unshimmed.png)

   De commentaren tonen in de sectie van de Details van het Doel van de pagina, in het Sluiten nota&#39;s gebied.

   >[!NOTE]
   >
   >Workfront verwijdert de afsluitende notities als u later een gesloten doel opnieuw opent.


## Doelstellingen opnieuw openen

U kunt gesloten doelstellingen opnieuw openen als u besluit dat zij opnieuw relevant zijn geworden en dat u hun vooruitgang moet blijven bijwerken.

<!--
Reopening goals differs depending on what environment you use.

### Reopen goals in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are closed.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).


1. Click a closed goal.

   This opens the Goal Details panel on the right. 

1. Click the **More icon** ![](assets/more-icon.png) to the right of the goal name, then click **Reopen** > **Reopen**.

   This reopens the goal and places it in a status of Active. The progress of the goal is recalculated starting with the current date. 

1. (Optional) Modify your filters again to display only active goals. The goals you opened display on the screen.

-->

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png)> **Doelen** in de rechterbovenhoek.

   De lijst met doelstellingen wordt geopend.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Optioneel) Wijzig de filters om alleen doelen weer te geven die zijn gesloten.

   Voor informatie over het filtreren van informatie in de Doelen van Workfront, zie [Gegevens filteren in Adobe Workfront Goals](../goal-management/filter-information-wf-goals.md).
1. Klik op de naam van een gesloten doel.

   De doelpagina wordt geopend.
1. Klik op de knop **Meer** menu ![](assets/more-icon.png) rechts van de doelnaam, en **Opnieuw openen** > **Opnieuw openen**.

   De volgende dingen doen zich voor:
   * Het doel is nu open en het heeft een status van Actief.
   * De voortgang van het doel wordt opnieuw berekend vanaf de huidige datum.
   * Alle afsluitende notities worden verwijderd van de pagina met algemene details. Verwijderde afsluitende notities kunnen niet worden hersteld.

1. (Optioneel) Wijzig de filters opnieuw om alleen actieve doelen weer te geven.

   De doelen die u hebt geopend, worden weergegeven op het scherm.

