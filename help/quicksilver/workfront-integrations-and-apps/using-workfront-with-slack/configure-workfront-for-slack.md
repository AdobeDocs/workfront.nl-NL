---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: Vorm  [!DNL Adobe Workfront]  voor Slack
description: Het integreren  [!DNL Adobe Workfront]  met Slack staat u toe om  [!DNL Workfront]  het werkpunten, goedkeuringen, favorieten, recente punten van Slack toegang te hebben en tot stand te brengen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 1%

---

# Configureren [!DNL Adobe Workfront for Slack]

Door [!DNL Adobe Workfront] te integreren met [!DNL Slack] kunt u het volgende doen:

* Open [!DNL Workfront] -werkitems, goedkeuringen, favorieten en recente items van [!DNL Slack] .
* Abonneren op, goedkeuren, werk toewijzen vanuit [!DNL Slack] .
* Maak taken en problemen vanuit [!DNL Slack] .
* Ontvang enkele [!DNL Workfront] -meldingen in [!DNL Slack] .

Afhankelijk van de configuratie van uw [!DNL Slack] -omgeving kunt u [!DNL Workfront for Slack] zelf installeren en configureren. Uw [!DNL Workfront] -beheerder moet deze eerst installeren en configureren voordat u deze voor uzelf kunt configureren.

Wanneer u de [!DNL Slack] -instantie integreert met [!DNL Workfront] kunnen gebruikers [!DNL Workfront] gebruiken terwijl ze samenwerken binnen hun [!DNL Slack] -kanalen. De integratie kan vanuit elke [!DNL Slack] -omgeving worden gebruikt, inclusief de mobiele app van [!DNL Slack] . ## Toegangsvereisten

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
   <td> <p>Alle</p>
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten voor het gebruik van [!DNL Workfront] met [!DNL Slack]

* U moet een [!DNL Slack] -instantie hebben.
* Uw [!DNL Slack] -systeembeheerder moet alle [!DNL Slack] -gebruikers toestaan [!DNL Workfront for Slack] te installeren.
* U moet een [!DNL Workfront] -licentie hebben om de geïntegreerde functies in [!DNL Workfront] te kunnen gebruiken.

  >[!NOTE]
  >
  >Gebruikers met een [!DNL Workfront] -licentietype hebben toegang tot [!DNL Workfront] vanuit [!DNL Slack] . De acties die u kunt uitvoeren vanuit [!DNL Slack] zijn beperkt tot uw licentie- en machtigingsniveaus voor [!DNL Workfront] .

Voor meer informatie over het beheren van apps in [!DNL Slack], zie [&#x200B; Toepassingen voor Uw Workspace beheren.](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## Installeren [!DNL Workfront for Slack]

Elke [!DNL Slack] -gebruiker moet de [!DNL Workfront] -app zelf installeren om [!DNL Workfront] van [!DNL Slack] te kunnen gebruiken.

U kunt de toepassing op de volgende manieren installeren:

* [Installeer buiten  [!DNL Workfront]  app  [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [Installeer  [!DNL Workfront]  app binnen  [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### Installeer de [!DNL Workfront] -toepassing buiten [!DNL Slack] {#install-the-workfront-app-outside-slack}

Voer de onderstaande stappen uit om het installatieproces uit te voeren en [!DNL Workfront for Slack] te autoriseren voor uw [!DNL Slack] -instantie.

>[!IMPORTANT]
>
>Wanneer een nieuwe versie van [!DNL Workfront] voor Slack wordt uitgebracht, moet u de app opnieuw autoriseren om deze te kunnen blijven gebruiken.

1. Bepaal de plaats van [!DNL Adobe Workfront] toe:voegen-op in de [[!DNL Slack]  opslag &#x200B;](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. Klik op **[!UICONTROL Open in [!DNL Slack]]**.

1. Meld u aan bij de werkruimte door de [!DNL Slack] URL op te geven en op **[!UICONTROL Continue]** te klikken.\

1. Onderzoek de toegang die [!DNL Slack] aanvraagt. Als u akkoord gaat met deze toegang, klikt u op **[!UICONTROL Allow Access]** om de [!DNL Workfront] -app te autoriseren.

U kunt tot [!DNL Workfront] van [!DNL Slack] nu toegang hebben, zoals die in [&#x200B; wordt beschreven Toegang  [!DNL Workfront]  van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront]  van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

### De [!DNL Workfront] -toepassing installeren in [!DNL Slack] {#install-the-workfront-app-within-slack}

U kunt de toepassing [!DNL Workfront] rechtstreeks vanuit de toepassing [!DNL Slack] installeren:

1. Navigeer naar uw [!DNL Slack] URL.

   Bijvoorbeeld: *`<YourTeamName>`.slack.com/apps*.

   of

   Klik op het pictogram **[!UICONTROL Add Apps]** in de [!DNL Slack] -instantie.

1. Typ *[!DNL Workfront]* in het zoekveld.
1. Druk op Enter.
1. Selecteer de app **[!DNL Workfront]** .
1. Klik op **[!UICONTROL Settings]**.

   De pagina App Directory wordt weergegeven.

1. Klik op **[!UICONTROL Visit App Site]**.
1. Klik op **[!UICONTROL Add to [!DNL Slack]]**.
1. Voer de stappen uit om de installatie te voltooien.
1. Wanneer de installatie voltooit, kunt u tot [!DNL Workfront] van [!DNL Slack] toegang hebben, zoals die in [[!UICONTROL Access [!DNL Workfront] van  [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront]  van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) wordt beschreven.
