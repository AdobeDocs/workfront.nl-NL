---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Een reader-account (service) maken voor Snowflake
description: Als u toegang wilt krijgen tot gegevens van Data Connect, moet u eerst een account voor een Snowflake-lezer maken.
author: Nolan
feature: Reports and Dashboards
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: 4c8b7e7f33ec593b2942725eb9160f7fbe2962e3
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# Een reader-account (service) maken voor Snowflake

Als u toegang wilt krijgen tot gegevens van Data Connect, moet u eerst een Snowflake reader (of service)-account maken voor elke nieuwe verbinding. Na het creëren van een verbinding, kunt u zijn bijbehorende URL en gebruikersbenaming vinden door op het op de **toegang van Gegevens** pagina (**Belangrijkste menu** > **Opstelling** > **Toegang van het Systeem** > **Gegevens**) onder **Bestaande Verbindingen** tabel te klikken.

Voor informatie bij het gebruiken van een pas gecreëerde verbinding met een extern product, zie [ een verbinding aan de Gegevens van Workfront vestigen verbind ](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td><p>Opgenomen in de volgende plannen:</p>
    <ul>
        <li>Ultieme</li> 
    </ul>    
   <p>Kan worden aangeschaft als een toevoeging bij de volgende plannen:</p> 
    <ul>
        <li>Selecteren</li> 
        <li>Eerste</li>
    </ul> 
    <p>Workfront Data Connect is niet beschikbaar voor oudere Workfront-plannen.</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een lezeraccount maken

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Opstelling**.

1. In het linkerpaneel, klik **Systeem** > **Toegang van Gegevens**.

1. Klik **creëren Nieuwe Verbinding**

1. In het venster dat verschijnt, ga een naam voor uw verbinding in **de verwijzingsbeschrijving van de Verbinding** en een gebruikersbenaming in **de gebruiker van de Verbinding** in, dan klik **produceert Verbinding**.

   ![ creeer reader rekening ](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. A **Standaardwachtwoord** zal, evenals URL worden geproduceerd waar uw gegevens door Snowflake kunnen worden bekeken. U moet het wachtwoord gebruiken in combinatie met de gebruikersnaam die u hebt gekozen om u voor het eerst aan te melden bij de Snowflake, zodat u een record en de URL bijhoudt. Controleer de doos die u verklaart dit hebt gedaan, dan klik **dicht**.

   ![ Standaard rekeningswachtwoord ](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Open Snowflake die browser gebruikt om aan URL van de vorige stap te navigeren, ga de gebruikersbenaming in u en het standaardwachtwoord van de vorige stap selecteerde, dan klik **binnen Teken**.

1. Nadat u zich voor het eerst hebt aangemeld, wordt u gevraagd een nieuw wachtwoord te kiezen. Ga een wachtwoord van uw keus in zowel het **Nieuwe wachtwoord** in en **bevestig wachtwoord** gebieden, dan klik **voorleggen**.

   ![ het wachtwoord van de Snowflake van het Terugstellen ](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. U kunt nu uw gebruikersnaam en nieuw wachtwoord gebruiken om toegang te krijgen tot uw Data Connect Data Lake in Snowflake of het hulpprogramma voor bedrijfsvisualisatie van uw keuze.

## Een lezeraccount intrekken

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Opstelling**.

1. In het linkerpaneel, klik **Systeem** > **Toegang van Gegevens**.

1. Klik op het trashcan pictogram van de Schrapping ![ pictogram van de Schrapping ](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) rechts van de rekening u zou willen intrekken.

1. In het venster dat verschijnt, controleer de doos om te bevestigen en dan **Schrapping** te klikken.
