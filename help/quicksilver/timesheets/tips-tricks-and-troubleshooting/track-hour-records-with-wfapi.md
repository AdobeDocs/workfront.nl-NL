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
source-wordcount: '337'
ht-degree: 0%

---

# Hour-records bijhouden met de Adobe Workfront API

Als uw organisatie gebruikmaakt van Adobe Workfront om het aantal gewerkte uren in te voeren, maar een ander hulpmiddel gebruikt als het systeem voor het opnemen van die gegevens, kunt u de Workfront API gebruiken om gegevens tussen de twee systemen te synchroniseren.

Eenvoudig het volgen van het uurverslag is niet haalbaar omdat, als de uuringang wordt verwijderd, het volledige verslag wordt geschrapt, die u vereisen om de volledige dataset te trekken en het met de oude dataset te vergelijken. Gelukkig worden alle uurtransacties geregistreerd in Workfront Journal-berichten.

Na het terugwinnen van een aanvankelijke reeks van alle huidige uren in het systeem, kunt u om het even welke en alle veranderingen door de Ingangen van het Dagboek volgen.
<pre>GET /attask/api/v5.0/JRNLE/search?subObjCode=HOUR&amp;fields=changeType,aux2,newNumberVal,oldNumberVal,subObjCode,subObjID</pre><pre><br> "data": [<br>&lbrace;<br> "ID": "5785406d008d93dd35665f14d90d4929", <br> "objCode": "JRNLE", <br> changeType": "A", <br> "aux2": "Brad Littler", <br> "newNumberVal": 1, <br> "oldNumberVal": null, <br> "subObjCode": "HOUR", <br> "subObjID": "5785406d00 8d93dce3f7f2e0e8eda4ea"<br>, <br>{<br> "identiteitskaart": "57854124008da2b9f372c01f8b9054bf", <br>} "objCode": "JRNLE", <br> "changeType": "D", <br> "aux2": "Brad Littler", <br> "newNumberVal": null, <br> "oldNumberVal": 1, <br> "subObjCode": "HOUR", {1Cf 9} "subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>, <br>{<br> "ID": "5785416f008db0 5ecee934663a968366", <br> "objCode": "JRNLE", <br> "changeType": "A", <br> "aux2": "Brad Littler", <br> "newNumberVal": 1, <br> 7} "oldNumberVal": null, <br> "subObjCode": "HOUR", <br> "subObjID": "5785416f008db05d9d2925c12b10f521"<br>,<br>&lbrace;<br> "identiteitskaart": "57854176008db22fe974b7c67feea6b2", <br> "objCode": "JRNLE", <br> "changeCode": "E", <br> "aux2": "Brad Littler", <br> "newNumberVal": 2, <br> "oldNumberVal": 1, <br> "subObjCode": "HOUR", <br> "subObjID": "578541 6f008db05d9d2925c12b10f521"<br> <br>] <br><br></pre>Hieronder volgt een beschrijving van de opgenomen velden:

* **changeType:** het type van verandering dat in het voorwerp wordt aangebracht:

   * **A:** voeg toe

   * **E:** geef uit

   * **D:** Schrapping

* **aux2:** De naam van de gebruiker het uurverslag is voor.

* **newNumberVal:** Nieuwe waarde van het uurverslag (Dit zal ongeldig zijn als changeType D is).

* **oldNumberVal:** Vorige waarde van het uurverslag.

* **subObjCode:** Type van verslag dat wordt gewijzigd (zou altijd HOUR moeten zijn).

* **subObjID:** identiteitskaart van het verslag van het Uur.

U kunt deze informatie gebruiken om te ontdekken welke uurverslagen zijn veranderd, uitgegeven, of geschrapt. U kunt subObjID dan gebruiken om meer informatie van de uurverslagen terug te winnen indien nodig.
