---
title: andere updates tijdens de releaseperiode van 22.3
description: andere updates tijdens de releaseperiode van 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 22.3 Andere verbeteringen

Op deze pagina worden alle andere verbeteringen beschreven die zijn aangebracht met de versie 22.3 voor de voorvertoningsomgeving. Deze verbeteringen zijn in de week van 11 juli 2022 beschikbaar gesteld in de productieomgeving. Voor een lijst van alle veranderingen beschikbaar met de versie 22.3, zie [&#x200B; overzicht van de Versie 22.3 &#x200B;](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Bijgewerkte tijdbladen

We blijven uw ervaring verbeteren en bijwerken wanneer we met tijdbladen werken. Hieronder vindt u een aantal functies die in deze update zijn opgenomen:

* Een nieuwe look en feel die passen bij de nieuwe Workfront-ervaring.

* De functionaliteit Automatisch opslaan om uw geregistreerde uren en urenopmerkingen automatisch op te slaan als u deze tweede keer toevoegt.

* Een intuïtievere pagina-indeling die overeenkomt met andere objectpagina&#39;s. We hebben bijvoorbeeld een linkerdeelvenster toegevoegd aan de tijdlijn. De tijdlijnupdates worden nu weergegeven in de sectie Updates in het linkerdeelvenster. U kunt een timesheet van de timesheet pagina ook schrappen evenals timesheet aan uw lijst van Favorieten toevoegen.

* Een betere ervaring wanneer het zoeken naar en het toevoegen van projecten, taken, of kwesties aan timesheet. Dit komt overeen met de ervaring in alle andere lijsten in Workfront.

* Het deelvenster Samenvatting is beschikbaar voor taken en problemen waarmee u direct vanuit de tijdlijn opmerkingen kunt toevoegen of gegevens kunt bijwerken.


Met de huidige update hebben we ook de volgende functies vervangen:

* Het maken van een taak uit een update is verwijderd. Deze functie is verwijderd sinds de release van 2018.2 uit de gebieden Updates van alle andere objecten, maar was nog steeds beschikbaar in de update-stream van het tijdblad.

* &quot;Voeg uitgaven van een timesheet toe. &quot;de voorkeur is verwijderd uit het gebied van de Voorkeur van Timesheet &amp; van Uren van Opstelling en u kunt geen uitgaven van timesheet meer registreren. U kunt nog uitgaven van de taak en projectpagina&#39;s registreren.


Raadpleeg de volgende artikelen voor meer informatie:

* [De lay-out Timesheet begrijpen](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)

* [Voorkeuren voor tijdpagina&#39;s en uren configureren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)


## Verbeteringen voor het linkernavigatievenster

We hebben verschillende verbeteringen aangebracht in het linkernavigatievenster in Adobe Workfront.

* De vormgeving van het linkernavigatievenster is aangepast aan de ontwerpstandaarden van de Adobe, waaronder kleuren en lettertypen.

* De koppeling &#39;Aangepaste sectie toevoegen&#39; onder aan het deelvenster heeft de naam &#39;Dashboard toevoegen&#39; gekregen om de functie beter uit te leggen.

## Automatisch vernieuwen van token-rotatie inschakelen in uw aangepaste OAuth2-toepassingen

Om u meer controle over de veiligheid van uw douaneOAuth2 toepassingen toe te staan, hebben wij aan optie toegevoegd om symbolenomwenteling toe te laten verfrissen. Wanneer deze optie wordt toegelaten, telkens als een vernieuwingstoken wordt gebruikt, creeert uw toepassing automatisch en verzendt nieuw verfrist teken, en maakt oude onbruikbaar.

Uw toepassing moet het nieuwe vernieuwingstoken opslaan na elke verfrissing. Workfront slaat dit token voor vernieuwen niet op.

Eerder, vernieuw tokens verliepen na een vastgestelde hoeveelheid tijd die in de douane OAuth2 toepassingsmontages wordt gevormd.

Voor meer informatie, zie [&#x200B; toepassingen OAuth2 voor de integratie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md) creëren.

## PKCE gebruiken in uw aangepaste OAuth2-integratie voor webtoepassingen van één pagina

U kunt nu webtoepassingen van één pagina maken in uw aangepaste integratie met PKCE. PKCE is een veilige autorisatiestroom die goed werkt bij dynamisch vernieuwende toepassingen zoals mobiele apps, maar waardevol is voor alle OAuth2-clients. In plaats van een statisch clientgeheim gebruikt PKCE een dynamisch gegenereerde tekenreeks, waardoor het risico van een gelekt clientgeheim wordt verwijderd.

Eerder, gebruikten de beschikbare opties voor douane OAuth2 toepassingen of de naam en het wachtwoord van een gebruiker, of een cliëntgeheim.

Voor meer informatie, zie [&#x200B; toepassingen OAuth2 voor de integratie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md) creëren.
