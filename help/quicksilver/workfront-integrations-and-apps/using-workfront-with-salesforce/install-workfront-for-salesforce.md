---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Installeren [!DNL Adobe Workfront] for [!DNL Salesforce]
description: De toepassing installeren voordat deze beschikbaar wordt in het dialoogvenster [!DNL Salesforce] AppExchange, zie Installeren [!DNL Workfront] voor Salesforce voordat het beschikbaar wordt in de AppExchange Marketplace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: e823589247a2231e038142ae8d19f366769060e2
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 1%

---

# Installeren [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 1/2024 -->

>[!NOTE]
>
>De toepassing installeren voordat deze beschikbaar wordt in het dialoogvenster [!DNL Salesforce AppExchange], zie [Installeren [!DNL Workfront for Salesforce] voordat het beschikbaar wordt in het dialoogvenster [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

Als [!DNL Salesforce] en [!DNL Adobe Workfront] beheerder, kunt u installeren [!DNL Workfront for Salesforce] om uw [!DNL Salesforce] gebruikers om te verzenden [!DNL Workfront] verzoeken en maken automatisch projecten zonder ooit Salesforce te verlaten.

Voor een algemeen begrip van wat u kunt verwachten door te installeren [!DNL Workfront for Salesforce], zie [[!DNL Adobe Workfront for Salesforce] overzicht](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [Vereisten voor installatie en gebruik [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [Installeren [!DNL Workfront for Salesforce]](#installing-workfrontfor-salesforce)

## Toegangsvereisten

U moet de volgende toegang hebben om de in dit artikel beschreven functionaliteit te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alle</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> <p>Nieuw: [!UICONTROL Standard]</p><p>of</p><p>Huidige: [!UICONTROL Plan]</p> </td> 
  </tr>  </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten voor installatie en gebruik [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* U moet een [!DNL Salesforce] instantie met toegang tot een systeembeheerdersaccount om de app te installeren.
* U moet een [!DNL Workfront] instantie met toegang tot een rekening van de systeembeheerder om de integratie te vormen.
* [!UICONTROL Salesforce] gebruikers moeten een [!DNL Workfront] rekening om:

   * Maken [!DNL Workfront] verzoeken van [!DNL Salesforce]
   * Weergave [!DNL Workfront] verzoeken of projecten in Salesforce

## Installeren [!DNL Workfront for Salesforce] {#installing-workfront-for-salesforce}

U moet een [!DNL Salesforce] en [!DNL Workfront] systeembeheerder om te installeren en te vormen [!DNL Workfront for Salesforce].

De volgende subsecties beschrijven hoe te installeren [!DNL Workfront] voor uw [!DNL Salesforce] Productieomgeving. U kunt dezelfde stappen volgen om te installeren [!DNL Workfront] voor uw [!DNL Salesforce] Sandbox-omgeving.

* [Installeren [!DNL Workfront for Salesforce] voordat het beschikbaar wordt in het dialoogvenster [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [Installeren [!DNL Workfront for Salesforce] in de [!DNL Salesforce Classic] Kader](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [Installeren [!DNL Workfront for Salesforce] in de [!DNL Salesforce Lightning Experience] Kader](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### Installeren [!DNL Workfront for Salesforce] voordat het beschikbaar wordt in het dialoogvenster [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] is beschikbaar in het [!DNL Salesforce AppExchange] binnenkort.

U kunt als volgt de app installeren voordat deze beschikbaar is:

1. Ga in uw productieomgeving naar

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r)

   Ga in uw Sandbox-omgeving naar

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r](https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r)

   >[!NOTE]
   >
   >U moet in Salesforce worden geregistreerd om tot deze pagina&#39;s toegang te hebben.

1. Controleer de **[!UICONTROL Yes, grant access to these third-party web sites]** doos.

   Er wordt een laadscherm weergegeven. De installatie kan enige tijd duren.

1. Klikken **[!UICONTROL Done]** als de installatie is voltooid.

1. Navigeren naar **[!UICONTROL Setup]** > **[!UICONTROL Security]Besturingselementen** > **[!UICONTROL Remote Site Settings]**.
1. (Voorwaardelijk) Selecteer Workfront in de lijst.

   of

   Als u uw [!DNL Workfront] URL vermeld in **[!UICONTROL All Remote Sites]** lijst, klik **[!UICONTROL New Remote Site]**.

1. (Voorwaardelijk) Geef bij het toevoegen van de site de **[!UICONTROL Remote Site Name]**.

   Bijvoorbeeld: *[!DNL Workfront]*.

1. (Voorwaardelijk) Geef bij het toevoegen van de site de **[!UICONTROL Remote Site URL]**.

   Bijvoorbeeld: *yourDomain.my.workfront.com*.

1. Klik op **[!UICONTROL Save]**.

   De [!DNL Workfront] de toepassing is nu geïnstalleerd op uw [!DNL Salesforce] en de **[!UICONTROL WorkfrontOpportunities]** en **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] Pagina&#39;s zijn gemaakt in uw omgeving.

   [!DNL Salesforce] gebruikers kunnen de app gebruiken nadat u de [!DNL Workfront] van hun [!UICONTROL Opportunity] of [!UICONTROL Account] paginalay-outs.\
   Voor informatie over het configureren van de sectie Workfront voor gebruikers raadpleegt u [De Adobe Workfront-sectie voor Salesforce-gebruikers configureren](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installeren [!DNL Workfront] for [!DNL Salesforce] in de [!DNL Salesforce Classic] Kader

1. Aanmelden bij [!DNL Salesforce] als systeembeheerder.
1. Ga naar **Instellen.**
1. In de **Opbouwen** sectie, klikken **AppExchange Marketplace**.

1. In de **AppExchange-apps zoeken** vak, tekst **Workfront**.

1. Klik op de Workfront-toepassing wanneer u deze vindt en klik vervolgens op **Nu ophalen**.
1. Klikken **[!UICONTROL Install in Production]** om de [!DNL Workfront] in uw [!DNL Salesforce] Productieomgeving. (aanbevolen)
1. Nadat u de voorwaarden hebt gelezen en ermee akkoord gaat, schakelt u de optie **[!UICONTROL I have read and agree to the terms and conditions]** veld.
1. Klik op **[!UICONTROL Confirm and Install]**.
1. Selecteren **[!UICONTROL Install for All Users]** (aanbevolen) en klik vervolgens op **[!UICONTROL Install]**.

1. (Voorwaardelijk) Als u wordt gevraagd of u een deregang wilt goedkeuren, moet u selecteren **[!UICONTROL Yes, grant access to these third-party web sites]** en klik vervolgens op **[!UICONTROL Continue]**.

1. Klikken **[!UICONTROL Done]** als de installatie is voltooid.

   De [!DNL Workfront] app is vermeld onder **[!UICONTROL Installed Packages]**.


1. Navigeren naar **[!UICONTROL Setup>Security Controls>Remote Site Settings]**.
1. (Voorwaardelijk) Als u uw [!DNL Workfront] URL vermeld in **[!UICONTROL All Remote Sites]** lijst, klik **[!UICONTROL New Remote Site]**.

1. (Voorwaardelijk) Geef bij het toevoegen van de site de **[!UICONTROL Remote Site Name]**.
Bijvoorbeeld: *[!DNL Workfront]*.

1. (Voorwaardelijk) Geef bij het toevoegen van de site de **[!UICONTROL Remote Site URL]**.
Bijvoorbeeld: *yourDomain.my.workfront.com*.

1. Klik op **[!UICONTROL Save]**.\
   De [!DNL Workfront] de toepassing is nu geïnstalleerd op uw [!DNL Salesforce] -instantie. De **[!UICONTROL WorkfrontOpportunities]** en **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] pagina&#39;s zijn gemaakt in uw omgeving.\
   [!DNL Salesforce] gebruikers kunnen de app nog niet gebruiken totdat u de [!DNL Workfront] van hun [!UICONTROL Opportunity] of [!UICONTROL Account] paginalay-outs.\
   Voor informatie over het configureren van de [!DNL Workfront] voor gebruikers, zie [Vorm [!DNL Adobe Workfront] sectie voor [!DNL Salesforce] gebruikers](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installeren [!DNL Workfront for Salesforce] in de [!DNL Salesforce Lightning Experience] Kader

1. Aanmelden bij [!DNL Salesforce] als systeembeheerder.
1. Klik op de knop **[!UICONTROL Setup]pictogram** en klik vervolgens op **[!UICONTROL Setup]**.

1. In de **[!UICONTROL PLATFORM TOOLS]** sectie, uitvouwen **[!UICONTROL Apps].**

1. Klik op **[!DNL AppExchange Marketplace]**.
1. In de **[!UICONTROL Search [!DNL AppExchange] Apps]** vak, tekst **[!DNL Workfront]**.

1. Klik op de Workfront-toepassing wanneer u deze vindt en klik vervolgens op **Nu ophalen**.
1. Klik op **[!UICONTROL Open Login Screen]**.\
   U moet zich aanmelden met uw [!DNL Workfront] beheerdersaccount voor [!DNL Salesforce].

1. Klik op **[!UICONTROL Allow]**.
1. In de **[!UICONTROL Install in This Org]** vak, klikt u op **[!UICONTROL Install Here]** installeren [!DNL Workfront] in uw [!DNL Salesforce] Productieomgeving. (aanbevolen)

1. Nadat u de voorwaarden hebt gelezen en ermee akkoord gaat, schakelt u de optie **[!UICONTROL I have read and agree to the terms and conditions]** veld.
1. Klik op **[!UICONTROL Confirm and Install]**.
1. Selecteren **[!UICONTROL Install for All Users]** (aanbevolen) en klik vervolgens op **[!UICONTROL Install]**.

1. (Voorwaardelijk) Als u wordt gevraagd of u een deregang wilt goedkeuren, moet u selecteren **[!UICONTROL Yes, grant access to these third-party web sites]** en klik vervolgens op **[!UICONTROL Continue]**.

1. Klikken **[!UICONTROL Done]** als de installatie is voltooid.

   De [!DNL Workfront] app is vermeld onder **[!UICONTROL Installed Packages]**.

1. Navigeren naar **[!UICONTROL Setup].**
1. In de **[!UICONTROL SETTINGS]** sectie, uitvouwen **[!UICONTROL Security].**

1. Klik op **[!UICONTROL Remote Site Settings]**.
1. (Voorwaardelijk) Als u uw [!DNL Workfront] URL vermeld in **[!UICONTROL All Remote Sites]** lijst, klik **[!UICONTROL New Remote Site]**.

1. (Voorwaardelijk) Geef bij het toevoegen van de site de **[!UICONTROL Remote Site Name]**.
Bijvoorbeeld: *[!DNL Workfront]*.

1. (Voorwaardelijk) Geef bij het toevoegen van de site de **[!UICONTROL Remote Site URL]**.
Bijvoorbeeld: *yourDomain.my.workfront.com*.

1. Klik op **[!UICONTROL Save]**.

   De [!DNL Workfront] de toepassing is nu geïnstalleerd op uw [!DNL Salesforce] en de **[!DNL Workfront]** wordt nu toegevoegd aan uw omgeving.

   [!UICONTROL Salesforce] gebruikers kunnen de [!DNL Workfront] app zodra u de [!DNL Workfront] van hun [!UICONTROL Opportunity] of [!UICONTROL Account] paginalay-outs.\
   Voor informatie over het configureren van de [!DNL Workfront] voor gebruikers, zie [Vorm [!DNL Adobe Workfront] sectie voor [!DNL Salesforce] gebruikers](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
