---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Installeren  [!DNL Adobe Workfront]  voor  [!DNL Salesforce]
description: Om app te installeren alvorens het in de  [!DNL Salesforce]  AppExchange beschikbaar wordt, zie het Installeren  [!DNL Workfront]  voor Salesforce alvorens het in de Marketplace van de AppExchange Beschikbaar wordt.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: c0e7340e2bf650b6f9931ae12aee07c5f7d5292b
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 1%

---

# Installeren [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 1/2024 -->

>[!NOTE]
>
>Om app te installeren alvorens het in [!DNL Salesforce AppExchange] beschikbaar wordt, zie [ Installerend  [!DNL Workfront for Salesforce]  alvorens het in  [!DNL AppExchange]  Marketplace ](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace) beschikbaar wordt.

Als [!DNL Salesforce] en [!DNL Adobe Workfront] beheerder kunt u [!DNL Workfront for Salesforce] installeren zodat [!DNL Salesforce] -gebruikers [!DNL Workfront] -aanvragen kunnen verzenden en automatisch projecten kunnen maken zonder dat Salesforce wordt verlaten.

Voor algemeen begrip over wat u kunt verwachten door [!DNL Workfront for Salesforce] te installeren, zie [[!DNL Adobe Workfront for Salesforce]  overzicht ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [Vereisten voor het Installeren en het Gebruiken  [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [Installeren  [!DNL Workfront for Salesforce]](#installing-workfrontfor-salesforce)

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten voor installatie en gebruik [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* U moet een [!DNL Salesforce] -instantie hebben met toegang tot een systeembeheerder-account om de app te installeren.
* U moet een [!DNL Workfront] -instantie hebben met toegang tot een systeembeheerder-account om de integratie te configureren.
* [!UICONTROL Salesforce] gebruikers moeten een [!DNL Workfront] -account hebben om het volgende te kunnen doen:

   * [!DNL Workfront] aanvragen maken van [!DNL Salesforce]
   * [!DNL Workfront] aanvragen of projecten weergeven in Salesforce

## Installeren [!DNL Workfront for Salesforce] {#installing-workfront-for-salesforce}

U moet een [!DNL Salesforce] - en [!DNL Workfront] -systeembeheerder zijn om [!DNL Workfront for Salesforce] te installeren en configureren.

In de volgende subsecties wordt beschreven hoe u [!DNL Workfront] kunt installeren voor uw [!DNL Salesforce] productieomgeving. U kunt dezelfde stappen volgen om [!DNL Workfront] voor uw [!DNL Salesforce] Sandbox-omgeving te installeren.

* [Het installeren van  [!DNL Workfront for Salesforce]  alvorens het in  [!DNL AppExchange]  Marketplace beschikbaar wordt](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [Het installeren van  [!DNL Workfront for Salesforce]  in het  [!DNL Salesforce Classic]  Kader](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [Het installeren van  [!DNL Workfront for Salesforce]  in het  [!DNL Salesforce Lightning Experience]  Kader](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### [!DNL Workfront for Salesforce] installeren voordat deze beschikbaar wordt in de [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] is binnenkort beschikbaar in [!DNL Salesforce AppExchange] .

U kunt als volgt de app installeren voordat deze beschikbaar is:

1. Ga in uw productieomgeving naar

   [ https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   Ga in uw Sandbox-omgeving naar

   [ https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   >[!NOTE]
   >
   >U moet in Salesforce worden geregistreerd om tot deze pagina&#39;s toegang te hebben.

1. Schakel het selectievakje **[!UICONTROL Yes, grant access to these third-party web sites]** in.

   Er wordt een laadscherm weergegeven. De installatie kan enige tijd duren.

1. Klik op **[!UICONTROL Done]** wanneer de installatie is voltooid.

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL Security]Besturingselementen** > **[!UICONTROL Remote Site Settings]** .
1. (Voorwaardelijk) Selecteer Workfront in de lijst.

   of

   Als de [!DNL Workfront] URL niet wordt weergegeven in de lijst **[!UICONTROL All Remote Sites]** , klikt u op **[!UICONTROL New Remote Site]** .

1. (Voorwaardelijk) Geef bij het toevoegen van de site de waarde **[!UICONTROL Remote Site Name]** op.

   Bijvoorbeeld *[!DNL Workfront]* .

1. (Voorwaardelijk) Geef bij het toevoegen van de site de waarde **[!UICONTROL Remote Site URL]** op.

   Bijvoorbeeld, *yourDomain.my.workfront.com*.

1. Klik op **[!UICONTROL Save]**.

   De [!DNL Workfront] -app is nu geïnstalleerd op uw [!DNL Salesforce] -instantie en de **[!UICONTROL WorkfrontOpportunities]** - en **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] -pagina&#39;s zijn gemaakt in uw omgeving.

   [!DNL Salesforce] -gebruikers kunnen de app gebruiken nadat u de sectie [!DNL Workfront] aan hun [!UICONTROL Opportunity] - of [!UICONTROL Account] -paginalay-outs hebt toegevoegd.\
   Voor informatie over het vormen van de sectie van Workfront voor gebruikers, zie [ de sectie van Adobe Workfront voor gebruikers Salesforce vormen ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### [!DNL Workfront] for [!DNL Salesforce] installeren in het [!DNL Salesforce Classic] framework

1. Meld u aan bij [!DNL Salesforce] als systeembeheerder.
1. Ga naar **Opstelling.**
1. In de **bouwt** sectie, klik **de Marketplace van de AppExchange**.

1. In de **AppExchange van het Onderzoek Apps** doos, type **Workfront**.

1. Klik Workfront app wanneer u het vindt, dan klik **krijgt het** nu.
1. Klik op **[!UICONTROL Install in Production]** om de [!DNL Workfront] -toepassing in uw [!DNL Salesforce] productieomgeving te installeren. (aanbevolen)
1. Nadat u de voorwaarden hebt gelezen en ermee akkoord gaat, schakelt u het veld **[!UICONTROL I have read and agree to the terms and conditions]** in.
1. Klik op **[!UICONTROL Confirm and Install]**.
1. Selecteer **[!UICONTROL Install for All Users]** (aanbevolen) en klik op **[!UICONTROL Install]** .

1. (Voorwaardelijk) Als u wordt gevraagd of u een toegang van derden wilt goedkeuren, moet u **[!UICONTROL Yes, grant access to these third-party web sites]** selecteren en vervolgens op **[!UICONTROL Continue]** klikken.

1. Klik op **[!UICONTROL Done]** wanneer de installatie is voltooid.

   De app [!DNL Workfront] wordt weergegeven onder **[!UICONTROL Installed Packages]** .


1. Navigeer naar **[!UICONTROL Setup>Security Controls>Remote Site Settings]** .
1. (Voorwaardelijk) Als de [!DNL Workfront] URL niet wordt weergegeven in de lijst **[!UICONTROL All Remote Sites]** , klikt u op **[!UICONTROL New Remote Site]** .

1. (Voorwaardelijk) Geef bij het toevoegen van de site de waarde **[!UICONTROL Remote Site Name]** op.
Bijvoorbeeld *[!DNL Workfront]* .

1. (Voorwaardelijk) Geef bij het toevoegen van de site de waarde **[!UICONTROL Remote Site URL]** op.
Bijvoorbeeld, *yourDomain.my.workfront.com*.

1. Klik op **[!UICONTROL Save]**.\
   De [!DNL Workfront] -app is nu geïnstalleerd op uw [!DNL Salesforce] -instantie. De **[!UICONTROL WorkfrontOpportunities]** - en **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] -pagina&#39;s zijn gemaakt in uw omgeving.\
   [!DNL Salesforce] -gebruikers kunnen de app nog niet gebruiken totdat u de sectie [!DNL Workfront] toevoegt aan hun [!UICONTROL Opportunity] - of [!UICONTROL Account] -paginalay-outs.\
   Voor informatie over het vormen van de [!DNL Workfront] sectie voor gebruikers, zie [ de  [!DNL Adobe Workfront]  sectie voor  [!DNL Salesforce]  gebruikers ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md) vormen.

### [!DNL Workfront for Salesforce] installeren in het [!DNL Salesforce Lightning Experience] Framework

1. Meld u aan bij [!DNL Salesforce] als systeembeheerder.
1. Klik op het pictogram **[!UICONTROL Setup]** en klik vervolgens op **[!UICONTROL Setup]** .

1. Vouw **[!UICONTROL Apps]uit in de sectie **[!UICONTROL PLATFORM TOOLS]**.**

1. Klik op **[!DNL AppExchange Marketplace]**.
1. Typ **[!DNL Workfront]** in het vak **[!UICONTROL Search [!DNL AppExchange] Apps]** .

1. Klik Workfront app wanneer u het vindt, dan klik **krijgt het** nu.
1. Klik op **[!UICONTROL Open Login Screen]**.\
   U moet zich aanmelden met uw [!DNL Workfront] beheerdersaccount voor [!DNL Salesforce] .

1. Klik op **[!UICONTROL Allow]**.
1. Klik in het vak **[!UICONTROL Install in This Org]** op **[!UICONTROL Install Here]** om [!DNL Workfront] te installeren in de [!DNL Salesforce] productieomgeving. (aanbevolen)

1. Nadat u de voorwaarden hebt gelezen en ermee akkoord gaat, schakelt u het veld **[!UICONTROL I have read and agree to the terms and conditions]** in.
1. Klik op **[!UICONTROL Confirm and Install]**.
1. Selecteer **[!UICONTROL Install for All Users]** (aanbevolen) en klik op **[!UICONTROL Install]** .

1. (Voorwaardelijk) Als u wordt gevraagd of u een toegang van derden wilt goedkeuren, moet u **[!UICONTROL Yes, grant access to these third-party web sites]** selecteren en vervolgens op **[!UICONTROL Continue]** klikken.

1. Klik op **[!UICONTROL Done]** wanneer de installatie is voltooid.

   De app [!DNL Workfront] wordt weergegeven onder **[!UICONTROL Installed Packages]** .

1. Ga naar **[!UICONTROL Setup].**
1. Vouw **[!UICONTROL Security]uit in de sectie **[!UICONTROL SETTINGS]**.**

1. Klik op **[!UICONTROL Remote Site Settings]**.
1. (Voorwaardelijk) Als de [!DNL Workfront] URL niet wordt weergegeven in de lijst **[!UICONTROL All Remote Sites]** , klikt u op **[!UICONTROL New Remote Site]** .

1. (Voorwaardelijk) Geef bij het toevoegen van de site de waarde **[!UICONTROL Remote Site Name]** op.
Bijvoorbeeld *[!DNL Workfront]* .

1. (Voorwaardelijk) Geef bij het toevoegen van de site de waarde **[!UICONTROL Remote Site URL]** op.
Bijvoorbeeld, *yourDomain.my.workfront.com*.

1. Klik op **[!UICONTROL Save]**.

   De [!DNL Workfront] -app is nu geïnstalleerd op uw [!DNL Salesforce] -instantie en de **[!DNL Workfront]** -component wordt nu toegevoegd aan uw omgeving.

   [!UICONTROL Salesforce] -gebruikers kunnen de [!DNL Workfront] -app gebruiken nadat u de [!DNL Workfront] -sectie hebt toegevoegd aan hun [!UICONTROL Opportunity] - of [!UICONTROL Account] -paginalay-outs.\
   Voor informatie over het vormen van de [!DNL Workfront] sectie voor gebruikers, zie [ de  [!DNL Adobe Workfront]  sectie voor  [!DNL Salesforce]  gebruikers ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md) vormen.
