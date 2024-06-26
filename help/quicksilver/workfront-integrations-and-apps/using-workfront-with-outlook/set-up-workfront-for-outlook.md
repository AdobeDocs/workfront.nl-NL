---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Instellen [!DNL Adobe Workfront] for [!DNL Outlook]
description: De [!DNL Adobe Workfront] [!DNL Outlook] met invoegtoepassing kunt u de toets uitvoeren [!DNL Workfront] taken rechtstreeks vanuit Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: 4cab7bed6cb4c25d96e70ccce2ece7f6d156f435
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 0%

---

# Instellen [!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

De [!DNL Adobe Workfront] [!DNL Outlook] Met invoegtoepassing kunt u de volgende toets uitvoeren [!DNL Workfront] taken rechtstreeks vanuit Outlook:

* Werk een bestaand project, een bestaande taak of een bestaand probleem bij met informatie uit een e-mail. Zie voor meer informatie [Een bestaand object bijwerken vanuit een [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* Een [!DNL Workfront] aanvraag gebaseerd op een e-mailbericht binnen [!DNL Outlook]. Zie voor meer informatie [Een Adobe Workfront-aanvraag maken van een [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* Voeg een e-mail als taak in uw [!UICONTROL My Work] gebied. Zie voor meer informatie [Een [!DNL Outlook] e-mailen als een taak naar uw werklijst](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* Reageren op opmerkingen via de [!DNL Workfront] invoegtoepassing voor [!DNL Outlook]. Voor informatie over het beantwoorden van opmerkingen van Workfront voor [!DNL Outlook], zie [Reageren op een opmerking van [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* Maak nieuwe taken en uitgaven of maak deze op basis van bestaande e-mails (gebruik van de functie slepen en neerzetten). Zie voor meer informatie [Een [!DNL Outlook] e-mailen naar een project als taak of probleem](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

U moet de opdracht [!DNL Workfront] invoegtoepassing in uw [!DNL Outlook] account voordat u kunt gebruiken [!DNL Workfront for Outlook].

Als u de [!DNL Workfront] add-in met uw [!DNL Outlook] account, neem contact op met uw [!DNL Workfront] beheerder om ervoor te zorgen dat [!DNL Outlook] add-ins worden ingeschakeld voor uw organisatie.

Voor informatie over hoe u de [!DNL Outlook] integratie voor uw organisatie, zie [Inschakelen [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> 
   <p>Nieuw plan: [!UICONTROL Standard]</p> 
   <p>Huidig plan:[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Uw [!DNL Workfront] beheerder moet inschakelen [!DNL Outlook for Office] with [!DNL Workfront] voordat u deze integratie kunt gebruiken.

## Systeemvereisten

De volgende toepassingen zijn beschikbaar:

* **[!DNL Outlook]op het web:** De [!DNL Workfront] invoegtoepassing is beschikbaar bij gebruik [!DNL Outlook] vanuit een webbrowser op een desktopcomputer of mobiel apparaat. Deze functionaliteit is ook beschikbaar wanneer u de [!DNL Outlook] Web App.
* **[!DNL Outlook]Bureaubladtoepassing:** De [!DNL Workfront] invoegtoepassing is beschikbaar wanneer u de [!DNL Windows] en [!DNL Mac] desktopversies van [!DNL Outlook] opgenomen in de [!DNL Office] pakket.

De [!DNL Workfront] invoegtoepassing voor [!DNL Outlook] wordt ondersteund in omgevingen die aan de volgende vereisten voldoen:

* [Clientvereisten](#client-requirements-client-requirements)
* [Vereisten voor mailservers](#mail-server-requirements-mail-server-requirements)

### Clientvereisten {#client-requirements}

Workfront ondersteunt de volgende versies van [!DNL Outlook]:

* [!DNL Outlook 2013] of hoger [!DNL Windows]
*[!DNL  Outlook 2016] of hoger [!DNL Windows]
* [!DNL Outlook] op [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] op [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] op het web

U moet verbinding hebben met een [!DNL Exchange Server] of [!DNL Office 365] via een directe verbinding.

Bij het configureren van de client moet de gebruiker een van de volgende accounttypen selecteren:

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]&#x200B;**&#x200B;**&#x200B; Als de client is geconfigureerd voor verbinding met POP3 of IMAP, wordt de [!DNL Workfront] add-in wordt niet geladen.

### Vereisten voor mailservers {#mail-server-requirements}

Standaard wordt aan de vereisten van de mailserver voldaan wanneer u verbinding maakt met [!DNL Office 365] of [!DNL Outlook.com]. Als u echter verbinding hebt met een on-premise installatie van [!DNL Exchange Server]zijn de volgende voorschriften van toepassing:

* Workfront ondersteunt alle [!DNL Exchange On-Premise] servers
* [!DNL Exchange Web Services] (EWS) moet zijn ingeschakeld en moet beschikbaar zijn op internet.
* De server moet een geldig verificatiecertificaat hebben voordat de server geldige id-tokens kan uitgeven. Nieuwe installaties van [!DNL Exchange Server] een standaardcertificaat voor verificatie opnemen.

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* Voor toegang tot [!DNL Workfront] toe:voegen-binnen van [[!DNL Office] Winkel](https://store.office.com/), moeten uw servers van de cliënttoegang met kunnen communiceren  [https://store.office.com](https://store.office.com/).

Voor meer gedetailleerde informatie over ondersteunde omgevingen raadpleegt u de [[!DNL Microsoft Office 365] homepage](https://products.office.com/en-us/office-365-home).

## De invoegtoepassing installeren

U kunt de Workfront add-in voor Outlook ophalen vanuit de [Microsoft-winkel](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview).

### [!DNL Workfront] for [!DNL Outlook 365] {#workfront-for-outlook-365}

1. In [!DNL Outlook 365]klikt u op de knop **[!UICONTROL Browse Add-ins]** pictogram ![](assets/outlook-add-in-26x26.png)boven aan de interface van Office 365 klikt u op **[!UICONTROL Manage add-ins]**.

1. In de **[!UICONTROL Search add-ins]** vak, zoeken naar **[!DNL Workfront]** dan drukken [!UICONTROL Enter].

1. Klik op **[!UICONTROL Add]**.

### [!DNL Workfront] for [!DNL Outlook] op het web {#workfront-for-outlook-on-the-web}

1. Openen [!DNL Microsoft Outlook] in een webbrowser.
1. Klik op de knop **[!UICONTROL Browse]add-ins** pictogram ![](assets/outlook-add-in-web-version-20x20.png).

   Ga naar [Invoegtoepassingen gebruiken [!DNL Outlook] op het web](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) in de documentatie van Microsoft.

1. Zoeken naar **[!DNL Workfront]** in de **[!UICONTROL Search add-ins]** veld, druk vervolgens op **[!UICONTROL Enter]**.

1. Wanneer het in de lijst wordt weergegeven, klikt u op **Toevoegen**.

### [!DNL Workfront for Outlook] op [!UICONTROL Windows] of [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. Klikken **[!UICONTROL Home]** > **[!UICONTROL Store]** op het lint.

1. Zoeken naar **[!DNL Workfront]** in de **[!UICONTROL Search]** veld, druk vervolgens op **[!UICONTROL Enter]**.

1. Klik op de schakeloptie om de optie **[!UICONTROL [!DNL Workfront] add-in]**.

## Aanmelden bij [!DNL Workfront] van [!DNL Outlook]

1. In [!DNL Outlook]selecteert u een e-mailbericht en klikt u op de knop **[!DNL Workfront]** in de koptekst van de e-mail.
1. Volg de aanwijzingen voor aanmelden [!DNL Workfront] het gebruiken van Verbeterde Authentificatie, OAuth 2.0, of uw Taal van de Prijsverhoging van de Veiligheid (SAML) URL.

   Voordat gebruikers zich kunnen aanmelden bij de [!DNL Workfront] add-in met gebruik van SAML, a [!DNL Workfront] de beheerder moet eerst toelaten [!DNL Office 365] toe:voegen-ins om voor authentiek te verklaren gebruikend een oplossing SAML 2.0. Zie de sectie voor meer informatie [Configureren [!DNL Adobe Workfront] met SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) in het artikel [Configureren [!DNL Adobe Workfront] met SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

   >[!NOTE]
   >
   >* Wanneer u wordt gevraagd het domein van uw [!DNL Workfront] -account, typt u deze notatie: *yourCompany&#39;sDomain.my.workfront.com*. Het domein van uw bedrijf is gewoonlijk de naam van uw bedrijf.
   >* Verbeterde verificatie is pas beschikbaar na een [!DNL Workfront] de beheerder laat het voor deze integratie toe.

