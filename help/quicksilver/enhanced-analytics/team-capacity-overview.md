---
title: De visualisatie van de teamcapaciteit bekijken in Verbeterde analyse
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: De de capaciteitsvisualisatie van het Team toont de totale hoeveelheid capaciteit een huisteam heeft, of zij of onderverdeeld zijn, en hoe dynamisch de capaciteit in tijd is.
author: Nolan
feature: Reports and Dashboards
exl-id: cfeb1a87-01be-4088-9e33-53a97e3871ad
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# De visualisatie van de teamcapaciteit bekijken in Verbeterde analyse

De de capaciteitsvisualisatie van het Team toont de totale hoeveelheid capaciteit een huisteam heeft, of zij of onderverdeeld zijn, en hoe dynamisch de capaciteit in tijd is.

![](assets/team-capacity-350x110.png)

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
   <td> <p>Weergave</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

Voor eerste vereisten voor het gebruik van Enhanced Analytics raadpleegt u de sectie &quot;Voorwaarden&quot; in [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

## Begrijp de capaciteit van het Team visualisatie

De de capaciteitsvisualisatie van het Team toont het volume van het werk dat aan het huisteam op een bepaalde dag wordt toegewezen.

* **Branden**: Wanneer de donkerdere blauwe vulkleur boven de stippellijn ligt, wordt aan het thuisteam meer werkuren toegewezen dan ze kunnen voltooien in het aantal uren dat het team beschikbaar is om te werken. Dit wijst erop dat het team oververdeeld is en zou burnout kunnen naderen.

   ![](assets/team-capacity-over-capacity.png)

* **Onbetwist**: Wanneer de donkerdere blauwe vulkleur onder de stippellijn ligt, heeft het home team meer werkuren dan de hoeveelheid werk die aan hen is toegewezen. Dit wijst erop dat het team onderverdeeld is en kan onbetwist zijn.

   ![](assets/team-capacity-under-capacity.png)

* **Balans**: Wanneer de lichtere of transparantere blauwe vulkleur net boven, net onder, of bij de stippellijn is, heeft het huisteam een hoeveelheid werkuren toegewezen aan hen die zij binnen hun beschikbare werkuren zouden moeten kunnen voltooien. Dit wijst erop dat de werklast van het team evenwichtiger is.

   ![](assets/team-capacity-at-capacity.png)

Als u de muis boven een punt in de visualisatie houdt, ziet u de volgende details voor een bepaalde dag:

* **Geplande uren**: Dit is het aantal geplande werkuren dat het team moet voltooien.
* **Beschikbare uren**: Dit is het aantal werkuren dat het team beschikbaar is om te werken.
* **Capaciteit**: Naast een capaciteitspercentage worden ook de benamingen At capacity, Under capacity of Over capaciteit weergegeven.

Aan de hand van deze informatie kunt u bepalen:

* Wanneer het huisteam werd oververdeeld of onderverdeeld.
* Als het huisteam dagelijks oververdeeld of onderverdeeld is.
* Hoe consistent de werklast van een thuisteam is van dag tot dag.
* Als u capaciteitsproblemen maakt met nieuw werk.

Ga voor meer informatie over de beste gegevens voor deze visualisatie naar [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

## De visualisatie van de teamcapaciteit weergeven

1. Klik op het pictogram Hoofdmenu ![](assets/main-menu-icon-16x12.png)selecteert u vervolgens **Analyse**.
1. Selecteer in het linkerdeelvenster de optie **Mensen**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Optioneel) Als u een ander datumbereik wilt gebruiken, selecteert u nieuwe begin- en einddatums in het filter voor het datumbereik.

   ![](assets/filters-select-date-range-350x344.png)

   Voor informatie over het gebruik van het filter Datumbereik raadpleegt u [Filters toepassen in uitgebreide analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Voorwaardelijk) als u uw filter van het Team niet hebt geplaatst, voeg de filter van het Team toe en selecteer elk team dat u gegevens voor wilt zien.

   Voor meer informatie over het toevoegen van filters in Verbeterde analysemogelijkheden raadpleegt u [Filters toepassen in uitgebreide analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nadat u filters hebt toegevoegd, worden er gegevens voor maximaal 50 projecten weergegeven en blijven de filters actief, zelfs nadat u de pagina hebt verlaten of zich hebt afgemeld bij Workfront.

1. Voor de capaciteitvisualisatie van het Middel, klik een team om meer informatie te zien.

   De de capaciteitvisualisatievertoningen van het Team.

   Voor meer informatie over de capaciteit van het Middel visualisatie, zie [De visualisatie van de bronnencapaciteit bekijken in Verbeterde analyse](../enhanced-analytics/resource-capacity-overview.md).

1. (Optioneel) Als u wilt inzoomen op een datumbereik, selecteert u een punt in de visualisatie voor het begin van het datumbereik en sleept u naar het einde van het datumbereik.

   Alle andere visualisaties worden bijgewerkt naar hetzelfde datumbereik en er wordt een tijdframefilter gemaakt.

   ![](assets/timeframe-filter-350x220.png)

1. Houd de muisaanwijzer over een punt op de gespecificeerde lijn om de geplande uren en geplande uren voor de opgegeven datum te zien, alsmede het capaciteitspercentage en of het huisteam op dat moment over, onder of op capaciteit beschikte.

   ![](assets/team-capacity-capacity-pop-up-350x351.png)

1. (Optioneel) Als u de visualisatiegegevens wilt exporteren, klikt u op de knop **Exportpictogram** ![](assets/export.png) in de rechterbovenhoek van de visualisatie selecteert u de exportindeling:

   * **Diagram (PNG)**
   * **Gegevenstabel (XSLX)**

