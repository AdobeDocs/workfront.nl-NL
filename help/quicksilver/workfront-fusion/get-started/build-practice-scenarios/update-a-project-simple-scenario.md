---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Een triggermodule toevoegen aan een basisscenario
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: f4588063-024f-4520-986e-45342a6b6777
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---

# Een functie gebruiken om een project in een eenvoudig scenario bij te werken in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ Gebruik een functie om een project in een basisscenario bij te werken ](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/use-function-to-build-practice-scenario.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

Het bijwerken van een Workfront-werkitem is een veelgebruikte manier om Workfront Fusion te gebruiken. In dit voorbeeld gebruikt u een functie om de naam van een project in hoofdletters te wijzigen.

Fusion omvat vele soorten functies die u toestaan om voorwaardelijke logica op uw gegevens om te zetten en uit te voeren. Voor meer informatie bij het gebruiken van functies, zie [ informatie van de Kaart van één module aan een andere in de Fusie van Adobe Workfront ](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).

Dit voorbeeld wijzigt het scenario dat in [ wordt gecreeerd leidt tot een basisscenario ](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Vereisten

U moet het scenario tot stand brengen dat in [ wordt beschreven leidt tot een basisscenario ](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) alvorens deze procedure te volgen.

## Een functie gebruiken om een project bij te werken

### Voeg de module Record bijwerken toe aan uw scenario

1. Open het scenario in de scenarioredacteur.
1. Beweeg de cursor over de gedeeltelijke cirkel rechts van de sectie van de module en klik vervolgens op **[!UICONTROL Add another module]** .
1. Selecteer [!DNL Adobe Workfront] in de lijst met toepassingen en kies vervolgens de module **[!UICONTROL Update Record]** .
1. Selecteer in het veld Id het ID-blok dat zich onder de module Object Convert bevindt. Dit is identiteitskaart van het project dat output door die module was.

   ![ identiteitskaart van voorwerp van de Bekeerling ](assets/id-convert-object.png)

1. Selecteer Project in het veld Type record, omdat het object dat u wilt bijwerken een project is.
1. Selecteer Naam in het gebied Selecteer velden voor kaart.

   Er wordt een naamveld geopend.

### De functie toewijzen voor de naamupdate

Wanneer dit scenario een verzoek in een project omzet, is de naam van het project het zelfde als het verzoek. De functie neemt deze naam en geeft alle letters in die naam een hoofdletter.

1. Klik het **gebied van de Naam**.

   Het deelvenster Toewijzing wordt geopend.
1. In het mappingpaneel, klik het **Tekst en binaire functies** pictogram. ![ de functies van de Tekst pictogram ](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-text&binary-functions.png)
1. Selecteer de functie **bovenaan**.

   De functie wordt weergegeven in het veld Naam, inclusief de opmaak voor de invoer die de functie verwacht.

   De invoer voor dit voorbeeld is de naam van de uitgave waaruit het project is geconverteerd.

1. Plaats de cursor tussen de ronde haakjes, want dit is waar de invoer naartoe gaat.
1. In het toewijzende paneel, klik het **pictogram van de 0} moduleoutput {.** ![ het outputpictogram van de Module ](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-functions-you-map-from-other-modules.png)
1. Selecteer het naamblok dat door de eerste module werd uitgevoerd.

   Het naamblok wordt weergegeven in de functie.

   ![ het blok van de Naam in functie ](assets/map-name.png)

1. Klik op OK om de moduleinstellingen op te slaan.

### Testen en activeren

1. Test het scenario door **in werking te stellen eens** in de laag-linkerhoek van het scherm te klikken.
1. Onderzoek de output om ervoor te zorgen dat het scenario zoals verwacht liep.
1. Wanneer u wordt tevreden dat het scenario zoals verwacht werkt, klik **plannend** knevel in laag-linkervan het scherm aan ****.

   Dit activeert het scenario. De actieve scenario&#39;s lopen volgens het programma dat in de trekkermodule wordt geplaatst.
1. Klik in [!DNL Workfront Fusion] in de linkerbenedenhoek op **[!UICONTROL Save]** om de voortgang van het scenario op te slaan.

   >[!IMPORTANT]
   >
   >Sla de bestanden vaak op terwijl u ze gebruikt en test een scenario.

## Bronnen:

* [Items toewijzen met behulp van functies in  [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)
