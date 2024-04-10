---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: scenario,prestaties
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion-prestatiehandleidingen
description: Adobe Workfront Fusion vereist naast een Adobe Workfront-licentie een Adobe Workfront Fusion-licentie.
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: 00ef33666bebe434739056cb38c3dff24285d682
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] prestatiegerichte

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] vereist een [!DNL Adobe Workfront Fusion] naast een [!DNL Adobe Workfront license].

Voor werkautomatisering is snelle verwerking vereist, dus [!DNL Adobe Workfront Fusion] is ontworpen voor hoge prestaties. Omdat langdurige scenario&#39;s het tempo van uw werk kunnen vertragen, hebben wij ontworpen [!DNL Workfront Fusion] met prestatiebestendige instructies die de uitvoeringstijd, gegevensgrootte en andere scenario-parameters beperken. [!DNL Workfront Fusion] ontwerpers dienen zich bewust te zijn van deze waarborgen en deze op te nemen in hun ontwerppraktijken.

## Browsers

Workfront Fusion ondersteunt alleen op Chrome gebaseerde browsers.

## Scenarios

* De standaarduitvoeringstijd van het scenario is **40 minuten**. Wanneer de uitvoering deze time-out bereikt, [!DNL Workfront Fusion] onderbreekt de uitvoering van het scenario na de volgende cyclus of verrichting, afhankelijk van het scenario. Dit dwingt het scenario om kort na het bereiken van de limiet van 40 minuten te stoppen
* De maximumgrootte van een scenario-blauwdruk is **5 MB**, maar we raden aan de grootte van scenario&#39;s onder **3 MB**.

  App-modules die gegevens met een groot aantal velden maken of bijwerken, kunnen zeer grote blauwdrukken veroorzaken.

   * Wanneer u de opdracht [!DNL Workfront] -app, moet u alleen velden selecteren die nodig zijn voor het maken of bijwerken van gebruiksgevallen.
   * Wanneer u andere toepassingen gebruikt, gebruikt u aangepaste API-modules voor interactie met elk recordtype met een groot aantal velden.

* Terwijl er geen maximum voor het aantal modules in een scenario is, beïnvloeden de scenario&#39;s met meer dan 150 modules negatief de prestaties van uw [!DNL Workfront Fusion] systeem. Daarom adviseren wij het creëren van scenario&#39;s met meer dan 150 modules niet.

## Bewerkingen

* De standaardtime-out van de bewerking is doorgaans **40 seconden**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## Bestanden

* De totale verwerkingscapaciteit van Fusion voor bestanden is **1 GB**. De limiet is gebaseerd op de totale geheugenkosten. Elke operatie draagt aan die kosten bij. Als één bestand van 400 MB wordt gedownload en geüpload, kost de totale bestandscapaciteit 800 MB.

## Gebruik van servergeheugen

* Het geheugengebruik van de server voor één enkele uitvoering wordt beperkt tot **1 GB**.

  Veel factoren, zoals grote bestanden of complexe modules, kunnen het servergeheugengebruik beïnvloeden op manieren die moeilijk te voorspellen of te controleren zijn. Daarom kan de uitvoering van uw scenario de geheugenlimiet van 1 GB overschrijden, zelfs als het scenario alle andere prestatiegaranties volgt. Als de geheugenlimiet wordt overschreden, mislukt de uitvoering.

## Webhaken

* De standaard maximumgrootte van een lading is **5 MB**.
* Webhaken zijn beperkt tot **100 verzoeken per seconde**. Wanneer deze limiet is bereikt, verzendt Workfront Fusion een 429 ([!UICONTROL Too Many Requests]).
* [!DNL Workfront Fusion] slaat webshpayloads op voor 30 dagen. Als u meer dan 30 dagen na ontvangst een payload van een webhaak opent, treedt de fout op &quot;[!UICONTROL Failed to read file from storage.]&quot;
* Webhaken worden automatisch gedeactiveerd als een van de volgende twee situaties van toepassing is:

   * De webhaak is langer dan 5 dagen niet verbonden met een scenario
   * De webhaak wordt alleen gebruikt in inactieve scenario&#39;s, die al meer dan 30 dagen inactief zijn.

* gedeactiveerde webhaken worden automatisch verwijderd en niet geregistreerd als ze niet zijn aangesloten op scenario&#39;s en meer dan 30 dagen in de gedeactiveerde status zijn geweest.

## Uitvoeringshistorie

* Logbestanden met uitvoeringshistorie zijn beperkt tot een grootte van **100 MB**. Als de uitvoeringsgeschiedenis deze grootte overschrijdt, slechts zal eerste 100 MB worden getoond.

## Opnieuw

Wanneer het gebruiken van de module van de Onderbreking en het specificeren van de richtlijn van het Opnieuw proberen, als een scenario achtereenvolgens 10 keer binnen een 2 minieme chronologie ontbreekt, zal het scenario automatisch worden gedeactiveerd.

