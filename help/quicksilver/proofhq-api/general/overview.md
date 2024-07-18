---
title: Overzicht
description: Overzicht
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Overzicht

**Onthaal aan Workfront Proof API**

De Workfront Proof API is een eenvoudige HTTP-service die is beveiligd met SSL. De API is bedoeld om u alle functionaliteit te bieden die in onze eigen toepassing wordt gebruikt.

## Ondersteunde indelingen

De openbare interface is SOAP 1.1 volgzaam met steun WSDL. Alle aanvragen worden daarom uitgevoerd met XML via HTTPS.

## API-versies

Om compatibiliteit met bestaande clientintegratie te behouden, hebben we vanaf onze release 12.1 API-versies geïntroduceerd. Zie de  [ API werkt ](https://api.proofhq.com/new-updates.html) pagina voor meer informatie bij. Als een methode of parameter geen versiegegevens heeft, betekent dit dat u dit als onderdeel van onze standaard-API zult vinden, raadpleegt u de sectie Aan de slag met de API hieronder.

## Aan de slag met de API

Het API-ingangspunt:

`https://soap.proofhq.com/soap` (let op het gebruik van HTTPS)

De WSDL is te vinden op:

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**This WSDL bevat alle veranderingen tot versie 12.1, waarna wij API versioning introduceerden. Zie de pagina met API-updates voor meer informatie over de verschillende WSDL-versies en aanstaande wijzigingen**

Voor elke API-aanvraag is een sessiesleutel vereist. Deze sessiesleutel identificeert de Workfront Proof-gebruiker die de handeling(en) uitvoert en wordt verkregen door de methode doLogin() aan te roepen en het e-mailadres en wachtwoord van de gebruiker door te geven. De methode doLogin() hoeft slechts één keer te worden aangeroepen voordat een reeks API-aanvragen wordt uitgevoerd. De zittingssleutel blijft actief voor een korte periode en op elke methodevraag vernieuwd. *wij zullen steun voor symbolische gebaseerde authentificatie zeer spoedig toevoegen.*

Voor alle aanvragen wordt de volgende indeling voor envelop, koptekst en tekst gebruikt:

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
       ... API function and data inserted here ...
    </soapenv:Body>
    </soapenv:Envelope>
```

