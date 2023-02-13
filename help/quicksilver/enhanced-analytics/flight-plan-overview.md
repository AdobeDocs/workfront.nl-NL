---
title: Bekijk de visualisatie van het vliegplan in de uitgebreide analyse
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Uit de visualisatie van het vliegplan blijkt hoeveel projecten (binnen de toegepaste filtercriteria) op de vlucht waren, welke veranderingen in de toestand zich gedurende de gehele looptijd van deze projecten hebben voorgedaan en in hoeverre deze projecten zich aan de geplande uiterste uitvoeringstermijnen hebben gehouden.
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 0%

---

# Bekijk de visualisatie van het vliegplan in de uitgebreide analyse

Uit de visualisatie van het vliegplan blijkt hoeveel projecten (binnen de toegepaste filtercriteria) op de vlucht waren, welke veranderingen in de toestand zich gedurende de gehele looptijd van deze projecten hebben voorgedaan en in hoeverre deze projecten zich aan de geplande uiterste uitvoeringstermijnen hebben gehouden.

![](assets/flight-plan-350x132.png)

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront-plan</a>*</td> 
   <td> <p>Zakelijk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Overzicht van Adobe Workfront-licenties</a>*</td> 
   <td> <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten weergeven</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt.<br>Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang tot het project weergeven</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

Voor eerste vereisten voor het gebruik van Enhanced Analytics raadpleegt u de sectie &quot;Voorwaarden&quot; in [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

## Begrijp de visualisatie van het vliegplan

In de daadwerkelijke duur van een project, kunt u slechts de volgende projectvoorwaarden zien:

* Op doel
* Risico
* In problemen

Ga voor meer informatie over de projectvoorwaarden naar [Overzicht van het type Projectvoorwaarde en Voorwaarde](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

De visualisatie van het vliegplan toont de volgende projectdetails:

* **Geplande duur**: De horizontale blauwe lijn geeft de geplande lengte van het project aan, waarbij de driehoeken aan een van de uiteinden van de regel de begindatum en einddatum aangeven.

   ![](assets/planned-duration-line-350x37.png)

* **Werkelijke duur**: De dikke, gekleurde lijn onder de geplande duur geeft de werkelijke lengte van het project aan. De kleur van de lijn verandert afhankelijk van de voorwaarde van het project op dat specifieke tijdstip in het leven van het project.

   ![](assets/actual-duration-line.png)

* **Werkelijke voorwaarde**: De dikke, gekleurde lijn laat ook de conditie van een project op verschillende momenten in de tijd zien. De kleur van de lijn verandert afhankelijk van de voorwaarde van het project:

   * **Groen**: Op doel
   * **Oranje**: Risico
   * **Rood**: In problemen

   ![](assets/actual-condition-color.png)

Door over een projectrij in de visualisatie van het Plan van de Vlucht te bewegen, kunt u informatie over geplande timeframe van het project, de huidige projectvoorwaarde, en-indien van toepassing-de douanevoorwaarde zien. Voor een diepgaandere weergave van wat de duur of de voorwaarde kan hebben beïnvloed, kunt u naar de andere visualisaties in het gedeelte Uitgebreide analyse kijken.

Aan de hand van deze informatie kunt u bepalen:

* Welke gebeurtenissen een project verlengen na de oorspronkelijke geplande einddatum.
* Wanneer een project op kwesties begint te lopen.
* Hoeveel projecten zijn er in dezelfde periode open?
* Hoeveel projecten zijn actief.
* Welke projecten hebben extra aandacht of steun nodig.

Voor informatie over hoe u de beste gegevens voor deze visualisatie kunt ophalen, raadpleegt u [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

## De visualisatie van het vliegplan bekijken

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon-16x12.png)selecteert u vervolgens **Analyse**.
1. (Optioneel) Als u een ander datumbereik wilt gebruiken, selecteert u nieuwe begin- en einddatums in het filter voor het datumbereik.

   ![](assets/filters-select-date-range-350x344.png)

   Voor informatie over het gebruik van het filter Datumbereik raadpleegt u [Filters toepassen in uitgebreide analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Voorwaardelijk) als u de reeks van projectgegevens moet beperken, selecteer en pas de filters toe die u wilt gebruiken.

   Voor meer informatie over het toevoegen van filters in Verbeterde analysemogelijkheden raadpleegt u [Filters toepassen in uitgebreide analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nadat u filters hebt toegevoegd, worden er gegevens voor maximaal 50 projecten weergegeven en blijven de filters actief, zelfs nadat u de pagina hebt verlaten of zich hebt afgemeld bij Workfront.

1. (Optioneel) Als u wilt inzoomen op een datumbereik, selecteert u een punt in de visualisatie voor het begin van het datumbereik en sleept u naar het einde van het datumbereik.

   Alle andere visualisaties worden bijgewerkt naar hetzelfde datumbereik en er wordt een tijdframefilter gemaakt.

   ![](assets/timeframe-filter-350x220.png)

1. (Optioneel) Als u de sortering van de projecten wilt wijzigen, klikt u op de knop **Sorteren op** in de rechterbovenhoek van de visualisatie van het vliegplan en selecteert u vervolgens een nieuwe sorteeroptie:

   * **A - Z**
   * **Z - A**
   * **Geplande voltooiingsdatum**
   * **Geplande begindatum**

   Alle andere visualisaties op de pagina worden bijgewerkt zodat deze overeenkomen met de geselecteerde sorteervolgorde.

1. (Voorwaardelijk) als er meer dan 50 projecten in uw gegevensreeks zijn, gebruik de pijlen in de bodem-linkerhoek van visualisatie om van één groep van 50 projecten aan volgende te navigeren.

   Alle andere visualisaties op de pagina worden bijgewerkt zodat deze overeenkomen met de geselecteerde pagina.

   ![](assets/pagination-350x118.png)

1. Houd de muisaanwijzer boven het diagram van de projectbalk om de blauwe datumlijn en de volgende details weer te geven:

   * Geplande tijdlijn
   * Huidige voorwaarde
   * Aangepaste voorwaarde (indien van toepassing)

   ![](assets/project-bar-graph-350x143.png)

1. (Optioneel) Als u de visualisatiegegevens wilt exporteren, klikt u op de knop **Exporteren** pictogram ![](assets/export.png) in de rechterbovenhoek van de visualisatie selecteert u de exportindeling:

   * **Diagram (PNG)**
   * **Gegevenstabel (XSLX)**

1. Om meer projectinformatie te zien, klik een project op visualisatie om de Doordrukking en Taken in vluchtvisualisaties te openen.

   Deze visualisaties kunnen u helpen dieper inzicht in krijgen wat het project ertoe heeft gebracht om weg te gaan. Bovendien is het zo eenvoudig om een lopend project in te checken.\
   Voor meer informatie over de Burndown visualisatie, zie [Bekijk de Burndown-visualisatie in de uitgebreide analyse](../enhanced-analytics/burndown-overview.md). Voor meer informatie over de Taken in vluchtvisualisatie, zie [De taken tijdens de visualisatie van de vlucht bekijken in Verbeterde analyse](../enhanced-analytics/tasks-in-flight-overview.md).

