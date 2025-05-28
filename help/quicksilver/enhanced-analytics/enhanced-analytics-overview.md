---
title: Overzicht van uitgebreide analyses
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Verbeterde analyses zijn een krachtig hulpmiddel in Adobe Workfront met vooraf gebouwde visualisaties waarmee u projectgegevens kunt bekijken en trends kunt identificeren met planning en voltooiing. Met deze insight in uw projecten kunt u uw huidige werk beheren en kunt u nauwkeuriger plannen voor toekomstige werkzaamheden.
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '1243'
ht-degree: 0%

---

# Overzicht van uitgebreide analyses

>[!IMPORTANT]
>
>Enhanced Analytics is op 27 mei uit Workfront verwijderd. Workfront Data Connect is een nieuwe, alternatieve oplossing die kan worden gebruikt om alle Enhanced Analytics-visualisaties die u momenteel gebruikt, te repliceren. <br> zie de [ Verbeterde 2} gids van de Afleiding van Analytics {voor meer informatie.](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)


Verbeterde analyses zijn een krachtig hulpmiddel in Adobe Workfront met vooraf gebouwde visualisaties waarmee u projectgegevens kunt bekijken en trends kunt identificeren met planning en voltooiing. Met deze insight in uw projecten kunt u uw huidige werk beheren en kunt u nauwkeuriger plannen voor toekomstige werkzaamheden.

Uitgebreide analyses kunnen u helpen identificeren:

* De manier waarop u projecten plant
* Wanneer werk wordt toegevoegd aan projecten
* De hoeveelheid werk die voor verschillende projecten wordt voltooid
* De hoeveelheid uren of dagen die vereist is om een project te voltooien in vergelijking met de uren of dagen die een huisteam gepland heeft
* Hoe vaak de gebruikers specifieke acties tijdens een project voltooien
* De voortgang van projecten en de individuele taken binnen een project

![ Analytics ](assets/nwe-full-screen-analytics-350x222.png)

Om gebruiksgevallen te zien of meer te leren over het beheren van huidig werk en het plannen voor toekomstig werk met Verbeterde analyses, zie [ Verbeterde analytische het Leren Wegen ](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home).

## Vereisten

Voor toegang tot het gebied Verbeterde analysemogelijkheden moet u:

* Een bedrijfs- of ondernemingsplan hebben.

  Voor meer informatie, zie [ plannen van Workfront ](https://business.adobe.com/products/workfront/pricing.html).

* Uw Workfront-beheerder uitgebreide analyses laten toevoegen aan uw lay-outsjabloon.

  Voor meer informatie, zie [ Verbeterde Analytics: Het toevoegen van analyses aan lay-outmalplaatjes ](https://experienceleague.adobe.com/en/docs/workfront/using/home).

Om informatie voor projecten en taken te zien, moet u:

* Heb de toestemming van de Mening aan de Projecten en gebieden van Taken in uw toegangsniveau.

  Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie [ tot douanetoegangsniveaus ](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.

* Heb toestemming van de Mening voor specifieke taken en/of projecten.

  Voor informatie bij het verzoeken van extra toegang, zie [ Toegang van het Verzoek tot voorwerpen ](../workfront-basics/grant-and-request-access-to-objects/request-access.md).

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
  >Voor meer informatie, zie de sectie [ mening van de Duur ](#duration-view) in dit artikel.

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
>Het kan tot 24 uur duren voor wijzigingen in taken en projecten worden doorgevoerd in Verbeterde analysemogelijkheden.

## Weergave Duur {#duration-view}

Standaard zijn de video&#39;s voor het branden en het betreden van projecten gebaseerd op de geplande uren. Als uw teams geen geplande uren gebruiken, kunt u deze visualisaties bekijken die op projectduur worden gebaseerd.

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
  >8 uren is het standaardaantal voor **Typische uren per het werkdag**. Een beheerder van Adobe Workfront kan de **Typische uren per het werkdag** bijwerken plaatsend onder **Opstelling** > **Voorkeur van het Project** > **Projecten** > **Tijdlijnen**.\
  >Meer leren, zie [ systeem-brede projectvoorkeur ](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

Voor informatie over Geplande Duur, zie [ Overzicht van de Duur van het project ](../manage-work/projects/planning-a-project/project-duration.md).

## Sneltoetsen

U kunt de volgende toetsen op het toetsenbord gebruiken om door specifieke handelingen te navigeren of deze uit te voeren in het gedeelte Uitgebreide analyse:

| Sleutel | Handeling |
|---|---|
| **Lusje** | Navigeer naar elk element op de pagina en naar een tabel met informatie over elke visualisatie die niet op de pagina wordt weergegeven |
| **ga** binnen | Open de kalenderwidget, verwijder een bestaand filter, open toevoegt filteropties, selecteert/deselecteert filterwaarden, past een filter toe dat u hebt gecreeerd, opent de uitvoeropties op elke visualisatie, opent de drop-down menu&#39;s op de Doordrukking, Taken in vlucht, en de visualisaties van de projectopsporing |
| **de sleutels van de Pijl** | Navigeer naar datums in de kalenderwidget, door filteropties wanneer u een filter toevoegt, en door opties in alle drop-down menu&#39;s op de visualisaties |
| **Spatiebar** | Selecteer datums in de kalenderwidget, selecteer een filtertype wanneer u een filter toevoegt, selecteer een exportoptie in het vervolgkeuzemenu voor elke visualisatie en selecteer opties in de vervolgkeuzemenu&#39;s voor de Burndown, Taken tijdens de vlucht en voor de weergave van de projectreemap. |

{style="table-layout:auto"}

Als u schermleessoftware of een plug-in gebruikt, leest de schermlezer de informatie op het scherm hardop en beschrijft hij de handelingen die u uitvoert terwijl u de bovenstaande toetsen gebruikt.

## Verbeterde analyseweergaven en -functies

Raadpleeg de volgende artikelen voor meer informatie over de details van een specifieke functie in de uitgebreide analyse, de acties die u kunt uitvoeren om meer insight te verkrijgen en wat u van deze gegevens kunt leren:

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
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref"> pas filters in Verbeterde analyses toe </a> </td> 
   <td> <p>U kunt douanefilters, de filters van het projectgebied, of teamfilters toepassen om slechts projecten te bekijken die specifieke criteria passen. Als u filters toevoegt, wordt het aantal projecten dienovereenkomstig bijgewerkt.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref"> Begrijp Verbeterde analyses KPIs </a> </td> 
   <td> <p>De zeer belangrijke prestatiesindicatoren (KPIs) voor alle projecten binnen een specifiek tijdkader worden gevestigd bij de bovenkant van het scherm.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref"> Mening de visualisatie van het Plan van de Vlucht in Verbeterde analyses </a> </p> </td> 
   <td> <p>Het <b> plan van de Vlucht </b> visualisatie toont u de voorwaarde over het leven van een project is veranderd. Door te communiceren met de visualisatie krijgt u meer informatie over specifieke datums. Als u een project selecteert, worden de functie Burndown en Taken in de vluchtvisualisatie geopend.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref"> Mening de Burndown visualisatie in Verbeterde analyses </a> </td> 
   <td> <p>De </b> visualisatie 0} Burndown toont u de geplande snelheid van een project in vergelijking met de daadwerkelijke hoeveelheid uren besteed aan een project. <b> Het in wisselwerking staan met visualisatie geeft u meer details over de voorwaarde van het project op een specifieke datum.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref"> Mening de Taken in vluchtvisualisatie in Verbeterde analyses </a> </td> 
   <td> <p>De <b> Taken in vlucht </b> visualisatie toont u het statuut van elke taak binnen een project. Door te communiceren met de visualisatie kunt u snel en eenvoudig wijzigingen aanbrengen in een taak.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref"> Mening de activiteit van het Project visualisatie in Verbeterde analyses </a> </td> 
   <td> <p>De <b> activiteit van het Project </b> visualisatie toont u een heatmap van wanneer de gebruikers aan een project dat aan Workfront worden toegewezen, het statuut van taak in dat project veranderden, en voltooide taken in dat project. Door te communiceren met de visualisatie kunt u deze details voor elke gebruiker zien. U kunt ook specifieke datums voor deze acties zien, evenals het aantal keren dat elke actie is voltooid.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref"> Mening de boomtopvisualisatie van het Project in Verbeterde analyses </a> </td> 
   <td> <p>De <b> treemap van het Project </b> visualisatie toont u hoeveel tijd aan sommige projecten is besteed in vergelijking met anderen. In interactie met de visualisatie krijgt u details over de staat van het project, de geplande projectvoltooiing en de daadwerkelijke voltooiing van het project.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref"> Mening de Activiteit door teamvisualisatie in Verbeterde analyses </a> </td> 
   <td> <p>De <b> Activiteit door team </b> visualisatie toont u een heatmap van wanneer de gebruikers op een huisteam in Workfront het programma werden geopend, het statuut van een taak veranderde, en een taak voltooiden. Door met de visualisatie te communiceren, kunt u deze details voor elke individuele gebruiker zien. U kunt ook specifieke datums voor deze acties zien, evenals het aantal keren dat elke actie is voltooid.</p> </td> 
  </tr> 
  <!-- Features permanently removed from Workfront
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">View the Resource capacity visualization in Enhanced analytics</a> </td> 
   <td> <p>The <b>Resource capacity</b> visualization shows you which home teams have the capacity to take on more work and which home teams have more work assigned to them than they can complete. Interacting with the visualization allows you to see more details about work completed and available hours for more work.&nbsp;Selecting a team opens the Team capacity visualization.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">View the Team capacity visualization in Enhanced analytics</a> </td> 
   <td> <p>The <b>Team capacity</b> visualization shows you a percentage of the amount of work a home team has completed out of the amount of work assigned to them. Interacting with the visualization allows you to see scheduled hours and planned hours for a specific date, as well as the capacity percentage and whether the home team was over, under, or at capacity on that day.</p> </td> 
  </tr>--> 
 </tbody> 
</table>
