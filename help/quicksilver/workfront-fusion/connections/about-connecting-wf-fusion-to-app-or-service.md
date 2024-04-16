---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Overzicht van verbindingen
description: Voor de meeste toepassingen is het nodig een verbinding te maken, waardoor [!DNL Adobe Workfront Fusion] kan met de bepaalde derdedienst volgens de montages van het specifieke scenario communiceren.
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Overzicht van verbindingen

<!-- Audited: 3/2024-->

Voor de meeste apps: [!DNL Workfront Fusion] vereist een verbinding, waardoor het met de bepaalde derdedienst volgens de montages van het specifieke scenario kan communiceren.

Bijvoorbeeld, als u een scenario wilt tot stand brengen dat informatie van terugwint [!DNL Workfront], moet u toegangsrechten verlenen voor [!DNL Workfront Fusion] om toegang te krijgen tot [!DNL Workfront] account.

Een verbinding vertegenwoordigt de vergunning en de toestemmingen die Fusion gebruikt om tot de toepassing toegang te hebben. U kunt één of meerdere verbindingen voor elke toepassing tot stand brengen, en kunt de zelfde verbinding in veelvoudige modules of scenario&#39;s gebruiken.

De meeste verbindingen worden gebruikt slechts voor één enkele toepassing. Bijvoorbeeld een [!DNL Workfront] verbinding kan niet worden gebruikt in [!UICONTROL Salesforce] -module. Sommige [!DNL Adobe] toepassingen kunnen verbindingen delen. Zie de artikelen voor deze toepassingen in [Apps en modules daarvan](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

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
   <td> <p>Nieuw: [!UICONTROL Standard]</p><p>of</p><p>Huidige: [!UICONTROL Work] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidig: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Verouderd: alle </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Nieuw:</p> <ul><li>[!UICONTROL Select] of [!UICONTROL Prime] [!DNL Workfront] Abonnement: uw organisatie moet aankopen [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] is opgenomen.</li></ul>
   <p>of</p>
   <p>Huidig: Uw organisatie moet het volgende aanschaffen [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Toegangsrechten

Voor elke verbinding, [!DNL Workfront Fusion] vereist slechts die toegangsrechten die noodzakelijk zijn om een bepaald scenario met succes te voltooien. Als u bijvoorbeeld een scenario maakt om documenten weer te geven van [!DNL Google Docs], [!DNL Workfront Fusion] vraagt niet om toestemming om de inhoud van de documenten op te halen. Later kunt u, als u ontdekt dat u tot de inhoud van de documenten moet toegang hebben, de verbinding bijwerken of een nieuwe creëren die tot die inhoud kan toegang hebben.

Niet alle diensten staan u toe om toegang tot specifieke taken te beperken. In deze gevallen [!DNL Workfront Fusion] moeten volledige toegangsrechten vereisen. Meer informatie over het beperken van [!DNL Workfront Fusion] toegang tot uw account die is geregistreerd voor deze services, raadpleegt u de toepassingsspecifieke documentatie die wordt vermeld in [Apps en modules daarvan](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

## Verbindingen beheren

U kunt alle verbindingen beheren via het dialoogvenster [!UICONTROL Connections] gebied.

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

1. Als u het dialoogvenster [!UICONTROL Connections] gebied, klikken <b>[!UICONTROL Connections]</b> in de linkernavigatie.
1. (Optioneel) Geef de omgeving en het type verbinding aan door te klikken op de vervolgkeuzelijst Omgeving en Type en een optie te selecteren.
1. (Optioneel) Bepalen aan welke machtigingen zijn verleend [!DNL Workfront Fusion] voor een verbinding, klik het pictogram van de Mening ![Verbindingsmachtigingen weergeven](assets/view-connection-permissions.png) voor die verbinding.
1. (Optioneel) Als u de naam van een verbinding wilt wijzigen, markeert u de naam van de verbinding en typt u de nieuwe naam.
1. (Optioneel) Als u een verbinding opnieuw wilt autoriseren, klikt u op **Opnieuw goedkeuren** voor die verbinding.
1. (Optioneel) Klik op **Verwijderen** voor die verbinding.
1. (Optioneel) Als u wilt controleren of de verbinding met de service tot stand is gebracht, klikt u op **Verifiëren** voor de verbinding.



## Een verbinding vernieuwen

[!DNL Workfront Fusion] verkrijgt gewoonlijk voor onbepaalde tijd toegangsrechten tot een bepaalde dienst. Sommige toepassingen vereisen de toegangstoestemming om na een bepaalde periode worden vernieuwd. In deze gevallen [!DNL Workfront Fusion] brengt u hiervan via e-mail op de hoogte kort voordat de toegangsrechten verlopen.

Een verbinding vernieuwen:

1. Klik op de knop **[!UICONTROL Reauthorize]** in de **[!UICONTROL Connections]** gebied.
