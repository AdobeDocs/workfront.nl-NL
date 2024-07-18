---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Roltoewijzing voor projecten en initiatieven weergeven in Workload Balancer
description: Nadat u projecten en initiatieven verbindt, kunt u hun middeltoewijzing naast elkaar beheren om ervoor te zorgen zij
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# Roltoewijzing voor projecten en initiatieven weergeven in het dialoogvenster [!UICONTROL Workload Balancer]

>[!IMPORTANT]
>
>Uw organisatie moet een extra licentie aanschaffen voor de [!DNL Adobe Workfront Scenario Planner] , zodat u de informatie over initiatieven in een project kunt bekijken. Voor informatie over het verkrijgen van [!DNL Workfront Scenario Planner], zie [ Toegang nodig om  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md) te gebruiken.

Nadat u projecten en initiatieven verbindt, kunt u hun middeltoewijzing naast elkaar beheren om ervoor te zorgen zij aanpassen. Hiermee vermijdt u overmatige of onderbenutte toewijzingen.

In dit artikel wordt beschreven hoe u bronnen kunt combineren met het deelvenster [!UICONTROL Role Allocation] in [!UICONTROL Workload Balancer] van een project.

Voor algemene informatie over het verzoenen van middelen tussen projecten en initiatieven, met inbegrip van eerste vereisten, zie [ Overzicht van het verzoenen van middeltoewijzingen tussen projecten en initiatieven ](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Toegangsvereisten

U moet het volgende doen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan* </b> </p> </td> 
   <td>[!UICONTROL Business] of hoger</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> license* </b> </p> </td> 
   <td> <p>[!UICONTROL Review] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td><b> Product </b> </td> 
   <td> <p>U moet een extra licentie voor de [!DNL Adobe Workfront Scenario Planner] aanschaffen om toegang te krijgen tot de functionaliteit die in dit artikel wordt beschreven.</p> <p>Voor informatie over het verkrijgen van [!DNL Workfront Scenario Planner], zie <a href="../scenario-planner/access-needed-to-use-sp.md"> Toegang nodig om [!DNL Scenario Planner]</a> te gebruiken. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong> het niveauconfiguraties van de Toegang* </strong> </td> 
   <td> <p>[!UICONTROL View] of betere toegang tot projecten </p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de [!DNL Workfront] -beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan veranderen, zie <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong> de toestemmingen van Objecten </strong> </p> </td> 
   <td> <p>[!UICONTROL View] of hogere toestemmingen aan het project</p> <p>Zie <a href="../scenario-planner/request-access-to-plan.md">[!UICONTROL Request] Toegang tot een abonnement in [!DNL Workfront Scenario Planner]</a> voor informatie over het aanvragen van aanvullende toegang tot een abonnement.</p> <p>Voor informatie over het vragen van om extra toegang tot een project, zie <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## Roltoewijzing voor projecten en initiatieven weergeven in het dialoogvenster [!UICONTROL Workload Balancer]

Als uw bedrijf een [!DNL Workfront Scenario Planner] -licentie heeft aangeschaft, kunt u de brontoewijzingen afstemmen op het initiatief en het project dat eraan is gekoppeld op projectniveau [!UICONTROL Workload Balancer] .

1. (Voorwaardelijk) Verbind een project met een initiatief gebruikend één van de methodes die in de volgende artikelen worden beschreven:

   * [ de projecten van de Invoer aan plannen in  [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [ werk of creeer projecten door initiatieven in  [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md) te publiceren bij.

   >[!IMPORTANT]
   >
   >Als u middelen op het initiatief verandert, moet u het scenario opnieuw publiceren dat het initiatief tot behoort opdat de recentste middelinformatie van het initiatief over het project kan bijwerken.

1. Ga naar het project waar u de toewijzing van baanrollen voor het project evenals voor het bijbehorende initiatief wilt herzien.
1. Klik op [!UICONTROL Workload Balancer] in het linkerdeelvenster.

   Mogelijk moet u eerst op **[!UICONTROL Scheduling]** en daarna op **[!UICONTROL Switch to Workload Balancer]** klikken.

1. Voer een van de volgende handelingen uit:

   * Klik op **[!UICONTROL Month]** om de werklastbalans per maand weer te geven, klik op het vervolgkeuzemenu naast een maand in de tijdlijn ![](assets/drop-down-next-to-month-month-view-wb.png) en klik vervolgens op **[!UICONTROL More]** .
   * Klik op het pictogram **[!UICONTROL Show role allocation]** ![](assets/show-role-allocation-icon.png) rechtsboven op de werkbalk.

   Het deelvenster [!UICONTROL Role Allocation] wordt weergegeven.

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >Hoewel u het deelvenster [!UICONTROL Role Allocation] kunt weergeven, zelfs als uw organisatie geen [!DNL Workfront Scenario Planner] -licentie heeft aangeschaft, kunt u geen informatie weergeven over de taakrollen van initiatieven.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Controleer de volgende informatie in het gebied **[!UICONTROL Project Totals]** van het deelvenster Roltoewijzing:

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
   >   * Wanneer taken of problemen een waarde [!UICONTROL Duration] nul hebben.
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

1. (Optioneel) Klik op het vervolgkeuzepictogram om een van de maanden in het deelvenster [!UICONTROL Role Allocation] of in de tijdlijn van [!UICONTROL Workload Balancer] uit te vouwen.

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   Voor elke maand wordt hetzelfde type informatie weergegeven in het gebied [!UICONTROL Project Totals] .

   >[!TIP]
   >
   >De maanden die in het deelvenster [!UICONTROL Role Allocation] worden weergegeven, zijn de maanden in de tijdlijn die op het scherm in de [!UICONTROL Workload Balancer] wordt weergegeven. Blader terug en door en door op de tijdlijn om extra maanden weer te geven.

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->


