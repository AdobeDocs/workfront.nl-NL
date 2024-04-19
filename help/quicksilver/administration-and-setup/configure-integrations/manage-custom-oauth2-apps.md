---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Aangepaste OAuth2-toepassingen weergeven en beheren
description: Als Adobe Workfront-beheerder kunt u de OAuth2-toepassingen voor uw exemplaar van Workfront weergeven en beheren, waarmee andere toepassingen toegang hebben tot Workfront.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Aangepaste OAuth2-toepassingen weergeven en beheren

Als [!DNL Adobe Workfront] beheerder, kunt u de toepassingen OAuth2 voor uw geval van bekijken en beheren [!DNL Workfront], die andere toepassingen toegang geven tot [!UICONTROL Workfront].

>[!NOTE]
>
>* In de context van OAuth2, verwijst de &quot;toepassing Oauth2&quot;naar dit soort toegangsverbinding tussen een app en een server zoals [!DNL Workfront]. Zie voor meer informatie [OAuth2-toepassingen maken voor [!DNL Workfront] integratie](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>* U kunt tot een totaal van tien Toepassingen OAuth2 in één keer hebben.

* Voor informatie over het maken van aangepaste OAuth2-toepassingen raadpleegt u [OAuth2-toepassingen maken voor [!DNL Workfront] integratie](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* Voor instructies bij het vormen van en het gebruiken van de toepassing OAuth2 met gebruikersgeloofsbrieven (de stroom van de vergunningscode), zie [Vorm en gebruik de douane OAuth 2 van uw organisatie toepassingen gebruikend de stroom van de vergunningscode](../../wf-api/api/oauth-app-code-token-flow.md).
* Voor instructies over het vormen van en het gebruiken van de toepassing OAuth2 gebruikend serverauthentificatie (stroom JWT), zie [Configureer en gebruik de aangepaste OAuth 2-toepassingen van uw organisatie met behulp van JWT-flow](../../wf-api/api/oauth-app-jwt-flow.md).
* Voor instructies bij het vormen van en het gebruiken van de toepassing OAuth2 die PKCE gebruikt, zie [Configureer en gebruik de aangepaste OAuth 2-toepassingen van uw organisatie met PKCE-stroom](../../wf-api/api/oauth-app-pkce-flow.md).

## Toegangsvereisten

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
   <td> U moet een [!DNL Workfront] beheerder. </p>
    <p>Voor informatie over [!DNL Workfront] beheerders, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Vereisten

U moet [!UICONTROL OAuth2] toepassingen voor uw organisatie voordat u deze kunt weergeven of beheren.

Zie voor meer informatie [OAuth2-toepassingen maken voor [!DNL Workfront] integratie](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Aangepaste OAuth2-toepassingen beheren

* [Aangepaste OAuth2-toepassingen weergeven en bewerken](#view-and-edit-custom-oauth2-applications)
* [Aangepaste OAuth2-toepassingen verwijderen](#delete-custom-oauth2-applications)

### Aangepaste OAuth2-toepassingen weergeven en bewerken {#view-and-edit-custom-oauth2-applications}

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik in het linkernavigatievenster op **[!UICONTROL System]** selecteert u vervolgens **[!UICONTROL OAuth Applications]**.
1. Klik op **[!UICONTROL Create app integration]**.
1. Houd de muis boven de toepassing en klik op **[!UICONTROL Edit]** ![](assets/edit-icon.png) wanneer deze zich helemaal rechts bevindt.
1. (Optioneel) Bewerk de toepassingsdetails.

   Voor velden die betrekking hebben op OAuth2- en JWT-toepassingen, raadpleegt u [OAuth2-toepassingen maken voor [!DNL Workfront] integratie](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### Aangepaste OAuth2-toepassingen verwijderen {#delete-custom-oauth2-applications}

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik in het linkernavigatievenster op **[!UICONTROL System]** selecteert u vervolgens **[!UICONTROL OAuth Applications]**.
1. Klik op ** **.
1. Houd de muis boven de toepassing en klik op **[!UICONTROL Delete]** ![](assets/delete.png) wanneer deze zich helemaal rechts bevindt.

## Clientgeheimen beheren in OAuth2-toepassingen

* [Gegevens over clientgeheim weergeven](#view-client-secret-details)
* [Notities voor clientgeheim toevoegen of bewerken](#add-or-edit-notes-for-client-secret)
* [Clientgeheim verwijderen](#delete-client-secret)

### Gegevens over clientgeheim weergeven {#view-client-secret-details}

>[!IMPORTANT]
>
>U kunt het clientgeheim zelf niet weergeven. Als u uw Geheim van de Cliënt hebt verloren, moet u het schrappen en nieuwe creëren.
>
>* Als u een clientgeheim wilt verwijderen, raadpleegt u [Clientgeheim verwijderen](#delete-client-secret) in dit artikel.
>* Als u een nieuw clientgeheim wilt maken, raadpleegt u [Een OAuth2-toepassing maken](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) in [OAuth2-toepassingen maken voor [!DNL Workfront] integratie](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>



1. Klik op de knop *[!UICONTROL *Main Menu]**, pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik in het linkernavigatievenster op **[!UICONTROL System]** selecteert u vervolgens **[!UICONTROL OAuth Applications]**.
1. Houd de muis boven de toepassing en klik op de knop **[!UICONTROL Edit]** pictogram als deze helemaal rechts wordt weergegeven.
1. Details weergeven in het gebied Clientgeheim:

   * Aanmaakdatum
   * Laatst gebruikte datum
   * Notities

     Als u notities wilt toevoegen aan een clientgeheim, raadpleegt u [Notities voor clientgeheim toevoegen of bewerken](#add-or-edit-notes-for-client-secret).

### Notities voor clientgeheim toevoegen of bewerken {#add-or-edit-notes-for-client-secret}

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik in het linkernavigatievenster op **[!UICONTROL System]** selecteert u vervolgens **[!UICONTROL OAuth Applications]**.
1. Klik op **[!UICONTROL Create app integration]**.
1. Houd de muis boven de toepassing en klik op de knop **[!UICONTROL Edit]** pictogram als deze helemaal rechts wordt weergegeven.
1. Zoek het clientgeheim waarvoor u een notitie wilt toevoegen of bewerken.
1. Klik de doos die details voor het Geheim van de Cliënt bevat.

   U kunt nu notitietekst toevoegen of bestaande notitietekst bewerken.

   >[!NOTE]
   >
   >De tekst van de nota heeft een maximum van 64 karakters.

1. Klik buiten het vak of druk op **[!UICONTROL Enter]** de notitietekst opslaan.

### Clientgeheim verwijderen {#delete-client-secret}

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik in het linkernavigatievenster op **[!UICONTROL System]** selecteert u vervolgens **[!UICONTROL OAuth Applications]**.
1. Klik op **[!UICONTROL Create app integration]**.
1. Houd de muis boven de toepassing en klik op de knop **[!UICONTROL Edit]** pictogram als deze helemaal rechts wordt weergegeven.
1. Zoek het clientgeheim dat u wilt verwijderen.
1. Klik op de knop **[!UICONTROL Delete]** pictogram ![](assets/delete.png) naast Clientgeheim.
