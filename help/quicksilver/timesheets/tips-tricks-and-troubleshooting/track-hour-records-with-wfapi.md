---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Hour-records bijhouden met de Adobe Workfront API
description: Als uw organisatie gebruikmaakt van Adobe Workfront om het aantal gewerkte uren in te voeren, maar een ander hulpmiddel gebruikt als het systeem voor het opnemen van die gegevens, kunt u de Workfront API gebruiken om gegevens tussen de twee systemen te synchroniseren.
author: Alina
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Hour-records bijhouden met de Adobe Workfront API

Als uw organisatie gebruikmaakt van Adobe Workfront om het aantal gewerkte uren in te voeren, maar een ander hulpmiddel gebruikt als het systeem voor het opnemen van die gegevens, kunt u de Workfront API gebruiken om gegevens tussen de twee systemen te synchroniseren.

Eenvoudig het volgen van het uurverslag is niet haalbaar omdat, als de uuringang wordt verwijderd, het volledige verslag wordt geschrapt, die u vereisen om de volledige dataset te trekken en het met de oude dataset te vergelijken. Gelukkig worden alle uurtransacties geregistreerd in Workfront Journal-berichten.

Na het terugwinnen van een aanvankelijke reeks van alle huidige uren in het systeem, kunt u om het even welke en alle veranderingen door de Ingangen van het Dagboek volgen.
<pre>GET /attask/api/v5.0/JRNLE/search?subObjCode=HOUR&amp;fields=changeType,aux2,newNumberVal,oldNumberVal,subObjCode,subObjID</pre><pre>{<br>"data": [<br>{<br>"ID": "5785406d008d93dd35665f14d90d4929",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1<br>"oldNumberVal": null,<br>"subObjCode": "UUR",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "57854124008da2b9f372c01f8b9054bf",<br>"objCode": "JRNLE",<br>"changeType": "D",<br>"aux2": "Brad Littler",<br>"newNumberVal": null,<br>"oldNumberVal": 1<br>"subObjCode": "UUR",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "5785416f008db05ecee93463a968366",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1<br>"oldNumberVal": null,<br>"subObjCode": "UUR",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>},<br>{<br>"ID": "57854176008db22fe974b7c67feea6b2",<br>"objCode": "JRNLE",<br>"changeType": "E",<br>"aux2": "Brad Littler",<br>"newNumberVal": 2<br>"oldNumberVal": 1<br>"subObjCode": "UUR",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>}<br>]<br>}</pre>Hieronder volgt een beschrijving van de opgenomen velden:

* **changeType:** Het type wijziging dat in het object wordt aangebracht:

   * **A:** Toevoegen

   * **E:** Bewerken

   * **D:** Verwijderen

* **aux2:** De naam van de gebruiker voor wie de uurrecord is.

* **newNumberVal:** Nieuwe waarde van het uurverslag (Dit zal ongeldig zijn als changeType D is).

* **oldNumberVal:** Vorige waarde van uurrecord.

* **subObjCode:** Type record dat wordt gewijzigd (moet altijd UUR zijn).

* **subObjID:** ID van de uurrecord.

U kunt deze informatie gebruiken om te ontdekken welke uurverslagen zijn veranderd, uitgegeven, of geschrapt. U kunt subObjID dan gebruiken om meer informatie van de uurverslagen terug te winnen indien nodig.
