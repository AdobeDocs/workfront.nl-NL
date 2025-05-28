---
title: Bekijk de visualisatie van het vliegplan in de uitgebreide analyse
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Uit de visualisatie van het vliegplan blijkt hoeveel projecten (binnen de toegepaste filtercriteria) op de vlucht waren, welke veranderingen in de toestand zich gedurende de gehele looptijd van deze projecten hebben voorgedaan en in hoeverre deze projecten zich aan de geplande uiterste uitvoeringstermijnen hebben gehouden.
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# Bekijk de visualisatie van het vliegplan in de uitgebreide analyse

>[!IMPORTANT]
>
>Enhanced Analytics is op 27 mei uit Workfront verwijderd. Workfront Data Connect is een nieuwe, alternatieve oplossing die kan worden gebruikt om alle Enhanced Analytics-visualisaties die u momenteel gebruikt, te repliceren. <br> zie de [ Verbeterde 2} gids van de Afleiding van Analytics {voor meer informatie.](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)


Uit de visualisatie van het vliegplan blijkt hoeveel projecten (binnen de toegepaste filtercriteria) op de vlucht waren, welke veranderingen in de toestand zich gedurende de gehele looptijd van deze projecten hebben voorgedaan en in hoeverre deze projecten zich aan de geplande uiterste uitvoeringstermijnen hebben gehouden.

![ vliegplan ](assets/flight-plan-350x132.png)

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank"> plan van Adobe Workfront </a>*</td> 
   <td> <p>Zakelijk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref"> het vergunningsoverzicht van Adobe Workfront </a>*</td> 
   <td> <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten weergeven</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld.<br> voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> creeer of wijzig douanetoegangsniveaus </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang tot het project weergeven</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Vereisten

Voor eerste vereisten aan het gebruiken van Verbeterde Analytics, zie de &quot;sectie van Eerste vereisten&quot;in [ Verbeterd analyseoverzicht ](../enhanced-analytics/enhanced-analytics-overview.md).

## Begrijp de visualisatie van het vliegplan

In de daadwerkelijke duur van een project, kunt u slechts de volgende projectvoorwaarden zien:

* Op doel
* Risico
* In problemen

Om over projectvoorwaarden te leren, zie [ Overzicht van het Type van de Voorwaarde en van de Voorwaarde van het Project ](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

De visualisatie van het vliegplan toont de volgende projectdetails:

* **Geplande duur**: De horizontale blauwe lijn vertegenwoordigt de geplande lengte van het project, met de driehoeken bij één van beide eind van de lijn die op de begindatum en einddatum wijzen.

  ![ Geplande duur ](assets/planned-duration-line-350x37.png)

* **Ware duur**: De dikke, gekleurde lijn onder de geplande duur vertegenwoordigt de daadwerkelijke lengte van het project. De kleur van de lijn verandert afhankelijk van de voorwaarde van het project op dat specifieke tijdstip in het leven van het project.

  ![ Ware duur ](assets/actual-duration-line.png)

* **Ware voorwaarde**: De dikke, gekleurde lijn toont ook de voorwaarde van een project op verschillende momenten in tijd. De kleur van de lijn verandert afhankelijk van de voorwaarde van het project:

   * **Groen**: Op Doel
   * **Oranje**: Bij Risico
   * **Rood**: In Problemen

  ![ Ware voorwaarde ](assets/actual-condition-color.png)

Door over een projectrij in de visualisatie van het Plan van de Vlucht te bewegen, kunt u informatie over geplande timeframe van het project, de huidige projectvoorwaarde, en-indien van toepassing-de douanevoorwaarde zien. Voor een diepgaandere weergave van wat de duur of de voorwaarde kan hebben beïnvloed, kunt u naar de andere visualisaties in het gedeelte Uitgebreide analyse kijken.

Aan de hand van deze informatie kunt u bepalen:

* Welke gebeurtenissen een project verlengen na de oorspronkelijke geplande einddatum.
* Wanneer een project op kwesties begint te lopen.
* Hoeveel projecten zijn er in dezelfde periode open?
* Hoeveel projecten zijn actief.
* Welke projecten hebben extra aandacht of steun nodig.

Voor informatie over hoe te om de beste gegevens voor deze visualisatie te krijgen, zie [ Verbeterd analyseoverzicht ](../enhanced-analytics/enhanced-analytics-overview.md).

## De visualisatie van het vliegplan bekijken

1. Klik het **pictogram ![ Belangrijkste het menupictogram van het 1} Hoofdmenu ](assets/main-menu-icon-16x12.png), dan uitgezochte** Analytics **.**
1. (Optioneel) Als u een ander datumbereik wilt gebruiken, selecteert u nieuwe begin- en einddatums in het filter voor het datumbereik.

   ![ Uitgezochte datumwaaier ](assets/filters-select-date-range-350x344.png)

   Voor informatie bij het gebruiken van de filter van de datumwaaier, zie [ filters in Verbeterde analyses toepassen ](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Voorwaardelijk) als u de reeks van projectgegevens moet beperken, selecteer en pas de filters toe die u wilt gebruiken.

   Voor meer informatie bij het toevoegen van filters in Verbeterde analyses, zie [ filters in Verbeterde analyses toepassen ](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nadat u filters hebt toegevoegd, worden er gegevens voor maximaal 50 projecten weergegeven en blijven de filters actief, zelfs nadat u de pagina hebt verlaten of zich hebt afgemeld bij Workfront.

1. (Optioneel) Als u wilt inzoomen op een datumbereik, selecteert u een punt in de visualisatie voor het begin van het datumbereik en sleept u naar het einde van het datumbereik.

   Alle andere visualisaties worden bijgewerkt naar hetzelfde datumbereik en er wordt een tijdframefilter gemaakt.

   ![ filter Tijdframe ](assets/timeframe-filter-350x220.png)

1. (Facultatief) om te veranderen hoe de projecten worden gesorteerd, klik de **Soort door** menu in de hoger-juiste hoek van de visualisatie van het vliegplan, dan selecteer een nieuwe sorterende optie:

   * **A - Z**
   * **Z - A**
   * **Geplande voltooiingsdatum**
   * **Geplande begindatum**

   Alle andere visualisaties op de pagina worden bijgewerkt zodat deze overeenkomen met de geselecteerde sorteervolgorde.

1. (Voorwaardelijk) als er meer dan 50 projecten in uw gegevensreeks zijn, gebruik de pijlen in de bodem-linkerhoek van visualisatie om van één groep van 50 projecten aan volgende te navigeren.

   Alle andere visualisaties op de pagina worden bijgewerkt zodat deze overeenkomen met de geselecteerde pagina.

   ![ Paginering ](assets/pagination-350x118.png)

1. Houd de muisaanwijzer boven het diagram van de projectbalk om de blauwe datumlijn en de volgende details weer te geven:

   * Geplande tijdlijn
   * Huidige voorwaarde
   * Aangepaste voorwaarde (indien van toepassing)

   ![ grafiek van de bar van het Project ](assets/project-bar-graph-350x143.png)

1. (Facultatief) om de visualisatiegegevens uit te voeren, klik het **pictogram van de Uitvoer ![ pictogram van de Uitvoer ](assets/export.png) in de hoogste juiste hoek van de visualisatie, dan selecteer het uitvoerformaat:**

   * **Grafiek (PNG)**
   * **Lijst van Gegevens (XSLX)**

1. Om meer projectinformatie te zien, klik een project op visualisatie om de Doordrukking en Taken in vluchtvisualisaties te openen.

   Deze visualisaties kunnen u helpen dieper insight te bereiken in wat het project ertoe heeft aangezet om van spoor te raken. Bovendien is het zo eenvoudig om een lopend project in te checken.\
   Voor meer informatie over de Visualisatie van de Doordrukking, zie [ Mening de Visualisatie van de Doordrukking in Verbeterde analyses ](../enhanced-analytics/burndown-overview.md). Voor meer informatie over de Taken in vluchtvisualisatie, zie [ Mening de Taken in vluchtvisualisatie in Verbeterde analyses ](../enhanced-analytics/tasks-in-flight-overview.md).

