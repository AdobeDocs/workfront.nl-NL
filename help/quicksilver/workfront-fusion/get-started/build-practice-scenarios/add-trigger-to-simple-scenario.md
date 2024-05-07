---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Een triggermodule toevoegen aan een basisscenario
description: Leer hoe te om een trekkermodule toe te voegen om het scenario toe te staan om periodiek naar nieuwe verzoeken te zoeken en hen in projecten om te zetten.
author: Becky
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Een triggermodule toevoegen aan een basisscenario

De triggermodules worden aan het begin van een scenario geplaatst. Deze modules beginnen een scenario uitvoering wanneer specifieke criteria wanneer er een verandering in een bepaalde dienst is geweest. De wijziging kan bestaan uit het maken van nieuwe records, het verwijderen van records, het bijwerken van records, enzovoort.

De modules van de opiniepeiling controleren de dienst bij een vastgestelde tijdinterval en keren informatie over veranderingen terug die tijdens dat tijdinterval voorkwamen. Als er geen veranderingen zijn geweest, voert de trekker niet het scenario uit.

In dit voorbeeld, zult u een trekkermodule toevoegen die om de 15 minuten in werking stelt en begint een scenario als om het even welke verzoeken aan een specifieke rij zijn voorgelegd. Het scenario zet dan die verzoeken in een project om.

In dit voorbeeld wordt het scenario gewijzigd dat in [Een basisscenario maken](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Vereisten

U moet het scenario creëren dat in wordt beschreven [Een basisscenario maken](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) voordat deze procedure wordt gevolgd.

## De triggermodule toevoegen en configureren

### De triggermodule toevoegen

1. Open het scenario in de scenarioredacteur.
1. Klik met de rechtermuisknop op de eerste module (Zoeken) en selecteer **Module verwijderen**.

   De module wordt verwijderd en er blijft een lege tijdelijke aanduiding achter.

1. Klik op de lege module en selecteer **Adobe Workfront** uit de lijst met apps.
1. Selecteren **Record bekijken**.
1. Zorg ervoor dat de module de zelfde verbinding zoals de rest modules in het scenario gebruikt.
1. Selecteer in het veld Filter de optie **Alleen nieuwe records**.
1. Selecteer in het vak Uitvoer de optie `ID`, `Name`, en `Project ID`.
1. Klikken **OK** om de module-instellingen op te slaan.

   Er verschijnt een venster waarin u wilt beginnen.

1. Selecteren **Vanaf nu**.

### De triggermodule inplannen

1. Klik op de klok in de module Controleverslagen.

   Het venster Schema-instelling wordt geopend.

1. Selecteer in het scenario Uitvoeren de optie **Op gezette tijden**.

1. Klikken **OK**.

### De tweede module bijwerken

Omdat de eerste module is vervangen, moet de tweede module aan de nieuwe eerste module worden in kaart gebracht.

1. Open de module Object omzetten.
1. Verwijder het zwarte-id-blok in het veld Uitgave-id. Het blok is zwart omdat de module waarvan het is toegewezen niet meer beschikbaar is.
1. Selecteer het blok van identiteitskaart onder de eerste module (de Verslagen van het Controle) om het aan de tweede module in kaart te brengen.
1. Klikken **OK**.

### Testen en activeren

1. Ga naar de Workfront-omgeving waarmee Fusion verbinding maakt en voeg een probleem toe.
1. Klikken **[!UICONTROL Run once]** in de linkerbenedenhoek van de scenario-editor.
1. Onderzoek de output om ervoor te zorgen dat het scenario zoals verwacht liep.
1. Wanneer u tevreden bent dat het scenario zoals verwacht werkt, klikt u op de knop **Planning** linksonder van het scherm schakelen naar **Aan**.

   Dit activeert het scenario.
1. In [!DNL Workfront Fusion], klikt u op **[!UICONTROL Save]** in de linkerbenedenhoek om de voortgang van het scenario op te slaan.

   >[!IMPORTANT]
   >
   >Sla de bestanden vaak op terwijl u ze gebruikt en test een scenario.

## Bronnen

* Voor meer informatie over webhooks raadpleegt u [Instant triggers (webhaken) in [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/webhooks/instant-triggers-webhooks.md).
