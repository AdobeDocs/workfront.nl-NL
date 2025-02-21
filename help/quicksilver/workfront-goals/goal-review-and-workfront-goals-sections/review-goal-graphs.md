---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Grafieken bekijken om trends in de voortgang van het doel in Adobe Workfront-doelen te begrijpen
description: U kunt de algemene gezondheid van uw doelstellingen en hun vooruitgangstendens in tijd in de sectie van Grafieken van de Doelen van Adobe Workfront bekijken. De grafieken in deze sectie breken niet de vooruitgang van elk doel af, maar geven u in plaats daarvan een holistische momentopname van de de vooruitgangsstatus van alle doelstellingen evenals hun vooruitgangstendens in tijd tijdens een gespecificeerde periode.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '987'
ht-degree: 0%

---

# Grafieken bekijken om trends in de voortgang van het doel in Adobe Workfront-doelen te begrijpen

<!-- drafted mostly for P&P release-->

U kunt de algemene gezondheid van uw doelstellingen en hun vooruitgangstendens in tijd in de sectie van Grafieken van de Doelen van Adobe Workfront bekijken. De grafieken in deze sectie breken niet de vooruitgang van elk doel af, maar geven u in plaats daarvan een holistische momentopname van de de vooruitgangsstatus van alle doelstellingen evenals hun vooruitgangstendens in tijd tijdens een gespecificeerde periode.

>[!IMPORTANT]
>
>U kunt een totaal aantal voor uw doelstellingen in de sectie van Grafieken voor een geselecteerde periode zien. Nochtans, neemt de Doelen van Workfront slechts doelstellingen met een status van Actief en Gesloten in aanmerking wanneer het berekenen van de algemene status van de doelvooruitgang en het percentage voltooide.

## Toegangsvereisten

U moet de volgende toegang hebben om de handelingen uit te voeren die in dit artikel worden beschreven:

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
 <p> Nieuwe productbehoefte, één van het volgende: </p>
<ul>
<li>Een Select- of Prime Adobe Workfront-abonnement en een extra Adobe Workfront Goals-licentie.</li>
<li>Een Ultimate Workfront-plan dat standaard Workfront Goals bevat. </li></ul>
 <p>of</p>
 <p>Huidige productvereiste: een Workfront-plan en een extra licentie voor Adobe Workfront Goals. </p> <p>Voor informatie, zie <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref"> Vereisten om de Doelen van Workfront </a> te gebruiken. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Toegangsniveau</p></td>
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

## Typen grafieken in Workfront-doelen

De volgende grafieken zijn beschikbaar in de sectie Grafieken of de Doelen van Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">The Goal Health Chart</td> 
   <td> <p>Een diagram dat het volgende weergeeft:</p> 
    <ul> 
     <li>Een totaal aantal doelstellingen voor de geselecteerde periode. Er wordt rekening gehouden met doelstellingen met elke status. </li> 
     <li>De voortgangsstatus van doelen met de status Actief en Gesloten.</li> 
    </ul> <p>Voor informatie over hoe de Doelen van Workfront vooruitgangsstatus berekent, zie <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref"> Overzicht van doelvooruitgang en voorwaarde in de Doelen van Adobe Workfront </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">The Goal Progress Chart</td> 
   <td> <p>Een lijngrafiek die updates toont die aan doelstellingen in wekelijkse toename tijdens de duur van het doel worden gemaakt. In het voortgangsdiagram voor het doel wordt het volgende weergegeven:</p> 
    <ul> 
     <li>Een gemiddeld verwacht en werkelijk percentage volledig van alle actieve en gesloten doelstellingen in de geselecteerde periode. Het percentage van de volledige voortgang wordt opgesplitst in wekelijkse stappen gemarkeerd door knooppunten. </li> 
     <li>Het totale gemiddelde percentage vorderingen voor actieve en afgeronde doelstellingen sinds de vorige week. </li> 
    </ul> <p>Tip: het grafiek van de doelvooruitgang zou geen informatie kunnen tonen wanneer de updates over de doelstellingen buiten de geselecteerde tijdspanne worden gemaakt. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Voortgang van doel van grafieken controleren

1. Klik het **pictogram van het 1} pictogram van het Belangrijkste Menu ![ ](assets/main-menu-icon.png) >** Doelen **in de hoger-juiste hoek.**

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Dit opent het gebied van de Doelen van Workfront.

1. Klik **Grafieken** in het linkerpaneel.

   ![ Grafieken in linkerpaneel ](assets/graphs-in-left-panel.png)

   De sectie Grafieken wordt weergegeven.

   Standaard worden de doelstellingen in de sectie Grafieken beperkt door de volgende criteria:

   * De filters die op het gebied van Grafieken worden toegepast.
   * De doelstellingen die in een status van Actief en Ontwerp zijn.

1. (Optioneel) Selecteer het type informatie dat u wilt weergeven door de filters in de rechterbovenhoek van de sectie Grafieken bij te werken.

   Voor meer informatie over het filtreren van doelstellingen, zie [ informatie van de Filter in de Doelen van Adobe Workfront ](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   >
   >Als u ervoor hebt gekozen om meer dan één tijdsperiode weer te geven, wordt voor elke tijdsperiode een gezondheidgrafiek (gauge) en een voortgangsgrafiek (lijn) weergegeven.

1. Bekijk de informatie in de onderstaande tabel wanneer u de Goal Health Chart bekijkt.

   ![ Grafiek van de Gang ](assets/gauge-graph-wf-align-350x230.png)

   | Totaal aantal doelstellingen | Het getal onder aan het diagram geeft het aantal doelen in de geselecteerde periode aan, in alle statussen die u hebt geselecteerd. |
   |---|---|
   | Gemiddeld percentage voltooid | Bij de bovenkant van de grafiek, wijst dit aantal op het gemiddelde percentage volledige van actieve en gesloten doelstellingen in de geselecteerde tijdspanne. |
   | Doelstellingen en vorderingen | Het aantal doelstellingen voor elk segment van de vooruitgangsstatus, wanneer u over de segmenten van de grafiek beweegt. Alleen doelen in een status Actief of Gesloten worden geteld in de segmenten. |


1. Bekijk de informatie in de onderstaande tabel wanneer u de grafiek van de voortgang van het beleid bekijkt.

   ![ grafiek van de Lijn ](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Voortgang van basislijn</td> 
      <td>De groene hellingslijn wijst op het verwachte algemene percentage volledige gemiddelde van actieve en gesloten doelstellingen voor de geselecteerde tijdspanne. Alle doelstellingen binnen een periode worden verwacht te voltooien, zodat is de basisvooruitgang altijd 100% aan het eind van de periode. </td> 
     </tr> 
     <tr> 
      <td>Werkelijke vooruitgang</td> 
      <td> <p>De blauwe lijn geeft het daadwerkelijke totale percentage aan van het volledige gemiddelde van actieve en gesloten doelen voor de geselecteerde tijdsperiode in wekelijkse stappen. Elke week tijdens de duur van het doel wordt duidelijk door een knoop in de lijn. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Houd een weekknooppunt boven in het voortgangsdiagram voor het doel en bekijk het volgende:

   * **de datum van de Week**: De maand, de dag, en het jaar van de geselecteerde week.
   * **Voortgang**: Een gemiddelde van het daadwerkelijke percentage voltooide van alle doelstellingen voor de geselecteerde week.
   * **Basislijn**: Een gemiddelde van het verwachte percentage voltooide van alle doelstellingen voor de geselecteerde week.

1. (Facultatief) klik **Voortgang** bij de bodem van de vooruitgangsgrafiek om de daadwerkelijke algemene vooruitgangslijn te verwijderen

   of

   Klik **Basislijn** bij de bodem van de vooruitgangsgrafiek om de verwachte vooruitgang uit de grafiek te verwijderen.

 
