---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: De begindag van de werkweek voor Timesheets corrigeren
description: De begindag van de week op mijn timesheet past niet de begindag van de week aan die op mijn timesheet profiel wordt gevormd.
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# De begindag van de werkweek voor Timesheets corrigeren

## Probleem

De begindag van de week op mijn timesheet past niet de begindag van de week aan die op mijn timesheet profiel (zoals die in [ wordt beschreven creeert, geeft uit, en wijst timesheet profielen ](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md) toe.)

## Oplossing

De begindag van de week van een tijdblad in Adobe Workfront gebruikt de taal- en landinstellingen in uw browser om de dag van de week te bepalen. Daarom moet u de taal- en landinstellingen voor uw browser bijwerken.

Als de browsertaal bijvoorbeeld is ingesteld op Engels en de landinstelling is ingesteld op Verenigde Staten, begint de week op zondag. Als alternatief is de browsertaal ingesteld op Engels en de landinstelling ingesteld op Verenigd Koninkrijk, de startdag is maandag.

Deze instelling heeft ook invloed op de begindag van de week in de pop-upkalenders op het systeem.

De wijziging van de landinstelling heeft geen invloed op de begindag van de week op het Resource Grid (of de weergave van het resourraster). De week begint altijd op zondag.

Hier volgt een overzicht van de aanwijzingen voor het wijzigen van de taal- en landinstellingen voor verschillende browsers die worden ondersteund door Workfront.

* **Chrome:** Kopieer en kleef de volgende verbinding in uw browser van Chrome: `chrome://settings/languages` ga dan naar Talen.
* **Firefox:**&#x200B;Kopieer en plak de volgende koppeling naar uw Firefox-browser: `about:preferences#content` ga vervolgens naar Talen.
* **IE 11:** Hulpmiddelen -> de Opties van Internet -> Algemeen -> Talen
* **Safari:** Jammer genoeg, staat Safari niet veranderende Web het doorbladeren talen toe zonder ook uw volledige werkend systeemtaal te veranderen. Het is waarschijnlijk gemakkelijker om een andere browser, zoals Chrome of Firefox, te installeren.


