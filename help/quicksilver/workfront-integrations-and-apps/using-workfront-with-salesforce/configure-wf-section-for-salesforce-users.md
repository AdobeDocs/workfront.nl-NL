---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: Configureer de [!DNL Adobe Workfront] sectie voor [!DNL Salesforce] gebruikers
description: Na de installatie [!DNL Adobe Workfront] voor Salesforce als [!DNL Workfront] beheerder, kunt u het ter beschikking stellen van uw gebruikers door het in een nieuwe sectie aan hun de paginalay-outs van de Kans en van de Rekening in Salesforce toe te voegen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 1%

---

# Configureer de [!DNL Adobe Workfront] sectie voor [!DNL Salesforce] gebruikers

A [!UICONTROL Pro] [!DNL Workfront] U moet een abonnement nemen om deze functie te kunnen gebruiken. Voor meer informatie over de verschillende beschikbare plannen raadpleegt u [[!DNL Workfront] Abonnementen.](https://www.workfront.com/plans)

Na de installatie [!DNL Adobe Workfront] for [!DNL Salesforce] als [!DNL Workfront] beheerder, kunt u het ter beschikking stellen van uw gebruikers door het in een nieuwe sectie aan hun toe te voegen [!UICONTROL Opportunity] en [!UICONTROL Account]
paginalay-outs in [!UICONTROL Salesforce].

Voor informatie over installeren [!DNL Workfront for Salesforce], zie [Installeren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Gebruikers moeten beschikken over [!DNL Workfront] beschikbaar in beide [!DNL Classic] en [!DNL Lightning Experience] frameworks, voegt u de [!DNL WorkfrontOpportunities] en de [!DNL WorkfrontAccounts] [!UICONTROL Visualforce] pagina&#39;s naar de [!UICONTROL Opportunity] en [!UICONTROL Accounts] paginalay-outs, respectievelijk.

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

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Vereisten

* U moet beschikken over een [!DNL Salesforce] instantie met toegang tot een systeembeheerdersaccount.
* U moet beschikken over een [!DNL Workfront] instantie met toegang tot een systeembeheerdersaccount.

## Configureer de [!DNL Workfront] in de [!DNL Salesforce Classic] kader

1. Aanmelden bij [!DNL Salesforce] als Workfront-beheerder.
1. Klik op **[!UICONTROL Setup].**
1. In de **[!UICONTROL Build]** sectie, uitvouwen **[!UICONTROL Customize].**

1. Uitbreiden **[!UICONTROL Opportunities]** en klik vervolgens op **[!UICONTROL Page Layouts]** om de [!DNL Workfront] aan een Opportunity.

   of

   Uitbreiden **[!UICONTROL Accounts]** en klik vervolgens op **[!UICONTROL Page Layouts]** om de [!DNL Workfront] aan een account.

1. Klikken **[!UICONTROL Edit]** op een bestaande lay-out.

   of

   Klikken **[!UICONTROL New]** om een nieuwe lay-out toe te voegen.

1. (Optioneel) Sleep de **[!UICONTROL Section]** naar de lay-out en zet deze op de gewenste positie neer.\

1. (Optioneel) Geef een naam op voor de nieuwe sectie.

   We raden u aan deze sectie een naam te geven **[!DNL Workfront]**.

1. (Optioneel) Geef het gewenste item op **[!UICONTROL Layout]** en **[!UICONTROL Tab-key Order]** voor de nieuwe sectie.

   We raden u aan **[!UICONTROL 1-Column]** layout voor de [!DNL Workfront] sectie.

1. Klik op **[!UICONTROL OK]**.
1. In de **[!UICONTROL Layout]** gebied, klikken **[!UICONTROL Visualforce Pages].**

1. Sleep de **[!UICONTROL WorkfrontOpportunities]** aan de nieuwe sectie in de **[!UICONTROL Opportunities]** Lay-out.

   of

   Sleep de **[!UICONTROL WorkfrontAccounts]** aan de nieuwe sectie in de  **[!UICONTROL Account]** Lay-out.\

1. Klik op de knop **[!UICONTROL Properties]** in de rechterbovenhoek van de zojuist toegevoegde component.\

1. Voor een optimale weergave geeft u de volgende eigenschappen op voor de [!DNL Workfront Visualforce] pagina:

   * **[!UICONTROL Width (in pixels or %)]**: 100%
   * **[!UICONTROL Height (in pixels)]**: 600
   * Selecteren **[!UICONTROL Show scrollbars]**.

1. Klik op **[!UICONTROL OK]**.
1. Klikken **[!UICONTROL Save]** om uw lay-out op te slaan.

   Alle gebruikers aan wie deze lay-out is toegewezen, kunnen nu de [!DNL Workfront] deel over hun [!UICONTROL Opportunities] of [!UICONTROL Accounts] objecten.

   Gebruikers zien een [!DNL Workfront] aanmeldingsscherm op het [!DNL Workfront] sectie. Als ze geen [!DNL Workfront] -account, kunnen ze de sectie samenvouwen, maar niet verwijderen uit hun layout.

## Configureer de [!DNL Workfront] in de [!DNL Salesforce Lightning Experience] kader

U kunt de [!DNL Workfront] aan de lay-out van een [!DNL Salesforce] [!UICONTROL Opportunity] of Account in de [!DNL Salesforce Lightning Experience] het kader of [!UICONTROL Setup] van een account of [!UICONTROL Opportunity] object.

* [Configureer de [!DNL Workfront] de [!UICONTROL Setup] niveau](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Configureer de [!DNL Workfront] Sectie op opportuniteits- of accountniveau](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### Configureer de [!DNL Workfront] de [!UICONTROL Setup] niveau {#configure-the-workfront-section-at-the-setup-level}

1. Aanmelden [!DNL Salesforce] als systeembeheerder.
1. Klik op de knop **[!UICONTROL Setup]** pictogram, klik vervolgens op **[!UICONTROL Setup]**.

1. Uitbreiden **[!UICONTROL Object and Fields]** en klik vervolgens op **[!UICONTROL Object Manager]**.

1. Klikken **[!UICONTROL Opportunity]** om de lay-out van een Kans aan te passen.

   of

   Klikken **[!UICONTROL Account]** om de indeling van een account aan te passen.

1. Klik op **[!UICONTROL Page Layouts]**.
1. Klik op de naam van een bestaande pagina-indeling om deze te bewerken.

   of

   Klikken **[!UICONTROL New]** om een nieuwe pagina-indeling te maken.

1. Doorgaan met [Configureer de [!DNL Workfront] Sectie op opportuniteits- of accountniveau](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) hieronder.

### Configureer de [!DNL Workfront] Sectie op opportuniteits- of accountniveau {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Aanmelden bij [!DNL Salesforce] als systeembeheerder.
1. Ga naar een **[!UICONTROL Opportunity]** of **[!UICONTROL Account]**.

1. Klik op de knop **[!UICONTROL Setup]** pictogram, klik vervolgens op **[!UICONTROL Edit Page]**.\

1. Vouw de sectie **[!UICONTROL Custom-Managed]** uit.
1. Sleep de **[!DNL Workfront]** component op uw [!UICONTROL Opportunity] of Accountpagina.

   We raden u aan de volledige breedte van de pagina te gebruiken voor de [!DNL Workfront] in plaats van een van de kolommen van de layout.

1. Klik op **[!UICONTROL Save]**.

   Alle gebruikers aan wie deze lay-out is toegewezen, kunnen nu de [!DNL Workfront] deel over hun [!UICONTROL Opportunities] of [!UICONTROL Accounts] objecten.

   >[!NOTE]
   >
   >Gebruikers zien een [!DNL Workfront] aanmeldingsscherm op het [!DNL Workfront] sectie. Als ze geen [!DNL Workfront] -account, kunnen ze de sectie samenvouwen, maar niet verwijderen uit hun layout. Gebruikers kunnen zich aanmelden met de verificatiemethode die u hebt ingeschakeld: Verbeterde verificatie of de URL van uw SAML (Security Assertion Markup Language).

