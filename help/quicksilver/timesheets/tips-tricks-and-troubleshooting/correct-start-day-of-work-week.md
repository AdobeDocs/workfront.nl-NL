---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: De begindag van de werkweek voor Timesheets corrigeren
description: De begindag van de week op mijn timesheet past niet de begindag van de week aan die op mijn timesheet profiel wordt gevormd.
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# De begindag van de werkweek voor Timesheets corrigeren

## Probleem

De begindag van de week op mijn timesheet komt niet overeen met de begindag van de week die op mijn timesheet-profiel is geconfigureerd (zoals beschreven in [Werkbladprofielen maken, bewerken en toewijzen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).).

## Oplossing

De begindag van de week van een tijdblad in Adobe Workfront gebruikt de taal- en landinstellingen in uw browser om de dag van de week te bepalen. Daarom moet u de taal- en landinstellingen voor uw browser bijwerken. 

Als de browsertaal bijvoorbeeld is ingesteld op Engels en de landinstelling is ingesteld op Verenigde Staten, begint de week op zondag. Als alternatief is de browsertaal ingesteld op Engels en de landinstelling ingesteld op Verenigd Koninkrijk, de startdag is maandag.

Deze instelling heeft ook invloed op de begindag van de week in de pop-upkalenders op het systeem.

De wijziging van de landinstelling heeft geen invloed op de begindag van de week op het Resource Grid (of de weergave van het resourraster). De week begint altijd op zondag.

Hier volgt een overzicht van de aanwijzingen voor het wijzigen van de taal- en landinstellingen voor verschillende browsers die worden ondersteund door Workfront.

* **Chroom:** Kopieer en plak de volgende koppeling in uw Chrome-browser: `chrome://settings/languages` ga vervolgens naar Talen.
* **Firefox:**Kopieer en plak de volgende koppeling in uw Firefox-browser: `about:preferences#content` ga vervolgens naar Talen.
* **IE 11:** Gereedschappen -> Internetopties -> Algemeen -> Talen
* **Safari:** Helaas is het met Safari niet mogelijk webbrowseringstalen te wijzigen zonder ook de taal van het besturingssysteem te wijzigen. Het is waarschijnlijk gemakkelijker om een andere browser zoals Chrome of Firefox te installeren.

 
