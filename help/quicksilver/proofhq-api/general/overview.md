---
title: Overzicht
description: Overzicht
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Overzicht

**Welkom bij de Workfront Proof API**

De Workfront Proof API is een eenvoudige HTTP-service die is beveiligd met SSL. De API is bedoeld om u alle functionaliteit te bieden die in onze eigen toepassing wordt gebruikt.

## Ondersteunde indelingen

De openbare interface is Volgzaam SOAP 1.1 met de steun van WSDL. Alle aanvragen worden daarom uitgevoerd met XML via HTTPS.

## API-versies

Om compatibiliteit met bestaande clientintegratie te behouden, hebben we vanaf onze release 12.1 API-versies geïntroduceerd. Zie de  [API-updates](http://api.proofhq.com/new-updates) voor meer informatie. Als een methode of parameter geen versiegegevens heeft, betekent dit dat u dit als onderdeel van onze standaard-API zult vinden, raadpleegt u de sectie Aan de slag met de API hieronder.

## Aan de slag met de API

Het API-ingangspunt:

`https://soap.proofhq.com/soap` (Let op het gebruik van HTTPS)

De WSDL is te vinden op:

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**Deze WSDL bevat alle wijzigingen tot de release 12.1, waarna we API-versies hebben geïntroduceerd. Zie de pagina met API-updates voor meer informatie over de verschillende WSDL-versies en aanstaande wijzigingen**

Voor elke API-aanvraag is een sessiesleutel vereist. Deze sessiesleutel identificeert de Workfront Proof-gebruiker die de handeling(en) uitvoert en wordt verkregen door de methode doLogin() aan te roepen en het e-mailadres en wachtwoord van de gebruiker door te geven. De methode doLogin() hoeft slechts één keer te worden aangeroepen voordat een reeks API-aanvragen wordt uitgevoerd. De zittingssleutel blijft actief voor een korte periode en op elke methodevraag vernieuwd. *We zullen binnenkort ondersteuning toevoegen voor tokenverificatie.*

Voor alle aanvragen wordt de volgende indeling voor envelop, koptekst en tekst gebruikt:

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
	   ... API function and data inserted here ...
	</soapenv:Body>
	</soapenv:Envelope>
```

## Veelgestelde vragen

Voor een verzameling veelgestelde vragen gaat u naar [dit](http://api.proofhq.com/faqs) pagina.
