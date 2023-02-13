---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Documentwebhooks foutverwerking
description: Documentwebhooks foutverwerking
author: John
feature: Workfront API
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
source-git-commit: 338cc745a7660ffed8e4d44e19dcadfdc13bc345
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%

---

# Documentwebhooks foutverwerking

Er kunnen zich problemen voordoen bij het verwerken van API-aanvragen. Dit moet op consistente wijze worden afgehandeld op alle API-eindpunten. Als er een fout optreedt, moet de websiteprovider een foutcode opnemen in de antwoordheader. Foutcodes zijn:

* 403 - Verboden. Geeft aan dat de aanvraagtokens ontbreken of ongeldig zijn of dat referenties die aan de tokens zijn gekoppeld, geen toegang hebben tot de opgegeven bron. Adobe Workfront probeert nieuwe toegangstokens op te halen voor webhaken die op OAuth zijn gebaseerd.

* 404 - Niet gevonden. Geeft aan dat het opgegeven bestand of de map niet bestaat.

* 500 - Interne serverfout. Een ander type fout.

* Beschrijving van de fout in de responsstructuur met de volgende indeling:

   ```
   {status: “error”
    error: “Sample error message”}
   ```
