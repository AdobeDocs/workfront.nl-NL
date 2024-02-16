---
product-previous: mobile
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: 2019.3 Integratie en mobiele verbeteringen
description: Deze pagina bevat een beschrijving van alle wijzigingen die zijn aangebracht in de integratie en mobiele verbeteringen van de release 2019.3. Het werd in de week van 19 augustus 2019 beschikbaar gesteld in de productieomgeving.
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 15e03405-63ff-48ea-b873-cf44f1f46282
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# 2019.3 Integratie en mobiele verbeteringen

Deze pagina bevat een beschrijving van alle wijzigingen die zijn aangebracht in de integratie en mobiele verbeteringen van de release 2019.3. Het werd in de week van 19 augustus 2019 beschikbaar gesteld in de productieomgeving.

Voor een lijst met alle wijzigingen die in 2019 zijn aangebracht, raadpleegt u [Overzicht van releaseactiviteiten 2019.3](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Ondersteuning voor gedeelde items in de MS OneDrive-integratie

Nu kunt u uw gedeelde OneDrive-bestanden en -mappen koppelen aan Workfront-objecten. Omgekeerd kunt u bestanden in Workfront uploaden naar gedeelde mappen in OneDrive.

Zie de secties voor meer informatie [Een extern document koppelen aan Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents), [Een of meer externe mappen koppelen](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-a-folder), en [Een document van Workfront bijwerken en koppelen aan een externe cloud provider](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) in het artikel [Documenten van externe toepassingen koppelen](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Zie de sectie [Een extern document koppelen aan Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in het artikel [Documenten van externe toepassingen koppelen](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Domeinspecificatie vereist voor alle Workfront-aanmeldingen

Alle Workfront-aanmeldingen vereisen nu dat de gebruiker het domein opgeeft als het domein nog niet is opgegeven in de Workfront-URL. Door deze gegevens te vereisen, wordt je Workfront-exemplaar veiliger. Als uw implementatie van Workfront meerdere exemplaren bevat, kunt u met deze verbetering dezelfde gebruiker toevoegen aan elke instantie van Workfront binnen uw implementatie.

Deze wijziging kan van invloed zijn op zowel gebruikersaanmeldingen als API-integratie:

* **Gebruikersaanmeldingen**

  Als uw bedrijfsdomein niet in Workfront URL wordt omvat, ziet u nu een nieuw gebied van het Domein op het login scherm naast de gebieden van de Gebruikersnaam en van het Wachtwoord.

  Voor de meeste klanten is geen wijziging vereist omdat de domeininformatie al in de Workfront-URL is opgenomen. Bijvoorbeeld &quot;*domein*.my.workfront.com.&quot;

* **API-integratie**

  Als u API-code hebt die naar een adres gaat dat uw domeinnaam niet bevat, werkt die API-code niet meer.

Zie voor meer informatie [Aanmelden bij Adobe Workfront](../../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/log-in-to-workfront.md).

## Taken en problemen converteren naar projecten met de mobiele app op iOS

U kunt nu afzonderlijke taken en uitgaven converteren naar projecten in de mobiele app Workfront op iOS.

## Meld u aan bij de mobiele app met vingerafdruk of gezicht-id

Afhankelijk van uw apparaat kunt u zich aanmelden bij de mobiele app van Workfront met vingerafdruk- of gezichts-id-technologie. Wanneer u zich bij mobiele app aanmeldt, wordt u gevraagd of u zich wilt aanmelden met de verificatiemethode die door uw telefoon wordt ondersteund.

Voor meer informatie over hoe te om deze eigenschap te beheren, zie [Adobe Workfront voor iOS](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md) of [Adobe Workfront voor Android](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md).

## Nieuwe instelling waarmee gebruikers automatisch worden afgemeld bij mobiele apparaten

Gebruikers worden na 15 dagen inactiviteit automatisch afgemeld om de mobiele app van Workfront veiliger te maken voor u en uw bedrijf. Workfront-beheerders kunnen deze tijdlimiet aanpassen in de webtoepassing via Setup > Systeem > Voorkeuren.

Zie voor meer informatie [Systeembeveiligingsvoorkeuren configureren](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Mobiele toepassing vereist domein bij aanmelden

Voor een betere beveiliging vereist de Workfront Mobile App nu dat u uw domein opgeeft als u zich niet aanmeldt met Single Sign-On-referenties.

>[!NOTE]
>
>Beschikbaarheid iOS: 12 juni 2019
>
>Beschikbaarheid van productie: 17 juni 2019

## Objecten verwijderen met de toepassing Mobile op iOS

>[!NOTE]
>
>Deze functie is in de week van 19 augustus 2019 beschikbaar gesteld in de App-winkels voor iOS.

U kunt nu objecten zoals taken, problemen en tijdbladen verwijderen in de mobiele app van iOS. U moet over de juiste machtigingen voor het object beschikken om het te verwijderen.

## Filteren op projecten met de dood in de mobiele app

>[!NOTE]
>
>Deze functie is beschikbaar in de app-winkels voor zowel iOS als Android in de week van 19 augustus 2019.

We hebben Dode projecten als filteroptie toegevoegd op het tabblad Projecten in de mobiele app.

## Wachtwoord opnieuw instellen met de mobiele toepassing

U kunt de Workfront Mobile-app gebruiken om uw wachtwoord opnieuw in te stellen als u het vergeten bent. Wachtwoord vergeten tikken? en volgt u de aanwijzingen op het scherm. U kunt uw SSO-wachtwoord niet opnieuw instellen in de mobiele app.

## Nieuwe look en feel voor mobiele apparaten

We hebben de volgende verbeteringen toegevoegd om uw ervaring in de Workfront Mobile-app te verbeteren.

* Verplaatst het volgende van de hoogste bar van de pagina van Details naar prominent gebieden op het scherm:

   * Het plusteken bevindt zich nu in de linkerbenedenhoek van het scherm
   * Het vinkje om aan een punt te beginnen werken is nu het Werk aan het knoop in het hoogste midden van het scherm

* U kunt bijgevoegde aangepaste formulieren nu weergeven door onder aan de pagina Details op Meer tonen te tikken.
* De weergave van de pagina&#39;s die u gebruikt om taken, problemen en verzoeken in te dienen, is gewijzigd.

