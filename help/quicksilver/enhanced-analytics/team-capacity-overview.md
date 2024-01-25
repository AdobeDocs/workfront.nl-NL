---
title: De visualisatie van de teamcapaciteit bekijken in Verbeterde analyse
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: De de capaciteitsvisualisatie van het Team toont de totale hoeveelheid capaciteit een huisteam heeft, of zij of onderverdeeld zijn, en hoe dynamisch de capaciteit in tijd is.
author: Nolan
feature: Reports and Dashboards
exl-id: cfeb1a87-01be-4088-9e33-53a97e3871ad
source-git-commit: 81118e794dca746b482b8355c24fa997a9f0edc9
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 0%

---

# De visualisatie van de teamcapaciteit bekijken in Verbeterde analyse

<!-- Audited: 01/2024 -->

De de capaciteitsvisualisatie van het Team toont de totale hoeveelheid capaciteit een huisteam heeft, of zij of onderverdeeld zijn, en hoe dynamisch de capaciteit in tijd is.

![Teamcapaciteit](assets/team-capacity.png)

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>
      <p>Nieuw: alle</p>
      <p>of</p>
      <p>Huidig: Zakelijk of hoger</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td>
   <td>
      <p>Nieuw: Licht of hoger</p>
      <p>of</p>
      <p>Huidig: Controleren of hoger</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>Toegang tot projecten weergeven</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>Weergave </td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten

Voor eerste vereisten voor het gebruik van Enhanced Analytics raadpleegt u de sectie &quot;Voorwaarden&quot; in [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

## Begrijp de capaciteit van het Team visualisatie

De de capaciteitsvisualisatie van het Team toont het volume van het werk dat aan het huisteam op een bepaalde dag wordt toegewezen.

* **Doordrukken**: Wanneer de donkerdere blauwe vulkleur zich boven de stippellijn bevindt, heeft het huisteam meer werkuren toegewezen aan hen dan zij kunnen voltooien in het aantal uren dat het team beschikbaar is om te werken. Dit wijst erop dat het team oververdeeld is en zou burnout kunnen naderen.

  ![Overcapaciteit](assets/team-capacity-over-capacity.png)

* **Onbetwist**: Wanneer de donkerdere blauwe vulkleur onder de stippellijn ligt, heeft het home team meer werkuren dan de hoeveelheid werk die aan hen is toegewezen. Dit wijst erop dat het team onderverdeeld is en kan onbetwist zijn.

  ![Minder capaciteit](assets/team-capacity-under-capacity.png)

* **Balans**: Wanneer de lichtere of meer transparante blauwe vulkleur zich net boven, net onder of op de stippellijn bevindt, krijgt het huisteam een hoeveelheid werkuren toegewezen die ze binnen hun beschikbare werkuren moeten kunnen voltooien. Dit wijst erop dat de werklast van het team evenwichtiger is.

  ![Op capaciteit](assets/team-capacity-at-capacity.png)

Als u de muis boven een punt in de visualisatie houdt, ziet u de volgende details voor een bepaalde dag:

* **Geplande uren**: Dit is het aantal geplande werkuren dat het team moet voltooien.
* **Beschikbare uren**: Dit is het aantal werkuren dat het team beschikbaar is om te werken.
* **Capaciteit**: Naast een capaciteitspercentage worden ook de capaciteitsaanduidingen Op capaciteit, Onder capaciteit of Overcapaciteit weergegeven.

Aan de hand van deze informatie kunt u bepalen:

* Wanneer het huisteam werd oververdeeld of onderverdeeld.
* Als het huisteam dagelijks oververdeeld of onderverdeeld is.
* Hoe consistent de werklast van een thuisteam is van dag tot dag.
* Als u capaciteitsproblemen maakt met nieuw werk.

Ga voor meer informatie over de beste gegevens voor deze visualisatie naar [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

## De visualisatie van de teamcapaciteit weergeven

{{step1-to-analytics}}

1. Selecteer in het linkerdeelvenster de optie **Mensen**.

   ![Personen selecteren](assets/people-area-cropped-qs-350x276.png)

1. (Optioneel) Als u een ander datumbereik wilt gebruiken, selecteert u nieuwe begin- en einddatums in het filter voor het datumbereik.

   ![Filter datumbereik](assets/filters-select-date-range-350x344.png)

   Voor informatie over het gebruik van het filter Datumbereik raadpleegt u [Filters toepassen in uitgebreide analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Voorwaardelijk) als u uw filter van het Team niet hebt geplaatst, voeg de filter van het Team toe en selecteer elk team dat u gegevens voor wilt zien.

   Zie voor meer informatie over het toevoegen van filters in Verbeterde analysemogelijkheden [Filters toepassen in uitgebreide analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nadat u filters hebt toegevoegd, worden er gegevens voor maximaal 50 projecten weergegeven en blijven de filters actief, zelfs nadat u de pagina hebt verlaten of zich hebt afgemeld bij Workfront.

1. Voor de capaciteitvisualisatie van het Middel, klik een team om meer informatie te zien.

   De de capaciteitvisualisatievertoningen van het Team.

   Voor meer informatie over de capaciteit van het Middel visualisatie, zie [De visualisatie van de bronnencapaciteit bekijken in Verbeterde analyse](../enhanced-analytics/resource-capacity-overview.md).

1. (Optioneel) Als u wilt inzoomen op een datumbereik, selecteert u een punt in de visualisatie voor het begin van het datumbereik en sleept u naar het einde van het datumbereik.

   Alle andere visualisaties worden bijgewerkt naar hetzelfde datumbereik en er wordt een tijdframefilter gemaakt.

   ![Tijdlijnfilter](assets/timeframe-filter-350x220.png)

1. Houd de muisaanwijzer over een punt op de gespecificeerde lijn om de geplande uren en geplande uren voor de opgegeven datum te zien, alsmede het capaciteitspercentage en of het huisteam op dat moment over, onder of op capaciteit beschikte.

   ![Pop-up Teamcapaciteit](assets/team-capacity-capacity-pop-up-350x351.png)

1. (Optioneel) Als u de visualisatiegegevens wilt exporteren, klikt u op **Exporteren** pictogram ![Exportpictogram](assets/export.png) in de rechterbovenhoek van de visualisatie selecteert u de exportindeling:

   * Diagram (PNG)
   * Gegevenstabel (XSLX)

