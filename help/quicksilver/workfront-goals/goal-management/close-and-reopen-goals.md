---
product-previous: workfront-goals
navigation-topic: goal-management
title: Doelen sluiten en opnieuw openen in Adobe Workfront-doelen
description: U kunt een doel sluiten wanneer u wilt aangeven dat u het hebt voltooid of dat u er niet meer aan werkt omdat het verouderd is.
author: Alina
feature: Workfront Goals
exl-id: bbb549c1-aea6-4f5e-8a6b-01fc04cf06ef
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Doelen sluiten en opnieuw openen in Adobe Workfront-doelen

<!--Audited for P&P only: 4/2025-->

U kunt een doel sluiten wanneer u het volgende wilt aangeven:

* Het doel wordt bereikt, omdat u het hebt bereikt of omdat de periode is verstreken.
* U werkt er niet meer aan en u bent ook niet van plan dit in de nabije toekomst te doen.

U kunt doelstellingen opnieuw openen die zijn gesloten wanneer zij opnieuw relevant worden.

## Toegangsvereisten

>[!NOTE]
>
>Uw bedrijf zou kunnen verkiezen om de Doelen van Adobe Workfront verder te gebruiken als zij dit pakket in het verleden kochten. U moet voor meer informatie contact opnemen met uw accountvertegenwoordiger.
>
>Adobe Workfront Goals kan niet meer worden aangeschaft.

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Adobe Workfront-pakket</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr> 
 <tr>
 <tr>
 <td role="rowheader">Adobe Workfront-licentie</td>
 <td>
 <p>Medewerker of hoger</p>
 <p>Aanvraag of hoger</p></td>
 </tr>
 <td role="rowheader">Configuratie op toegangsniveau</td>
 <td> <p>Toegang tot doelen bewerken</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Objectmachtigingen</td>
 <td>
  <div>
  <p>De toestemmingen van de mening of hoger aan het doel om het te bekijken</p>
  <p>Machtigingen beheren om het te bewerken</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Systeembeheerders, moet een lay-outsjabloon worden toegewezen die het gebied Doelen in het hoofdmenu bevat. </p>  
</td>
  </tr>
</tbody>
</table>

Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
  <p> New product requirement: Workfront</p>
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
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
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Overwegingen bij het sluiten of opnieuw openen van doelen

* U moet toegang tot Edit Doelstellingen in uw toegangsniveau hebben alvorens u doelstellingen kunt sluiten en heropenen. Voor informatie over het verlenen van toegang tot Doelen, zie [ Toegang verlenen tot de Doelen van Adobe Workfront ](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).
* U kunt alleen actieve doelen sluiten. U kunt geen doelstellingen sluiten die in het statuut van Ontwerp zijn.

  Voor informatie over doelstatussen, zie [ overzicht van de Goal status in de Doelen van Adobe Workfront ](../../workfront-goals/goal-management/goal-status-overview.md).

* Het sluiten van doelstellingen sluit in zijn vooruitgang en staat u toe om te schatten hoe goed u in het verwezenlijken van het deed.

  >[!CAUTION]
  >
  >Wanneer het sluiten van een doel dat actieve bijdragende doelstellingen heeft, verandert zijn vooruitgang na het sluiten om de vooruitgang van de bijdragende actieve doelstellingen te wijzen. Voor informatie over het richten van doelstellingen, zie [ doelstellingen door hen in de Doelen van Adobe Workfront ](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md) te verbinden.

* Werk de voortgangsindicatoren van het doel bij voordat u het doel sluit om ervoor te zorgen dat het doel wordt gesloten met een nauwkeurige voortgangswaarde. Als alle voortgangsindicatoren zijn bereikt, moet het streefpercentage voltooid 100% zijn en is uw doel bereikt. Voor informatie over het bijwerken van uw doelstellingen, zie [ het doel van de Update vooruitgang in de Doelen van Adobe Workfront ](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).
* Laat eventuele laatste opmerkingen staan als een update van de doelen die u sluit. Voor informatie over het toevoegen van commentaren aan doelstellingen, zie [ doelcommentaren in de Doelen van Adobe Workfront beheren ](../../workfront-goals/goal-management/manage-goal-comments.md).
* U kunt de voortgang van resultaten en activiteiten niet meer bijwerken voor een doel dat u sluit.
* U kunt een gesloten doel opnieuw openen als u aan het wilt blijven werken.
* Als het doel niet is bereikt, kunt u overwegen de meeste informatie naar de volgende periode (kwartaal of jaar) te kopiëren. Dit is een grote optie voor doelstellingen die van één tijdspanne aan volgende of doelstellingen hetzelfde zijn die u misschien nog moet proberen te bereiken in het volgende tijdsbestek. Voor informatie over het kopiëren van doelstellingen, zie [ doelstellingen van het Exemplaar in de Doelen van Adobe Workfront ](../../workfront-goals/goal-management/copy-goals.md). U kunt ook de tijdsperiode voor het doel bijwerken in plaats van deze naar een andere periode te kopiëren.
* Workfront verwijdert de opmerkingen van een gesloten doel wanneer u het opnieuw opent. Als u de commentaren moet houden, adviseren wij kopiëren het gesloten doel met inbegrip van om het even welke resultaten verbonden aan het, eerder dan het heropenen van het.


## Sluiten, doelen

<!--
Closing goals differs depending on what environment you use. 

### Close goals in the Production environment

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are active.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md). 

1. Click an active goal.

   The Goal Details panel displays on the right. 

1. (Optional and recommended) Click the **Updates** tab and add an update in the **Comment here** field about the reason you are closing the goal, then click **Post**. 

1. Click the **More icon** ![More icon](assets/more-icon.png) to the right of the goal name, then click **Close** > **Close Goal**.

   This closes the goal and saves the current progress on the goal and its results and activities.

   >[!IMPORTANT]
   >
   >If the goal has contributing goals that are still active, the progress of the goal continues to update based on the progress of the aligned goals.
   >
   >
   >![Closing goals with active aligned goals](assets/closing-goals-with-active-aligned-goals-warning-350x71.png)   >
   >

1. (Optional) Modify your filters again to display only closed goals. The goals you closed display on the screen.
-->

{{step1-to-goals}}

De lijst met doelstellingen wordt geopend.

1. (Optioneel) Wijzig de filters om alleen actieve doelen weer te geven.

   Voor informatie over het filtreren van informatie in de Doelen van Workfront, zie [ informatie van de Filter in de Doelen van Adobe Workfront ](../goal-management/filter-information-wf-goals.md).
1. Klik op een actief doel.

   De doelpagina wordt geopend.

   ![ Goal pagina ](assets/goal-page-unshimmed.png)
1. Klik het **Meer** menu ![ Meer pictogram ](assets/more-icon.png) aan het recht van de doelnaam, dan klik **dicht**.

   Het doel wordt gesloten en u ontvangt een bevestiging in de hoger-juiste hoek van het scherm.

   ![ de dichte bevestiging van het Doel ](assets/goal-close-confirmation-with-add-closing-notes-link.png)

1. (Facultatief) in de bevestigingsdoos, klik **toevoegen sluitende nota&#39;s** om commentaren over dit doel toe te voegen en waarom u het moet sluiten.
1. Voeg sluitende nota&#39;s toe, dan klik **nota&#39;s** toevoegen.

   ![ voeg sluitende nota&#39;s doos ](assets/add-closing-notes-box-unshimmed.png) toe

   De commentaren tonen in de sectie van de Details van het Doel van de pagina, in het Sluiten nota&#39;s gebied.

   >[!NOTE]
   >
   >Workfront verwijdert de afsluitende notities als u later een gesloten doel opnieuw opent.


## Doelstellingen opnieuw openen

U kunt gesloten doelstellingen opnieuw openen als u besluit dat zij opnieuw relevant zijn geworden en dat u hun vooruitgang moet blijven bijwerken.

<!--
Reopening goals differs depending on what environment you use.

### Reopen goals in the Production environment

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are closed.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).


1. Click a closed goal.

   This opens the Goal Details panel on the right. 

1. Click the **More icon** ![More icon](assets/more-icon.png) to the right of the goal name, then click **Reopen** > **Reopen**.

   This reopens the goal and places it in a status of Active. The progress of the goal is recalculated starting with the current date. 

1. (Optional) Modify your filters again to display only active goals. The goals you opened display on the screen.

-->

{{step1-to-goals}}

De lijst met doelstellingen wordt geopend.

1. (Optioneel) Wijzig de filters om alleen doelen weer te geven die zijn gesloten.

   Voor informatie over het filtreren van informatie in de Doelen van Workfront, zie [ informatie van de Filter in de Doelen van Adobe Workfront ](../goal-management/filter-information-wf-goals.md).
1. Klik op de naam van een gesloten doel.

   De doelpagina wordt geopend.
1. Klik het **Meer** menu ![ Meer pictogram ](assets/more-icon.png) aan het recht van de doelnaam, dan **heropen** > **opnieuw open**.

   De volgende dingen doen zich voor:
   * Het doel is nu open en het heeft een status van Actief.
   * De voortgang van het doel wordt opnieuw berekend vanaf de huidige datum.
   * Alle afsluitende notities worden verwijderd van de pagina met algemene details. Verwijderde afsluitende notities kunnen niet worden hersteld.

1. (Optioneel) Wijzig de filters opnieuw om alleen actieve doelen weer te geven.

   De doelen die u hebt geopend, worden weergegeven op het scherm.

