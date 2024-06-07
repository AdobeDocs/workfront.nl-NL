---
title: Overzicht van de sectie Historie
description: U kunt wijzigingen controleren die in de record zijn aangebracht en door het systeem zijn opgenomen in het rechterdeelvenster van een record in Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 8258589f-a7c3-4d77-9abe-c99e9184bd21
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Overzicht van de sectie Historie

{{planning-important-intro}}

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

U kunt aan de verslagen van de Planning van Adobe Workfront samenwerken, door commentaren of antwoorden in het juiste paneel van een verslag toe te voegen. U kunt ook andere wijzigingen bekijken die in de record zijn aangebracht en door het systeem in dit gebied zijn opgenomen.

In het rechterdeelvenster van een record worden de volgende secties weergegeven:

* **Opmerkingen**: Hiermee geeft u opmerkingen en antwoorden weer die gebruikers aan records toevoegen. Voor meer informatie over het beheren van commentaren in de verslagen van de Planning van Workfront, zie [Opnameopmerkingen beheren](/help/quicksilver/planning/records/manage-record-comments.md).
* **Historie**: Hiermee geeft u door het systeem opgenomen wijzigingen weer die gebruikers in de recordvelden aanbrengen.

## De sectie Historie van een record zoeken

{{step1-to-planning}}

1. Klik op de kaart van een werkruimte.

   De werkruimte wordt geopend en de recordtypen worden op kaarten weergegeven.

1. Klik op een opnametype.
De recordtypepagina wordt geopend en alle records van dat type worden weergegeven.

1. Kies een tabelweergave in het menu **Weergave** vervolgkeuzelijst.
1. Klik op de naam van een record in de tabelweergave.

   De pagina van de record wordt geopend. Het gebied Opmerkingen wordt standaard in het rechtervenster geopend.
1. Klik op de knop **Historie tonen** pictogram ![](assets/show-history-icon.png). Alle wijzigingen die in de velden van de record zijn aangebracht, worden in het rechterdeelvenster weergegeven, te beginnen met de meest recente.
1. (Optioneel) Klik op de knop **Historie verbergen** pictogram ![](assets/hide-history-icon.png) om het rechterdeelvenster te sluiten.

## Overwegingen bij de sectie Historie

U kunt de wijzigingen die zijn aangebracht in recordvelden, bekijken in de sectie Historie van het rechterdeelvenster van de pagina van een record.

![](assets/history-area-in-comments.png)

* Workfront Planning registreert de volgende informatie in de sectie van de Geschiedenis:

   * Alle veldwijzigingen

   * De oude en nieuwe waarden van velden, wanneer de waarden veranderen. De oude waarden worden doorgehaald weergegeven.

   * De volledige naam van de gebruiker die de wijziging heeft aangebracht

   * Een datum- en tijdstempel van wanneer de wijziging heeft plaatsgevonden.

* Velden van de volgende typen geven altijd de oude waarde (in doorhalingsformaat) en de nieuwe waarde weer:

   * Tekst
   * Alinea
   * Valuta
   * Datum
   * Getal
   * Percentage
   * Enkel selecteren

* Velden van de volgende typen tonen alleen de oude waarde in doorhalingsformaat als ten minste een van de meerdere waarden is verwijderd:

   * Meerdere selecties
   * Gekoppelde recordvelden
   * Mensen

  Als de wijziging alleen waarden aan het veld toevoegt, wordt de oude waarde niet weergegeven en wordt alleen de nieuwe veldwaarde weergegeven.

* In velden van het type selectievakje wordt de oude waarde nooit doorgehaald weergegeven. Als het veld wordt bewerkt, wordt alleen het huidige frame weergegeven op het moment dat de wijziging is aangebracht.

  Voor meer informatie over de gebieden van de Planning van Workfront, zie [Velden maken](/help/quicksilver/planning/fields/create-fields.md).

* Wijzigingen in velden van de volgende typen worden niet weergegeven in de sectie Historie:

   * Gekoppelde (opzoekbare) velden
   * Formule
   * Gemaakt door
   * Gemaakt op datum
   * Laatst gewijzigd door
   * Laatst gewijzigd

* Als een veld uit het systeem wordt verwijderd, blijven de in dat veld aangebrachte updates in de sectie Historie staan. Er zijn geen aanwijzingen dat het veld is verwijderd in de sectie Historie van een record.
