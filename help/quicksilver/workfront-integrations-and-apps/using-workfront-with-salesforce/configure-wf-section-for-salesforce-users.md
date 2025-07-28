---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: Vorm de  [!DNL Adobe Workfront]  sectie voor  [!DNL Salesforce]  gebruikers
description: Nadat u  [!DNL Adobe Workfront]  voor Salesforce als a  [!DNL Workfront]  beheerder installeert, kunt u het ter beschikking stellen van uw gebruikers door het in een nieuwe sectie aan hun de paginalay-outs van de Kans en van de Rekening in Salesforce toe te voegen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---

# De sectie [!DNL Adobe Workfront] voor [!DNL Salesforce] -gebruikers configureren

>[!IMPORTANT]
>
>Om stabielere en scalable integratie te leveren, verschuiven wij naar een moderne, flexibele integratiebenadering gebruikend Workfront Automation and Integration (Fusion). Als deel van dit overgangsproces, zal Workfront voor de integratie van Salesforce niet beschikbaar na **28 Februari, 2026** zijn.
>
>We raden u aan Workfront Automation and Integration te gebruiken voor de integratiebehoeften van uw organisatie met Salesforce.
>
>Voor een overzicht van de Automatisering en de Integratie van Workfront, zie [ het overzicht van de Fusie van Adobe Workfront ](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Voor informatie over de specifieke mogelijkheden van de modules van de Automatisering en van de Integratie van Workfront voor Salesforce, zie [ modules van Salesforce ](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

U hebt een [!UICONTROL Pro] [!DNL Workfront] -abonnement nodig om deze functie te kunnen gebruiken. Voor meer informatie over de diverse beschikbare plannen, zie [[!DNL Workfront]  Plannen.](https://business.adobe.com/products/workfront/pricing.html)

Nadat u [!DNL Adobe Workfront] for [!DNL Salesforce] as a [!DNL Workfront] administrator hebt geïnstalleerd, kunt u deze beschikbaar maken voor uw gebruikers door deze in een nieuwe sectie toe te voegen aan hun [!UICONTROL Opportunity] en [!UICONTROL Account]
paginalay-outs in [!UICONTROL Salesforce] .

Voor informatie over het installeren van [!DNL Workfront for Salesforce], zie [ installeren  [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Als u wilt dat [!DNL Workfront] beschikbaar is in zowel de [!DNL Classic] - als [!DNL Lightning Experience] -frameworks, moet u de pagina&#39;s [!DNL WorkfrontOpportunities] en [!DNL WorkfrontAccounts] [!UICONTROL Visualforce] toevoegen aan respectievelijk de [!UICONTROL Opportunity] - en [!UICONTROL Accounts] -paginalay-outs.

## Toegangsvereisten

U moet de volgende toegang hebben om de in dit artikel beschreven functionaliteit te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## Vereisten

* U moet een [!DNL Salesforce] -instantie hebben met toegang tot een systeembeheerdersaccount.
* U moet een [!DNL Workfront] -instantie hebben met toegang tot een systeembeheerdersaccount.

## De sectie [!DNL Workfront] in het [!DNL Salesforce Classic] -framework configureren

1. Meld u aan bij [!DNL Salesforce] als Workfront-beheerder.
1. Klik op **[!UICONTROL Setup].**
1. Vouw **[!UICONTROL Build]** uit in de sectie **[!UICONTROL Customize].**

1. Vouw **[!UICONTROL Opportunities]** uit en klik op **[!UICONTROL Page Layouts]** om de sectie [!DNL Workfront] aan een opportunity toe te voegen.

   of

   Vouw **[!UICONTROL Accounts]** uit en klik op **[!UICONTROL Page Layouts]** om de sectie [!DNL Workfront] aan een account toe te voegen
.

1. Klik op **[!UICONTROL Edit]** in een bestaande lay-out.

   of

   Klik op **[!UICONTROL New]** om een nieuwe indeling toe te voegen.

1. (Optioneel) Sleep de component **[!UICONTROL Section]** naar de lay-out en zet deze op de gewenste positie neer.\

1. (Optioneel) Geef een naam op voor de nieuwe sectie.

   We raden u aan deze sectie een naam te geven **[!DNL Workfront]** .

1. (Optioneel) Geef de gewenste **[!UICONTROL Layout]** en **[!UICONTROL Tab-key Order]** op voor de nieuwe sectie.

   We raden u aan **[!UICONTROL 1-Column]** -lay-out te selecteren voor de [!DNL Workfront] -sectie.

1. Klik op **[!UICONTROL OK]**.
1. Klik in het **[!UICONTROL Layout]** -gebied op **[!UICONTROL Visualforce Pages].**

1. Sleep de component **[!UICONTROL WorkfrontOpportunities]** naar de nieuwe sectie in de **[!UICONTROL Opportunities]** -layout.

   of

   Sleep de component **[!UICONTROL WorkfrontAccounts]** naar de nieuwe sectie in de **[!UICONTROL Account]** layout.\

1. Klik op het pictogram **[!UICONTROL Properties]** rechtsboven in de nieuw toegevoegde component.\

1. Voor een optimale weergave geeft u de volgende eigenschappen op voor de pagina [!DNL Workfront Visualforce] :

   * **[!UICONTROL Width (in pixels or %)]**: 100%
   * **[!UICONTROL Height (in pixels)]**: 600
   * Selecteer **[!UICONTROL Show scrollbars]** .

1. Klik op **[!UICONTROL OK]**.
1. Klik op **[!UICONTROL Save]** om de lay-out op te slaan.

   Alle gebruikers aan wie deze lay-out is toegewezen, kunnen nu de sectie [!DNL Workfront] op hun [!UICONTROL Opportunities] - of [!UICONTROL Accounts] -objecten bekijken.

   Gebruikers zien een [!DNL Workfront] aanmeldingsscherm in de [!DNL Workfront] -sectie. Als ze geen [!DNL Workfront] -account hebben, kunnen ze de sectie samenvouwen, maar niet verwijderen uit hun layout.

## De sectie [!DNL Workfront] in het [!DNL Salesforce Lightning Experience] -framework configureren

U kunt de sectie [!DNL Workfront] toevoegen aan de lay-out van een [!DNL Salesforce] [!UICONTROL Opportunity] of account
in het [!DNL Salesforce Lightning Experience] -framework ofwel door toegang te krijgen tot het [!UICONTROL Setup] -gebied, ofwel via een account
of [!UICONTROL Opportunity] -object.

* [Vorm de  [!DNL Workfront]  sectie op het [!UICONTROL Setup] niveau](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Vorm de  [!DNL Workfront]  Sectie op het niveau van de Kans of van de Rekening](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### De sectie [!DNL Workfront] op [!UICONTROL Setup] -niveau configureren {#configure-the-workfront-section-at-the-setup-level}

1. Meld u aan bij [!DNL Salesforce] als systeembeheerder.
1. Klik op het pictogram **[!UICONTROL Setup]** en klik vervolgens op **[!UICONTROL Setup]** .

1. Vouw **[!UICONTROL Object and Fields]** uit en klik op **[!UICONTROL Object Manager]** .

1. Klik op **[!UICONTROL Opportunity]** om de indeling van een opportunity aan te passen.

   of

   Klik op **[!UICONTROL Account]** om de indeling van een account aan te passen.

1. Klik op **[!UICONTROL Page Layouts]**.
1. Klik op de naam van een bestaande pagina-indeling om deze te bewerken.

   of

   Klik op **[!UICONTROL New]** om een nieuwe pagina-indeling te maken.

1. Ga met [ verder vormen de  [!DNL Workfront]  Sectie op het niveau van de Kans of van de Rekening ](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) hieronder.

### Configureer de sectie [!DNL Workfront] op het niveau Opportunity of Account {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Meld u aan bij [!DNL Salesforce] als systeembeheerder.
1. Ga naar een **[!UICONTROL Opportunity]** of **[!UICONTROL Account]** .

1. Klik op het pictogram **[!UICONTROL Setup]** en klik vervolgens op **[!UICONTROL Edit Page]**\.

1. Vouw de sectie **[!UICONTROL Custom-Managed]** uit.
1. Sleep de component **[!DNL Workfront]** naar uw [!UICONTROL Opportunity] of account
pagina.

   We raden u aan de volledige breedte van de pagina voor de sectie [!DNL Workfront] te gebruiken in plaats van een van de kolommen van de lay-out.

1. Klik op **[!UICONTROL Save]**.

   Alle gebruikers aan wie deze lay-out is toegewezen, kunnen nu de sectie [!DNL Workfront] op hun [!UICONTROL Opportunities] - of [!UICONTROL Accounts] -objecten bekijken.

   >[!NOTE]
   >
   >Gebruikers zien een [!DNL Workfront] aanmeldingsscherm in de [!DNL Workfront] -sectie. Als ze geen [!DNL Workfront] -account hebben, kunnen ze de sectie samenvouwen, maar niet verwijderen uit hun layout. Gebruikers kunnen zich aanmelden met de verificatiemethode die u hebt ingeschakeld: uitgebreide verificatie of de URL van de SAML (Security Assetup Language).

