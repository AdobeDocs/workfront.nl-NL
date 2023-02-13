---
title: De visualisatie van projectactiviteit weergeven in Verbeterde analyse
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: De de activiteitenvisualisatie van het Project toont een gezamenlijke mening van activiteiten op het projectniveau-de activiteiten van elke persoon toegewezen aan project-die tijdens een specifiek tijdkader gebeurde. U kunt uw focus beperken om de activiteiten binnen een project te begrijpen, of u kunt projectactiviteiten vergelijken met andere projecten in Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# De visualisatie van projectactiviteit weergeven in Verbeterde analyse

De de activiteitenvisualisatie van het Project toont een gezamenlijke mening van activiteiten op het projectniveau-de activiteiten van elke persoon toegewezen aan project-die tijdens een specifiek tijdkader gebeurde. U kunt uw focus beperken om de activiteiten binnen een project te begrijpen, of u kunt projectactiviteiten vergelijken met andere projecten in Adobe Workfront.

>[!NOTE]
>
>De activiteit door teamvisualisatie gedraagt zich gelijkaardig aan deze visualisatie, maar de Activiteit door teamvisualisatie toont huisteamactiviteit voor alle projecten.\
>Voor informatie over de Activiteit door teamvisualisatie, zie [De activiteit per teamvisualisatie bekijken in Uitgebreide analyse](../enhanced-analytics/activity-by-team-overview.md).

<!--WRITER bad link; there is no Activity by Team.png
[![](assets/project-activity-350x114.png)](../Resources/Images/Analytics/Activity by Team.png)
-->

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront-plan</a>*</td> 
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

## Begrijp de activiteit van het Project visualisatie

Projectactiviteiten worden in verschillende kleuren weergegeven om een overzicht te geven van specifieke gebeurtenissen in een project over een bepaalde periode:

* **Gebruikers aangemeld**: De paarse dozen tonen dat de mensen die aan het project worden toegewezen het programma opende op die dag het programma. Een donkerdere tint geeft een groter aantal personen aan die zich aanmelden.

   ![](assets/project-activity-users-logged-in.png)

* **Wijziging taakstatus**: Roze dozen tonen dat mensen de status van een taak voor het project op die dag veranderden. Een donkerdere schaduw geeft aan dat er een groter aantal taakstatussen wordt gewijzigd.

   ![](assets/project-activity-task-status-changes.png)

* **Voltooide taken**: Blauwe vakken laten zien dat mensen een taak voor het project hebben uitgevoerd. Een donkerdere schaduw geeft een hoger aantal taken aan die worden voltooid.

   ![](assets/project-activity-tasks-completed.png)

Als u de muisaanwijzer boven een vak houdt, wordt exact aangegeven hoe vaak de handeling op een bepaalde dag is voltooid. U kunt een project selecteren om een verdeling van deze activiteiten door elke individuele medewerker op het project te zien.

Aan de hand van deze informatie kunt u bepalen:

* De activiteit op een specifiek project.
* De activiteit van één project in vergelijking met andere projecten.
* Welke gebruikers werken aan een project en met welke frequentie.

Ga voor meer informatie over de beste gegevens voor deze visualisatie naar [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

## De projectactiviteit visualiseren

1. Klik op het pictogram Hoofdmenu ![](assets/main-menu-icon-16x12.png)selecteert u vervolgens **Analyse**.
1. (Optioneel) Als u een ander datumbereik wilt gebruiken, selecteert u nieuwe begin- en einddatums in het filter voor het datumbereik.

   ![](assets/filters-select-date-range-350x344.png)

   Voor informatie over het gebruik van het filter Datumbereik raadpleegt u [Filters toepassen in uitgebreide analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

   >[!NOTE]
   >
   >Als u een datumbereik selecteert voor een periode van meer dan drie maanden, worden in de visualisatie van de projectactiviteit geen gegevens weergegeven.

1. (Voorwaardelijk) als u de reeks van projectgegevens moet beperken, selecteer en pas de filters toe die u wilt gebruiken.

   Voor meer informatie over het toevoegen van filters in Verbeterde analysemogelijkheden raadpleegt u [Filters toepassen in uitgebreide analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nadat u filters hebt toegevoegd, worden er gegevens voor maximaal 50 projecten weergegeven en blijven de filters actief, zelfs nadat u de pagina hebt verlaten of zich hebt afgemeld bij Workfront.

1. (Optioneel) Als u wilt inzoomen op een datumbereik, selecteert u een punt in de visualisatie voor het begin van het datumbereik en sleept u naar het einde van het datumbereik.

   Alle andere visualisaties worden bijgewerkt naar hetzelfde datumbereik en er wordt een tijdframefilter gemaakt.

   ![](assets/timeframe-filter-350x220.png)

1. (Optioneel) Als u de sortering van de projecten wilt wijzigen, klikt u op de knop **Sorteren op** selecteert u vervolgens een nieuwe sorteeroptie:

   * **A - Z**
   * **Z - A**
   * **Geplande voltooiingsdatum**
   * **Geplande begindatum**

   Alle andere visualisaties op de pagina worden bijgewerkt zodat deze overeenkomen met de geselecteerde sorteervolgorde.

1. (Voorwaardelijk) als er meer dan 50 projecten in uw gegevensreeks zijn, gebruik de pijlen in de bodem-linkerhoek van visualisatie om van één groep van 50 projecten aan volgende te navigeren.

   Alle andere visualisaties op de pagina worden bijgewerkt zodat deze overeenkomen met de geselecteerde pagina.

   ![](assets/pagination-350x118.png)

1. Klik een project in visualisatie om meer details voor het project te zien.

   De lijst breidt zich uit om de activiteiten van elke individuele medewerker op het project te tonen.

1. Plaats de muis boven een vak om de datum te zien waarop de gebruikers een handeling hebben uitgevoerd en het aantal keren dat de handeling voor die dag is voltooid.

   ![](assets/project-activity-activity-pop-up-350x137.png)

1. (Optioneel) Als u de visualisatiegegevens wilt exporteren, klikt u op de knop **Exportpictogram** ![](assets/export.png) in de rechterbovenhoek van de visualisatie selecteert u de exportindeling:

   * **Diagram (PNG)**
   * **Gegevenstabel (XSLX)**

