---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Aangepaste OAuth2-toepassingen weergeven en beheren
description: Als Adobe Workfront-beheerder kunt u de OAuth2-toepassingen voor uw exemplaar van Workfront weergeven en beheren, waarmee andere toepassingen toegang hebben tot Workfront.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Becky
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---

# Aangepaste OAuth2-toepassingen weergeven en beheren

Als [!DNL Adobe Workfront] beheerder kunt u de OAuth2-toepassingen voor uw instantie van [!DNL Workfront] weergeven en beheren, waarmee andere toepassingen toegang hebben tot [!UICONTROL Workfront] .

>[!NOTE]
>
>* In de context van OAuth2, verwijst de &quot;toepassing Oauth2&quot;naar dit soort toegangsverbinding tussen een app en een server zoals [!DNL Workfront]. Voor meer informatie, zie [ toepassingen OAuth2 voor  [!DNL Workfront]  integraties ](../../administration-and-setup/configure-integrations/create-oauth-application.md) creëren
>* U kunt tot een totaal van tien Toepassingen OAuth2 in één keer hebben.

* Voor informatie bij het creëren van douaneOAuth2 toepassingen, zie [ toepassingen OAuth2 voor  [!DNL Workfront]  integraties ](../../administration-and-setup/configure-integrations/create-oauth-application.md) creëren
* Voor instructies bij het vormen van en het gebruiken van de toepassing OAuth2 met gebruikersgeloofsbrieven (de stroom van de vergunningscode), zie [ vormen en gebruiken de douane OAuth 2 van uw organisatie toepassingen gebruikend de stroom van de vergunningscode ](../../wf-api/api/oauth-app-code-token-flow.md).
* Voor instructies bij het vormen van en het gebruiken van de toepassing OAuth2 die serverauthentificatie (stroom JWT) gebruiken, zie [ vormen en gebruiken de douane OAuth 2 van uw organisatie toepassingen gebruikend stroom JWT ](../../wf-api/api/oauth-app-jwt-flow.md).
* Voor instructies bij het vormen van en het gebruiken van de toepassing OAuth2 die PKCE gebruiken, zie [ vorm en gebruik de douane OAuth 2 van uw organisatie toepassingen gebruikend de stroom van PKCE ](../../wf-api/api/oauth-app-pkce-flow.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Plan] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> U moet een [!DNL Workfront] beheerder zijn. </p>
    <p>Voor informatie over [!DNL Workfront] beheerders, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> een gebruiker volledige administratieve toegang verlenen </a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

+++

## Vereisten

U moet [!UICONTROL OAuth2] -toepassingen voor uw organisatie maken voordat u deze kunt weergeven of beheren.

Voor meer informatie, zie [ toepassingen OAuth2 voor  [!DNL Workfront]  integraties ](../../administration-and-setup/configure-integrations/create-oauth-application.md) creëren

## Aangepaste OAuth2-toepassingen beheren

* [Aangepaste OAuth2-toepassingen weergeven en bewerken](#view-and-edit-custom-oauth2-applications)
* [Aangepaste OAuth2-toepassingen verwijderen](#delete-custom-oauth2-applications)

### Aangepaste OAuth2-toepassingen weergeven en bewerken {#view-and-edit-custom-oauth2-applications}

{{step-1-to-setup}}

1. Klik in het navigatievenster aan de linkerkant op **[!UICONTROL System]** en selecteer vervolgens **[!UICONTROL OAuth Applications]** .
1. Klik op **[!UICONTROL Create app integration]**.
1. Houd de muis boven de toepassing en klik op **[!UICONTROL Edit]** ![](assets/edit-icon.png) wanneer deze helemaal rechts wordt weergegeven.
1. (Optioneel) Bewerk de toepassingsdetails.

   Voor gebieden met betrekking tot OAuth2 en JWT apps, zie [ toepassingen OAuth2 voor  [!DNL Workfront]  integraties ](../../administration-and-setup/configure-integrations/create-oauth-application.md) creëren.

### Aangepaste OAuth2-toepassingen verwijderen {#delete-custom-oauth2-applications}

{{step-1-to-setup}}

1. Klik in het navigatievenster aan de linkerkant op **[!UICONTROL System]** en selecteer vervolgens **[!UICONTROL OAuth Applications]** .
1. Klik op ** **.
1. Houd de muis boven de toepassing en klik op **[!UICONTROL Delete]** ![](assets/delete.png) wanneer deze helemaal rechts wordt weergegeven.

## Clientgeheimen beheren in OAuth2-toepassingen

* [Gegevens over clientgeheim weergeven](#view-client-secret-details)
* [Notities voor clientgeheim toevoegen of bewerken](#add-or-edit-notes-for-client-secret)
* [Clientgeheim verwijderen](#delete-client-secret)

### Gegevens over clientgeheim weergeven {#view-client-secret-details}

>[!IMPORTANT]
>
>U kunt het clientgeheim zelf niet weergeven. Als u uw Geheim van de Cliënt hebt verloren, moet u het schrappen en nieuwe creëren.
>
>* Om een Geheim van de Cliënt te schrappen, zie [ Geheim van de Cliënt van de Schrapping ](#delete-client-secret) in dit artikel.
>* Om een nieuw Geheim van de Cliënt tot stand te brengen, zie [ een toepassing OAuth2 ](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) in [ creëren toepassingen OAuth2 voor  [!DNL Workfront]  integraties ](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>

{{step-1-to-setup}}

1. Klik in het navigatievenster aan de linkerkant op **[!UICONTROL System]** en selecteer vervolgens **[!UICONTROL OAuth Applications]** .
1. Houd de muisaanwijzer boven de toepassing en klik op het pictogram **[!UICONTROL Edit]** wanneer deze helemaal rechts wordt weergegeven.
1. Details weergeven in het gebied Clientgeheim:

   * Aanmaakdatum
   * Laatst gebruikte datum
   * Notities

     Om nota&#39;s aan een Geheim van de Cliënt toe te voegen, zie [ nota&#39;s voor Geheim van de Cliënt ](#add-or-edit-notes-for-client-secret) toevoegen of uitgeven.

### Notities voor clientgeheim toevoegen of bewerken {#add-or-edit-notes-for-client-secret}

{{step-1-to-setup}}

1. Klik in het navigatievenster aan de linkerkant op **[!UICONTROL System]** en selecteer vervolgens **[!UICONTROL OAuth Applications]** .
1. Klik op **[!UICONTROL Create app integration]**.
1. Houd de muisaanwijzer boven de toepassing en klik op het pictogram **[!UICONTROL Edit]** wanneer deze helemaal rechts wordt weergegeven.
1. Zoek het clientgeheim waarvoor u een notitie wilt toevoegen of bewerken.
1. Klik de doos die details voor het Geheim van de Cliënt bevat.

   U kunt nu notitietekst toevoegen of bestaande notitietekst bewerken.

   >[!NOTE]
   >
   >De tekst van de nota heeft een maximum van 64 karakters.

1. Klik uit het vakje of druk **[!UICONTROL Enter]** om de notitietekst te bewaren.

### Clientgeheim verwijderen {#delete-client-secret}

{{step-1-to-setup}}

1. Klik in het navigatievenster aan de linkerkant op **[!UICONTROL System]** en selecteer vervolgens **[!UICONTROL OAuth Applications]** .
1. Klik op **[!UICONTROL Create app integration]**.
1. Houd de muisaanwijzer boven de toepassing en klik op het pictogram **[!UICONTROL Edit]** wanneer deze helemaal rechts wordt weergegeven.
1. Zoek het clientgeheim dat u wilt verwijderen.
1. Klik op het pictogram **[!UICONTROL Delete]** ![](assets/delete.png) naast Client Secret.
