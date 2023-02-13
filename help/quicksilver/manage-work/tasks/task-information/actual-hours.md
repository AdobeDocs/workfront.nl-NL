---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Werkelijke uren weergeven
description: De uren die u in Adobe Workfront inlogt op uw werkitems worden beschouwd als Werkelijke uren.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Werkelijke uren weergeven

De uren die u in Adobe Workfront inlogt op uw werkitems worden beschouwd als Werkelijke uren.

Werkelijke uren geven de werkelijke tijd aan waarin u een taak, uitgave of project hebt voltooid.

Wij adviseren dat de uren op het werkpunten zouden moeten worden geregistreerd, die taken en kwesties zijn.

Nochtans, als beheerder van Workfront, kunt u gebruikers toestaan om tijd op projecten, afhankelijk van wat de werkschema&#39;s in uw organisatie zijn te registreren.

Voor meer informatie over hoe te opstelling uw systeem om gebruikers toe te staan om tijd op projecten te registreren, zie [Voorkeuren voor tijdpagina&#39;s en uren configureren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>De mening of hogere toegang tot Taken, Projecten, of Kwesties</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Bekijk of hogere toestemmingen aan een taak, een project, of een kwestie</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Werkelijke uren voor taken en problemen versus Werkelijke uren voor projecten

De Werkelijke Uren op taken en kwesties vertegenwoordigen het aantal uren die rechtstreeks op de taken en de kwesties worden geregistreerd.

>[!NOTE]
>
>Werkelijke uren van onderliggende taken lopen door tot de werkelijke uren van de bovenliggende taak. De volgende formule is van toepassing voor de Werkelijke Uren op een oudertaak:

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

Werkelijke uren voor Projecten vertegenwoordigen een totaal van Werkelijke Uren van alle taken op het project (met inbegrip van uren die direct op oudertaken worden geregistreerd), alle kwesties op het project evenals de Werkelijke Uren die op het project zelf worden geregistreerd.

De volgende formule is van toepassing voor de Werkelijke Uren op een project:

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## Werkelijke uren zoeken

Het vinden van de waarde voor Werkelijke Uren voor een punt is identiek voor taken, projecten, en kwesties.

U vindt de informatie Werkelijke uren over taken op de volgende locaties:

* [Werkelijke uren in de sectie Details](#actual-hours-in-the-details-section)
* [Werkelijke uren in de sectie Uren](#actual-hours-in-the-hours-section)
* [Werkelijke uren in rapporten](#actual-hours-in-reports)
* [Werkelijke uren aan hulpmiddelen voor bronnenbeheer](#actual-hours-in-resource-management-tools)

### Werkelijke uren in de sectie Details {#actual-hours-in-the-details-section}

Werkelijke uren zoeken in de sectie Details is identiek voor projecten, taken en problemen.

Werkelijke uren zoeken in taakdetails:

1. Ga naar een taak waarvoor u de Werkelijke Uren wilt herzien.
1. Klikken **Taakdetails** in het linkerdeelvenster.
1. Klikken **Overzicht** en de **Werkelijke uren** waarde.

   Dit is het totaal aantal uren dat op deze taak is aangemeld.

### Werkelijke uren in de sectie Uren {#actual-hours-in-the-hours-section}

Het vinden van Werkelijke Uren in de sectie van Uren is identiek voor projecten, taken, en kwesties.

Werkelijke uren zoeken in de sectie Uren:

1. Ga naar een taak waarvoor u de Werkelijke Uren wilt herzien.
1. Klikken **Uren** in het linkerdeelvenster.

   Afhankelijk van uw configuratie, zou de sectie van Uren onder kunnen worden vermeld **Meer weergeven**.

   Dit toont een lijst van uuringangen die op de taak worden geregistreerd.

1. Zorg ervoor dat de **Standaard** en de **Project** groeperen wordt toegepast op deze lijst.

   Het getal dat wordt weergegeven in de groeperingsregel voor de **Uren** de kolom is het totale aantal Werkelijke Uren op de taak.

### Werkelijke uren in rapporten {#actual-hours-in-reports}

Wanneer het bouwen van taken, kwesties, of projectrapporten, kunt u de Werkelijke waarde van Uren voor elke taak, kwestie, of project in het rapport tonen.

Het toevoegen van de kolom Werkelijke uren aan een taakmening is gelijkaardig aan het bouwen van een mening in een rapport.

Werkelijke uren weergeven in een taakrapport:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Rapporten**.
1. Klikken **Nieuw rapport** en kiest u **Taak** als uw object.

1. Klikken **Kolom toevoegen** en begint te typen **Werkelijke uren** wanneer de **Tonen in deze kolom** vervolgkeuzelijst wordt weergegeven. Selecteer het veld wanneer dit in de lijst wordt weergegeven.

1. Klikken **Opslaan + Sluiten** om het rapport op te slaan.

   In de kolom Werkelijke uren wordt het aantal uren weergegeven dat voor elke taak is aangemeld.

### Werkelijke uren aan hulpmiddelen voor bronnenbeheer {#actual-hours-in-resource-management-tools}

Als u de vooruitgang wilt zien van het werk uw gebruikers aan hun toegewezen taken en kwesties doen, kunt u hen in de volgende hulpmiddelen van het Beheer van het Middel bekijken:

* Gebruiksrapport.\
   Voor informatie over het gebruiksrapport raadpleegt u [Overzicht van het verslag over het gebruik van hulpbronnen](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* Bronplanner.

   Voor informatie over het bekijken van Werkelijke Uren in de Planner van het Middel, zie [Beschikbare, geplande en Werkelijke uren of FTE weergeven in de bronnenplanner bij gebruik van de gebruikersweergave](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## Logtijd

U kunt tijd op taken, kwesties, en projecten op veelvoudige manieren registreren.

Voor meer informatie over het registreren van tijd in Workfront, zie [Logtijd](../../../timesheets/create-and-manage-timesheets/log-time.md).
