---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: Configureren [!DNL Adobe Workfront] voor Slack
description: Integreren [!DNL Adobe Workfront] met Slack kunt u toegang krijgen tot [!DNL Workfront] arbeidsartikelen, goedkeuringen, favorieten, recente artikelen van Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 09b4644a63241fa9e0a213bfa6f1a7e4264a1703
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 1%

---

# Configureren [!DNL Adobe Workfront for Slack]

Integreren [!DNL Adobe Workfront] with [!DNL Slack] kunt u het volgende doen:

* Toegang tot uw [!DNL Workfront] Werkstukken, goedkeuringen, favorieten, recente artikelen van [!DNL Slack].
* Abonneren op, goedkeuren, werk toewijzen van [!DNL Slack].
* Taken en uitgaven maken van [!DNL Slack].
* Sommige ontvangen [!DNL Workfront] meldingen in [!DNL Slack].

Afhankelijk van hoe uw [!DNL Slack] omgeving is geconfigureerd, kunt u installeren en configureren [!DNL Workfront for Slack] of uw [!DNL Workfront] de beheerder moet het eerst installeren en vormen alvorens u het voor zich kunt vormen.

Wanneer u uw [!DNL Slack] instantie met [!DNL Workfront] gebruikers kunnen [!DNL Workfront] tijdens het samenwerken binnen hun [!DNL Slack] kanalen. De integratie kan vanaf elk [!DNL Slack] milieu, met inbegrip van [!DNL Slack] mobiele app.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] of hoger</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.\

## Vereisten voor het gebruik [!DNL Workfront] with [!DNL Slack]

* U moet beschikken over een [!DNL Slack] -instantie.
* Uw [!DNL Slack] de systeembeheerder moet allen toestaan [!DNL Slack] te installeren gebruikers [!DNL Workfront for Slack].
* U moet beschikken over een [!DNL Workfront] licentie om de geïntegreerde functies te kunnen gebruiken in [!DNL Workfront].

   >[!NOTE]
   >
   >Gebruikers met [!DNL Workfront] licentietype kan toegang krijgen [!DNL Workfront] van [!DNL Slack]. De handelingen die u kunt uitvoeren [!DNL Slack] zijn beperkt tot uw [!DNL Workfront] licentieniveaus en machtigingsniveaus.

Voor meer informatie over het beheren van apps in [!DNL Slack], zie [Toepassingen voor uw werkruimte beheren.](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## Installeren [!DNL Workfront for Slack]

Elk [!DNL Slack] gebruiker moet de [!DNL Workfront] zelf te gebruiken [!DNL Workfront] van [!DNL Slack].

U kunt de toepassing op de volgende manieren installeren:

* [Installeer de [!DNL Workfront] app buiten [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [Installeer de [!DNL Workfront] app binnen [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### Installeer de [!DNL Workfront] app buiten [!DNL Slack] {#install-the-workfront-app-outside-slack}

Voer de onderstaande stappen uit om het installatieproces uit te voeren en autorisatie uit te voeren [!DNL Workfront for Slack] op uw [!DNL Slack] -instantie.

>[!IMPORTANT]
>
>Wanneer een nieuwe versie van [!DNL Workfront] Als Slack wordt uitgebracht, moet u de app opnieuw autoriseren om deze te kunnen blijven gebruiken.

1. Zoek de [!DNL Adobe Workfront] toe:voegen-aan in [[!DNL Slack] winkel](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. Klik op **[!UICONTROL Open in [!DNL Slack]]**.

1. Meld u aan bij uw werkruimte door uw [!DNL Slack] URL en klikken **[!UICONTROL Continue]**.\
   ![Screen_Shot_2017-10-17_at_8.27.38_AM.png](assets/screen-shot-2017-10-17-at-8.27.38-am-350x432.png)

1. Onderzoek de toegang die [!DNL Slack] vraagt. Klik op **[!UICONTROL Allow Access]** om de [!DNL Workfront] app.

   ![](assets/integrations-access-screen-350x429.png)

U hebt nu toegang tot [!DNL Workfront] van [!DNL Slack], zoals beschreven in de [Toegang [!DNL Workfront] van [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] van [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

### Installeer de [!DNL Workfront] app binnen [!DNL Slack] {#install-the-workfront-app-within-slack}

U kunt de [!DNL Workfront] rechtstreeks vanuit de [!DNL Slack] toepassing:

1. Ga naar uw [!DNL Slack] URL.

   Bijvoorbeeld: *`<YourTeamName>`.slack.com/apps*.

   of

   Klik op de knop **[!UICONTROL Add Apps]** pictogram in uw [!DNL Slack] -instantie.

   ![add_apps_in_Slack.png](assets/add-apps-in-slack-350x112.png)

1. Begin met typen *[!DNL Workfront]* in het zoekveld.
1. Druk op Enter.
1. Selecteer **[!DNL Workfront]** app.
1. Klik op **[!UICONTROL Settings]**.

   De pagina App Directory wordt weergegeven.

1. Klik op **[!UICONTROL Visit App Site]**.
1. Klik op **[!UICONTROL Add to [!DNL Slack]]**.
1. Voer de stappen uit om de installatie te voltooien.
1. Wanneer de installatie is voltooid, hebt u toegang tot [!DNL Workfront] van [!DNL Slack], zoals beschreven in de [[!UICONTROL Access [!DNL Workfront] van [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] van [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).
