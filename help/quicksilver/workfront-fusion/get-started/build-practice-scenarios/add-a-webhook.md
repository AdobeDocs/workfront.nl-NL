---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Webhaak toevoegen aan een basisscenario
description: Webhooks, ook wel 'instant triggers' genoemd, zijn een specifiek type triggermodule dat een scenario kan starten wanneer een wijziging wordt aangebracht in plaats van volgens een bepaald schema.
author: Becky
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Webhaak toevoegen aan een basisscenario in [!DNL Adobe Workfront Fusion]

Webhooks, ook wel &#39;instant triggers&#39; genoemd, zijn een specifiek type triggermodule dat een scenario kan starten wanneer een wijziging wordt aangebracht in plaats van volgens een bepaald schema.

In dit voorbeeld, zult u een website toevoegen om een scenario te beginnen zodra om het even welke verzoeken aan een specifieke rij zijn voorgelegd. Het scenario zet dan die verzoeken in een project om.

In dit voorbeeld wordt het scenario gewijzigd dat in [Een basisscenario maken](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Vereisten

U moet het scenario creëren dat in wordt beschreven [Een basisscenario maken](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) voordat deze procedure wordt gevolgd.

## Webhaak toevoegen en configureren

1. Open de module Object omzetten.
1. Verwijder het zwarte-id-blok in het veld Uitgave-id. Het blok is zwart omdat de module waarvan het is toegewezen niet meer beschikbaar is.
1. Selecteer het blok van identiteitskaart onder de eerste module (de Gebeurtenissen van het Controle) om het aan de tweede module in kaart te brengen.
1. Klikken **OK**.

### De module Webhaak toevoegen

1. Open het scenario in de scenarioredacteur.
1. Klik met de rechtermuisknop op de eerste module en selecteer **Module verwijderen**.

   De module wordt verwijderd en er blijft een lege tijdelijke aanduiding achter.

1. Klik op de lege module en selecteer **Adobe Workfront** uit de lijst met apps.
1. Selecteren **Gebeurtenissen bekijken**.
1. Klikken **Toevoegen** naast het veld Webhaak.
1. Selecteer in het veld Recordtype de optie **Probleem**, zodat zal de module voor veranderingen in kwesties teweegbrengen.
1. Selecteer in het veld Staat de optie **Nieuw frame**. Dit is een verplicht veld dat wordt gebruikt voor het filter, dat in dit voorbeeld niet wordt weergegeven.
1. Selecteer in het veld Oorsprong record de optie **Alleen nieuwe record**. Dit staat het scenario toe om te teweegbrengen wanneer een kwestie wordt toegevoegd, niet wanneer men wordt bijgewerkt of geschrapt.
1. Klikken **Opslaan** om de moduleconfiguratie te bewaren.


