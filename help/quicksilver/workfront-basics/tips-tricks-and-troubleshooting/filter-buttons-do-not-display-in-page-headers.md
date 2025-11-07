---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filterknoppen worden niet weergegeven in paginakoppen
description: Lees dit artikel om filterknoppen problemen op te lossen die niet in paginakoppen worden weergegeven.
feature: Get Started with Workfront
author: Courtney
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 1%

---

# Filterknoppen worden niet weergegeven in paginakoppen

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table>
  <tr>
   <td>Adobe Workfront-pakket
   </td>
   <td> <p>Prime of Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Adobe Workfront-licenties
   </td>
   <td><p>Standard</p>
   <p>Plan</p>
   </td>
  </tr>
   <tr>
   <td>Configuraties op toegangsniveau
   </td>
   <td>U moet een [!DNL Workfront] beheerder zijn.
   </td>
  </tr>
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Probleem

De volgende filterknoppen worden niet weergegeven in de desbetreffende gebieden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] gebied</strong></td> 
   <td><strong>Filterknoppen</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Projects] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects I'm On]</p> </li> 
     <li> <p>[!UICONTROL Projects I Own]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL Timesheets]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL My Timesheet Approvals]</span> </p> </li> 
     <li> <p><span>[!UICONTROL My Timesheets]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Oplossing

De filterknoppen in het gebied [!UICONTROL Projects and Timesheets] worden niet weergegeven omdat de bijbehorende filters niet zijn opgenomen in de lay-outsjabloon die op de gebruiker is toegepast. De [!DNL Workfront] -beheerder moet een lay-outsjabloon toewijzen die de filters bevat.

>[!NOTE]
>
>Soms worden de filters verwijderd uit het [!UICONTROL List Controls] -gebied in [!UICONTROL Setup] . De [!DNL Workfront] -beheerder moet deze in de lijsten in dit gebied opnemen, anders zijn ze niet beschikbaar in de lay-outsjablonen.

1. Controleer of in de lay-outsjabloon de volgende filters worden weergegeven:

   * [!UICONTROL Projects I'm On] en [!UICONTROL Projects I Own] in het [!UICONTROL Projects] -gebied
   * [!UICONTROL My Timesheet Approvals] en [!UICONTROL My Timesheets] in het [!UICONTROL Timesheet] -gebied

   Dit doet u als volgt:

   1. Open de lay-outsjabloon.
   1. Selecteer **[!UICONTROL Lists]** onder **[!UICONTROL Customize what users see]** .
   1. Selecteer **[!UICONTROL Projects]** of **[!UICONTROL Timesheets]** onder **[!UICONTROL Select a list to customize]** .
   1. Controleer in de sectie **[!UICONTROL Filter]** of **[!UICONTROL Projects I'm On]** , **[!UICONTROL Projects I Own]** (voor projecten) en **[!UICONTROL My Timesheet Approvals]** en **[!UICONTROL My Timesheets]** (voor tijdbladen) zijn geselecteerd.
   1. Klik op **[!UICONTROL Save]**.

   Voor meer informatie, zie [ Filters, Mening, en Groepen aanpassen gebruikend een lay-outmalplaatje ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Wijs het lay-outmalplaatje aan de correcte gebruikers, baanrollen, teams, of groepen toe. Voor informatie, zie [ gebruikers aan een lay-outmalplaatje ](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md) toewijzen.
