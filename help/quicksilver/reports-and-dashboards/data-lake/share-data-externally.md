---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Verbinding maken met Workfront Data Connect
description: Met Workfront Data Connect kunt u de Workfront-gegevens van uw organisatie gebruiken met de tools voor bedrijfsintelligentie of deze opslaan in een extern gegevenspakhuis.
author: Nolan
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: ea9c674b798c48927c7a0a542d36d5ded15ea3f1
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Verbinding maken met Workfront Data Connect

Met Workfront Data Connect kunt u de Workfront-gegevens van uw organisatie gebruiken met de tools voor bedrijfsintelligentie of deze opslaan in een extern gegevenspakhuis.

Om uw Gegevens aan te sluiten verbind gegevens meer met een extern product, moet u een verbinding eerst tot stand brengen zoals die in [&#x200B; wordt beschreven leidt tot een lezerrekening of een verbinding voor Snowflake &#x200B;](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md). Dan, moet u om het even welke vereiste IPs aan de lijst van gewenste personen toevoegen zoals die in [&#x200B; wordt beschreven voeg IPs aan de lijst van gewenste personen &#x200B;](#add-ips-to-the-allowlist) hieronder toe.

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

*For informatie over waar te om **Gegevens te vinden verbindt** pagina die uw verbindingen bevat, zie [&#x200B; een reader rekening of verbinding voor Snowflake &#x200B;](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md) creëren.

>[!IMPORTANT]
>
>Zodra één ingang aan de IP lijst van gewenste personen wordt toegevoegd, zijn alle andere IP adressen niet meer toegestaan. Zorg ervoor dat u alle vereiste IP-adressen hebt ingevoerd, zowel voor het maken als voor het lezen van uw visualisatieprogramma, voordat u het gereedschap gaat gebruiken. Als dat niet het geval is, kan er een fout optreden met betrekking tot ongeldige referenties.
>
>Als u geen IP adressen inbegrepen in uw lijst van gewenste personen hebt maar nog problemen heeft die met een hulpmiddel verbinden BI, controleer de configuratie van de volmachtsserver voor het hulpmiddel van BI.

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
        <li><p>Ultimate</p></li> 
    </ul>    
   <!--<p>Can be purchased as an add-on to the following plans:</p> 
    <ul>
        <li>Select</li> 
        <li>Prime</li>
    </ul>--> 
    <p>Workfront Data Connect is niet beschikbaar voor oudere Workfront-plannen.</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voeg IPs aan de lijst van gewenste personen toe

1. Klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Opstelling**.

1. In het linkerpaneel, klik **Systeem** > **Gegevens verbinden**.

1. Klik op het **Toegestane IPs** lusje, dan klik op **een IP Adres aan uw Lijst van gewenste personen** knoop toevoegen.

1. Ga een naam voor het IP adres in **IP de beschrijving van het Adres** in en ga het IP adres (of blok CIDR) voor het hulpmiddel in u in **IP Adres** zou willen gebruiken, dan klik **IP aan Lijst van gewenste personen** toevoegen.

   ![&#x200B; voeg IP adres &#x200B;](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) toe {width="500"}

## Verwijder een IP adres uit de lijst van gewenste personen

1. Klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Opstelling**.

1. In het linkerpaneel, klik **Systeem** > **Gegevens verbinden**.

1. Klik op het **Toegestane IPs** lusje, dan klik op het trashcan pictogram ![&#x200B; pictogram van de Schrapping &#x200B;](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) rechts van het IP adres u zou willen verwijderen.

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
