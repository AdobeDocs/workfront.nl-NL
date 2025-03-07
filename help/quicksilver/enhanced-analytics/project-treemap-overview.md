---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: Bekijk de visie van de projectreemap in Verbeterde analyse
description: De het treemapvisualisatie van het Project is een mening van uren-of dagen-die in een specifiek venster van tijd in vergelijking met andere het werkinspanningen in grootte zijn gewerkt. Hierdoor kunt u begrijpen hoeveel tijd mensen aan een project hebben besteed.
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 59e021aa3ae66e4fc8d9ce9eb57616f948e6cd90
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---

# Bekijk de visie van de projectreemap in Verbeterde analyse

>[!IMPORTANT]
>
>Enhanced Analytics wordt de week van 26 mei uit Workfront verwijderd. Workfront Data Connect is een nieuwe, alternatieve oplossing die kan worden gebruikt om alle Enhanced Analytics-visualisaties die u momenteel gebruikt, te repliceren. <br> zie de [ Verbeterde 2} gids van de Afleiding van Analytics {voor meer informatie.](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)


<!-- Audited: 12/2023 -->

De het treemapvisualisatie van het Project is een mening van uren-of dagen-die in een specifiek venster van tijd in vergelijking met andere het werkinspanningen in grootte zijn gewerkt. Hierdoor kunt u begrijpen hoeveel tijd mensen aan een project hebben besteed.

![ de treemap van het Project ](assets/project-treemap-350x126.png){width="700"}

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront-plan</a></td> 
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

+++

## Vereisten

Voor eerste vereisten aan het gebruiken van Verbeterde Analytics, zie de &quot;sectie van Eerste vereisten&quot;in [ Verbeterd analyseoverzicht ](../enhanced-analytics/enhanced-analytics-overview.md).

## Begrijp de het treemap visualisatie van het Project

De dozen in de het treemap van het Project visualisatie vertegenwoordigen projecten en de grootte van de dozen toont een vergelijking van hoeveel tijd aan verschillende projecten werd besteed. Hoe groter de doos, hoe meer tijd wordt besteed aan het project.

De projectreemap-visualisatie bestaat uit:

* **Kleinere, lichtblauwe dozen**: De projecten die minder uren-of dagen-vertoning als kleinere dozen met een lichtblauwe kleur hebben.

  ![ Kleinere doos ](assets/project-treemap-smaller-box.png)

* **Grotere, donkerblauwe dozen**: Projecten die meer uren-of dagen-vertoning als grotere dozen met een donkerblauwe kleur hebben.

  ![ Grotere doos ](assets/project-treemap-larger-box-350x205.png)

* **Medium-Grootte, blauwe dozen**: De projecten die binnen tussen de twee categorieën vallen tonen als middelgrote dozen met een schaduw van blauw tussen de donkerblauwe en lichtblauwe kleuren. Er zijn drie mogelijke tinten blauw voor de middelgrote dozen.

De legenda aan de rechterkant toont een uitsplitsing van voltooide uren voor elke schaduw van blauw. Deze legenda is dynamisch en wordt bijgewerkt op basis van de gegevens.

![ voltooide uren Treemap ](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>Als u de triomfvisualisatie van het Project door duur in plaats van door geplande uren bekijkt, toont deze legenda een verdeling van gewerkte dagen voor elke schaduw van blauw.\
>![ de gewerkte dagen van de Treemap ](assets/project-treemap-days-worked.png)>

Aan de hand van deze informatie kunt u bepalen:

* De prioriteit van zaken die tijdens de geselecteerde datumwaaier worden gewerkt.
* Aan welke teams besteden we tijd.
* Als teams zich richten op de juiste dingen.
* Wanneer een specifiek project wordt geklikt, hoeveel het werkingsgebied van een project in die tijdspanne veranderde.

Leren hoe te om de beste gegevens voor deze visualisatie te krijgen, zie [ Verbeterd analyseoverzicht ](../enhanced-analytics/enhanced-analytics-overview.md).

## De webstream van het project visualiseren

1. Klik het Belangrijkste pictogram van het Menu ![ Belangrijkste menupictogram ](assets/main-menu-icon-16x12.png), dan uitgezochte **Analytics**.
1. (Optioneel) Als u een ander datumbereik wilt gebruiken, selecteert u nieuwe begin- en einddatums in het filter voor het datumbereik.

   ![ Uitgezochte datumwaaier ](assets/filters-select-date-range-350x344.png)

   Voor informatie bij het gebruiken van de filter van de datumwaaier, zie [ filters in Verbeterde analyses toepassen ](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Voorwaardelijk) als u de reeks van projectgegevens moet beperken, selecteer en pas de filters toe die u wilt gebruiken.

   Voor meer informatie bij het toevoegen van filters in Verbeterde analyses, zie [ filters in Verbeterde analyses toepassen ](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nadat u filters hebt toegevoegd, worden er gegevens voor maximaal 50 projecten weergegeven en blijven de filters actief, zelfs nadat u de pagina hebt verlaten of zich hebt afgemeld bij Workfront.

1. (Facultatief) om te veranderen hoe de projecten worden gesorteerd, klik de **Soort door** menu in de hoger-juiste hoek van de het treemap van het Project visualization, dan selecteer een nieuwe sorterende optie:

   * **A - Z**
   * **Z - A**
   * **Geplande voltooiingsdatum**
   * **Geplande begindatum**

   Alle andere visualisaties op de pagina worden bijgewerkt zodat deze overeenkomen met de geselecteerde sorteervolgorde.

1. (Voorwaardelijk) als er meer dan 50 projecten in uw gegevensreeks zijn, gebruik de pijlen in de bodem-linkerhoek van visualisatie om van één groep van 50 projecten aan volgende te navigeren.

   Alle andere visualisaties op de pagina worden bijgewerkt zodat deze overeenkomen met de geselecteerde pagina.

   ![ Paginering ](assets/pagination-350x118.png)

1. (Facultatief) verander de mening van **geplande uren** aan **duur**.

   Geplande uren zijn standaard geselecteerd.

1. Beweeg over een project om de projectvoorwaarde, evenals het aantal geplande uren, het aantal voltooide uren in totaal, en het gemiddelde aantal uren aan het project per dag te zien.

   ![ het projectdetails van de Treemap ](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >Als u de **duur** mening selecteerde, zult u de volgende duurdetails zien:
   >
   >* **Gepland Tijdframe**: Het aantal dagen gepland om het project te voltooien.
   >* **Werkte Dagen**: De geplande duur voor elke taak die binnen de geselecteerde datumwaaier bij de bovenkant werd voltooid, die door het aantal uren in een dag wordt gedeeld.
   >   
   >![ duur Treemap ](assets/duration-treemap-350x159.png)
   >
   >Voor meer informatie over duur, zie de sectie &quot;mening van de Duur&quot;in [ Verbeterde analyse overzicht ](../enhanced-analytics/enhanced-analytics-overview.md).

1. (Facultatief) om de visualisatiegegevens uit te voeren, klik het **pictogram van de Uitvoer** ![ pictogram van de Uitvoer ](assets/export.png) in de hoogste juiste hoek van de visualisatie, dan selecteer het uitvoerformaat:

   * **Grafiek (PNG)**
   * **Lijst van Gegevens (XSLX)**

1. Klik een project om de Indruk en Taken in vluchtvisualisaties te openen om een dieper inzicht van te krijgen hoe de taken en uren-of dagen-bijgedragen aan de grootte van een project.

Voor meer informatie over de Visualisatie van de Doordrukking, zie [ Mening de Visualisatie van de Doordrukking in Verbeterde analyses ](../enhanced-analytics/burndown-overview.md). Voor meer informatie over de Taken in vluchtvisualisatie, zie [ Mening de Taken in vluchtvisualisatie in Verbeterde analyses ](../enhanced-analytics/tasks-in-flight-overview.md).

