---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Tableau Desktop kan geen verbinding tot stand brengen
description: Wanneer u probeert om Desktop van Tableau aan Gegevens te verbinden verbindt, krijgt u een fout.
author: Courtney
feature: Reports and Dashboards
source-git-commit: e8b1d553ac4761e2b6eae79ae384956105939d90
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# Tableau Desktop kan geen verbinding tot stand brengen

## Probleem

Wanneer u probeert om Desktop van Tableau aan Gegevens te verbinden verbindt, ziet u de volgende fout:

`Cannot load data into PowerBI. Receiving an HY000 [Microsoft][Snowflake] (25) message`

## Oorzaak

Deze fout wordt veroorzaakt door een proxyinstelling op uw lokale computer die voorkomt dat gegevens worden geladen via Data Connect.

Data Connect wordt geleverd via Snowflake-cloudservices van derden. Voor tableau is een netwerk nodig dat is geopend voor communicatie met Snowflake.

## Oplossing

U kunt het volgende proberen om dit probleem op te lossen:

* **lost problemen door uw veiligheidshulpmiddel** onbruikbaar te maken op: Draai van uw veiligheidshulpmiddel, zoals Zscaler of Cisco, om te zien of lost het de connectiviteitskwestie op. Als dit de verbindingskwestie verhelpt, zorg ervoor dat uw veiligheidshulpmiddel aan de recentste versie wordt bevorderd, voeg het adres van Gegevens toe verbindt (Snowflake) IP aan de lijst van gewenste personen van VPN met uw intern netwerkteam.

* **voegt IP Adressen aan Lijst van gewenste personen** toe: Zorg ervoor dat uw firewallmontages de IP adressen toestaan die door Gegevens worden gebruikt verbinden. Gebruik het bevel `SYSTEM$ALLOWLIST()` om het IP adres te verkrijgen, dat u dan lijst van gewenste personen in VPN kunt.

* **de firewall en Montages van de Volmacht van de Controle**: Controle als om het even welke firewall of volmachtsconfiguraties op uw netwerk toegang tot Snowflake endpoints blokkeren. U zou uw netwerkbeheerder kunnen moeten contacteren om de vereiste Snowflake IP adressen en de havens aan de lijst van gewenste personen van uw bedrijf toe te voegen.

* **Optie van de Oplossing**: Creeer een extract van een aantekenvelscherm in plaats van de ruit van Gegevens Source in Tableau. De verbinding gaat niet verloren en het extractieproces is voltooid.

