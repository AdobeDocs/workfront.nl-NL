---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Richt doelstellingen door resultaten en activiteiten aan doelstellingen om te zetten
description: U kunt twee doelstellingen manueel richten of u kunt de resultaten en de activiteiten van een bestaand doel in een ander doel omzetten. Het omgezette resultaat of de omgezette activiteit wordt het kinddoel van het originele doel. Voor informatie over het manueel richten van twee doelstellingen, zie richten doelstellingen door hen in de Doelen van Adobe Workfront aan te sluiten.
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: c24adf93172d002ea636904d62f531a8e69aace4
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 0%

---

# Richt doelstellingen door resultaten en activiteiten aan doelstellingen om te zetten

U kunt twee doelstellingen manueel richten of u kunt de resultaten en de activiteiten van een bestaand doel in een ander doel omzetten. Het omgezette resultaat of de omgezette activiteit wordt het kinddoel van het originele doel.
Voor informatie over het manueel richten van twee doelstellingen, zie [Richt doelstellingen door hen in de Doelen van Adobe Workfront te verbinden](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Toegangsvereisten


<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront-abonnement*</td>
   <td>
   <p>Nieuw abonnement: Selecteren of hoger</p>
   of
   <p>Huidig abonnement: Pro of hoger</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront-licentie*</td>
   <td>
   <p>Huidige licentie: contribuant of hoger</p>
   of
   <p>Verouderde licentie: aanvragen of hoger</p> <p>Zie voor meer informatie <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Overzicht van Adobe Workfront-licenties</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product*</td>
   <td>
   <p> Nieuwe productbehoefte, één van het volgende: </p>
<ul>
<li>Een Select- of Prime Adobe Workfront-abonnement en een extra Adobe Workfront Goals-licentie.</li>
<li>Een Ultimate Workfront-plan dat standaard Workfront Goals bevat. </li></ul>
   <p>of</p>
   <p>Huidige productvereiste: een Workfront-plan en een extra licentie voor Adobe Workfront Goals. </p> <p>Zie voor meer informatie <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Vereisten voor het gebruik van Workfront-doelen</a>. </p> </td>
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
     <p>Voor informatie over het delen van doelstellingen, zie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Een doel delen in Workfront-doelen</a>. </p>
    </div> </td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het gebied Doelen in het hoofdmenu bevat. </p>  
</td>
  </tr>
 </tbody>
</table>

*Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten

U moet het volgende hebben voordat u kunt beginnen:

* Een lay-outsjabloon die het gebied Doelen in het hoofdmenu bevat.
* Een bestaand doel met bestaande resultaten en activiteiten.

  Voor informatie over het creëren van doelstellingen, zie [Doelen maken voor Adobe Workfront-doelen](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Een doel kan tot 1000 voortgangsindicatoren hebben.

<!--drafted for goal redesign: At PRODUCTION: update the sentence above to remove Production/ Preview references-->

## Overwegingen bij het omzetten van resultaten en activiteiten in doelen

Soms kan een resultaat of een activiteit een grotere reikwijdte hebben dan verwacht en het zou meer zin hebben dat ze doelstellingen worden. U kunt resultaten en activiteiten van een bestaand doel omzetten in een nieuw doel. Dit is een bottom-up benadering van het richten van doelstellingen.

Overweeg het volgende wanneer het omzetten van resultaten en activiteiten in doelstellingen:

* Het omgezette resultaat of de omgezette activiteit wordt het kinddoel van het oorspronkelijke doel, en de twee doelstellingen worden gericht.
* Het nieuwe doel wordt de enige voortgangsindicator voor het oorspronkelijke doel, als er geen extra resultaten of activiteiten op het oorspronkelijke doel zijn. U moet resultaten en activiteiten aan het kinddoel toevoegen om vooruitgang op het te kunnen volgen.
* Het omzetten van een resultaat of activiteit in een doel is onomkeerbaar. Na omgezette, kan het nieuwe kinddoel nooit een resultaat of activiteit voor het ouderdoel opnieuw worden.

## Een resultaat of activiteit omzetten in een doel

<!--
<span class="preview">Converting results and activities differs depending on what environment you use. </span>

### Convert a result or activity to a goal in the Production environment

1. Go to a goal that has a result or an activity that you want to convert to a goal.
1. Click the name of the goal to open the **Goal Details** panel.
1. Expand the **Results** or **Activities** right-pointing arrows to see a list of results or activities for the goal. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. Ga naar een doel dat een resultaat of een activiteit heeft die u in een doel wilt omzetten.
1. Klik op de doelpagina op **Voortgangsindicatoren** in het linkerdeelvenster.
1. Selecteer een resultaat of activiteit in de lijst met voortgangsindicatoren en klik op de knop **Omzetten in doel** pictogram ![](assets/convert-to-goal-icon-unshimmed.png) boven aan de lijst van voortgangsindicatoren. Het vak Omzetten in doel wordt geopend.

   ![](assets/convert-to-goal-box-unshimmed.png)
1. Werk de volgende gegevens bij:
   * **Doelnaam**: Standaard heeft het nieuwe doel dezelfde naam als het oorspronkelijke resultaat of de oorspronkelijke activiteit.
   * **Periode**: Standaard is de periode van het nieuwe doel het huidige kwartaal. U kunt de **Aangepaste datums inschakelen** het plaatsen om een periode van de douanetijd voor het nieuwe doel te bepalen.
   * **Goedereneigenaar**: Standaard is de eigenaar van het nieuwe doel de eigenaar van het oorspronkelijke resultaat of de oorspronkelijke activiteit.
   * **Beschrijving**: Voeg meer informatie toe over het nieuwe doel.
1. Klikken **Opslaan**

   Het resultaat of de activiteit wordt nu omgezet in een kinddoel van het originele doel. Het wordt vermeld als doel in de lijst van voortgangsindicatoren van het oorspronkelijke doel.



