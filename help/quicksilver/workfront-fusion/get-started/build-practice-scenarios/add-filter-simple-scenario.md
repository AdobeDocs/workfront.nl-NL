---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Een filter toevoegen aan een basisscenario
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: b43355ed-9329-4080-8e61-7177eb580994
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Een filter toevoegen aan een basisscenario in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ voeg een filter aan een basisscenario ](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/add-filter-basic-scenario.html) toe
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

Met filters kunt u ervoor zorgen dat het scenario alleen vordert als aan bepaalde voorwaarden is voldaan.

In dit voorbeeld, zult u een filter aan uw scenario toevoegen dat een nieuw project om van een verzoek toelaat worden gecreeerd slechts als het verzoek aan een specifieke verzoekrij werd voorgelegd.

Dit voorbeeld wijzigt het scenario dat in [ wordt gecreeerd leidt tot een basisscenario ](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

>[!NOTE]
>
>Workfront-triggermodules bevatten filters waarmee een scenario alleen kan worden gestart als aan bepaalde voorwaarden is voldaan. Omdat filters tussen modules echter worden gebruikt voor alle niet-triggertoepassingen en niet-Workfront-gebruiksscenario&#39;s, is het belangrijk te leren hoe u filters tussen modules kunt gebruiken. In dit voorbeeld wordt een filter tussen modules gebruikt voor functionaliteit waaraan een filter in de module kan worden voldaan.

## Vereisten

U moet het scenario tot stand brengen dat in [ wordt beschreven leidt tot een basisscenario ](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) alvorens deze procedure te volgen.

## Een filter toevoegen

### Toevoegen van filter voorbereiden

1. Open het eerste scenario.
1. In het **gebied van Output**, uitgezochte `Project`.
Nu moeten `ID` , `Name` en `Project` zijn geselecteerd.
1. Klik op OK om de moduleinstellingen op te slaan.
1. Open Workfront.
1. In Workfront, bepaal de plaats van het project dat de verzoekrij vertegenwoordigt dat het scenario van de Fusie zal werken met.

   Dit project moet zich op dezelfde Workfront-account bevinden als de Fusion-verbinding.

1. Noteer de project-id in de URL.

   Voorbeeld: https://\&lt;MyDomain\>.my.workfront.com/project/\&lt;ProjectID\>/tasks

### Filter toevoegen en configureren

1. Open het scenario in de scenarioredacteur.
1. Klik het moersleutelpictogram ![ pictogram van de Sleutel ](assets/wrench-icon.png) tussen de eerste en tweede module, en selecteer **Opstelling een filter**.
1. Voer in het veld Label een label voor dit filter in, bijvoorbeeld &#39;Filter voor aanvraagwachtrij&#39;.
1. Op het **gebied van de Voorwaarde**, op het hoogste gebied, kaart `projectID` van de eerste module.

   ![ het projectidentiteitskaart van de Kaart ](assets/map-proj-id.png)
1. Verlaat de **exploitant van de Voorwaarde** als Gelijk aan.
1. Op het bodemgebied van het **gebied van de Voorwaarde**, deeg in projectidentiteitskaart die u nota van van project URL in [ maakte voorbereidingen om de filter ](#prepare-to-add-the-filter) toe te voegen.
1. Klik **O.K.** om de filtermontages te bewaren.

### Testen en activeren

1. Ga naar de Workfront-omgeving waarmee Fusion verbinding maakt en voeg een probleem toe aan het project dat u in het filter hebt opgegeven. Voeg een andere kwestie aan een verschillend project toe.
1. Klik op **[!UICONTROL Run once]** in de linkerbenedenhoek van de scenarioeditor.
1. Onderzoek de output om ervoor te zorgen dat het scenario zoals verwacht liep.

   Beide kwesties zouden in de output van het eerste scenario moeten verschijnen, maar slechts zou de kwestie in het gespecificeerde project als input in het tweede scenario moeten verschijnen,
1. Wanneer u wordt tevreden dat het scenario zoals verwacht werkt, klik **plannend** knevel in laag-linkervan het scherm aan ****.

   Dit activeert het scenario.
1. Klik in [!DNL Workfront Fusion] in de linkerbenedenhoek op **[!UICONTROL Save]** om de voortgang van het scenario op te slaan.

   >[!IMPORTANT]
   >
   >Sla de bestanden vaak op terwijl u ze gebruikt en test een scenario.

## Bronnen

* Voor meer informatie over filters, zie [ een filter aan een scenario ](/help/quicksilver/workfront-fusion/scenarios/add-a-filter-to-a-scenario.md) toevoegen.
