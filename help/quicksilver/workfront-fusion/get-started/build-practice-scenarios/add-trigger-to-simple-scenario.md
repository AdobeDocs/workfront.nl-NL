---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Een triggermodule toevoegen aan een basisscenario
description: Leer hoe te om een trekkermodule toe te voegen om het scenario toe te staan om periodiek naar nieuwe verzoeken te zoeken en hen in projecten om te zetten.
author: Becky
feature: Workfront Fusion
exl-id: 067ee6a1-f4c1-4602-ac39-0283255cced8
source-git-commit: 7ad3fbcfa5be5074016f399560cca509d81f4714
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# Een triggermodule toevoegen aan een basisscenario

De triggermodules worden aan het begin van een scenario geplaatst. Deze modules beginnen een scenario uitvoering wanneer specifieke criteria wanneer er een verandering in een bepaalde dienst is geweest. De wijziging kan bestaan uit het maken van nieuwe records, het verwijderen van records, het bijwerken van records, enzovoort.

De modules van de opiniepeiling controleren de dienst bij een vastgestelde tijdinterval en keren informatie over veranderingen terug die tijdens dat tijdinterval voorkwamen. Als er geen veranderingen zijn geweest, voert de trekker niet het scenario uit.

In dit voorbeeld, zult u een trekkermodule toevoegen die om de 15 minuten in werking stelt en begint een scenario als om het even welke verzoeken aan een specifieke rij zijn voorgelegd. Het scenario zet dan die verzoeken in een project om.

Dit voorbeeld wijzigt het scenario dat in [ wordt gecreeerd leidt tot een basisscenario ](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Vereisten

U moet het scenario tot stand brengen dat in [ wordt beschreven leidt tot een basisscenario ](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) alvorens deze procedure te volgen.

## De triggermodule toevoegen en configureren

### De triggermodule toevoegen

1. Open het scenario in de scenarioredacteur.
1. Klik op de eerste (Onderzoek) module met de rechtermuisknop aan en selecteer **module van de Schrapping**.

   De module wordt verwijderd en er blijft een lege tijdelijke aanduiding achter.

1. Klik de lege module, en selecteer **Adobe Workfront** van de lijst van apps.
1. Selecteer **Verslag van het Controle**.
1. Zorg ervoor dat de module de zelfde verbinding zoals de rest modules in het scenario gebruikt.
1. Op het gebied van de Filter, uitgezochte **Alleen Nieuwe Verslagen**.
1. Op het gebied van het Type van Verslag, uitgezochte **Uitgave**.
1. Selecteer `ID`, `Name` en `Project ID` in het vak Uitvoer.
1. Klik **O.K.** om de modulemontages te bewaren.

   Er verschijnt een venster waarin u wilt beginnen.

1. Selecteer **van nu op**.

### De triggermodule inplannen

1. Klik op de klok in de module Controleverslagen.

   Het venster Schema-instelling wordt geopend.

1. Op het het scenario van de Looppas gebied, selecteer **met regelmatige intervallen**.

1. Klik **OK**.

### De tweede module bijwerken

Omdat de eerste module is vervangen, moet de tweede module aan de nieuwe eerste module worden in kaart gebracht.

1. Open de module Object omzetten.
1. Verwijder het zwarte-id-blok in het veld Uitgave-id. Het blok is zwart omdat de module waarvan het is toegewezen niet meer beschikbaar is.
1. Selecteer het blok van identiteitskaart onder de eerste module (de Verslagen van het Controle) om het aan de tweede module in kaart te brengen.
1. Klik **OK**.

### Testen en activeren

1. Ga naar de Workfront-omgeving waarmee Fusion verbinding maakt en voeg een probleem toe.
1. Klik op **[!UICONTROL Run once]** in de linkerbenedenhoek van de scenarioeditor.
1. Onderzoek de output om ervoor te zorgen dat het scenario zoals verwacht liep.
1. Wanneer u wordt tevreden dat het scenario zoals verwacht werkt, klik **plannend** knevel in laag-linkervan het scherm aan ****.

   Dit activeert het scenario.
1. Klik in [!DNL Workfront Fusion] in de linkerbenedenhoek op **[!UICONTROL Save]** om de voortgang van het scenario op te slaan.

   >[!IMPORTANT]
   >
   >Sla de bestanden vaak op terwijl u ze gebruikt en test een scenario.

## Bronnen

* Voor meer informatie over webhooks, zie [ Onmiddellijke trekkers (webhooks) in  [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/webhooks/instant-triggers-webhooks.md).
