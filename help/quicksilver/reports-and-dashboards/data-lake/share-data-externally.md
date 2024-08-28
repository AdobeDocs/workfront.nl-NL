---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Een verbinding tot stand brengen met het datumpigment van Workfront
description: Met Workfront-datumpigment kunt u de Workfront-gegevens van uw organisatie gebruiken met populaire tools voor bedrijfsintelligentie of deze opslaan in een extern gegevenspakhuis.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: 16809b2d1801dd7aa4ab1f452e4687601fc1ac59
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 0%

---

# Verbinding maken met Workfront Data Connect

Met Workfront Data Connect kunt u de Workfront-gegevens van uw organisatie gebruiken met de tools voor bedrijfsintelligentie of deze opslaan in een extern gegevenspakhuis.

Om uw Gegevens aan te sluiten verbind gegevens meer met een extern product, moet u om het even welke vereiste IPs aan de lijst van gewenste personen eerst toevoegen zoals die in [ wordt beschreven toevoegt IPs aan de lijst van gewenste personen ](#add-ips-to-the-allowlist) hieronder. Bovendien zullen de meeste producten extra informatie over uw gegevens meer vereisen om een verbinding te vestigen:

| Veldnaam | Waarde |
|---------------|-------------|
| Server | URL voor de verbinding, zonder het `https://` gedeelte (dat op de **toegang van Gegevens** pagina in Workfront* wordt gevonden) |
| Poort | `443` |
| Database | `WORKFRONT` |
| Warehouse | `READER_WH` |
| Schema | `WF` |
| Rol | `READER_ROLE` |
| Gebruikersnaam | De gebruikersbenaming die wanneer het creëren van de verbinding wordt gekozen (die op de **toegang van Gegevens** pagina in Workfront* wordt gevonden) |
| Wachtwoord | Het wachtwoord dat is gekozen bij de eerste Snowflake-aanmelding* |

*For informatie over waar te om de **de toegang van Gegevens** pagina te vinden die uw Gegevens bevatten verbindt verbindingen, zie [ een lezer (dienst) rekening voor Snowflake ](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md) creëren.

>[!IMPORTANT]
>
>Zodra één ingang aan de IP lijst van gewenste personen wordt toegevoegd, zijn alle andere IP adressen niet meer toegestaan. Zorg ervoor dat u alle vereiste IP-adressen hebt ingevoerd, zowel voor het maken als voor het lezen van uw visualisatieprogramma, voordat u het gereedschap gaat gebruiken. Als dat niet het geval is, kan er een fout optreden met betrekking tot ongeldige referenties.
>
>Als u geen IP adressen inbegrepen in uw lijst van gewenste personen hebt maar nog problemen heeft die met een hulpmiddel verbinden BI, controleer de configuratie van de volmachtsserver voor het hulpmiddel van BI.

## Voeg IPs aan de lijst van gewenste personen toe

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Opstelling**.

1. In het linkerpaneel, klik **Systeem** > **Toegang van Gegevens**.

1. Klik op het **Toegestane IPs** lusje, dan klik op **een IP Adres aan uw Lijst van gewenste personen** knoop toevoegen.

1. Ga een naam voor het IP adres in **IP de beschrijving van het Adres** in en ga het IP adres (of blok CIDR) voor het hulpmiddel in u in **IP Adres** zou willen gebruiken, dan klik **IP aan Lijst van gewenste personen** toevoegen.

   ![ voeg IP adres ](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) toe {width="500"}

## Verwijder een IP adres uit de lijst van gewenste personen

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Opstelling**.

1. In het linkerpaneel, klik **Systeem** > **Toegang van Gegevens**.

1. Klik op het **Toegestane IPs** lusje, dan klik op het trashcan pictogram ![ pictogram van de Schrapping ](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) rechts van het IP adres u zou willen verwijderen.

1. In het venster dat verschijnt, controleer de doos om te bevestigen en dan **Schrapping** te klikken.

## Gegevens delen met Business Intelligence-tools

Een aantal gemeenschappelijke hulpmiddelen van de bedrijfsintelligentie wordt hieronder vermeld; de verbindingen zullen u aan de documentatieplaats van de dienst nemen om meer over het verbinden met uw gegevens meer te leren.

* [ Tableau ](https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm)
* [ Power BI ](https://learn.microsoft.com/power-query/connectors/snowflake)
* [ Domo ](https://www.domo.com/appstore/connector/snowflake-connector/overview)
* SAP HANA

## Gegevens opslaan in een extern gegevenspakhuis

Een aantal gemeenschappelijke gegevenspakhuizen wordt hieronder vermeld; de verbindingen zullen u aan de documentatieplaats van elke dienst brengen waar u meer over het verbinden met uw gegevens meer kunt leren.

* [ Gegevensbestanden ](https://docs.databricks.com/en/connect/index.html)
* [ AWS Redshift ](https://docs.aws.amazon.com/redshift/latest/gsg/federated-query.html)
