---
title: Overzicht van uitgebreide analyses
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Verbeterde analyses zijn een krachtig hulpmiddel in Adobe Workfront met vooraf gebouwde visualisaties waarmee u projectgegevens kunt bekijken en trends kunt identificeren met planning en voltooiing. Dit inzicht in uw projecten helpt u uw huidige werk te beheren en laat u toe om nauwkeuriger voor toekomstig werk te plannen.
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 0%

---

# Overzicht van uitgebreide analyses

Verbeterde analyses zijn een krachtig hulpmiddel in Adobe Workfront met vooraf gebouwde visualisaties waarmee u projectgegevens kunt bekijken en trends kunt identificeren met planning en voltooiing. Dit inzicht in uw projecten helpt u uw huidige werk te beheren en laat u toe om nauwkeuriger voor toekomstig werk te plannen.

Uitgebreide analyses kunnen u helpen identificeren:

* De manier waarop u projecten plant
* Wanneer werk wordt toegevoegd aan projecten
* De hoeveelheid werk die voor verschillende projecten wordt voltooid
* De hoeveelheid uren of dagen die vereist is om een project te voltooien in vergelijking met de uren of dagen die een huisteam gepland heeft
* Hoe vaak de gebruikers specifieke acties tijdens een project voltooien
* De voortgang van projecten en de individuele taken binnen een project

![](assets/nwe-full-screen-analytics-350x222.png)

Raadpleeg voor meer informatie over het gebruik of over het beheer van het huidige werk en de planning voor toekomstig werk met uitgebreide analysemogelijkheden de [Verbeterde analytische leerpaden](https://one.workfront.com/s/enhanced-analytics-program).

## Vereisten

Voor toegang tot het gebied Verbeterde analysemogelijkheden moet u:

* Een bedrijfs- of ondernemingsplan hebben.

   Zie voor meer informatie [Workfront-plannen](https://www.workfront.com/plans).

* Uw Workfront-beheerder uitgebreide analyses laten toevoegen aan uw lay-outsjabloon.

   Zie voor meer informatie [Verbeterde analysemogelijkheden: Analyses toevoegen aan lay-outsjablonen](https://one.workfront.com/s/managed-content-videos/enhanced-analytics-adding-analytics-to-layout-templates-MCH7URDSIXRREHHHF7TRTYYP2LTE).

Om informatie voor projecten en taken te zien, moet u:

* Heb de toestemming van de Mening aan de Projecten en gebieden van Taken in uw toegangsniveau.

   Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie [Aangepaste toegangsniveaus maken of wijzigen](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Heb toestemming van de Mening voor specifieke taken en/of projecten.

   Voor informatie over het aanvragen van aanvullende toegang raadpleegt u [Toegang tot objecten aanvragen](../workfront-basics/grant-and-request-access-to-objects/request-access.md).

## Aanbevolen werkwijzen voor verbeterde analysemogelijkheden

Om de beste gegevens voor uw projecten te krijgen, gebruik malplaatjes die nauwkeurige geplande uren en duurdagen hebben. U moet er ook voor zorgen dat uw gebruikers de onderstaande velden zo nauwkeurig mogelijk invoeren en bijwerken.

>[!NOTE]
>
>Sommige van de volgende velden zijn berekeningen die Workfront uitvoert op basis van informatie die gebruikers invoeren. U kunt deze velden niet handmatig bijwerken.

* Geplande uren

   Dit is het belangrijkste veld dat moet worden ingevuld.

   >[!NOTE]
   >
   >Als uw teams niet geplande uren gebruiken, kunt u sommige gegevens nog zien die op projectduur worden gebaseerd.\
   >Zie de sectie voor meer informatie [Weergave Duur](#duration-view) in dit artikel.

* Projectnaam

   De naam moet een beschrijving van het project zijn.

* Projectvoorwaarde
* Projectstatus
* Begindatum van project
* Geplande afsluitdatum
* Werkelijke begindatum van project
* Werkelijke einddatum van project
* Tijdsduur project
* Werkelijke uren van project
* Taakstatus (dit omvat het markeren van voltooide taken.)
* Taaknaam
* Taakpercentage voltooid
* Begindatum van taak gepland
* Taak geplande voltooiingsdatum

>[!IMPORTANT]
>
>Het kan tot 24 uur duren voor wijzigingen in taken en projecten worden doorgevoerd in Verbeterde analyses.

## Weergave Duur {#duration-view}

Standaard zijn de video&#39;s voor het branden en het betreden van projecten gebaseerd op geplande uren. Als uw teams geen geplande uren gebruiken, kunt u deze visualisaties bekijken die op projectduur worden gebaseerd.

In de uitgebreide analyse wordt de duur van een project berekend aan de hand van de volgende formules:

* Gepland tijdschema:

   ```
   Planned Completion Date of the project - Start Date of the project
   ```

* Aantal werkdagen:

   ```
   Planned Duration for tasks completed in the selected date range / Typical hours per work day
   ```

   >[!NOTE]
   >
   >8 uur is het standaardnummer voor **Normaal aantal uren per werkdag**. Een Adobe Workfront-beheerder kan de **Normaal aantal uren per werkdag** instellen onder **Instellen** > **Projectvoorkeuren** > **Projecten** > **Tijdlijnen**.\
   >Zie voor meer informatie [Projectvoorkeuren voor het hele systeem configureren](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Voor informatie over Geplande Duur, zie [Overzicht van de duur van het project](../manage-work/projects/planning-a-project/project-duration.md).

## Sneltoetsen

U kunt de volgende toetsen op het toetsenbord gebruiken om door specifieke handelingen te navigeren of deze uit te voeren in het gedeelte Uitgebreide analyse:

| Sleutel | Handeling |
|---|---|
| **Tab** | Navigeer naar elk element op de pagina en naar een tabel met informatie over elke visualisatie die niet op de pagina wordt weergegeven |
| **Enter** | Open de kalenderwidget, verwijder een bestaand filter, open toevoegt filteropties, selecteert/deselecteert filterwaarden, past een filter toe dat u hebt gecreeerd, opent de uitvoeropties op elke visualisatie, opent de drop-down menu&#39;s op de Doordrukking, Taken in vlucht, en de visualisaties van de projectopsporing |
| **Pijltoetsen** | Navigeer naar datums in de kalenderwidget, door filteropties wanneer u een filter toevoegt, en door opties in alle drop-down menu&#39;s op de visualisaties |
| **Spatiebalk** | Selecteer datums in de kalenderwidget, selecteer een filtertype wanneer u een filter toevoegt, selecteer een exportoptie in het vervolgkeuzemenu voor elke visualisatie en selecteer opties in de vervolgkeuzemenu&#39;s voor de Burndown, Taken tijdens de vlucht en voor de weergave van de projectreemap. |

{style=&quot;table-layout:auto&quot;}

Als u schermleessoftware of een plug-in gebruikt, leest de schermlezer de informatie op het scherm hardop en beschrijft hij de handelingen die u uitvoert terwijl u de bovenstaande toetsen gebruikt.

## Verbeterde analyseweergaven en -functies

Raadpleeg de volgende artikelen voor meer informatie over de details van een specifieke functie in de uitgebreide analyse, de handelingen die u kunt uitvoeren om meer inzicht te krijgen en wat u van deze gegevens kunt leren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Artikel</th> 
   <th>Toelichting</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Filters toepassen in uitgebreide analyse</a> </td> 
   <td> <p>U kunt douanefilters, de filters van het projectgebied, of teamfilters toepassen om slechts projecten te bekijken die specifieke criteria passen. Als u filters toevoegt, wordt het aantal projecten dienovereenkomstig bijgewerkt.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref">Uitgebreide KPI's voor analysemogelijkheden begrijpen</a> </td> 
   <td> <p>De zeer belangrijke prestatiesindicatoren (KPIs) voor alle projecten binnen een specifiek tijdkader worden gevestigd bij de bovenkant van het scherm.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">Bekijk de visualisatie van het vliegplan in de uitgebreide analyse</a> </p> </td> 
   <td> <p>De <b>Vliegplan</b> visualisatie laat zien dat de conditie is veranderd gedurende de levensduur van een project. Door te communiceren met de visualisatie krijgt u meer informatie over specifieke datums. Als u een project selecteert, worden de functie Branden en Taken in de vluchtvisualisatie geopend.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">Bekijk de Burndown-visualisatie in de uitgebreide analyse</a> </td> 
   <td> <p>De <b>Burndown</b> de visualisatie toont u de geplande snelheid van een project in vergelijking met de daadwerkelijke hoeveelheid uren besteed aan een project. Het in wisselwerking staan met visualisatie geeft u meer details over de voorwaarde van het project op een specifieke datum.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">De taken tijdens de visualisatie van de vlucht bekijken in Verbeterde analyse</a> </td> 
   <td> <p>De <b>Taken tijdens de vlucht</b> de visualisatie toont u het statuut van elke taak binnen een project. Door te communiceren met de visualisatie kunt u snel en eenvoudig wijzigingen aanbrengen in een taak.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref">De visualisatie van projectactiviteit weergeven in Verbeterde analyse</a> </td> 
   <td> <p>De <b>Projectactiviteit</b> de visualisatie toont u een heatmap van wanneer de gebruikers aan een project dat aan Workfront worden toegewezen, de status van taak in dat project veranderden, en taken in dat project voltooiden. Door te communiceren met de visualisatie kunt u deze details voor elke gebruiker zien. U kunt ook specifieke datums voor deze acties zien, evenals het aantal keren dat elke actie is voltooid.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">Bekijk de visie van de projectreemap in Verbeterde analyse</a> </td> 
   <td> <p>De <b>Projectreemap</b> de visualisatie laat zien hoeveel tijd er is besteed aan bepaalde projecten in vergelijking met andere projecten . In interactie met de visualisatie krijgt u details over de staat van het project, de geplande projectvoltooiing en de daadwerkelijke voltooiing van het project.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref">De activiteit per teamvisualisatie bekijken in Uitgebreide analyse</a> </td> 
   <td> <p>De <b>Activiteit per team</b> de visualisatie toont u een heatmap van wanneer de gebruikers op een huisteam in Workfront het programma werden geopend, de status van een taak veranderden, en een taak voltooiden. Door met de visualisatie te communiceren, kunt u deze details voor elke individuele gebruiker zien. U kunt ook specifieke datums voor deze acties zien, evenals het aantal keren dat elke actie is voltooid.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">De visualisatie van de bronnencapaciteit bekijken in Verbeterde analyse</a> </td> 
   <td> <p>De <b>Broncapaciteit</b> de visualisatie toont u welke huisteams de capaciteit hebben om meer werk over te nemen en welke huisteams meer werk toegewezen aan hen hebben dan zij kunnen voltooien. Door te communiceren met de visualisatie kunt u meer informatie zien over voltooide en beschikbare uren voor meer werk. Het selecteren van een team opent de capaciteit van het Team visualisatie.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">De visualisatie van de teamcapaciteit bekijken in Verbeterde analyse</a> </td> 
   <td> <p>De <b>Teamcapaciteit</b> de visualisatie toont u een percentage van de hoeveelheid werk een huisteam uit de hoeveelheid werk heeft voltooid dat aan hen wordt toegewezen. Door te communiceren met de visualisatie kunt u geplande uren en geplande uren voor een bepaalde datum zien, evenals het capaciteitspercentage en of het team van de woning op die dag over, onder of op capaciteit was.</p> </td> 
  </tr> 
 </tbody> 
</table>
