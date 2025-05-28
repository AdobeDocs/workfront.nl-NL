---
title: De visualisatie van projectactiviteit weergeven in Verbeterde analyse
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: De de activiteitenvisualisatie van het Project toont een gezamenlijke mening van activiteiten op het projectniveau-de activiteiten van elke persoon toegewezen aan project-die tijdens een specifiek tijdkader gebeurde. U kunt uw focus beperken om de activiteiten binnen een project te begrijpen, of u kunt projectactiviteiten vergelijken met andere projecten in Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# De visualisatie van projectactiviteit weergeven in Verbeterde analyse

>[!IMPORTANT]
>
>Enhanced Analytics is op 27 mei uit Workfront verwijderd. Workfront Data Connect is een nieuwe, alternatieve oplossing die kan worden gebruikt om alle Enhanced Analytics-visualisaties die u momenteel gebruikt, te repliceren. <br> zie de [ Verbeterde 2} gids van de Afleiding van Analytics {voor meer informatie.](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)


<!-- Audited: 12/2023 -->

De de activiteitenvisualisatie van het Project toont een gezamenlijke mening van activiteiten op het projectniveau-de activiteiten van elke persoon toegewezen aan project-die tijdens een specifiek tijdkader gebeurde. U kunt uw focus beperken om de activiteiten binnen een project te begrijpen, of u kunt projectactiviteiten vergelijken met andere projecten in Adobe Workfront.

>[!NOTE]
>
>De activiteit door teamvisualisatie gedraagt zich gelijkaardig aan deze visualisatie, maar de Activiteit door teamvisualisatie toont huisteamactiviteit voor alle projecten.\
>Voor informatie over de Activiteit door teamvisualisatie, zie [ de Activiteit door teamvisualisatie in Verbeterde analyses ](../enhanced-analytics/activity-by-team-overview.md) bekijken.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">Workfront-plan</a></td> 
   <td> <p>Zakelijk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Overzicht van Adobe Workfront-licenties</a></td> 
   <td>   <p>Nieuw:</p> 
   <ul><li>Licht of hoger</li></ul>
   <p>Huidige:</p>
   <ul><li>Controleren of hoger</li></ul>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten weergeven</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Weergave</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten

Voor eerste vereisten aan het gebruiken van Verbeterde Analytics, zie de &quot;sectie van Eerste vereisten&quot;in [ Verbeterd analyseoverzicht ](../enhanced-analytics/enhanced-analytics-overview.md).

## Begrijp de activiteit van het Project visualisatie

Projectactiviteiten worden in verschillende kleuren weergegeven om een overzicht te geven van specifieke gebeurtenissen in een project over een bepaalde periode:

* **Gebruikers het programma opende**: De paarse dozen tonen dat de mensen aan het project dat op die dag het programma worden geopend worden toegewezen. Een donkerdere tint geeft een groter aantal personen aan die zich aanmelden.

  ![ Gebruikers het programma geopend ](assets/project-activity-users-logged-in.png)

* **de statusverandering van de Taak**: De roze dozen tonen dat de mensen het statuut van een taak voor het project op die dag veranderden. Een donkerdere schaduw geeft aan dat er een groter aantal taakstatussen wordt gewijzigd.

  ![ de statusverandering van de Taak ](assets/project-activity-task-status-changes.png)

* **voltooide Taken**: De blauwe dozen tonen dat de mensen een taak voor het project voltooiden. Een donkerdere schaduw geeft een hoger aantal taken aan die worden voltooid.

  ![ voltooide Taken ](assets/project-activity-tasks-completed.png)

Als u de muisaanwijzer boven een vak houdt, wordt exact aangegeven hoe vaak de handeling op een bepaalde dag is voltooid. U kunt een project selecteren om een verdeling van deze activiteiten door elke individuele medewerker op het project te zien.

Aan de hand van deze informatie kunt u bepalen:

* De activiteit op een specifiek project.
* De activiteit van één project in vergelijking met andere projecten.
* Welke gebruikers werken aan een project en met welke frequentie.

Leren hoe te om de beste gegevens voor deze visualisatie te krijgen, zie [ Verbeterd analyseoverzicht ](../enhanced-analytics/enhanced-analytics-overview.md).

## De projectactiviteit visualiseren

1. Klik het Belangrijkste pictogram van het Menu ![ Belangrijkste menupictogram ](assets/main-menu-icon-16x12.png), dan uitgezochte **Analytics**.
1. (Optioneel) Als u een ander datumbereik wilt gebruiken, selecteert u nieuwe begin- en einddatums in het filter voor het datumbereik.

   ![ Uitgezochte datumwaaier ](assets/filters-select-date-range-350x344.png)

   Voor informatie bij het gebruiken van de filter van de datumwaaier, zie [ filters in Verbeterde analyses toepassen ](../enhanced-analytics/use-enhanced-analytics-filters.md).

   >[!NOTE]
   >
   >Als u een datumbereik selecteert voor een periode van meer dan drie maanden, worden in de visualisatie van de projectactiviteit geen gegevens weergegeven.

1. (Voorwaardelijk) als u de reeks van projectgegevens moet beperken, selecteer en pas de filters toe die u wilt gebruiken.

   Voor meer informatie bij het toevoegen van filters in Verbeterde analyses, zie [ filters in Verbeterde analyses toepassen ](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nadat u filters hebt toegevoegd, worden er gegevens voor maximaal 50 projecten weergegeven en blijven de filters actief, zelfs nadat u de pagina hebt verlaten of zich hebt afgemeld bij Workfront.

1. (Optioneel) Als u wilt inzoomen op een datumbereik, selecteert u een punt in de visualisatie voor het begin van het datumbereik en sleept u naar het einde van het datumbereik.

   Alle andere visualisaties worden bijgewerkt naar hetzelfde datumbereik en er wordt een tijdframefilter gemaakt.

   ![ filter Tijdframe ](assets/timeframe-filter-350x220.png)

1. (Facultatief) om te veranderen hoe de projecten worden gesorteerd, klik de **Soort door** menu, dan selecteer een nieuwe sorteeroptie:

   * **A - Z**
   * **Z - A**
   * **Geplande voltooiingsdatum**
   * **Geplande begindatum**

   Alle andere visualisaties op de pagina worden bijgewerkt zodat deze overeenkomen met de geselecteerde sorteervolgorde.

1. (Voorwaardelijk) als er meer dan 50 projecten in uw gegevensreeks zijn, gebruik de pijlen in de bodem-linkerhoek van visualisatie om van één groep van 50 projecten aan volgende te navigeren.

   Alle andere visualisaties op de pagina worden bijgewerkt zodat deze overeenkomen met de geselecteerde pagina.

   ![ Paginering ](assets/pagination-350x118.png)

1. Klik een project in visualisatie om meer details voor het project te zien.

   De lijst breidt zich uit om de activiteiten van elke individuele medewerker op het project te tonen.

1. Plaats de muis boven een vak om de datum te zien waarop de gebruikers een handeling hebben uitgevoerd en het aantal keren dat de handeling voor die dag is voltooid.

   ![ popup van de Activiteit ](assets/project-activity-activity-pop-up-350x137.png)

1. (Facultatief) om de visualisatiegegevens uit te voeren, klik het **pictogram van de Uitvoer** ![ pictogram van de Uitvoer ](assets/export.png) in de hoogste juiste hoek van de visualisatie, dan selecteer het uitvoerformaat:

   * **Grafiek (PNG)**
   * **Lijst van Gegevens (XSLX)**

