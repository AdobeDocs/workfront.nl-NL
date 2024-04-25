---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data lake
title: Een verbinding tot stand brengen met het datumpigment van Workfront
description: Met Workfront-datumpigment kunt u de Workfront-gegevens van uw organisatie gebruiken met populaire tools voor bedrijfsintelligentie of deze opslaan in een extern gegevenspakhuis.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: e5bd25315062ad15ccd3448e008dfe94f1b616da
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Een verbinding tot stand brengen met het datumpigment van Workfront

Met Workfront-datumpigment kunt u de Workfront-gegevens van uw organisatie gebruiken met de tools voor bedrijfsintelligentie of deze opslaan in een extern gegevenspakhuis.

Om uw gegevens van het gegevensMeer van Workfront met een extern product te verbinden, moet u om het even welke vereiste IPs aan de lijst van gewenste personen eerst toevoegen zoals die in wordt beschreven [Voeg IPs aan de lijst van gewenste personen toe](#add-ips-to-the-allowlist) hieronder. Bovendien zullen de meeste producten extra informatie over uw gegevens meer vereisen om een verbinding te vestigen:

| Veldnaam | Waarde |
|---------------|-------------|
| Server | De URL voor de verbinding, zonder `https://` gedeelte (aangetroffen op de **Toegang tot gegevens** pagina in Workfront*) |
| Poort | `443` |
| Database | `WORKFRONT` |
| Warehouse | `READER_WH` |
| Schema | `WF` |
| Rol | `READER_ROLE` |
| Gebruikersnaam | De gebruikersnaam die u hebt gekozen bij het maken van de verbinding (bevindt zich op het tabblad **Toegang tot gegevens** pagina in Workfront*) |
| Wachtwoord | Het wachtwoord dat is gekozen bij de eerste Snowflake-aanmelding* |

*Voor informatie over waar u de **Toegang tot gegevens** pagina die uw gegevens bevat, zie [Een reader-account (service) maken voor Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Zodra één ingang aan de IP lijst van gewenste personen wordt toegevoegd, zijn alle andere IP adressen niet meer toegestaan. Zorg ervoor dat u alle vereiste IP-adressen hebt ingevoerd, zowel voor het maken als voor het lezen van uw visualisatieprogramma, voordat u het gereedschap gaat gebruiken. Als dat niet het geval is, kan er een fout optreden met betrekking tot ongeldige referenties.

## Voeg IPs aan de lijst van gewenste personen toe

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon-left-nav.png) in de linkerbovenhoek klikt u op **Instellen**.

1. Klik in het linkerdeelvenster op **Systeem** > **Gegevenstoegang**.

1. Klik op de knop **Toegestane IPs** en klikt u op de knop **Voeg een IP Adres aan uw Lijst van gewenste personen toe** knop.

1. Voer een naam in voor het IP-adres in **Beschrijving van IP-adres** en voer het IP-adres in voor het gereedschap waarin u wilt gebruiken **IP-adres** en klik vervolgens op **IP toevoegen aan Lijst van gewenste personen**.

   ![IP-adres toevoegen](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Verwijder een IP adres uit de lijst van gewenste personen

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon-left-nav.png) in de linkerbovenhoek klikt u op **Instellen**.

1. Klik in het linkerdeelvenster op **Systeem** > **Gegevenstoegang**.

1. Klik op de knop **Toegestane IPs** en klik vervolgens op het pictogram van de prullenbak ![Pictogram Verwijderen](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) rechts van het IP-adres dat u wilt verwijderen.

1. Schakel in het venster dat wordt weergegeven het selectievakje ter bevestiging in en klik op **Verwijderen**.

## Gegevens delen met Business Intelligence-tools

Een aantal gemeenschappelijke hulpmiddelen van de bedrijfsintelligentie wordt hieronder vermeld; de verbindingen zullen u aan de documentatieplaats van de dienst nemen om meer over het verbinden met uw gegevens meer te leren.

* [Tableau](https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm)
* [Power BI](https://learn.microsoft.com/power-query/connectors/snowflake)
* [Domo](https://www.domo.com/appstore/connector/snowflake-connector/overview)
* SAP HANA

## Gegevens opslaan in een extern gegevenspakhuis

Een aantal gemeenschappelijke gegevenspakhuizen wordt hieronder vermeld; de verbindingen zullen u aan de documentatieplaats van elke dienst brengen waar u meer over het verbinden met uw gegevens meer kunt leren.

* [Databricks](https://docs.databricks.com/en/connect/index.html)
* [AWS Redshift](https://docs.aws.amazon.com/redshift/latest/gsg/federated-query.html)
