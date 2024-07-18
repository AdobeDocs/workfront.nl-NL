---
content-type: reference
product-area: workfront-integrations
keywords: native,ootb
navigation-topic: workfront-integrations-navigation-topic
title: Adobe Workfront-integratiemethoden
description: U kunt  [!DNL Adobe Workfront]  met derdetoepassingen integreren. Deze integraties kunnen het nut van  [!DNL Workfront]  uitbreiden en het aan de behoeften van uw organisatie aanpassen. U kunt al deze integraties gebruiken, afhankelijk van welke integratie het meest geschikt is voor een bepaalde taak.
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 328d3a8d16ace22100d86efc127874d7edd6cb6d
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# Adobe Workfront-integratiemethoden

U kunt [!DNL Adobe Workfront] integreren met toepassingen van derden en met andere [!DNL Adobe] -producten. Deze integratie kan het nut van [!DNL Workfront] uitbreiden en het aanpassen aan de behoeften van uw organisatie. U kunt al deze integraties gebruiken, afhankelijk van welke integratie het meest geschikt is voor een bepaalde taak.

## Ingebouwde integratie

Workfront biedt diverse integraties die u rechtstreeks vanuit Workfront kunt configureren, of vanuit een andere toepassing door de Workfront-invoegtoepassing voor die toepassing te installeren. Deze ingebouwde integratie bestrijkt veel veelvoorkomende gebruiksscenario&#39;s en richt zich op het uitbreiden en verbinden van gebruikerservaring voor eindgebruikers.

De ingebouwde integratie van Workfront richt zich hoofdzakelijk op persoonlijke productiviteit en samenwerking. Deze integratie reduceert onderbrekingen in de workflow van een individuele gebruiker, zodat deze Workfront-meldingen kan ontvangen, toegang krijgt tot informatie en op Workfront-werkitems kan reageren zonder de geïntegreerde toepassing te verlaten.

De voordelen van ingebouwde integratie kunnen het volgende omvatten:

* Veel van deze ingebouwde integraties zijn zonder extra kosten beschikbaar. (Andere gebruikers hebben wel een extra aankoop nodig.)
* De ingebouwde integratie heeft betrekking op veel van de meest gebruikte toepassingen in bedrijven, zoals [!DNL Slack] -, [!DNL Google Drive] - of [!DNL Adobe] -producten zoals de [!DNL Adobe Creative Cloud] - of [!DNL Adobe Experience Manager] Assets. Als uw bedrijf deze apps al gebruikt, verloopt de integratie probleemloos in de bestaande workflow van uw gebruikers.
* Door [!DNL Workfront] te integreren met een veelgebruikte toepassing, kan de acceptatie bij uw gebruikers toenemen.

>[!INFO]
>
>**Voorbeeld:**
>
>Met [!DNL Workfront for Microsoft Teams integration] kunt u meldingen ontvangen in [!DNL Microsoft Teams] over uw [!DNL Workfront] werkitems. Zonder [!DNL Microsoft Teams] te verlaten, kunt u acties uitvoeren zoals het goedkeuren van, het becommentariëren van, of het veranderen van de status van het werkpunten. Wijzigingen die u aanbrengt in werkitems vanuit [!DNL Microsoft Teams] , worden ook doorgevoerd in [!DNL Workfront] .

Voor meer informatie over ingebouwde integratie, met inbegrip van een lijst van momenteel beschikbare ingebouwde integratie, zie [[!DNL Adobe Workfront]  ingebouwd integratieoverzicht ](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## Aangepaste OAuth2-toepassingen

Adobe [!DNL Workfront] -beheerders kunnen OAuth2-toepassingen maken voor uw instantie van [!DNL Workfront] , waarmee andere toepassingen toegang hebben tot [!DNL Workfront] . Uw gebruikers kunnen deze andere toepassingen vervolgens toestemming geven om toegang te krijgen tot hun [!DNL Workfront] -gegevens. Op deze manier kunt u Workfront integreren met uw eigen toepassingen, inclusief uw eigen interne toepassingen.

>[!NOTE]
>
>In de context van OAuth2 verwijst het maken van een app naar het maken van dit soort toegangskoppelingen tussen een app en een server zoals Workfront.

De voordelen van het maken van een [!UICONTROL OAuth2] -toepassing kunnen het volgende zijn:

* Gebruikers kunnen deze integratie rechtstreeks in [!DNL Workfront] gebruiken, net als ingebouwde integratie.
* Voor het instellen of gebruiken van een [!UICONTROL OAuth2] -toepassing is geen aanvullende technische kennis vereist, zoals de vertrouwdheid met de [!DNL Workfront] API.
* Uw organisatie kan software gebruiken die niet als [!DNL Workfront] ingebouwde toepassing wordt aangeboden. U kunt deze software nog steeds met [!DNL Workfront] integreren door een [!UICONTROL OAuth2] -toepassing te gebruiken, zelfs als de software eigendom van uw organisatie is.

Voor meer informatie, zie [ toepassingen OAuth2 voor de integratie van Workfront ](../administration-and-setup/configure-integrations/create-oauth-application.md) creëren.

## [!DNL Workfront] API

[!DNL Workfront] biedt een openbare API (programmeerinterface voor toepassingen) waarmee u uw Workfront-ervaring kunt uitbreiden en verbeteren. Het doel voor de [!DNL Workfront] API is het eenvoudig maken van uw eigen integraties met [!DNL Workfront] door een REST-architectuur te introduceren die werkt via HTTP. De API van [!DNL Workfront] vereist enige technische kennis, maar het is een zeer krachtig hulpmiddel om, gegevens terug te winnen tot stand te brengen en te wijzigen. U kunt API-aanroepen aanpassen om specifieke functies uit te voeren.

Daarnaast biedt [!DNL Workfront] een API voor abonnementen op gebeurtenissen aan. Wanneer een actie op een [!DNL Workfront] voorwerp voorkomt dat door gebeurtenisabonnementen wordt gesteund, kunt u [!DNL Workfront] vormen om een reactie naar uw gewenste eindpunt te verzenden. Dit betekent dat toepassingen van derden updates van [!DNL Workfront] -interacties kunnen ontvangen via de [!DNL Workfront] -API kort nadat deze plaatsvinden.

De volgende voordelen van de API van [!DNL Workfront] zijn mogelijk:

* U kunt de [!DNL Workfront] API gebruiken om verbinding te maken met bijna elke andere webservice of toepassing die een openbare API aanbiedt. Daarom is het mogelijk om [!DNL Workfront] te integreren met vrijwel elke gewenste webservice of toepassing.
* De flexibiliteit van de API van [!DNL Workfront] is ook van toepassing op de eigen software van uw bedrijf. U kunt [!DNL Workfront] -gegevens gebruiken en wijzigen vanuit uw eigen software.
* Aangezien APIs zo gemeenschappelijk voor software zijn, zijn uw interne ontwikkelaars waarschijnlijk vertrouwd met hen. [!DNL Workfront] gebruikt een REST-ful API, het gemeenschappelijkste type van API, die het voor uw ontwikkelaars nog gemakkelijker maakt om snel op te komen.

>[!INFO]
>
>**Voorbeeld:**
>
>De volgende API-aanroep plaatst een opmerking in de updatestream van de taak met de opgegeven id.
>
>```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

Voor meer informatie over [!DNL Workfront] API, zie [ API grondbeginselen ](../wf-api/general/api-basics.md).

Voor meer informatie over gebeurtenisabonnementen, zie [ Abonnement API van de Gebeurtenis ](../wf-api/general/event-subs-api.md).

## [!DNL Adobe Workfront Fusion]

Met [!DNL Workfront Fusion] kunt u workflows automatiseren. Met de [!DNL Workfront Fusion for Work Automation and Integration] -licentie kunt u die automatiseringen maken voor meerdere apps en webservices en zo scenario&#39;s maken waarin de apps samenwerken om een taak uit te voeren. Een scenario is een visuele vertegenwoordiging van de taak of het werkschema dat gebruikend modules wordt gebouwd, die discrete taken zoals &quot;Download een document&quot;of &quot;Create een project zijn.&quot; U plaatst modules in een keten om de workflow te definiëren en vervolgens wordt de workflow automatisch uitgevoerd wanneer aan een triggervoorwaarde wordt voldaan.

De voordelen van [!DNL Workfront Fusion] kunnen het volgende zijn:

* [!DNL Workfront Fusion] vereist niet zoveel technische kennis als de API, omdat de visuele interface u helpt de workflow te begrijpen en in te stellen. Dit betekent dat het door individuen buiten een ontwikkelingsteam kan worden gebruikt, wat uw organisatietijd en geld kan besparen.
* Omdat [!DNL Workfront Fusion] via de API werkt, heeft het toegang tot de meeste apps en webservices. Veel apps hebben modules om API-aanroepen te maken, of u kunt de HTTP-, SOAP- of JSON-modules gebruiken om te communiceren met webservices die geen toegewezen [!DNL Workfront Fusion] -connector hebben.

>[!INFO]
>
>**Voorbeeld:**
>
>De volgende [!DNL Workfront] module in [!DNL Workfront Fusion] is ingesteld om een opmerking toe te voegen aan het geselecteerde project. Nadat de module is uitgevoerd, is de opmerking zichtbaar in de updatestream van het project in Workfront.
>
>![](assets/fusion-example-comment-350x416.png)

Zie [[!DNL Adobe Workfront Fusion]](../workfront-fusion/workfront-fusion-2.md) voor meer informatie over [!DNL Workfront Fusion] .
