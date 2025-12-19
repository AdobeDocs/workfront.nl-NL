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
source-git-commit: 31e5f5e039e25fa25f3038c23ee579ba1f830bb7
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Aangepaste OAuth2-toepassingen weergeven en beheren

Als [!DNL Adobe Workfront] beheerder kunt u de OAuth2-toepassingen voor uw instantie van [!DNL Workfront] weergeven en beheren, waarmee andere toepassingen toegang hebben tot [!UICONTROL Workfront] .

>[!NOTE]
>
>* In de context van OAuth2, verwijst de &quot;toepassing Oauth2&quot;naar dit soort toegangsverbinding tussen een app en een server zoals [!DNL Workfront]. Voor meer informatie, zie [ toepassingen OAuth2 voor  [!DNL Workfront]  integraties ](../../administration-and-setup/configure-integrations/create-oauth-application.md) creëren
>* U kunt tot een totaal van tien Toepassingen OAuth2 in één keer hebben.

* Voor informatie, instructies, en details voor het creëren van douaneOAuth2 toepassingen, zie [ toepassingen OAuth2 voor  [!DNL Workfront]  integraties ](../../administration-and-setup/configure-integrations/create-oauth-application.md) creëren
* Voor informatie, instructies, en details voor het vormen van en het gebruiken van de toepassing OAuth2 met gebruikersgeloofsbrieven (de stroom van de vergunningscode), zie [ vormen en gebruiken de douane OAuth 2 van uw organisatie toepassingen gebruikend de stroom van de vergunningscode ](../../wf-api/api/oauth-app-code-token-flow.md).
* Voor informatie, zien de instructies, en de details voor het vormen en het gebruiken van de toepassing OAuth2 gebruikend serverauthentificatie (stroom JWT), [ de douaneOAuth 2 van uw organisatie toepassingen vormen en gebruiken gebruikend stroom JWT ](../../wf-api/api/oauth-app-jwt-flow.md).
* Voor instructies bij het vormen van en het gebruiken van de toepassing OAuth2 die PKCE gebruiken, zie [ vorm en gebruik de douane OAuth 2 van uw organisatie toepassingen gebruikend de stroom van PKCE ](../../wf-api/api/oauth-app-pkce-flow.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>U moet een Workfront-beheerder zijn. </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
1. Beweeg over de toepassing en klik **[!UICONTROL Edit]** ![ uitgeven pictogram ](assets/edit-icon.png) wanneer het op uiterst rechts verschijnt.
1. (Optioneel) Bewerk de toepassingsdetails.

   Voor gebieden met betrekking tot OAuth2 en JWT apps, zie [ toepassingen OAuth2 voor  [!DNL Workfront]  integraties ](../../administration-and-setup/configure-integrations/create-oauth-application.md) creëren.

### Aangepaste OAuth2-toepassingen verwijderen {#delete-custom-oauth2-applications}

{{step-1-to-setup}}

1. Klik in het navigatievenster aan de linkerkant op **[!UICONTROL System]** en selecteer vervolgens **[!UICONTROL OAuth Applications]** .
1. Beweeg over de toepassing en klik **[!UICONTROL Delete]** ![ Schrapping ](assets/delete.png) wanneer het op uiterst rechts verschijnt.

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
1. Klik het **[!UICONTROL Delete]** pictogram ![ Schrapping ](assets/delete.png) naast het Geheim van de Cliënt.
