---
product-previous: workfront-goals
navigation-topic: goal-management
title: Doelen kopiëren in Adobe Workfront-doelen
description: U kunt doelstellingen in de Doelen van Adobe Workfront kopiëren om een doel tot stand te brengen. Enkele originele doelinformatie brengt naar het nieuwe doel over.
author: Alina
feature: Workfront Goals
exl-id: 690a6030-ee29-4e50-869f-cd014050b364
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '788'
ht-degree: 0%

---

# Doelstellingen kopiëren in Adobe Workfront-doelen

<!--Audited for P&P only: 4/2025-->

U kunt doelstellingen in de Doelen van Adobe Workfront kopiëren om een doel tot stand te brengen. Enkele originele doelinformatie brengt naar het nieuwe doel over.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> 
   <p>Voor het nieuwe plan en de nieuwe licentiestructuur:
  <ul><li>Een Ultimate-abonnement </li></ul>
   </p>
<p>Voor het huidige plan en de licentiestructuur: 
<ul><li> Een Pro of hoger </li>
  <li>Een Adobe Workfront Goals-licentie in aanvulling op een Workfront-licentie.</li></ul></p>
   </td>  
  </tr>
 <tr>
 <tr>
 <td role="rowheader">Adobe Workfront-licentie*</td>
 <td>
 <p>Nieuwe licentie: Medewerker of hoger</p>
 of
 <p>Huidige licentie: aanvragen of hoger</p> <p>Voor meer informatie, zie <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref"> het vergunningsoverzicht van Adobe Workfront </a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
  <p> Nieuwe productvereisten: Workfront</p>
 <p>of</p>
  <p>Huidige productvereiste: Naast een Workfront-licentie moet u een licentie aanschaffen voor Adobe Workfront Goals. </p> <p>Voor informatie, zie <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref"> Vereisten om de Doelen van Workfront </a> te gebruiken. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Toegangsniveau</td>
 <td> <p>Toegang tot doelen bewerken</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objectmachtigingen</td>
 <td>
  <div>
  <p>De toestemmingen van de mening of hoger aan het doel om het te bekijken</p>
  <p>Machtigingen beheren om het te bewerken</p>
  <p>Voor informatie over het delen van doelstellingen, zie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref"> een doel in de Doelen van Workfront delen </a>. </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het gebied Doelen in het hoofdmenu bevat. </p>  
</td>
  </tr>
</tbody>
</table>

*Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het kopiëren van doelstellingen

U moet toegang tot Edit Doelstellingen in uw toegangsniveau hebben alvorens u doelstellingen kunt kopiëren. Voor informatie over het verlenen van toegang tot Doelen, zie [ Toegang verlenen tot de Doelen van Adobe Workfront ](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Een aantal redenen waarom u een bestaand doel wilt kopiëren zijn:

* Aan het eind van een tijdsperiode (kwartaal of jaar), wanneer u het zelfde doel voor de volgende periode wilt opnieuw creëren.
* Aan het eind van een periode, wanneer het doel niet kan worden voltooid, en u wilt aan het voor een andere tijdspanne werken.
* Wanneer de veelvoudige teamleden gelijkaardige doelstellingen hebben en u zou voor elk van hen kunnen moeten tot stand brengen.

>[!TIP]
>
>U kunt een doel in om het even welke status kopiëren. Voor informatie over doelstatussen, zie [ overzicht van de Goal status in de Doelen van Adobe Workfront ](../../workfront-goals/goal-management/goal-status-overview.md).

Houd rekening met het volgende wanneer u doelstellingen kopieert:

* Alle informatie over het doel wordt ook gekopieerd naar het nieuwe doel.
* U kunt selecteren om de resultaten van een bestaand doel te kopiëren. De naam van de resultaten wordt overgedragen naar het nieuwe doel, maar de huidige voortgang van de resultaten met betrekking tot het bestaande doel wordt niet gekopieerd naar het nieuwe doel. De gekopieerde resultaten worden standaard toegewezen aan dezelfde eigenaar.

  >[!NOTE]
  >
  >Als de oorspronkelijke eigenaar uit Workfront is verwijderd of gedeactiveerd, wordt het nieuwe resultaat toegewezen aan de aangemelde gebruiker.

* U kunt de activiteiten van een doel niet kopiëren wanneer u het doel kopieert.

## Doelstellingen kopiëren

<!--
Copying goals differs depending on what environment you use. 

To copy goals in the Production environment:

1. Go to a goal and click it to open the Goal Details panel.

   For information about accessing an individual goal, see the "Access individual goals" section in [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md).

   This opens the Goal Details panel.

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Copy**. 

1. Update any of the following information for the copied goal:

   | Field |Description  |
   |---|---|
   | New Goal |The name of the new goal. The default is the name of the original goal.  |
   | Period |The time period during which you want to achieve the goal. Select a time period from the drop-down menu or click **Define custom dates** to indicate a custom time period. By default, the Period is always the current quarter. |
   | Owner |The owner of the goal. It can be a user, team, group, or a company. The default is the owner of the original goal.  |
   | Description |Additional information about the goal.  |

1. (Conditional) Select **Copy results** if the original goal had results added to it and you want to copy them to the new goal. This duplicates the original results to the new goal. The results of the copied goal have the same owner, names and measured values as the results of the original goal.

   >[!TIP]
   >
   >* The progress of the original result does not transfer to the copied goal. 
   >* If the original owner was deleted or deactivated from Workfront, the new result is assigned to the logged in user.

1. Click **Save**.

   The copied goal is saved with a status of Draft and displays in the Goal Details panel.

   >[!IMPORTANT]
   >
   >If you have not copied the results from the original goal, you must first associate the new goal with a progress indicator before you can activate it and start working towards achieving it. 
   >
   >Do at least one of the following to be able to activate a goal: 
   >   
   >* Add a Result
   >   
   >  For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   >   
   >* Add an Activity
   >   
   >  For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 
   >   
   >* Align another goal to it
   >   
   >  For information about aligning goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).
   >
   > For information about activating a goal, see [Activate goals in Adobe Workfront Goals](../goal-management/activate-goals.md). 

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

   The copied goal displays in the following sections:

   * Goal List 
   * Check-in (after it is activated)
   * Goal Alignment section (after it is activated) 
   * Pulse
(!--drafted - this was important when we could not update the goal timeframe in the past but we can do that now - not needed
1. (Optional and conditional) If you have copied a goal that was not achieved in a previous time period to continue working on it in the following time period, do the following:

   1. Go to the original goal in the Goal List, Check-in page, or Pulse section and comment on the goal, to indicate that this goal was copied to another, more current goal. For information about commenting on a goal, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md).
   1. Close the original goal, to preserve the progress in its original time period. For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   1. Update the the **Initial** value of the new Result to match the **End At** value of the previous result, so that your new goal progress will start calculating from the point you achieved in the previous period.
   
-->


1. Ga naar een doel en klik **Meer** menu ![ Meer pictogram ](assets/more-icon.png), dan klik **Goal van het Exemplaar**.

   ![ het doelvakje van het Exemplaar ](assets/copy-goal-box-unshimmed.png)

1. Werk de volgende informatie voor het gekopieerde doel bij:
   * **naam van het Doel**: De naam van het nieuwe doel. De standaardnaam voor het gekopieerde doel is &quot;Kopie van &lt;origineel doel>&quot;.
   * **Periode**: De tijdspanne waarin u het doel wilt bereiken. Een tijdsperiode selecteren in het keuzemenu

     of

     Selecteer **douanedata** toelaten om douanedata voor het 2} Begin van het doel **en** Eind data **te specificeren.** De instelling Aangepaste datums inschakelen is standaard uitgeschakeld.

     >[!TIP]
     >
     >   Als u de selectie van Aangepaste datums inschakelen opheft, wordt de tijdsperiode van het oorspronkelijke doel hersteld.

      * **Goal owner**: De eigenaar van het doel. Het kan een gebruiker, een team, een groep, of een bedrijf zijn. Het gebrek is de eigenaar van het originele doel.
      * **Beschrijving**: Aanvullende informatie over het doel.
      * **Resultaten van het Exemplaar**: Selecteer deze optie als u de resultaten van het huidige doel aan het gekopieerde doel wilt overbrengen. Hiermee dupliceert u de oorspronkelijke resultaten en koppelt u deze aan het gekopieerde doel. De resultaten van het gekopieerde doel hebben de zelfde eigenaar, de namen, en de gemeten waarden zoals de resultaten van het originele doel.

        >[!NOTE]
        >
        >* De voortgang van het oorspronkelijke resultaat wordt niet overgedragen naar het gekopieerde doel.
        >* Als de oorspronkelijke eigenaar uit Workfront is verwijderd of gedeactiveerd, wordt het nieuwe resultaat toegewezen aan de aangemelde gebruiker.

1. Klik **doel van het Exemplaar**.

   Er wordt een doel gemaakt dat vergelijkbaar is met het oorspronkelijke doel en het bevindt zich in de status Concept.

   >[!NOTE]
   >
   >Als u de resultaten van het oorspronkelijke doel niet hebt gekopieerd, moet u het nieuwe doel eerst aan een voortgangsindicator koppelen voordat u het kunt activeren en beginnen te werken om het te bereiken.
   >Zie de volgende artikelen voor informatie over het koppelen van doelen aan voortgangsindicatoren:
   >* [ voeg resultaten aan doelstellingen in de Doelen van Adobe Workfront toe ](../results-and-activities/add-results-to-goals.md)
   >* [ voeg activiteiten aan doelstellingen in de Doelen van Adobe Workfront toe ](../results-and-activities/add-activities-to-goals.md)
   >* [ richt doelstellingen door hen in de Doelen van Adobe Workfront te verbinden ](../goal-alignment/align-goals-by-connecting-them.md)
   >
   >Voor informatie over het activeren van doelstellingen, zie [ doelstellingen ](../goal-management/activate-goals.md) activeren.

