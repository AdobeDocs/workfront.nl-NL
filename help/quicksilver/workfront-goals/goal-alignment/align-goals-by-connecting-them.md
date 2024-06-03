---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Richt doelstellingen door hen in de Doelen van Adobe Workfront te verbinden
description: Als u een individuele medewerker bent die een persoonlijk doel heeft, kunt u het aan de doelstellingen van uw team willen richten om de vooruitgang van uw eigen doel in de grotere context van de strategie van uw organisatie effectief te tonen.
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 330ee20ad14ea7409db1c6f627ed6aa0e0c5c014
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 0%

---

# Richt doelstellingen door hen in de Doelen van Adobe Workfront te verbinden

Als u een individuele medewerker bent die een persoonlijk doel heeft, kunt u het aan de doelstellingen van uw team willen richten om de vooruitgang van uw eigen doel in de grotere context van de strategie van uw organisatie effectief te tonen.

Wanneer iedereen in uw organisatie hun doelstellingen heeft die aan de doelstellingen van uw organisatie worden gericht, kunnen zij duidelijk zien hoe hun individuele bijdragen en teaminspanningen helpen om de naald op grotere, bedrijf-vlakke prioriteiten vooruit te bewegen. Voor meer informatie over de beste praktijken voor het richten van doelstellingen, zie [Overzicht van uitlijning van doelstellingen in Adobe Workfront](../../workfront-goals/goal-alignment/goal-alignment-overview.md).

Er zijn twee manieren om doelen te verbinden in Adobe Workfront Goals:

* U kunt groepering tussen doelstellingen tot stand brengen door doelstellingen met elkaar te verbinden.

* U kunt twee doelstellingen manueel richten of u kunt resultaten en activiteiten van een bestaand doel in een ander doel omzetten. Het omgezette resultaat of de omgezette activiteit wordt het kinddoel van het originele doel.

>[!IMPORTANT]
>
>Een doel kan in totaal 1000 voortgangsindicatoren hebben.

In dit artikel wordt beschreven hoe u doelen kunt uitlijnen door ze met elkaar te verbinden. Voor informatie over het richten van doelstellingen door resultaten en activiteiten in doelstellingen om te zetten, zie [Richt doelstellingen door resultaten en activiteiten aan doelstellingen om te zetten](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Adobe Workfront-plan</td>
 <td>
 <p>Alle</p>

</td>
 </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-licentie*</td>
 <td>
 <p>Nieuwe licentie: Medewerker of hoger</p>
 of
 <p>Huidige licentie: aanvragen of hoger</p> </td>
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
 <tr>
 <td role="rowheader">Objectmachtigingen</td>
 <td>

<p>De toestemmingen van de mening of hoger aan het doel om het te bekijken</p>
  <p>Machtigingen beheren om het te bewerken</p>
  <p>Voor informatie over het delen van doelstellingen, zie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Een doel delen in Workfront-doelen</a>. </p>
   </td>
 </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het gebied Doelen in het hoofdmenu bevat. </p>  
</td>
  </tr>
</tbody>
</table>

*Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Richt doelstellingen door hen met elkaar te verbinden

<!--
Aligning goals by connecting them differs depending on what environment you use. 

### Align goals by connecting them in the Production environment

1. Create two goals that you want to align. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Activate the goals that you want to align. You can align goals that have a Draft, Active, or Inactive status. For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
1. Go to the goal that you want to align (child goal) to another goal (parent goal) and click its name to open the **Goal Details** panel.

   For example, if you want Goal 2 to influence the progress of Goal 1, you must go to Goal 2. 

1. Click **Align to another goal** in the upper-right corner of the right panel.

   ![](assets/align-to-another-goal-link-highlighted-350x128.png)

1. Start typing the name of an existing goal or the name of an owner in the **Align to another goal** field, then select it when it appears in the list. Only goals that are from the same or future periods display in the list. 
1. Click **Save**.

   The goal you started with (Goal 2) is now the child goal of the goal you aligned it with (Goal 1).   
   The aligned goals display connected in the Goal Alignment section with Goal 2 as secondary to Goal 1.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) To view the goals in the Goal Alignment section, do one of the following:

   * Click the Goal Alignment section in the left panel and find the goals by applying the correct filter. For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).
   * Click the Goal List, Check-in, or Pulse sections in the left panel and find one of the goals, then click the **Alignment icon** ![](assets/align-icon.png) next to the goal name to go directly to the goal in the Goal Alignment section.

   For information about the Goal Alignment section, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md). 

1. (Optional) Add activities and results to either goal to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Remove the alignment between two goals, when you consider that no longer is relevant to your organization's overall strategy For information about removing alignment between goals, see [Remove goal alignment in Adobe Workfront Goals](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

-->
1. Maak twee doelen die u wilt uitlijnen. Voor informatie over het creëren van doelstellingen, zie [Doelen maken voor Adobe Workfront-doelen](../../workfront-goals/goal-management/create-goals.md).
1. (Optioneel) Activeer de doelen die u wilt uitlijnen. U kunt doelstellingen richten die een Ontwerp, Actief, of Inactieve status hebben. Voor informatie over het activeren van doelstellingen, zie [Doelen in Adobe Workfront-doelen activeren](../../workfront-goals/goal-management/activate-goals.md).
1. Ga naar het doel dat u (kinddoel) aan een ander doel (ouderdoel) wilt richten en zijn naam klikken om de doelpagina te openen.

   >[!INFO]
   >
   >Als u bijvoorbeeld wilt dat doelstelling 2 de voortgang van doelstelling 1 beïnvloedt, moet u naar doelstelling 2 gaan.

1. Klikken **Doelgegevens** in het linkerdeelvenster.

1. In de **Informatie over bovenliggende doelen** gebied, klikken **Toevoegen** in de **Bovenliggende doelstelling** veld indien er geen hoofddoel is;

   of

   Klik op de naam van het bovenliggende doel om een ander doel te kiezen.

1. Begin de naam van een bestaand doel in te typen **Bovenliggende doelstelling** en selecteert u deze wanneer deze in de lijst wordt weergegeven. Alleen doelen die afkomstig zijn van dezelfde of toekomstige perioden worden weergegeven in de lijst.

1. Klikken **Wijzigingen opslaan**.

   Het doel waarmee u bent begonnen (doelstelling 2) is nu het onderliggende doel van het bovenliggende doel waarmee u het hebt uitgelijnd (doelstelling 1).\
   De uitgelijnde doelweergave die is verbonden in de sectie Goal Alignment met doelstelling 2 als secundair aan doelstelling 1.
Het kinddoel toont in de de indicatorensectie van de Voortgang van het ouderdoel aangezien zijn vooruitgang de vooruitgang van het ouderdoel bijwerkt.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optioneel) Als u de doelen wilt weergeven in het gedeelte Doeluitlijning van Workfront, gaat u naar het gebied Doelen en klikt u op de knop **Goal Alignment** in het linkerdeelvenster. Voor informatie over de sectie van de Groepering van het Beleid, zie [Navigeren in de sectie Goal Alignment in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. (Optioneel) Voeg activiteiten en resultaten toe aan beide doelen om de voortgang ervan aan te geven. Raadpleeg de volgende artikelen voor informatie over het toevoegen van activiteiten en resultaten:

   * [Activiteiten toevoegen aan doelen in Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [Resultaten toevoegen aan doelen in Adobe Workfront-doelen](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optioneel) Verwijder de uitlijning tussen twee doelen wanneer u van mening bent dat deze niet langer relevant zijn voor de algemene strategie van uw organisatie. Voor informatie over het verwijderen van groepering tussen doelstellingen, zie [Doeluitlijning van Adobe Workfront-doelen verwijderen](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

