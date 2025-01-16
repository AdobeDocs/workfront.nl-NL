---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Overzicht van verbindingen
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# Overzicht van verbindingen

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in de artikelen:
>
>* [ Overzicht van de Verbinding ](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/connection-overview.html)
>* [ beheert verbindingen ](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/manage-connections.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

<!-- Audited: 3/2024-->

Voor de meeste toepassingen vereist [!DNL Workfront Fusion] een verbinding, waardoor het kan communiceren met de opgegeven service van derden volgens de instellingen van het specifieke scenario.

Als u bijvoorbeeld een scenario wilt maken dat informatie ophaalt uit [!DNL Workfront] , moet u [!DNL Workfront Fusion] toegangsrechten geven voor toegang tot uw [!DNL Workfront] -account.

Een verbinding vertegenwoordigt de vergunning en de toestemmingen die Fusion gebruikt om tot de toepassing toegang te hebben. U kunt één of meerdere verbindingen voor elke toepassing tot stand brengen, en kunt de zelfde verbinding in veelvoudige modules of scenario&#39;s gebruiken.

De meeste verbindingen worden gebruikt slechts voor één enkele toepassing. Een [!DNL Workfront] -verbinding kan bijvoorbeeld niet worden gebruikt in een [!UICONTROL Salesforce] -module. Sommige [!DNL Adobe] -toepassingen kunnen verbindingen delen. Voor details, zie de artikelen voor die toepassingen, die in [ worden vermeld Apps en hun modules ](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

De verbindingen worden beheerd op het teamniveau. Alle leden van een team hebben toegang tot de verbindingen van het team en gebruikers buiten een team hebben geen toegang tot de verbindingen van het team.

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> <p>Nieuw: [!UICONTROL Standard]</p><p>of</p><p>Huidig: [!UICONTROL Work] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidig: Geen [!DNL Workfront Fusion] vereiste licentie.</p>
   <p>of</p>
   <p>Verouderd: alle </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Nieuw:</p> <ul><li>[!UICONTROL Select] of [!UICONTROL Prime] [!DNL Workfront] Plan: Uw organisatie moet het abonnement aanschaffen [!DNL Adobe Workfront Fusion] .</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Overzicht: [!DNL Workfront Fusion] is opgenomen.</li></ul>
   <p>of</p>
   <p>Huidig: Uw organisatie moet [!DNL Adobe Workfront Fusion] aanschaffen.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Toegangsrechten

Voor elke verbinding vereist [!DNL Workfront Fusion] alleen de toegangsrechten die nodig zijn om een bepaald scenario te voltooien. Als u bijvoorbeeld een scenario maakt om documenten van [!DNL Google Docs] weer te geven, vraagt [!DNL Workfront Fusion] niet om toestemming om de inhoud van de documenten op te halen. Later kunt u, als u ontdekt dat u tot de inhoud van de documenten moet toegang hebben, de verbinding bijwerken of een nieuwe creëren die tot die inhoud kan toegang hebben.

Niet alle diensten staan u toe om toegang tot specifieke taken te beperken. In deze gevallen moet [!DNL Workfront Fusion] volledige toegangsrechten vereisen. Voor meer informatie over hoe te om [!DNL Workfront Fusion] toegang tot uw rekening te beperken die tot die diensten wordt geregistreerd, zie de toepassing-specifieke documentatie die in [ wordt vermeld Apps en hun modules ](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

## Verbindingen beheren

U kunt alle verbindingen vanuit het [!UICONTROL Connections] -gebied beheren.

>[!NOTE]
>
>Verbindingen zijn eigendom van teams. Als u niet de verbinding kunt vinden u zoekt, controleer dat u het correcte team bekijkt.
>
>Een nieuw team selecteren:
>
>* Klik op de naam van het team in de linkernavigatie en selecteer een nieuw team.
>
>    of
>
>* Klik het overzicht van het Team in de linkernavigatie, dan klik de drop-down pijl naast de teamnaam dichtbij de bovenkant van de pagina. Selecteer een nieuw team.

1. Als u het [!UICONTROL Connections] -gebied wilt openen, klikt u op <b>[!UICONTROL Connections]</b> in de linkernavigatie.
1. (Optioneel) Geef de omgeving en het type verbinding aan door te klikken op de vervolgkeuzelijst Omgeving en Type en een optie te selecteren.
1. (Facultatief) om te bekijken welke toestemmingen aan [!DNL Workfront Fusion] voor een verbinding werden gegeven, klik het pictogram van de Mening ![ de verbindingstoestemmingen van de Mening ](assets/view-connection-permissions.png) voor die verbinding.
1. (Optioneel) Als u de naam van een verbinding wilt wijzigen, markeert u de naam van de verbinding en typt u de nieuwe naam.
1. (Facultatief) om een verbinding opnieuw toe te staan, klik **opnieuw machtigen** voor die verbinding.
1. (Facultatief) om een verbinding te schrappen, klik **Schrapping** voor die verbinding.
1. (Facultatief) om te verifiëren dat de verbinding aan de dienst met succes werd gevestigd, klik **verifieer** voor de verbinding.



## Een verbinding vernieuwen

[!DNL Workfront Fusion] verkrijgt gewoonlijk toegangsrechten tot een bepaalde dienst voor een onbeperkte periode. Sommige toepassingen vereisen de toegangstoestemming om na een bepaalde periode worden vernieuwd. In deze gevallen meldt [!DNL Workfront Fusion] u kort voordat de toegangsrechten verlopen via e-mail.

Een verbinding vernieuwen:

1. Klik op de knop **[!UICONTROL Reauthorize]** in het **[!UICONTROL Connections]** -gebied.
