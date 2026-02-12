---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Een lezeraccount maken voor Snowflake
description: Als u toegang wilt krijgen tot gegevens van Data Connect, moet u eerst een Snowflake Reader-account maken.
author: Nolan
feature: Reports and Dashboards
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: 9cf221bda04614856a6a3670100742340fb73aee
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---

# Een reader-account of -verbinding maken voor Snowflake

Als u toegang wilt krijgen tot gegevens van Data Connect, moet u eerst een Snowflake-lezer (of service)-account voor uw organisatie maken en vervolgens een nieuwe verbinding maken voor elke gebruiker of elk hulpprogramma dat u toegang wilt hebben tot Data Connect.

Nadat u een verbinding hebt gemaakt, kunt u de bijbehorende URL en gebruikersnaam vinden door erop te klikken op de pagina Data Connect (Hoofdmenu > Setup > Systeem > Data Connect) onder het tabblad Bestaande verbindingen.

Voor informatie bij het gebruiken van een pas gecreëerde verbinding met een extern product, zie [ een verbinding aan de Gegevens van Workfront vestigen verbind ](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td><p>Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een lezeraccount maken

U moet een nieuwe Snowflake-lezeraccount voor uw organisatie maken voordat u verbinding kunt maken.

>[!IMPORTANT]
>
>Dit proces moet slechts eenmaal per organisatie worden voltooid. Als **de Create knoop van de Rekening van Reader** niet in de hieronder beschreven plaats aanwezig is, dan is uw reader rekening reeds gecreeerd.

Een lezeraccount maken:

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Opstelling**.

1. In het linkerpaneel, klik **Systeem** > **Gegevens verbinden**.

1. Klik de **Create knoop van de Rekening van Reader** beginnen creërend de reader van uw organisatie rekening. Het proces is automatisch, maar kan tot 24 uur duren.

1. Na voltooiing wordt een dialoogvenster weergegeven waarin wordt uitgelegd dat uw lezeraccount nu actief is. Vernieuw de browser pagina om toegang tot **te krijgen creeer Nieuwe Verbinding** knoop.

![ de rekening van Reader creeerde dialoog ](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-reader-account-created.png)

## Verbinding maken

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Opstelling**.

1. In het linkerpaneel, klik **Systeem** > **Gegevens verbinden**.

1. Klik **creëren Nieuwe Verbinding**

1. In het venster dat verschijnt, ga een naam voor uw verbinding in **de verwijzingsbeschrijving van de Verbinding** en een gebruikersbenaming in **de gebruiker van de Verbinding** in, dan klik **produceert Verbinding**.

   ![ creeer nieuwe verbinding ](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. A **Standaardwachtwoord** zal, evenals URL worden geproduceerd waar uw gegevens door Snowflake kunnen worden bekeken. U moet het wachtwoord gebruiken in combinatie met de gebruikersnaam die u hebt gekozen om u voor het eerst aan te melden bij Snowflake, zodat u een record en de URL kunt bijhouden. Controleer de doos die u verklaart dit hebt gedaan, dan klik **dicht**.

   ![ Standaard rekeningswachtwoord ](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Open Snowflake gebruikend browser om aan URL van de vorige stap te navigeren, ga de gebruikersbenaming in u en het standaardwachtwoord van de vorige stap selecteerde, dan klik **binnen Teken**.

1. Nadat u zich voor het eerst hebt aangemeld, wordt u gevraagd een nieuw wachtwoord te kiezen. Ga een wachtwoord van uw keus in zowel het **Nieuwe wachtwoord** in en **bevestig wachtwoord** gebieden, dan klik **voorleggen**.

   ![ het wachtwoord van Snowflake van het Terugstellen ](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. U kunt nu uw gebruikersnaam en nieuw wachtwoord gebruiken om toegang te krijgen tot uw Data Connect Data Lake in Snowflake of het hulpprogramma voor bedrijfsvisualisatie van uw keuze.

## Een lezeraccount intrekken

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Opstelling**.

1. In het linkerpaneel, klik **Systeem** > **Toegang van Gegevens**.

1. Klik op het trashcan pictogram van de Schrapping ![ pictogram van de Schrapping ](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) rechts van de rekening u zou willen intrekken.

1. In het venster dat verschijnt, controleer de doos om te bevestigen en dan **Schrapping** te klikken.
