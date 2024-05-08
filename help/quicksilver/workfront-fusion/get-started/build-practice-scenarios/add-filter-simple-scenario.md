---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Een filter toevoegen aan een basisscenario
description: Met filters kunt u ervoor zorgen dat het scenario alleen vordert als aan bepaalde voorwaarden is voldaan.
author: Becky
feature: Workfront Fusion
source-git-commit: 5ba5b2e37e2ce58d96d11f24786feef57f8eb638
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Een filter toevoegen aan een basisscenario in [!DNL Adobe Workfront Fusion]

Met filters kunt u ervoor zorgen dat het scenario alleen vordert als aan bepaalde voorwaarden is voldaan.

In dit voorbeeld, zult u een filter aan uw scenario toevoegen dat een nieuw project om van een verzoek toelaat worden gecreeerd slechts als het verzoek aan een specifieke verzoekrij werd voorgelegd.

In dit voorbeeld wordt het scenario gewijzigd dat in [Een basisscenario maken](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

>[!NOTE]
>
>Workfront-triggermodules bevatten filters waarmee een scenario alleen kan worden gestart als aan bepaalde voorwaarden is voldaan. Omdat filters tussen modules echter worden gebruikt voor alle niet-triggertoepassingen en niet-Workfront-gebruiksscenario&#39;s, is het belangrijk te leren hoe u filters tussen modules kunt gebruiken. In dit voorbeeld wordt een filter tussen modules gebruikt voor functionaliteit waaraan een filter in de module kan worden voldaan.

## Vereisten

U moet het scenario creëren dat in wordt beschreven [Een basisscenario maken](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) voordat deze procedure wordt gevolgd.

## Een filter toevoegen

### Toevoegen van filter voorbereiden

1. Open het eerste scenario.
1. In de **Uitvoer** gebied, selecteren `Project`.
U moet nu `ID`, `Name`, en `Project` geselecteerd.
1. Klik op OK om de moduleinstellingen op te slaan.
1. Open Workfront.
1. In Workfront, bepaal de plaats van het project dat de verzoekrij vertegenwoordigt dat het scenario van de Fusie zal werken met.

   Dit project moet zich op dezelfde Workfront-account bevinden als de Fusion-verbinding.

1. Noteer de project-id in de URL.

   Voorbeeld: https://\&lt;mydomain>.my.workfront.com/project/\&lt;projectid>/taken

### Filter toevoegen en configureren

1. Open het scenario in de scenarioredacteur.
1. Klik op het moersleutelpictogram ![Perictogram](assets/wrench-icon.png) tussen de eerste en de tweede module en selecteer **Een filter instellen**.
1. Voer in het veld Label een label voor dit filter in, bijvoorbeeld &#39;Filter voor aanvraagwachtrij&#39;.
1. In de **Voorwaarde** in het bovenste veld de `projectID` uit de eerste module.

   ![Project-id toewijzen](assets/map-proj-id.png)
1. Laat de **Voorwaarde** operator als gelijk aan.
1. In het onderste veld van de **Voorwaarde** gebied, plak in de project-id die u hebt genoteerd via de project-URL in [Toevoegen van filter voorbereiden](#prepare-to-add-the-filter).
1. Klikken **OK** om de filterinstellingen op te slaan.

### Testen en activeren

1. Ga naar de Workfront-omgeving waarmee Fusion verbinding maakt en voeg een probleem toe aan het project dat u in het filter hebt opgegeven. Voeg een andere kwestie aan een verschillend project toe.
1. Klikken **[!UICONTROL Run once]** in de linkerbenedenhoek van de scenario-editor.
1. Onderzoek de output om ervoor te zorgen dat het scenario zoals verwacht liep.

   Beide kwesties zouden in de output van het eerste scenario moeten verschijnen, maar slechts zou de kwestie in het gespecificeerde project als input in het tweede scenario moeten verschijnen,
1. Wanneer u tevreden bent dat het scenario zoals verwacht werkt, klikt u op de knop **Planning** linksonder van het scherm schakelen naar **Aan**.

   Dit activeert het scenario.
1. In [!DNL Workfront Fusion], klikt u op **[!UICONTROL Save]** in de linkerbenedenhoek om de voortgang van het scenario op te slaan.

   >[!IMPORTANT]
   >
   >Sla de bestanden vaak op terwijl u ze gebruikt en test een scenario.

## Bronnen

* Zie voor meer informatie over filters [Een filter toevoegen aan een scenario](/help/quicksilver/workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

