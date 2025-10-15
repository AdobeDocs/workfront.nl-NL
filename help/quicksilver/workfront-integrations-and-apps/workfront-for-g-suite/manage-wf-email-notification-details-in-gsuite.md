---
product-area: workfront-integrations
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Beheer  [!DNL Adobe Workfront]  berichtdetails van Google Workspace
description: In Google Workspace, wanneer u een bericht e-mail opent Adobe  [!DNL Workfront]  heeft verzonden, kunt u de bijbehorende details van het het werkpunt bekijken en antwoorden zonder uw Postvak te verlaten. Als er acties beschikbaar zijn, zoals het goedkeuren van een aanvraag, kunt u die acties rechtstreeks uitvoeren vanuit Workfront voor Google Workspace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# [!DNL Adobe Workfront] -meldingsgegevens beheren vanuit [!DNL Google Workspace]

>[!IMPORTANT]
>
>Om stabielere en scalable integratie te leveren, verschuiven wij naar een moderne, flexibele integratiebenadering gebruikend Workfront Automation and Integration (Fusion). Als deel van dit overgangsproces, zal volgende Workfront voor de functionaliteit van Google Workspace niet beschikbaar na **28 Februari, 2026** zijn:
>
>* Google Workspace-functionaliteit openen vanuit Workfront
>
>* Workfront-taken weergeven en beheren vanuit Gmail of het Google Calendar-sitevenster
>
>We raden u aan Workfront Automation and Integration te gebruiken voor de integratiebehoeften van uw organisatie met Google Workspace.
>
>Voor een overzicht van de Automatisering en de Integratie van Workfront, zie [&#x200B; het overzicht van de Fusie van Adobe Workfront &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Voor informatie over de specifieke mogelijkheden van de modules van de Automatisering en van de Integratie van Workfront voor Google Workspace, zie [&#x200B; modules van Gmail &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) en [&#x200B; modules van de Kalender van Google &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

Wanneer u in [!DNL Google Workspace] een e-mailbericht opent dat [!DNL Adobe Workfront] heeft verzonden, kunt u de bijbehorende details van het werkitem weergeven en reageren zonder uw [!UICONTROL Inbox] te verlaten. Als er acties beschikbaar zijn, zoals het goedkeuren van een aanvraag, kunt u die acties rechtstreeks vanuit [!DNL Workfront for Google Workspace] uitvoeren.

>[!NOTE]
>
> [!DNL Workfront for Google Workspace] ondersteunt bijna elk type e-mailmelding dat u kunt ontvangen van [!DNL Workfront] (ongeveer 120 verschillende typen). [!UICONTROL Daily digest] e-mailberichten die vanuit [!DNL Workfront] zijn verzonden, worden niet weergegeven in [!DNL Workfront for Google Workspace] . Voor informatie over de [!DNL Workfront] types van e-mailbericht, zie [&#x200B; uw eigen e-mailberichten wijzigen &#x200B;](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p><p>Werk of hoger</p>
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Voordat u meldingsgegevens kunt beheren vanuit [!DNL Google Workspace] , moet u

* Installeren [!DNL Workfront for Google Workspace]\
   Voor instructies, zie [&#x200B; installeren  [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## [!DNL Adobe Workfront] -meldingsgegevens beheren vanuit [!DNL Google Workspace]

1. Als het [!DNL Workfront for Google Workspace] paneel niet wordt getoond, klik het [!DNL Workfront] pictogram ![&#x200B; pictogram van Workfront &#x200B;](assets/wf-lion-icon.png) in [!DNL Google Workspace] toe:voegen-ons sidebar bij uiterst rechts van de pagina.
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
