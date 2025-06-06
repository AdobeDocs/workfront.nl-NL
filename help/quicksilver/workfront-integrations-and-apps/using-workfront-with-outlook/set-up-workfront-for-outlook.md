---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Opstelling  [!DNL Adobe Workfront]  voor  [!DNL Outlook]
description: ' [!DNL Adobe Workfront] [!DNL Outlook] toe:voegen-binnen laat u de zeer belangrijke  [!DNL Workfront]  taken van Vooruitzichten direct uitvoeren.'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Instellen [!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

>[!IMPORTANT]
>
>[ Microsoft is in het proces om steun voor de online tokens van de erfenisUitwisseling ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) onbruikbaar te maken, die momenteel door de toe:voegen-binnen van Workfront Vooruitzichten voor authentificatie worden gebruikt. Deze verandering door Microsoft is al begonnen met gevolgen voor de klanten en zal tot oktober 2025 in fasen blijven doorlopen.
>
>* **nadat Microsoft volledig deze tokens onbruikbaar maakt, zal Workfront voor de integratie van Microsoft Outlook niet meer functioneren.**
>
>Als onderdeel van deze wijziging heeft Microsoft besloten om de manier te wijzigen waarop tokens opnieuw worden ingeschakeld. Na **Juni 30, 2025**, zullen de beheerders niet meer tokens kunnen re-toelaten zelf-slechts de Steun van Microsoft kan uitzonderingen verlenen. **Op 1 Oktober, 2025, zullen de erfenistokens voor alle huurders worden uitgezet. Er worden geen uitzonderingen toegestaan.**

Met de [!DNL Adobe Workfront] [!DNL Outlook] add-in kunt u de volgende belangrijke [!DNL Workfront] taken rechtstreeks vanuit Outlook uitvoeren:

* Werk een bestaand project, een bestaande taak of een bestaand probleem bij met informatie uit een e-mail. Voor meer informatie, zie [ een bestaand voorwerp van a  [!DNL Outlook]  e-mail ](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md) bijwerken.
* Maak een [!DNL Workfront] -aanvraag op basis van een e-mail in [!DNL Outlook] . Voor meer informatie, zie [ een verzoek van Adobe Workfront van a  [!DNL Outlook]  e-mail ](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md) creëren.
* Voeg een e-mail als taak toe in uw [!UICONTROL My Work] gebied. Voor meer informatie, zie [ een  [!DNL Outlook]  e-mail als taak aan uw het werklijst ](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md) toevoegen.
* Reageer op opmerkingen via de [!DNL Workfront] add-in voor [!DNL Outlook] . Voor informatie over het antwoorden op commentaren van Workfront voor [!DNL Outlook], zie [ Reageren op een commentaar van  [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* Maak nieuwe taken en uitgaven of maak deze op basis van bestaande e-mails (gebruik van de functie slepen en neerzetten). Voor meer informatie, zie [ een  [!DNL Outlook]  e-mail aan een project als taak of een kwestie ](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md) toevoegen.

U moet de [!DNL Workfront] add-in toevoegen aan uw [!DNL Outlook] -account voordat u [!DNL Workfront for Outlook] kunt gebruiken.

Als u de [!DNL Workfront] add-in niet kunt installeren met uw [!DNL Outlook] -account, neemt u contact op met de [!DNL Workfront] -beheerder om ervoor te zorgen dat [!DNL Outlook] add-ins zijn ingeschakeld voor uw organisatie.

Voor informatie over hoe te om de [!DNL Outlook] integratie voor uw organisatie toe te laten, zie [ toelaten  [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

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

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Uw [!DNL Workfront] beheerder moet [!DNL Outlook for Office] with [!DNL Workfront] inschakelen voordat u deze integratie kunt gebruiken.

## Systeemvereisten

De volgende toepassingen zijn beschikbaar:

* **[!DNL Outlook]op het web:** De [!DNL Workfront] invoegtoepassing is beschikbaar wanneer u [!DNL Outlook] gebruikt vanuit een webbrowser op een desktopcomputer of een mobiel apparaat. Deze functionaliteit is ook beschikbaar wanneer u de [!DNL Outlook] Web App gebruikt.
* **[!DNL Outlook]Bureaubladtoepassing:** De [!DNL Workfront] invoegtoepassing is beschikbaar wanneer u de [!DNL Windows] - en [!DNL Mac] desktopversies van [!DNL Outlook] gebruikt die bij het [!DNL Office] -pakket zijn geleverd.

De [!DNL Workfront] add-in voor [!DNL Outlook] wordt ondersteund in omgevingen die aan de volgende vereisten voldoen:

* [Clientvereisten](#client-requirements-client-requirements)
* [Vereisten voor mailservers](#mail-server-requirements-mail-server-requirements)

### Clientvereisten {#client-requirements}

Workfront ondersteunt de volgende versies van [!DNL Outlook] :

* [!DNL Outlook 2013] of hoger op [!DNL Windows]
* [!DNL Outlook 2016] of hoger op [!DNL Windows]
* [!DNL Outlook] on [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] on [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] op het web

U moet verbinding hebben met een [!DNL Exchange Server] - of [!DNL Office 365] -verbinding via een directe verbinding.

Bij het configureren van de client moet de gebruiker een van de volgende accounttypen selecteren:

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com] Als de client is geconfigureerd voor verbinding met POP3 of IMAP, wordt de [!DNL Workfront] -invoegtoepassing niet geladen.

### Vereisten voor mailservers {#mail-server-requirements}

Aan de vereisten voor de mailserver wordt standaard voldaan wanneer u verbinding maakt met [!DNL Office 365] of [!DNL Outlook.com] . Als u echter verbinding hebt met een on-premise installatie van [!DNL Exchange Server] , gelden de volgende vereisten:

* Workfront ondersteunt alle [!DNL Exchange On-Premise] -servers
* [!DNL Exchange Web Services] (EWS) moet zijn ingeschakeld en beschikbaar zijn via internet.
* De server moet een geldig verificatiecertificaat hebben voordat de server geldige id-tokens kan uitgeven. Nieuwe installaties van [!DNL Exchange Server] bevatten een standaardverificatiecertificaat.

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* Om tot [!DNL Workfront] toe:voegen-binnen van de [[!DNL Office]  Opslag ](https://store.office.com/) toegang te hebben, moeten uw servers van de cliënttoegang met [ https://store.office.com ](https://store.office.com/) kunnen communiceren.

Voor meer gedetailleerde informatie over gesteunde milieu&#39;s, zie de [[!DNL Microsoft Office 365]  homepage ](https://products.office.com/en-us/office-365-home).

## De invoegtoepassing installeren

U kunt Workfront toe:voegen-binnen voor Vooruitzichten van de [ opslag van Microsoft ](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview) krijgen.

### [!DNL Workfront] for [!DNL Outlook 365] {#workfront-for-outlook-365}

1. In [!DNL Outlook 365], klik het **[!UICONTROL Browse Add-ins]** pictogram ![ doorbladert toe:voegen-ins ](assets/outlook-add-in-26x26.png) bij de bovenkant van de interface van Bureau 365, dan klik **[!UICONTROL Manage add-ins]**.

1. Zoek in het vak **[!UICONTROL Search add-ins]** naar **[!DNL Workfront]** en druk op [!UICONTROL Enter] .

1. Klik op **[!UICONTROL Add]**.

### [!DNL Workfront] for [!DNL Outlook] on the Web {#workfront-for-outlook-on-the-web}

1. Open [!DNL Microsoft Outlook] in een webbrowser.
1. Klik **[!UICONTROL Browse]toe:voegen-ins** pictogram ![ doorbladeren toe:voegen-ins ](assets/outlook-add-in-web-version-20x20.png).

   Om van het pictogram de plaats te bepalen, zie [ Gebruikend toe:voegen-ins in  [!DNL Outlook]  op het Web ](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) in de documentatie van Microsoft.

1. Zoek naar **[!DNL Workfront]** in het **[!UICONTROL Search add-ins]** gebied, dan druk **[!UICONTROL Enter]**.

1. Wanneer het op de lijst verschijnt, voegt de klik **** toe.

### [!DNL Workfront for Outlook] on [!UICONTROL Windows] of [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. Klik op **[!UICONTROL Home]** > **[!UICONTROL Store]** op het lint.

1. Zoek naar **[!DNL Workfront]** in het **[!UICONTROL Search]** gebied, dan druk **[!UICONTROL Enter]**.

1. Klik op de schakeloptie om **[!UICONTROL [!DNL Workfront] add-in]** in te schakelen.

## Aanmelden bij [!DNL Workfront] vanuit [!DNL Outlook]

1. Selecteer in [!DNL Outlook] een e-mailbericht en klik vervolgens op het pictogram **[!DNL Workfront]** in de e-mailkop.
1. Voor de login pagina, klik **Login aan Workfront**.
1. Volg de aanwijzingen om u aan te melden bij [!DNL Workfront] met OAuth 2.0. <!--Enhanced Authentication or your Security Assertion Markup Language (SAML) URL.-->

   <!--Before users can log in to the [!DNL Workfront] add-in using SAML, a [!DNL Workfront] administrator must first enable [!DNL Office 365] add-ins to authenticate using a SAML 2.0 solution. For more information, see the section [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) in the article [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).-->

   >[!NOTE]
   >
   >* Als u wordt ertoe aangezet om het domein van uw [!DNL Workfront] rekening in te gaan, typ het gebruikend dit formaat: *yourCompany&#39;sDomain.my.workfront.com*. Het domein van uw bedrijf is gewoonlijk de naam van uw bedrijf.

<!--ADDITIONAL BULLET REMOVED FROM NOTE BOX: Enhanced Authentication is not available until a Workfront administrator enables it for this integration.-->
