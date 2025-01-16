---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Webhaak toevoegen aan een basisscenario
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 6694b883-6f94-449c-bcfe-5a4053e8655a
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# Een webhaak toevoegen aan een basisscenario in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ voeg een webhaak aan een basisscenario ](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/add-a-webhook-to-basic-scenario.html) toe
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

Webhooks, ook wel &#39;instant triggers&#39; genoemd, zijn een specifiek type triggermodule dat een scenario kan starten wanneer een wijziging wordt aangebracht in plaats van volgens een bepaald schema.

In dit voorbeeld, zult u een website toevoegen om een scenario te beginnen zodra om het even welke verzoeken aan een specifieke rij zijn voorgelegd. Het scenario zet dan die verzoeken in een project om.

Dit voorbeeld wijzigt het scenario dat in [ wordt gecreeerd leidt tot een basisscenario ](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Vereisten

U moet het scenario tot stand brengen dat in [ wordt beschreven leidt tot een basisscenario ](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) alvorens deze procedure te volgen.

## Webhaak toevoegen en configureren

1. Open de module Object omzetten.
1. Verwijder het zwarte-id-blok in het veld Uitgave-id. Het blok is zwart omdat de module waarvan het is toegewezen niet meer beschikbaar is.
1. Selecteer het blok van identiteitskaart onder de eerste module (de Gebeurtenissen van het Controle) om het aan de tweede module in kaart te brengen.
1. Klik **OK**.

### De module Webhaak toevoegen

1. Open het scenario in de scenarioredacteur.
1. Klik op de eerste module met de rechtermuisknop aan en selecteer **module van de Schrapping**.

   De module wordt verwijderd en er blijft een lege tijdelijke aanduiding achter.

1. Klik de lege module, en selecteer **Adobe Workfront** van de lijst van apps.
1. Selecteer **Gebeurtenissen van het Controle**.
1. Klik **toevoegen** naast het gebied van de Webhaak.
1. op het gebied van het Type van Verslag, uitgezochte **Uitgave**, zodat zal de module voor veranderingen in kwesties teweegbrengen.
1. Op het gebied van de Staat, uitgezochte **Nieuwe staat**. Dit is een verplicht veld dat wordt gebruikt voor het filter, dat in dit voorbeeld niet wordt weergegeven.
1. Op het gebied van de Oorsprong van het Verslag, selecteer **Nieuw slechts Verslag**. Dit staat het scenario toe om te teweegbrengen wanneer een kwestie wordt toegevoegd, niet wanneer men wordt bijgewerkt of geschrapt.
1. Klik **sparen** om de moduleconfiguratie te bewaren.
