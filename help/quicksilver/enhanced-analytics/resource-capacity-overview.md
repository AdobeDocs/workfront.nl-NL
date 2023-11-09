---
title: De visualisatie van de bronnencapaciteit bekijken in Verbeterde analyse
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: De capaciteitvisualisatie van het Middel toont of een team over, onder, of bij capaciteit is.
author: Nolan
feature: Reports and Dashboards
exl-id: 5bb45ef6-9e49-4063-8e53-c9f3bc994870
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---

# De visualisatie van de bronnencapaciteit bekijken in Verbeterde analyse

De capaciteitvisualisatie van het Middel toont of een team over, onder, of bij capaciteit is.

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
   <td> <p>Toegang tot projecten weergeven</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld.<br>Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Weergave</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

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

Het over een rij bedekken toont het nauwkeurige aantal uren voor geplande capaciteit en beschikbare capaciteit, evenals het aantal uren het huisteam over of onder capaciteit is.

Aan de hand van deze informatie kunt u bepalen:

* Als het huisteam werd oververdeeld of onderverdeeld.
* Wat de grootste projecten waren, was dat het thuisteam zich daarop richtte.
* Welke huisteams beschikbaar voor het werk zijn.

Ga voor meer informatie over de beste gegevens voor deze visualisatie naar [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

## De visualisatie van de bronnencapaciteit weergeven

1. Klik op het pictogram Hoofdmenu ![](assets/main-menu-icon-16x12.png)selecteert u vervolgens **Analyse**.
1. Selecteer in het linkerdeelvenster de optie **Mensen**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Optioneel) Als u een ander datumbereik wilt gebruiken, selecteert u nieuwe begin- en einddatums in het filter voor het datumbereik.

   ![](assets/filters-select-date-range-350x344.png)

   Voor informatie over het gebruik van het filter Datumbereik raadpleegt u [Filters toepassen in uitgebreide analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Voorwaardelijk) als u uw filter van het Team niet hebt geplaatst, voeg de filter van het Team toe en selecteer elk team dat u gegevens voor wilt zien.

   Zie voor meer informatie over het toevoegen van filters in Verbeterde analysemogelijkheden [Filters toepassen in uitgebreide analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nadat u filters hebt toegevoegd, worden er gegevens voor maximaal 50 projecten weergegeven en blijven de filters actief, zelfs nadat u de pagina hebt verlaten of zich hebt afgemeld bij Workfront.

1. (Optioneel) Als u wilt inzoomen op een datumbereik, selecteert u een punt in de visualisatie voor het begin van het datumbereik en sleept u naar het einde van het datumbereik.

   Alle andere visualisaties worden bijgewerkt naar hetzelfde datumbereik en er wordt een tijdframefilter gemaakt.

   ![](assets/timeframe-filter-350x220.png)

1. Houd de muisaanwijzer boven de teamlijn van het thuisteam om te zien hoeveel uren er nog gepland zijn, hoeveel uren het thuisteam gepland heeft om te voltooien en hoeveel uren er zijn gewerkt, met het label over, onder of op capaciteit.

   ![](assets/resource-capacity-capacity-pop-up-350x213.png)

1. (Optioneel) Als u de visualisatiegegevens wilt exporteren, klikt u op **Exportpictogram** ![](assets/export.png) in de rechterbovenhoek van de visualisatie selecteert u de exportindeling:

   * **Diagram (PNG)**
   * **Gegevenstabel (XSLX)**

1. Klik een naam van het huisteam om meer informatie in de de capaciteitsvisualisatie van het Team te zien.

   Meer over de capaciteitvisualisatie van het Team leren, zie [De visualisatie van de teamcapaciteit bekijken in Verbeterde analyse](../enhanced-analytics/team-capacity-overview.md).


