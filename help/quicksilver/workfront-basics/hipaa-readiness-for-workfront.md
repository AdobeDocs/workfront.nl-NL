---
content-type: reference
navigation-topic: get-started-with-workfront
title: HIPAA-gereedheid voor Workfront
description: Een Workfront-klant die, zoals gedefinieerd in HIPAA, een Business Associate en/of de Covered Entiteit is namens wie de Business Associate Adobe Workfront verstrekt, moet de volgende richtlijnen gebruiken om Workfront voor gebruik geschikt voor HIPAA te configureren.
feature: Get Started with Workfront
author: Courtney
exl-id: e3cdaa03-d523-46a4-954b-8456d5f190e4
source-git-commit: 15a703e2292883427e371603f77a99765ed9d00a
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# HIPAA-gereedheid voor Workfront

Een Workfront-klant die, zoals gedefinieerd in HIPAA, een Business Associate en/of de Covered Entiteit is namens wie de Business Associate Adobe Workfront verstrekt, moet de volgende richtlijnen gebruiken om Workfront voor HIPAA-Ready gebruik te configureren:


## Wachtwoordvereisten

| **het Plaatsen van de Veiligheid** | **wat is het?** | **Vereiste** |
|----------------------|------------------|------------------|
| Minimale wachtwoordsterkte voor overeenkomsten | Wat is de minimumsterkte voor overeenkomstwachtwoorden? | Niet minder dan 8 tekens |
| Minimale wachtwoordsterkte voor gebruikerswachtwoorden | Wat is de minimumsterkte voor de wachtwoorden van gebruikers? | Teken van drie van de volgende categorieën:<br> * Hoofdletters (Latijn alfabet) <br> * Kleine letters (Latijn alfabet) <br> * Basis 10 cijfers <br> * Niet alfanumerieke karakters |
| Wachtwoordduur | Hoe lang zouden de wachtwoorden moeten worden toegestaan om onveranderd te blijven? | Wachtwoorden moeten ten minste om de 90 dagen worden gewijzigd |
| Wachtwoordgeschiedenis | Hoeveel wachtwoorden uit het verleden moeten worden onthouden en niet toegestaan? | Minimaal 5 |


## Aanmeldingsvereisten

| **het Plaatsen van de Veiligheid** | **wat is het?** | **Vereiste** |
|----------------------|------------------|------------------|
| Maximum aantal aanmeldfouten | Hoeveel mislukte login pogingen veroorzaken dat de gebruiker wordt gesloten uit? | Maximaal 5 pogingen binnen een periode van 5 minuten; probeer het na 30 minuten opnieuw |
| Maximale fout bij SSO-verificatie | Hoeveel mislukte SSO controlepogingen veroorzaken een lockout? | Maximaal 5 (alleen van toepassing op klanten die SSO gebruiken) |


## Sessievereisten

| **het Plaatsen van de Veiligheid** | **wat is het?** | **Vereiste** |
|----------------------|------------------|------------------|
| Time-out sessie | Hoeveel minuten van inactiviteit veroorzaken een logout? | Maximaal 15 minuten |

## Klantverantwoordelijkheden

Ervoor zorgen dat alle werknemers, vertegenwoordigers en/of agenten op de hoogte zijn van en begrip hebben voor de voorwaarden in de licentieovereenkomst en/of de dienstenovereenkomst(en) die tussen de partijen zijn gesloten, voor zover van toepassing, die relevant zijn voor het gebruik van gegevens met Workfront.

Met name moeten de volgende verantwoordelijkheden en verplichtingen worden herzien en meegedeeld: 

* De klant is verantwoordelijk voor het gebruik van de Workfront-service door alle gebruikers. 

* De klant moet voldoen aan alle voorwaarden van zijn overeenkomst met Adobe, die het uploaden van gegevens naar Workfront verbiedt. 

* Alle gevoelige gegevens, inclusief, maar niet beperkt tot ePHI, worden op eigen risico van de klant geüpload.  De klant is altijd verantwoordelijk voor alle klantgegevens. 


## Gegevensbescherming en naleving

>[!IMPORTANT]
>
>Workfront is niet ontworpen als gegevensopslagplaats voor elektronische medische dossiers (EHR&#39;s). ePHI mag alleen worden verwerkt indien Adobe hiervoor uitdrukkelijk schriftelijk toestemming heeft verleend. 

* Voor om het even welk gegevensbestand van Workfront waar ePHI toegankelijk zou kunnen zijn, verzeker **Encryptie bij Rest (EAR)** wordt toegelaten.
   * Neem contact op met uw accountmanager (AE) om te controleren of EAR is opgenomen in uw Workfront-aankoop.
   * Systemen/databases die via Workfront toegankelijk zijn, configureren om aan de verplichtingen te voldoen.
* Zorg ervoor dat ePHI niet wordt overgedragen, gekoppeld of gedeeld met andere Adobe-oplossingen die niet geschikt zijn voor HIPAA.
* Zorg ervoor dat patiëntenfoto&#39;s die via Workfront worden verwerkt, veilig en niet openbaar worden opgeslagen.
