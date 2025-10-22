---
title: 23.2 Verbeteringen in het beheer van hulpbronnen
description: 23.2 Verbeteringen in het beheer van hulpbronnen
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b225ae19-eee7-4329-a42d-2a2bf9adad01
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# 23.2 Verbeteringen in het beheer van hulpbronnen

Op deze pagina worden alle verbeteringen in het bronnenbeheer beschreven die zijn aangebracht met de release 23.2 voor de voorvertoningsomgeving. Deze verbeteringen worden beschikbaar gesteld in de productieomgeving met de release 23.2.

Voor een lijst van alle veranderingen beschikbaar op dit punt in de 23.2 versiecyclus, zie [&#x200B; 23.2 Overzicht van de Versie &#x200B;](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Het veld Werktijd introduceren om de gebruikerscapaciteit nauwkeurig te berekenen

>[!NOTE]
>
>Voorvertoningsrelease: 16 februari 2023; Planned Production release: 2 maart 2023

Om middelmanagers toe te staan om de beschikbaarheid van hun gebruikers nauwkeurig te berekenen en rekenschap te geven voor de tijd die de gebruikers aan daadwerkelijke, projectgerelateerde werk wijden, introduceren wij het concept van de Tijd van het Werk aan Adobe Workfront.

U kunt de waarde van het gebied van de Tijd van het Werk voor elke gebruiker bepalen, wanneer u creeert of hun profiel uitgeeft. Voor meer informatie, zie [&#x200B; het profiel van een gebruiker &#x200B;](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

Het gebied van de Tijd van het Werk vertegenwoordigt het percentage van de Equivalente tijd van de Volledige (FTE) tijd dat de gebruiker voor werkelijk werk, exclusief overheadkosten beschikbaar is. De Tijd van het werk moet een decimaal aantal met een waarde tussen 0 en 1 zijn. Een beschikbaarheid van 20% voor werkelijk werk zou bijvoorbeeld 0,2 zijn.

Het gebrek van het gebied is 1, erop wijzend dat een gebruiker hun volledige VTE op werkelijk besteedt, project-verwant werk.

Als gevolg van deze update berekent Workfront de beschikbaarheid van de gebruiker aan de hand van de onderstaande formules, afhankelijk van uw keuze in het voorkeurengebied voor resourcebeheer:

* Standaardschema:
* Gebruikerscapaciteit = [ (Planninguren - Planningsuitzonderingen) `*` VTE - Afgestane tijd ] `*` Tijdstip
* Planning gebruiker:
* Gebruikerscapaciteit = (Planninguren - Planningsuitzonderingen - Tijd uit) `*` Tijdstip van het werk.

Voor meer informatie, zie [&#x200B; [!UICONTROL Resource Management] voorkeur &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md) vormen.

[&#x200B; Bekijk een videodemonstratie van deze eigenschap &#x200B;](https://video.tv.adobe.com/v/3415608/){target=_blank}
