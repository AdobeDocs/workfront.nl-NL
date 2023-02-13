---
content-type: reference
product-area: workfront-integrations
keywords: native,ootb
navigation-topic: workfront-integrations-navigation-topic
title: Adobe Workfront-integratiemethoden
description: U kunt [!DNL Adobe Workfront] met toepassingen van derden. Deze integratie kan het nut van [!DNL Workfront] en aan de behoeften van uw organisatie aanpassen. U kunt al deze integraties gebruiken, afhankelijk van welke integratie het meest geschikt is voor een bepaalde taak.
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 685186f76cd89e69eac0a07bff9a39e2e28f9429
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 0%

---

# Adobe Workfront-integratiemethoden

U kunt [!DNL Adobe Workfront] met toepassingen van derden. Deze integratie kan het nut van [!DNL Workfront] en aan de behoeften van uw organisatie aanpassen. U kunt al deze integraties gebruiken, afhankelijk van welke integratie het meest geschikt is voor een bepaalde taak.

## Ingebouwde integratie

Workfront biedt diverse integraties die u rechtstreeks vanuit Workfront kunt configureren, of vanuit een andere toepassing door de Workfront-invoegtoepassing voor die toepassing te installeren. Deze ingebouwde integratie bestrijkt veel veelvoorkomende gebruiksscenario&#39;s en richt zich op het uitbreiden en verbinden van gebruikerservaring voor eindgebruikers.

De ingebouwde integratie van Workfront richt zich hoofdzakelijk op persoonlijke productiviteit en samenwerking. Deze integratie reduceert onderbrekingen in de workflow van een individuele gebruiker, zodat deze Workfront-meldingen kan ontvangen, toegang krijgt tot informatie en op Workfront-werkitems kan reageren zonder de geïntegreerde toepassing te verlaten.

De voordelen van ingebouwde integratie kunnen het volgende omvatten:

* Veel van deze ingebouwde integraties zijn zonder extra kosten beschikbaar. (Andere gebruikers hebben wel een extra aankoop nodig.)
* De ingebouwde integratie omvat veel van de gemeenschappelijkste toepassingen die door ondernemingen, zoals Slack worden gebruikt, [!DNL Google Drive]of Adobe-producten zoals [!DNL Adobe Creative Cloud] of [!DNL Adobe Experience Manager] Elementen. Als uw bedrijf deze apps al gebruikt, verloopt de integratie probleemloos in de bestaande workflow van uw gebruikers.
* Integreren [!DNL Workfront] met een veelgebruikte toepassing kan de acceptatie bij uw gebruikers verhogen.

>[!INFO]
>
>**Voorbeeld:**
>
>Met de [!DNL Workfront for Microsoft integration], kunt u meldingen ontvangen in [!DNL Microsoft Teams] over uw [!DNL Workfront] werkitems. Zonder vertrek [!DNL Microsoft Teams]kunt u handelingen uitvoeren zoals goedkeuren, opmerkingen plaatsen of de status van werkitems wijzigen. Alle wijzigingen die u aanbrengt in werkitems van [!DNL Microsoft] Teams worden weerspiegeld in [!DNL Workfront] ook.

Voor meer informatie over ingebouwde integratie, met inbegrip van een lijst van momenteel beschikbare ingebouwde integratie, zie [[!DNL Adobe Workfront] overzicht van ingebouwde integratie](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## Aangepaste OAuth2-toepassingen

Adobe [!DNL Workfront] beheerders kunnen OAuth2-toepassingen maken voor uw exemplaar van [!DNL Workfront], waarmee andere toepassingen toegang kunnen krijgen tot Workfront. Uw gebruikers kunnen deze andere toepassingen vervolgens toestemming geven om toegang te krijgen tot hun Workfront-gegevens. Op deze manier kunt u Workfront integreren met uw eigen toepassingen, inclusief uw eigen interne toepassingen.

>[!NOTE]
>
>In de context van OAuth2 verwijst het maken van een app naar het maken van dit soort toegangskoppelingen tussen een app en een server zoals Workfront.

De voordelen van het creëren van [!UICONTROL OAuth2] de aanvraag kan het volgende omvatten:

* Gebruikers kunnen deze integratie rechtstreeks gebruiken in [!DNL Workfront], vergelijkbaar met ingebouwde integratie.
* Een [!UICONTROL OAuth2] de toepassing geen aanvullende technische kennis vereist, zoals kennis van de [!DNL Workfront] API.
* Uw organisatie kan software gebruiken die niet als [!DNL Workfront] ingebouwde toepassing. U kunt deze software nog steeds integreren met [!DNL Workfront] door een [!UICONTROL OAuth2] zelfs als de software eigendom van uw organisatie is.

Zie voor meer informatie [OAuth2-toepassingen maken voor Workfront-integratie](../administration-and-setup/configure-integrations/create-oauth-application.md).

## Workfront API

Workfront biedt een openbare API (programmeerinterface voor toepassingen) waarmee u uw Workfront-ervaring kunt uitbreiden en verbeteren. Het doel voor de Workfront API is om het bouwen van uw eigen integraties met Workfront te vereenvoudigen door een REST-ful architectuur in te voeren die werkt via HTTP. De Workfront API vereist wel enige technische kennis, maar is een zeer krachtig hulpmiddel voor het ophalen, maken en wijzigen van gegevens. U kunt API-aanroepen aanpassen om specifieke functies uit te voeren.

Daarnaast [!DNL Workfront] biedt een API voor abonnementen op gebeurtenissen aan. Wanneer een handeling plaatsvindt op een [!DNL Workfront] object dat wordt ondersteund door gebeurtenisabonnementen, kunt u configureren [!DNL Workfront] om een reactie naar uw gewenste eindpunt te verzenden. Dit betekent dat toepassingen van derden updates kunnen ontvangen van [!DNL Workfront] interacties via de [!DNL Workfront] API kort nadat deze voorkomen.

Voordelen om de [!DNL Workfront] API kan het volgende bevatten:

* U kunt de [!DNL Workfront] API om verbinding te maken met bijna elke andere webservice of toepassing die een openbare API biedt. Het is derhalve mogelijk [!DNL Workfront] met bijna elke webservice of -app die u wilt gebruiken.
* De [!DNL Workfront] De flexibiliteit van de API strekt zich ook tot de merkgebonden software van uw bedrijf uit. U kunt [!DNL Workfront] gegevens in uw eigen software.
* Aangezien APIs zo gemeenschappelijk voor software zijn, zijn uw interne ontwikkelaars waarschijnlijk vertrouwd met hen. [!DNL Workfront] gebruikt een REST-ful API, het gemeenschappelijkste type van API, die het voor uw ontwikkelaars nog gemakkelijker maakt om snel op te komen.

>[!INFO]
>
>**Voorbeeld:**
>
>De volgende API-aanroep plaatst een opmerking in de updatestream van de taak met de opgegeven id.
>
>
```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

Voor meer informatie over de [!DNL Workfront] API, zie [Basisbeginselen van API](../wf-api/general/api-basics.md).

Zie voor meer informatie over gebeurtenisabonnementen [Event Subscription API](../wf-api/general/event-subs-api.md).

## Adobe Workfront Fusion

Met Workfront Fusion kunt u workflows automatiseren. Met de [!DNL Workfront Fusion for Work Automation and Integration] licentie, kunt u die automatiseringen maken voor meerdere apps en webservices en zo scenario&#39;s creëren waarin de apps samenwerken om een taak uit te voeren. Een scenario is een visuele vertegenwoordiging van de taak of het werkschema dat gebruikend modules wordt gebouwd, die discrete taken zoals &quot;Download een document&quot;of &quot;Create een project zijn.&quot; U plaatst modules in een keten om de workflow te definiëren en vervolgens wordt de workflow automatisch uitgevoerd wanneer aan een triggervoorwaarde wordt voldaan.

Voordelen voor [!DNL Workfront Fusion] kan het volgende omvatten:

* Workfront Fusion vereist niet zoveel technische kennis als de API, omdat de visuele interface helpt bij het begrijpen en instellen van de workflow. Dit betekent dat het door individuen buiten een ontwikkelingsteam kan worden gebruikt, wat uw organisatietijd en geld kan besparen.
* Sinds [!DNL Workfront Fusion] Via de API hebt u toegang tot de meeste apps en webservices. Vele apps hebben modules om API vraag te maken, of u kunt de modules van HTTP, SOAP, of JSON gebruiken om met Webdiensten in wisselwerking te staan die geen specifieke hebben [!DNL Workfront Fusion] -aansluiting.

>[!INFO]
>
>**Voorbeeld:**
>
>Het volgende [!DNL Workfront] module in [!DNL Workfront Fusion] is ingesteld om een opmerking toe te voegen aan het geselecteerde project. Nadat de module is uitgevoerd, is de opmerking zichtbaar in de updatestream van het project in Workfront.
>
>![](assets/fusion-example-comment-350x416.png)

Zie voor meer informatie over Workfront Fusion [Adobe Workfront Fusion](../workfront-fusion/workfront-fusion-2.md).
