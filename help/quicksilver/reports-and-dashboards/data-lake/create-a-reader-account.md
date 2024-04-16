---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Een reader-account (service) maken voor Snowflake
description: Als u toegang wilt krijgen tot de gegevens in het Workfront Data Lake, moet u eerst een leesaccount voor Snowflake maken.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: 912f46c87170d6b678d885ccc1fb0170526578df
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Een reader-account (service) maken voor Snowflake

Als u toegang wilt tot gegevens over het meer van Workfront, moet u eerst een leesaccount voor Snowflake maken. Bovendien, moet u IPs aan de lijst van gewenste personen voor om het even welke externe hulpmiddelen toevoegen u op het verbinden met de gegevens van plan bent.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>TBD</td> 
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

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Een lezeraccount maken

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon-left-nav.png) in de linkerbovenhoek klikt u op **Instellen**.

1. Klik in het linkerdeelvenster op **Systeem** > **Gegevenstoegang**.

1. Klikken **Nieuwe verbinding maken**

1. Voer in het venster dat wordt weergegeven een naam in voor uw verbinding in **Beschrijving van verbindingsverwijzing** en een gebruikersnaam in **Verbinding maken, gebruiker** en klik vervolgens op **Verbinding genereren**.

   ![Reader-account maken](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. A **Standaardwachtwoord** wordt gegenereerd, evenals een URL waar uw gegevens via Snowflake kunnen worden weergegeven. U moet het wachtwoord gebruiken in combinatie met de gebruikersnaam die u hebt gekozen om u voor het eerst aan te melden bij de Snowflake, zodat u een record en de URL bijhoudt. Schakel het selectievakje in als u dat hebt gedaan en klik op **Sluiten**.

   ![Standaardaccountwachtwoord](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Open Snowflake met een browser om naar de URL te navigeren vanuit de vorige stap, voer de door u geselecteerde gebruikersnaam en het standaardwachtwoord uit de vorige stap in en klik op **Aanmelden**.

1. Nadat u zich voor het eerst hebt aangemeld, wordt u gevraagd een nieuw wachtwoord te kiezen. Voer een wachtwoord naar keuze in het dialoogvenster **Nieuw wachtwoord** en **Wachtwoord bevestigen** velden, klik vervolgens op **Verzenden**.

   ![Wachtwoord Snowflake opnieuw instellen](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. U kunt nu uw gebruikersnaam en nieuw wachtwoord gebruiken om toegang te krijgen tot uw Workfront-datumpigment in de Snowflake of het bedrijfsvisualisatieprogramma van uw keuze.

## Voeg IPs aan de lijst van gewenste personen toe

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon-left-nav.png) in de linkerbovenhoek klikt u op **Instellen**.

1. Klik in het linkerdeelvenster op **Systeem** > **Gegevenstoegang**.

1. Klik op de knop **Toegestane IPs** en klikt u op de knop **Voeg een IP Adres aan uw Lijst van gewenste personen toe** knop.

1. Voer een naam in voor het IP-adres in **Beschrijving van IP-adres** en voer het IP-adres in voor het gereedschap waarin u wilt gebruiken **IP-adres** en klik vervolgens op **IP toevoegen aan Lijst van gewenste personen**.

   ![IP-adres toevoegen](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Een lezeraccount intrekken of een IP-adres uit de lijst van gewenste personen verwijderen

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon-left-nav.png) in de linkerbovenhoek klikt u op **Instellen**.

1. Klik in het linkerdeelvenster op **Systeem** > **Gegevenstoegang**.

1. Klik op het pictogram van de trashcan ![Pictogram Verwijderen](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) rechts van de account die u wilt intrekken.

   OF

   Klik op de knop **Toegestane IPs** en klik vervolgens op het pictogram van de prullenbak ![Pictogram Verwijderen](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) rechts van het IP-adres dat u wilt verwijderen.

1. Schakel in het venster dat wordt weergegeven het selectievakje ter bevestiging in en klik op **Verwijderen**.
