---
title: De activiteit per teamvisualisatie bekijken in Uitgebreide analyse
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: De activiteit door teamvisualisatie toont activiteiten die tijdens een specifiek tijdkader voor een huisteam gebeuren, toestaand u om te begrijpen hoe de verschillende huisteams hun tijd in Adobe Workfront besteedden. Afhankelijk van de manier waarop uw team in Workfront is ingesteld, kan deze visualisatie u verschillende inzichten geven en verschillende vragen beantwoorden.
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '766'
ht-degree: 0%

---

# De activiteit per teamvisualisatie bekijken in Uitgebreide analyse

>[!IMPORTANT]
>
>Enhanced Analytics is op 27 mei uit Workfront verwijderd. Workfront Data Connect is een nieuwe, alternatieve oplossing die kan worden gebruikt om alle Enhanced Analytics-visualisaties die u momenteel gebruikt, te repliceren. <br> zie de [ Verbeterde 2} gids van de Afleiding van Analytics {voor meer informatie.](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)



<!-- Audited: 12/2023 -->

De activiteit door teamvisualisatie toont activiteiten die tijdens een specifiek tijdkader voor een huisteam gebeuren, toestaand u om te begrijpen hoe de verschillende huisteams hun tijd in Adobe Workfront besteedden. Afhankelijk van de manier waarop uw team in Workfront is ingesteld, kan deze visualisatie u verschillende inzichten geven en verschillende vragen beantwoorden.

>[!NOTE]
>
>De activiteitenvisualisatie van het Project is gelijkaardig aan deze visualisatie, maar het toont activiteit die op mensen wordt gebaseerd die aan projecten eerder dan aan mensen worden toegewezen aan een huisteam wordt toegewezen.\
>Voor informatie over de activiteitenvisualisatie van het Project, zie [ de activiteitenvisualisatie van het Project in Verbeterde analyses ](../enhanced-analytics/project-activity-overview.md) bekijken.

![ Activiteit door team ](assets/activity-by-team-350x113.png){width="700"}

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

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
   <td>
      <p>Nieuw:</p> 
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

+++

## Vereisten

Voor eerste vereisten aan het gebruiken van Verbeterde Analytics, zie de &quot;sectie van Eerste vereisten&quot;in [ Verbeterd analyseoverzicht ](../enhanced-analytics/enhanced-analytics-overview.md).

## Begrijp de Activiteit door teamvisualisatie

De verschillende activiteiten worden in verschillende kleuren weergegeven om een overzicht te geven van specifieke gebeurtenissen tijdens de gefilterde periode:

* **Gebruikers het programma opende**: De paarse dozen tonen dat de mensen op het huisteam op die dag het programma opende. Een donkerdere tint geeft een groter aantal personen aan die zich aanmelden.

  ![ Gebruikers het programma geopend ](assets/project-activity-users-logged-in.png)

* **verandering van de status van de Taak**: De roze dozen tonen dat de mensen op het huisteam de status van een taak op die dag veranderden. Een donkerdere schaduw geeft aan dat er een groter aantal taakstatussen wordt gewijzigd.

  ![ de statusveranderingen van de Taak ](assets/project-activity-task-status-changes.png)

* **voltooide Taken**: De blauwe dozen tonen dat de mensen op het huisteam een taak op die dag voltooiden. Een donkerdere schaduw geeft een hoger aantal taken aan die worden voltooid.

  ![ voltooide Taken ](assets/project-activity-tasks-completed.png)

Als u de muisaanwijzer boven een vak houdt, wordt exact aangegeven hoe vaak de handeling op een bepaalde dag is voltooid. U kunt een team selecteren om een onderbreking van deze activiteiten door elke persoon op het huisteam te zien.

Aan de hand van deze informatie kunt u bepalen:

* Welke activiteiten doen zich voor binnen een huisteam en in welk tempo?
* Welke huisteams worden overwerkt of gebruiken meer het systeem.
* Als de distributie van het werk voor het huisteam aangewezen is.

Leren hoe te om de beste gegevens voor deze visualisatie te krijgen, zie [ Verbeterd analyseoverzicht ](../enhanced-analytics/enhanced-analytics-overview.md).

## De activiteit per teamvisualisatie weergeven

1. Klik het Belangrijkste pictogram van het Menu ![ Belangrijkste menupictogram ](assets/main-menu-icon-16x12.png), dan uitgezochte **Analytics**.
1. In het linkerpaneel, uitgezochte **Mensen**.

   ![ Gebied van Mensen ](assets/people-area-cropped-qs-350x276.png)

1. (Optioneel) Als u een ander datumbereik wilt gebruiken, selecteert u nieuwe begin- en einddatums in het filter voor het datumbereik.

   ![ Uitgezochte datumwaaier ](assets/filters-select-date-range-350x344.png)

   Voor informatie bij het gebruiken van de filter van de datumwaaier, zie [ filters in Verbeterde analyses toepassen ](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Voorwaardelijk) als u uw filter van het Team niet hebt geplaatst, voeg de filter van het Team toe en selecteer elk team dat u gegevens voor wilt zien.

   Voor meer informatie bij het toevoegen van filters in Verbeterde analyses, zie [ filters in Verbeterde analyses toepassen ](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nadat u filters hebt toegevoegd, worden er gegevens voor maximaal 50 projecten weergegeven en blijven de filters actief, zelfs nadat u de pagina hebt verlaten of zich hebt afgemeld bij Workfront.

1. (Optioneel) Als u wilt inzoomen op een datumbereik, selecteert u een punt in de visualisatie voor het begin van het datumbereik en sleept u naar het einde van het datumbereik.

   Alle andere visualisaties worden bijgewerkt naar hetzelfde datumbereik en er wordt een tijdframefilter gemaakt.

   ![ filter Tijdframe ](assets/timeframe-filter-350x220.png)

1. Klik op een teamnaam

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   or role
   </MadCap:conditionalText>
   -->

   meer details te zien over de activiteiten die door het team van de woning zijn voltooid.

   De lijst breidt zich uit om de activiteiten van elke persoon te tonen die aan het huisteam wordt toegewezen.

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Role not available</span>
   -->

1. Houd de muisaanwijzer boven een gekleurd vak om de datum te zien waarop gebruikers een handeling hebben uitgevoerd en het aantal keren dat de handeling die dag is voltooid.

   Donkere kleuren geven een hogere activiteit aan.

   ![ Activiteit door team ](assets/activity-by-team-activity-pop-up-350x155.png)

1. (Facultatief) om de visualisatiegegevens uit te voeren, klik het pictogram van de Uitvoer ![ ](assets/export.png) in de hoogste juiste hoek van de visualisatie, dan selecteer het uitvoerformaat:

   * **Grafiek (PNG)**
   * **Lijst van Gegevens (XSLX)**

