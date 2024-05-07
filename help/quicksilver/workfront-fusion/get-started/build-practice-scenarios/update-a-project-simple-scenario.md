---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Een triggermodule toevoegen aan een basisscenario
description: Leer hoe te om een trekkermodule toe te voegen om het scenario toe te staan om periodiek naar nieuwe verzoeken te zoeken en hen in projecten om te zetten.
author: Becky
feature: Workfront Fusion
source-git-commit: 91d3dcde8eda416286c6781f6eef85404fd382c2
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Gebruik een functie om een project in een eenvoudig scenario bij te werken in [!DNL Adobe Workfront Fusion]

Het bijwerken van een Workfront-werkitem is een veelgebruikte manier om Workfront Fusion te gebruiken. In dit voorbeeld gebruikt u een functie om de naam van een project in hoofdletters te wijzigen.

Fusion omvat vele soorten functies die u toestaan om voorwaardelijke logica op uw gegevens om te zetten en uit te voeren. Zie voor meer informatie over het gebruik van functies [Informatie van de ene module toewijzen aan de andere in Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).

In dit voorbeeld wordt het scenario gewijzigd dat in [Een basisscenario maken](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Vereisten

U moet het scenario creëren dat in wordt beschreven [Een basisscenario maken](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) voordat deze procedure wordt gevolgd.

## Een functie gebruiken om een project bij te werken

### Voeg de module Record bijwerken toe aan uw scenario

1. Open het scenario in de scenarioredacteur.
1. Houd de muis boven de gedeeltelijke cirkel rechts van de module en klik vervolgens op **[!UICONTROL Add another module]**.
1. Selecteren [!DNL Adobe Workfront] van de lijst van toepassingen, dan kies de module **[!UICONTROL Update Record]**.
1. Selecteer in het veld Id het ID-blok dat zich onder de module Object Convert bevindt. Dit is identiteitskaart van het project dat output door die module was.

   ![ID van object Converteren](assets/id-convert-object.png)

1. Selecteer Project in het veld Type record, omdat het object dat u wilt bijwerken een project is.
1. Selecteer Naam in het gebied Selecteer velden voor kaart.

   Er wordt een naamveld geopend.

### De functie toewijzen voor de naamupdate

Wanneer dit scenario een verzoek in een project omzet, is de naam van het project het zelfde als het verzoek. De functie neemt deze naam en geeft alle letters in die naam een hoofdletter.

1. Klik op de knop **Naam** veld.

   Het deelvenster Toewijzing wordt geopend.
1. Klik in het deelvenster Toewijzing op de knop **Tekst- en binaire functies** pictogram. ![Pictogram Tekstfuncties](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-text&binary-functions.png)
1. Selecteer de functie **bovenste**.

   De functie wordt weergegeven in het veld Naam, inclusief de opmaak voor de invoer die de functie verwacht.

   De invoer voor dit voorbeeld is de naam van de uitgave waaruit het project is geconverteerd.

1. Plaats de cursor tussen de ronde haakjes, want dit is waar de invoer naartoe gaat.
1. Klik in het deelvenster Toewijzing op de knop **module-uitvoer** pictogram. ![Moduleuitvoerpictogram](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-functions-you-map-from-other-modules.png)
1. Selecteer het naamblok dat door de eerste module werd uitgevoerd.

   Het naamblok wordt weergegeven in de functie.

   ![Name block in function](assets/map-name.png)

1. Klik op OK om de moduleinstellingen op te slaan.

### Testen en activeren

1. Test het scenario door te klikken **Eenmaal uitvoeren** linksonder in het scherm.
1. Onderzoek de output om ervoor te zorgen dat het scenario zoals verwacht liep.
1. Wanneer u tevreden bent dat het scenario zoals verwacht werkt, klikt u op de knop **Planning** linksonder van het scherm schakelen naar **Aan**.

   Dit activeert het scenario. De actieve scenario&#39;s lopen volgens het programma dat in de trekkermodule wordt geplaatst.
1. In [!DNL Workfront Fusion], klikt u op **[!UICONTROL Save]** in de linkerbenedenhoek om de voortgang van het scenario op te slaan.

   >[!IMPORTANT]
   >
   >Sla de bestanden vaak op terwijl u ze gebruikt en test een scenario.

## Bronnen:

* [Items toewijzen met behulp van functies in [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)
