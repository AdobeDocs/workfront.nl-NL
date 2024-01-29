---
title: De visualisatie van de bronnencapaciteit bekijken in Verbeterde analyse
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: U kunt beoordelen of een team over, onder, of bij capaciteit wanneer het bekijken van de Verbeterde grafiek van de het middelcapaciteit van de Analyse in Adobe Workfront is.
author: Nolan
feature: Reports and Dashboards
exl-id: 5bb45ef6-9e49-4063-8e53-c9f3bc994870
source-git-commit: d9a8af627c8d3da4a7625cd5180bfca69da43b3d
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 0%

---

# De visualisatie van de bronnencapaciteit bekijken in Verbeterde analyse

<!--Audited: 01/2024-->

U kunt beoordelen of een team over, onder, of bij capaciteit wanneer het bekijken van de Verbeterde grafiek van de het middelcapaciteit van de Analyse in Adobe Workfront is.

De teams die in de middelvisualisatie worden geïllustreerd verwijzen naar het huisteam van gebruikers die aan het werk tijdens de gespecificeerde periode worden toegewezen.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-plan</a>*</td> 
   <td> <p>Huidig: Zakelijk of hoger</p>
   of
   <p>Nieuw: alle</p>
    </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie*</td> 
   <td> <p>Huidig: Controleren of hoger</p>
   of
   <p>Nieuw: Standaard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuratie op toegangsniveau</td> 
   <td> <p>Toegang tot projecten weergeven</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toestemming weergeven voor een project</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt. Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten

Voor eerste vereisten voor het gebruik van Enhanced Analytics raadpleegt u de sectie &quot;Voorwaarden&quot; in [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

## Begrijp de capaciteit van het Middel visualisatie

De capaciteitvisualisatie van het Middel toont of een team over, onder, of bij capaciteit is. Deze berekening is gebaseerd op:

* **Beschikbare capaciteit**: Het totale aantal uren dat een huisteam beschikbaar heeft om in de gefilterde periode te werken

  >[!NOTE]
  >
  >Als u naar een toekomstige periode kijkt, wordt de beschikbare capaciteit berekend op basis van de capaciteit van het team gedurende de laatste 7 dagen. Daarom wordt geen rekening gehouden met een geplande PTO.

* **Geplande capaciteit**: De totale hoeveelheid geplande arbeidsuren die tijdens de gefilterde periode van het team van herkomst wordt verwacht

Deze vergelijking van de geplande uren en de daadwerkelijke geplande uren van een huisteam kan u helpen bepalen als u niet genoeg werk aan het huisteam toewijst of als zij last van een zware werkbelasting kunnen ervaren.

![](assets/resource-capacity-350x110.png)

Voor de capaciteitvisualisatie van het Middel, kunt u de volgende details zien:

* **Geplande capaciteit**: In lijn met een naam van een huisteam, vertegenwoordigt de blauwe cirkel het aantal geplande uren die aan het huisteam worden toegewezen.

  ![](assets/resource-capacity-blue-circle.png)

* **Werkelijke capaciteit**: In lijn met een naam van het huisteam, vertegenwoordigt de verticale lijn het aantal uren beschikbaar voor het huisteam.

  ![](assets/resource-capacity-vertical-line.png)

* **Overcapaciteit**: Wanneer de horizontale lijn en de blauwe cirkel rechts van de verticale lijn worden weergegeven, is aan het home team meer werk toegewezen dan ze in het aantal beschikbare uren kunnen voltooien. Dit betekent dat het team gedurende de gefilterde periode over capaciteit kan zijn. Het resterende aantal uren dat het team nodig heeft om te voltooien, wordt rechts van de blauwe cirkel weergegeven.

  ![](assets/resource-capacity-over-capacity.png)

* **Minder capaciteit**: Wanneer de horizontale lijn en de blauwe cirkel links van de verticale lijn worden weergegeven, heeft het huisteam meer beschikbare uren dan het aantal geplande werkuren dat zij hebben toegewezen. Dit betekent dat het team gedurende de gefilterde periode mogelijk onder de capaciteit is. Het extra aantal beschikbare uren voor het huisteam om het werk te voltooien toont links van de blauwe cirkel.

  ![](assets/resource-capacity-under-capacity.png)

Het over de rij van een team hangen toont het nauwkeurige aantal uren voor geplande capaciteit en beschikbare capaciteit, evenals het aantal uren het huisteam over of onder capaciteit is.

Aan de hand van deze informatie kunt u bepalen:

* Als het team wordt oververdeeld of onderverdeeld.
* Wat de grootste projecten zijn is dat het huisteam zich op concentreert.
* Welke teams beschikbaar voor het werk zijn.

Ga voor meer informatie over de beste gegevens voor deze visualisatie naar [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

## De visualisatie van de bronnencapaciteit weergeven

{{step1-to-analytics}}

1. Selecteer in het linkerdeelvenster de optie **Mensen**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Optioneel) Als u een ander datumbereik wilt gebruiken, selecteert u nieuwe begin- en einddatums in het filter voor het datumbereik rechtsboven in het diagram.

   ![](assets/filters-select-date-range-350x344.png)

   Voor informatie over het gebruik van het filter Datumbereik raadpleegt u [Filters toepassen in uitgebreide analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Voorwaardelijk) als u uw filter van het Team niet hebt geplaatst, voeg de filter van het Team toe en selecteer elk team dat u gegevens voor wilt zien.

   Zie voor meer informatie over het toevoegen van filters in Verbeterde analysemogelijkheden [Filters toepassen in uitgebreide analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nadat u filters hebt toegevoegd, worden er gegevens voor maximaal 50 projecten weergegeven en blijven de filters actief, zelfs nadat u de pagina hebt verlaten of zich hebt afgemeld bij Workfront.

1. (Optioneel) Als u wilt inzoomen op een datumbereik, selecteert u een punt in de visualisatie voor het begin van het datumbereik en sleept u naar het einde van het datumbereik.

   Alle andere visualisaties worden bijgewerkt naar hetzelfde datumbereik en er wordt een tijdframefilter gemaakt.

   ![](assets/timeframe-filter-350x220.png)

1. Houd de muisaanwijzer boven de lijn van het huisteam om het volgende weer te geven:

   * Hoeveel uren zijn nog te plannen
   * De hoeveelheid uren die het huisteam heeft gepland om te voltooien
   * Het totale aantal gewerkte uren. Het totale aantal gewerkte uren zou de volgende etiketten kunnen hebben:

      * Boven
      * Onder
      * Op capaciteit.

   ![](assets/resource-capacity-capacity-pop-up-350x213.png)

1. (Optioneel) Als u de visualisatiegegevens wilt exporteren, klikt u op **Exportpictogram** ![](assets/export.png) in de rechterbovenhoek van de visualisatie selecteert u de exportindeling:

   * **Diagram (PNG)**
   * **Gegevenstabel (XSLX)**

1. Klik een naam van het huisteam om meer informatie in de de capaciteitsvisualisatie van het Team te zien.

   Meer over de capaciteitvisualisatie van het Team leren, zie [De visualisatie van de teamcapaciteit bekijken in Verbeterde analyse](../enhanced-analytics/team-capacity-overview.md).


