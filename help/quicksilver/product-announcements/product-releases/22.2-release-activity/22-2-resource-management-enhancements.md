---
title: 22.2 Verbeteringen in het beheer van hulpbronnen
description: 22.2 Verbeteringen in het beheer van hulpbronnen
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# 22.2 Verbeteringen in het beheer van hulpbronnen

Op deze pagina worden alle verbeteringen in het beheer van bronnen beschreven die zijn aangebracht met de release 22.2 voor de voorvertoningsomgeving. Deze verbeteringen worden beschikbaar gesteld in de productieomgeving

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

de week van 4 april 2022.

Voor een lijst met alle wijzigingen die beschikbaar zijn in de release 22.2 raadpleegt u [22.2 Overzicht van de release](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Verbeteringen voor de navigatie van Workload Balancer

Om uw ervaring te verbeteren wanneer het gebruiken van de Balancer van de Werkbelasting, hebben wij de volgende verhogingen geïntroduceerd:

* De knoppen Annuleren en Opslaan bij het aanpassen van toewijzingen blijven nu behouden, zelfs als de taak langer is dan de tijdlijn die op het scherm wordt weergegeven of als het deelvenster Samenvatting wordt weergegeven.
* Het linkerpaneel dat de namen van gebruikers en het werkpunten toont is nu kleverig, om u toe te staan horizontaal voor langere chronologie te scrollen en de namen van punten nog te kunnen lezen die in het paneel worden vermeld.
* U kunt alle items in het linkerdeelvenster samenvouwen en uitvouwen met één klik in plaats van op gebruiker- of projectniveau.
* U kunt nu ook het formaat van het linkerdeelvenster wijzigen.
* Er is nu een modus Volledig scherm voor werklastbalans.

Zie voor meer informatie over het navigeren in Workload Balancer [Navigeren door werklastbalans](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Toegang tot geavanceerde toewijzingen in Workload Balancer

Om het toewijzen van werkitems eenvoudiger en nauwkeuriger te maken, kunt u nu geavanceerde toewijzingen maken wanneer u handmatig werkitems toewijst in Workload Balancer. Voorafgaand aan deze verbetering, kon u tot Geavanceerde Toewijzingen toegang hebben wanneer het uitgeven van punten, van de kopballen van punten, of in lijsten.

Zie voor meer informatie [Handmatig werk toewijzen met Workload Balancer](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Nieuwe formule voor het berekenen van de beschikbaarheid van gebruikers wanneer de voorkeur Standaardschema wordt geselecteerd

Om nauwkeuriger informatie in middelbeheersinstrumenten te verstrekken, hebben wij de formule veranderd die Workfront gebruikt om gebruikersbeschikbaarheid te berekenen wanneer de beheerder van Workfront het StandaardProgramma in de Voorkeur van het Beheer van het Middel selecteert. Met de nieuwe update gebruikt Workfront de volgende formule om de beschikbaarheid van de gebruiker te berekenen:

Beschikbare uren gebruiker = (standaardplanninguren - Uitzonderingen) &#42; FTE - Uitgestelde tijd

Vóór deze update gebruikte Workfront de volgende formule om de beschikbaarheid van de gebruiker te berekenen toen het standaardschema werd geselecteerd:

Beschikbare uren gebruiker = (Standaardplanninguren - (Uitzonderingen schema + Verkeerde uren)) &#42; FTE-waarde gebruiker

Zie voor meer informatie [Voorkeuren voor beheer van bronnen configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

