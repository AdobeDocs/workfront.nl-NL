---
content-type: reference
navigation-topic: announcements
title: De klanten op Clusters 1, 2, en 3 moeten om het even welke lijst van gewenste personen IP blokken bijwerken om het blokkeren van de diensten van Adobe Workfront te verhinderen
description: Om onze kerninfrastructuur te verbeteren en te verbeteren, migreren we binnenkort Adobe Workfront-klanten in clusters 01, 02 en 03 naar de AWS-cloud.
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# De klanten op Clusters 1, 2, en 3 moeten om het even welke lijst van gewenste personen IP blokken bijwerken om het blokkeren van de diensten van Adobe Workfront te verhinderen

Om onze kerninfrastructuur te verbeteren en te verbeteren, migreren we binnenkort Adobe Workfront-klanten in clusters 01, 02 en 03 naar de AWS-cloud.

Als deel van deze verandering, moet u de volgende IPs aan uw lijst van gewenste personen IP blokken toevoegen om het blokkeren van de diensten van Workfront te verhinderen:

Voor SSO en POP:

* 34 215 145 168
* 54 69 155 48
* 35 160 44 226
* 34 213 96 218
* 3.16.2010,22
* 3.16.229,153
* 18 224 117 99
* 3.18.123.153
* 3 211 159 196
* 3 85 255,45
* 3 210 78 197
* 3 211 23 183

Voor e-mail:

* 54 240 60 174
* 54 240 60 175

Gelieve te verzekeren uw lijst van gewenste personen IP blokken tegen 13 mei 2019 worden bijgewerkt. Voor meer informatie, zie [ de lijst van gewenste personen van uw firewall ](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) vormen.

Hartelijk dank voor uw voortdurende ondersteuning van Workfront, aangezien wij werken aan een betrouwbaardere en robuustere ervaring voor onze klanten.

Als u nog vragen hebt, kunt u contact opnemen met ons ondersteuningsteam door naar experience.workfront.com te gaan of door 844.306.4357 (VS) of +44.1256.274200 (EMEA) te bellen.

## Veelgestelde vragen

### Waarom brengt Workfront deze verandering?

In een poging onze klanten consequent de best mogelijke service te bieden, zoekt Workfront voortdurend naar manieren om de gebruikerservaring te verbeteren. Deze verandering maakt gebruik van nieuwe technologieën die ons in staat stellen de beste ervaring mogelijk te maken en ons reeds robuuste veiligheidsmodel te verbeteren.

### Welke acties vereist ik als Workfront-beheerder?

Contacteer uw interne IT of veiligheidsafdeling voor hulp bij het herzien van uw lijst van gewenste personen IP blokken en in het toevoegen van hierboven vermelde IPs.

### Wat kan mijn organisatie verwachten als we deze wijziging niet doorvoeren?

U zult de diensten van Workfront niet kunnen toegang hebben aangezien wij de diensten aan nieuwe IPs migreren.
