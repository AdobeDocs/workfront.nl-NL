---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Roltoewijzing voor projecten en initiatieven weergeven in de takenlijst
description: Nadat u projecten en initiatieven verbindt, kunt u hun middeltoewijzing naast elkaar beheren om ervoor te zorgen zij aanpassen. Hiermee vermijdt u overmatige of onderbenutte toewijzingen.
author: Alina
feature: Workfront Scenario Planner
exl-id: 77152e46-0b7b-4937-9d16-1a20c2a7fdf1
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Roltoewijzing voor projecten en initiatieven weergeven in de takenlijst

<!--Audited: 07/2024-->

Nadat u projecten en initiatieven verbindt, kunt u hun middeltoewijzing naast elkaar beheren om ervoor te zorgen zij aanpassen. Hiermee vermijdt u overmatige of onderbenutte toewijzingen.

In dit artikel wordt beschreven hoe u bronnen kunt combineren met het deelvenster [!UICONTROL Role Allocation] in de takenlijst van een project.

Voor algemene informatie over het verzoenen van middelen tussen projecten en initiatieven, met inbegrip van eerste vereisten, zie [ Overzicht van het verzoenen van middeltoewijzingen tussen projecten en initiatieven ](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

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
   <p>Het Scenario-abonnement is niet beschikbaar voor het nieuwe Workfront Select- of Workfront-abonnement. </p>
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
   <td> <p>De mening of hogere toegang tot Projecten.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objectmachtigingen </p> </td> 
   <td> <p> Weergave of hogere machtigingen voor een project.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang tot de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Roltoewijzing voor projecten en initiatieven weergeven in de takenlijst

Als uw bedrijf een [!DNL Workfront Scenario Planner] -licentie heeft aangeschaft, kunt u de brontoewijzingen afstemmen tussen het initiatief en het project dat eraan is gekoppeld in het [!UICONTROL Tasks] -gedeelte van het project.

1. (Voorwaardelijk) een project moet met een initiatief worden verbonden gebruikend één van de methodes die in de sectie [ worden beschreven tonen roltoewijzing voor projecten en initiatieven in de taaklijst ](#show-role-allocation-for-projects-and-initiatives-in-the-task-list) van dit artikel.

   >[!IMPORTANT]
   >
   >Als u middelen op het initiatief verandert, moet u het scenario opnieuw publiceren dat het initiatief tot behoort opdat de recentste middelinformatie van het initiatief over het project kan bijwerken.

1. Ga naar het project waar u de toewijzing van baanrollen voor het project evenals voor het bijbehorende initiatief wilt herzien.
1. Klik op **[!UICONTROL Tasks]** in het linkerdeelvenster.
1. Klik op het pictogram **[!UICONTROL Show role allocation]** ![](assets/show-role-allocation-icon.png) rechtsboven op de werkbalk.

   Het deelvenster [!UICONTROL Role Allocation] wordt weergegeven.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Controleer de volgende informatie in het gebied **[!UICONTROL Project Totals]** van het deelvenster [!UICONTROL Role Allocation] :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Job Role]</td> 
      <td> <p>De namen van de functies die aan een van de volgende taken zijn gekoppeld:</p> 
       <ul> 
        <li> <p>taken betreffende het project</p> </li> 
        <li> <p>kwesties in verband met het project</p> </li> 
        <li> <p>initiatief in verband met het project</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Hours]</td> 
      <td>Het aantal vereiste uren voor elke functie op initiatief gedurende de totale duur van het initiatief. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Planned Hours]</td> 
      <td>Het aantal geplande uren dat is gekoppeld aan elke taakrol in de taken of problemen van het project voor de totale duur van het project. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Variance]</td> 
      <td> <p>Het verschil tussen de voor het initiatief vereiste uren en de geplande uren voor de werkzaamheden aan het project. [!DNL Workfront] berekent de [!UICONTROL Variance] aan de hand van de volgende formule:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>Wanneer bronnen langer dan vereist voor het initiatief gepland zijn, is de waarde van [!UICONTROL Variance] negatief en wordt deze in rood weergegeven. Dit betekent dat uw middelen worden oververdeeld. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >De geplande uren van het project tonen niet in de volgende scenario&#39;s:
   >
   >   
   >   
   >   * Wanneer taken of kwesties niet aan baanrollen worden toegewezen, of gebruikers met een baanrol verbonden aan hen.
   >   * Wanneer de taken of de kwesties een Duur van nul hebben.
   >   
   >



1. (Optioneel) Als in de kolom [!UICONTROL Variance] wordt aangegeven dat uw bronnen zijn oververdeeld, past u een van de volgende opties aan:

   * Verlaag het aantal Geplande Uren voor één baanrol die overtoegewezen toont of meer middelen aan de taken toevoegt en meer Geplande Uren aan de nieuwe middelen verdeelt. U kunt toewijzingen of het aantal geplande uren voor taken of problemen bijwerken wanneer u deze bewerkt. Zie de volgende artikelen voor meer informatie:

      * [ geef taken ](../manage-work/tasks/manage-tasks/edit-tasks.md) uit
      * [Problemen bewerken](../manage-work/issues/manage-issues/edit-issues.md)

     >[!NOTE]
     >
     >U moet over aanvullende toegang en machtigingen beschikken om taken en problemen te kunnen bewerken.

   * Verhoog het aantal vereiste uren voor de rol die de overtoewijzing op het initiatief toont. Voor meer informatie, zie [ initiatieven in  [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md) creëren en uitgeven.

     >[!NOTE]
     >
     >U moet over extra toegang en toestemmingen beschikken om plannen uit te geven.


