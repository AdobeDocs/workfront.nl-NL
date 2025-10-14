---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Richt doelstellingen door resultaten en activiteiten aan doelstellingen om te zetten
description: U kunt twee doelstellingen manueel richten of u kunt de resultaten en de activiteiten van een bestaand doel in een ander doel omzetten. Het omgezette resultaat of de omgezette activiteit wordt het kinddoel van het originele doel. Voor informatie over het manueel richten van twee doelstellingen, zie richten doelstellingen door hen in de Doelen van Adobe Workfront aan te sluiten.
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# Richt doelstellingen door resultaten en activiteiten aan doelstellingen om te zetten

<!--Audited P&P only: 4/2025-->

U kunt twee doelstellingen manueel richten of u kunt de resultaten en de activiteiten van een bestaand doel in een ander doel omzetten. Het omgezette resultaat of de omgezette activiteit wordt het kinddoel van het originele doel.
Voor informatie over het manueel richten van twee doelstellingen, zie [&#x200B; doelstellingen door hen in de Doelen van Adobe Workfront &#x200B;](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md) aan te sluiten.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U hebt de volgende toegang nodig om activiteiten uit te voeren die in dit artikel worden vermeld:

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
   of
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

*Voor meer informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

U moet het volgende hebben voordat u kunt beginnen:

* Een bestaand doel met bestaande resultaten en activiteiten.

  Voor informatie over het creëren van doelstellingen, zie [&#x200B; doelstellingen in de Doelen van Adobe Workfront &#x200B;](../../workfront-goals/goal-management/create-goals.md) creëren.

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

1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![Convert to goal](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. Ga naar een doel dat een resultaat of een activiteit heeft die u in een doel wilt omzetten.
1. Van de pagina van het doel, klik **indicatoren van de Voortgang** in het linkerpaneel.
1. Selecteer een resultaat of een activiteit in de lijst van vooruitgangsindicatoren, dan klik de **Bekeerling in doel** pictogram ![&#x200B; Bekeerling aan doel &#x200B;](assets/convert-to-goal-icon-unshimmed.png) bij de bovenkant van de lijst van de vooruitgangsindicator. Het vak Omzetten in doel wordt geopend.

   ![&#x200B; Bekeerling aan doeldoos &#x200B;](assets/convert-to-goal-box-unshimmed.png)
1. Werk de volgende gegevens bij:
   * **Goal naam**: Door gebrek, heeft het nieuwe doel de zelfde naam zoals het originele resultaat of de activiteit.
   * **Periode**: Door gebrek, is de periode van het nieuwe doel het huidige kwart. U kunt **selecteren laat douanedata** plaatsen toe om een periode van de douanetijd voor het nieuwe doel te bepalen.
   * **Eigenaar van het Doel**: Door gebrek, is de nieuwe doeleigenaar de eigenaar van het originele resultaat of de activiteit.
   * **Beschrijving**: Voeg meer informatie over het nieuwe doel toe.
1. Klik **sparen**

   Het resultaat of de activiteit wordt nu omgezet in een kinddoel van het originele doel. Het wordt vermeld als doel in de lijst van voortgangsindicatoren van het oorspronkelijke doel.



