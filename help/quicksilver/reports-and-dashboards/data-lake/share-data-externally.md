---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Verbinding maken met Workfront Data Connect
description: Met Workfront Data Connect kunt u de Workfront-gegevens van uw organisatie gebruiken met de tools voor bedrijfsintelligentie of deze opslaan in een extern gegevenspakhuis.
author: Nolan
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: 7764e512a3fb30a89e6645a4d8544a5fcffee231
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# Verbinding maken met Workfront Data Connect

Met Workfront Data Connect kunt u de Workfront-gegevens van uw organisatie gebruiken met de tools voor bedrijfsintelligentie of deze opslaan in een extern gegevenspakhuis.

Om uw Gegevens aan te sluiten verbind gegevens meer met een extern product, moet u een verbinding eerst tot stand brengen zoals die in [ wordt beschreven leidt tot een lezerrekening of een verbinding voor Snowflake ](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md). Dan, moet u om het even welke vereiste IPs aan de lijst van gewenste personen toevoegen zoals die in [ wordt beschreven voeg IPs aan de lijst van gewenste personen ](#add-ips-to-the-allowlist) hieronder toe.

De meeste producten zullen de volgende informatie over uw gegevens meer vereisen om een verbinding te vestigen:

| Veldnaam | Waarde |
|---------------|-------------|
| Server | URL voor de verbinding, zonder het `https://` gedeelte (dat op **Gegevens wordt gevonden verbindt** pagina in Workfront*) |
| Poort | `443` |
| Database | `WORKFRONT` |
| Warehouse | `READER_WH` |
| Schema | `WF` |
| Rol | `READER_ROLE` |
| Gebruikersnaam | De gebruikersbenaming die wanneer het creëren van de verbinding wordt gekozen (die op **Gegevens wordt gevonden verbindt** pagina in Workfront*) |
| Wachtwoord | Het wachtwoord dat is gekozen bij de eerste Snowflake-aanmelding* |

*For informatie over waar te om **Gegevens te vinden verbindt** pagina die uw verbindingen bevat, zie [ een reader rekening of verbinding voor Snowflake ](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md) creëren.

>[!IMPORTANT]
>
>Zodra één ingang aan de IP lijst van gewenste personen wordt toegevoegd, zijn alle andere IP adressen niet meer toegestaan. Zorg ervoor dat u alle vereiste IP-adressen hebt ingevoerd, zowel voor het maken als voor het lezen van uw visualisatieprogramma, voordat u het gereedschap gaat gebruiken. Als dat niet het geval is, kan er een fout optreden met betrekking tot ongeldige referenties.
>
>Als u geen IP adressen inbegrepen in uw lijst van gewenste personen hebt maar nog problemen heeft die met een hulpmiddel verbinden BI, controleer de configuratie van de volmachtsserver voor het hulpmiddel van BI.

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

## Voeg IPs aan de lijst van gewenste personen toe

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Opstelling**.

1. In het linkerpaneel, klik **Systeem** > **Gegevens verbinden**.

1. Klik op het **Toegestane IPs** lusje, dan klik op **een IP Adres aan uw Lijst van gewenste personen** knoop toevoegen.

1. Ga een naam voor het IP adres in **IP de beschrijving van het Adres** in en ga het IP adres (of blok CIDR) voor het hulpmiddel in u in **IP Adres** zou willen gebruiken, dan klik **IP aan Lijst van gewenste personen** toevoegen.

   ![ voeg IP adres ](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"} toe

## Verwijder een IP adres uit de lijst van gewenste personen

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Opstelling**.

1. In het linkerpaneel, klik **Systeem** > **Gegevens verbinden**.

1. Klik op het **Toegestane IPs** lusje, dan klik op het trashcan pictogram ![ pictogram van de Schrapping ](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) rechts van het IP adres u zou willen verwijderen.

1. In het venster dat verschijnt, controleer de doos om te bevestigen en dan **Schrapping** te klikken.

## Gegevens delen met Business Intelligence-tools

Een aantal gemeenschappelijke hulpmiddelen van de bedrijfsintelligentie wordt hieronder vermeld; bezoek hun documentatieplaatsen om meer te leren over het verbinden met uw gegevens meer.

* Tableau
* Power BI
* Domo
* SAP HANA

## Gegevens opslaan in een extern gegevenspakhuis

Een aantal gemeenschappelijke gegevensopslagplaatsen zijn hieronder vermeld; bezoek hun documentatieplaatsen om meer te leren over het verbinden met uw gegevens meer.

* Databricks
* AWS Redshift
