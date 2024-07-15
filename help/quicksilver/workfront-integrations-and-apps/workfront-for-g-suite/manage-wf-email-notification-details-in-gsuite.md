---
product-area: workfront-integrations
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Beheer  [!DNL Adobe Workfront]  berichtdetails van Google Workspace
description: In Google Workspace, wanneer u een bericht e-mailbericht  [!DNL Workfront]  opent heeft verzonden, kunt u de bijbehorende details van het het werkpunt bekijken en antwoorden zonder uw Postvak te verlaten. Als er acties beschikbaar zijn, zoals het goedkeuren van een aanvraag, kunt u die acties rechtstreeks uitvoeren vanuit Workfront voor Google Workspace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# [!DNL Adobe Workfront] -meldingsgegevens beheren vanuit [!DNL Google Workspace]

>[!NOTE]
>
>De meest recente versie van de Adobe Workfront-insteekmodule voor Google is uitgebracht op 26 juni 2023.

Wanneer u in [!DNL Google Workspace] een e-mailbericht opent dat [!DNL Adobe Workfront] heeft verzonden, kunt u de bijbehorende details van het werkitem weergeven en reageren zonder uw [!UICONTROL Inbox] te verlaten. Als er acties beschikbaar zijn, zoals het goedkeuren van een aanvraag, kunt u die acties rechtstreeks vanuit [!DNL Workfront for Google Workspace] uitvoeren.

>[!NOTE]
>
> [!DNL Workfront for Google Workspace] ondersteunt bijna elk type e-mailmelding dat u kunt ontvangen van [!DNL Workfront] (ongeveer 120 verschillende typen). [!UICONTROL Daily digest] e-mailberichten die vanuit [!DNL Workfront] zijn verzonden, worden niet weergegeven in [!DNL Workfront for Google Workspace] . Voor informatie over de [!DNL Workfront] types van e-mailbericht, zie [ uw eigen e-mailberichten wijzigen ](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
  </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## Vereisten

Voordat u meldingsgegevens kunt beheren vanuit [!DNL Google Workspace] , moet u

* Installeren [!DNL Workfront for Google Workspace]\
   Voor instructies, zie [ installeren  [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## [!DNL Adobe Workfront] -meldingsgegevens beheren vanuit [!DNL Google Workspace]

1. Als het deelvenster [!DNL Workfront for Google Workspace] niet wordt weergegeven, klikt u op het [!DNL Workfront] pictogram ![](assets/wf-lion-icon.png) in de zijbalk met invoegtoepassingen uiterst rechts op de pagina. [!DNL Google Workspace]
1. Open in [!DNL Google Workspace] een [!DNL Workfront] -meldingsbericht.
1. Klik op **[!UICONTROL View all updates]** als deze boven in het deelvenster wordt weergegeven.
1. Klik op **[!UICONTROL Details]**.
1. Klik op de beschikbare opties.

   De opties die worden weergegeven, hebben betrekking op het type e-mailmelding dat u hebt geopend. Als het bijvoorbeeld een e-mailmelding is waarin u wordt gevraagd een taak goed te keuren, ziet u **[!UICONTROL Approve]** en **[!UICONTROL Reject]** in plaats van opties zoals **[!UICONTROL Work on It]** of **[!UICONTROL Done]** :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Type e-mailmelding</th> 
      <th>Handeling</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Taak of probleem</td> 
      <td><strong>[!UICONTROL Approve]</strong> het, <strong>[!UICONTROL Reject]</strong> het, <strong>[!UICONTROL Grant]</strong> toegang tot het, <strong>[!UICONTROL Ignore]</strong> een verzoek om toegang tot het, <strong>[!UICONTROL Work on it]</strong>, of klik een optie om erop te wijzen dat u <strong>[!UICONTROL Done]</strong> met het bent</td> 
     </tr> 
     <tr> 
      <td>Project</td> 
      <td><strong>[!UICONTROL Approve]</strong> het, <strong>[!UICONTROL Reject]</strong> het, <strong>[!UICONTROL Grant]</strong> toegang tot het, of <strong>[!UICONTROL Ignore]</strong> een verzoek om toegang tot het</td> 
     </tr> 
     <tr> 
      <td>Document</td> 
      <td><strong>[!UICONTROL Approve]</strong> het, <strong>[!UICONTROL Reject]</strong> het, <strong>[!UICONTROL Grant]</strong> toegang tot het, of <strong>[!UICONTROL Ignore]</strong> een verzoek om toegang tot het</td> 
     </tr> 
     <tr> 
      <td>Bijwerken </td> 
      <td> <p>Geef een gedeelte van de volledige lijst met updates voor het item weer, zodat u de context hebt die u nodig hebt voor <strong>[!UICONTROL Post]</strong> een nieuwe update of een <strong>[!UICONTROL Reply]</strong> . U kunt op <strong>[!UICONTROL Notify]</strong> klikken om bepaalde gebruikers te waarschuwen voor uw reactie. </p> <p>Zie <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref"> Reageren op een [!DNL Adobe Workfront] updatemelding van [!DNL Google Workspace]</a> voor meer informatie.</p> </td> 
     </tr> 
     <tr> 
      <td>Goedkeuringsaanvraag</td> 
      <td><strong>[!UICONTROL Approve]</strong> of <strong>[!UICONTROL Reject]</strong> het (u kunt uw mening veranderen door de andere optie te klikken), het downloaden, zijn eigenaar bekijken of zijn verwijzingsaantal bekijken</td> 
     </tr> 
     <tr> 
      <td>Een wijziging in de status van een project</td> 
      <td> Bekijk alle huidige informatie over het project, inclusief aangepaste formulieren. </td> 
     </tr> 
    </tbody> 
   </table>
