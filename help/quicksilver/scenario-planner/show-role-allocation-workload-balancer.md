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

# Toon roltoewijzing voor projecten en initiatieven in [!UICONTROL Workload Balancer]

>[!IMPORTANT]
>
>Uw organisatie moet een extra licentie aanschaffen voor de [!DNL Adobe Workfront Scenario Planner] zodat u de informatie over een initiatief kunt bekijken over een project. Voor informatie over het verkrijgen van de [!DNL Workfront Scenario Planner], zie [Toegang nodig om de [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Nadat u projecten en initiatieven verbindt, kunt u hun middeltoewijzing naast elkaar beheren om ervoor te zorgen zij aanpassen. Hiermee vermijdt u overmatige of onderbenutte toewijzingen.

In dit artikel wordt beschreven hoe u bronnen met behulp van de [!UICONTROL Role Allocation] in [!UICONTROL Workload Balancer] van een project.

Zie voor algemene informatie over het in overeenstemming brengen van middelen tussen projecten en initiatieven, inclusief voorwaarden [Overzicht van de afstemming van de toewijzingen van middelen tussen projecten en initiatieven](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Toegangsvereisten

U moet het volgende doen:

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
   <td> <p>U moet een extra licentie aanschaffen voor de [!DNL Adobe Workfront Scenario Planner] voor toegang tot de functionaliteit die in dit artikel wordt beschreven.</p> <p>Voor informatie over het verkrijgen van de [!DNL Workfront Scenario Planner], zie <a href="../scenario-planner/access-needed-to-use-sp.md">Toegang nodig om de [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraties op toegangsniveau*</strong> </td> 
   <td> <p>[!UICONTROL View] of betere toegang tot projecten </p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau veranderen, zie <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objectmachtigingen</strong> </p> </td> 
   <td> <p>[!UICONTROL View] of hogere machtigingen voor het project</p> <p>Voor informatie over het vragen van om extra toegang tot een plan, zie <a href="../scenario-planner/request-access-to-plan.md">[!UICONTROL Request] toegang tot een plan in het [!DNL Workfront Scenario Planner]</a>.</p> <p>Voor informatie over het vragen van om extra toegang tot een project, zie <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Toon roltoewijzing voor projecten en initiatieven in [!UICONTROL Workload Balancer]

Als uw bedrijf een [!DNL Workfront Scenario Planner] vergunning, kunt u de middeltoewijzingen tussen het initiatief en het project met betrekking tot het op projectniveau met elkaar in overeenstemming brengen [!UICONTROL Workload Balancer].

1. (Voorwaardelijk) Verbind een project met een initiatief gebruikend één van de methodes die in de volgende artikelen worden beschreven:

   * [Projecten importeren naar plannen in het dialoogvenster [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [Werk of creeer projecten bij door initiatieven in te publiceren [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md).

   >[!IMPORTANT]
   >
   >Als u middelen op het initiatief verandert, moet u het scenario opnieuw publiceren dat het initiatief tot behoort opdat de recentste middelinformatie van het initiatief over het project kan bijwerken.

1. Ga naar het project waar u de toewijzing van baanrollen voor het project evenals voor het bijbehorende initiatief wilt herzien.
1. Klikken [!UICONTROL Workload Balancer] in het linkerdeelvenster.

   Mogelijk moet u op **[!UICONTROL Scheduling]** vervolgens **[!UICONTROL Switch to Workload Balancer]**.

1. Voer een van de volgende handelingen uit:

   * Klikken **[!UICONTROL Month]** Klik op het vervolgkeuzemenu naast een maand in de tijdlijn om de taakverdeling per maand weer te geven ![](assets/drop-down-next-to-month-month-view-wb.png)en klik vervolgens op **[!UICONTROL More]**.
   * Klik op de knop **[!UICONTROL Show role allocation]** pictogram ![](assets/show-role-allocation-icon.png) in de rechterbovenhoek van de werkbalk.

   De [!UICONTROL Role Allocation] wordt weergegeven.

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >Hoewel u de [!UICONTROL Role Allocation] zelfs als uw organisatie geen [!DNL Workfront Scenario Planner] licentie, kunt u geen informatie weergeven over de functies van initiatieven.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Controleer de volgende informatie in het dialoogvenster **[!UICONTROL Project Totals]** gebied van het deelvenster Roltoewijzing:

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
      <td> <p>Het verschil tussen de voor het initiatief vereiste uren en de geplande uren voor de werkzaamheden aan het project. [!DNL Workfront] berekent de [!UICONTROL Variance] aan de hand van deze formule:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>Wanneer de middelen voor meer uren zijn gepland dan voor het initiatief vereist is, [!UICONTROL Variance] is negatief en wordt rood weergegeven. Dit betekent dat uw middelen worden oververdeeld. </p> </td> 
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
   >   * Wanneer taken of problemen een [!UICONTROL Duration] van nul.




1. (Optioneel) Als de [!UICONTROL Variance] in de kolom wordt aangegeven dat uw bronnen zijn oververdeeld, past u een van de volgende opties aan:

   * Verlaag het aantal Geplande Uren voor één baanrol die overtoegewezen toont of meer middelen aan de taken toevoegt en meer Geplande Uren aan de nieuwe middelen verdeelt. U kunt toewijzingen of het aantal geplande uren voor taken of problemen bijwerken wanneer u deze bewerkt. Zie de volgende artikelen voor meer informatie:

      * [Taken bewerken](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [Problemen bewerken](../manage-work/issues/manage-issues/edit-issues.md)

      >[!NOTE]
      >
      >U moet over aanvullende toegang en machtigingen beschikken om taken en problemen te kunnen bewerken.

   * Verhoog het aantal vereiste uren voor de rol die de overtoewijzing op het initiatief toont. Zie voor meer informatie [Initiatieven maken en bewerken in het dialoogvenster [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

      >[!NOTE]
      >
      >U moet over extra toegang en toestemmingen beschikken om plannen uit te geven.


1. (Optioneel) Klik op het vervolgkeuzepictogram om een van de maanden in het dialoogvenster [!UICONTROL Role Allocation] of in de tijdlijn van het deelvenster [!UICONTROL Workload Balancer].

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   Hetzelfde type informatie dat wordt weergegeven in het dialoogvenster [!UICONTROL Project Totals] wordt ook weergegeven voor elke maand.

   >[!TIP]
   >
   >De in de [!UICONTROL Role Allocation] zijn de maanden in de tijdlijn die op het scherm in de [!UICONTROL Workload Balancer]. Blader terug en door en door op de tijdlijn om extra maanden weer te geven.

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->


