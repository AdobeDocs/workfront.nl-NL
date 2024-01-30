---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: Bekijk de visie van de projectreemap in Verbeterde analyse
description: De het treemapvisualisatie van het Project is een mening van uren-of dagen-die in een specifiek venster van tijd in vergelijking met andere het werkinspanningen in grootte zijn gewerkt. Hierdoor kunt u begrijpen hoeveel tijd mensen aan een project hebben besteed.
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Bekijk de visie van de projectreemap in Verbeterde analyse

<!-- Audited: 12/2023 -->

De het treemapvisualisatie van het Project is een mening van uren-of dagen-die in een specifiek venster van tijd in vergelijking met andere het werkinspanningen in grootte zijn gewerkt. Hierdoor kunt u begrijpen hoeveel tijd mensen aan een project hebben besteed.

![](assets/project-treemap-350x126.png){width="700"}

## Toegangsvereisten

U moet het volgende hebben:

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

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten

Voor eerste vereisten voor het gebruik van Enhanced Analytics raadpleegt u de sectie &quot;Voorwaarden&quot; in [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

## Begrijp de het treemap visualisatie van het Project

De dozen in de het treemap van het Project visualisatie vertegenwoordigen projecten en de grootte van de dozen toont een vergelijking van hoeveel tijd aan verschillende projecten werd besteed. Hoe groter de doos, hoe meer tijd wordt besteed aan het project.

De projectreemap-visualisatie bestaat uit:

* **Kleinere, lichtblauwe vakken**: Projecten met minder uren (of dagen) worden weergegeven als kleinere vakken met een lichtblauwe kleur.

  ![](assets/project-treemap-smaller-box.png)

* **Grotere, donkerblauwe vakken**: Projecten met meer uren (of dagen) worden weergegeven als grotere vakken met een donkerblauwe kleur.

  ![](assets/project-treemap-larger-box-350x205.png)

* **Blauwe vakken van standaardgrootte**: Projecten die tussen de twee categorieën vallen, worden weergegeven als middelgrote vakken met een blauwe tint tussen de donkerblauwe en lichtblauwe kleuren. Er zijn drie mogelijke tinten blauw voor de middelgrote dozen.

De legenda aan de rechterkant toont een uitsplitsing van voltooide uren voor elke schaduw van blauw. Deze legenda is dynamisch en wordt bijgewerkt op basis van de gegevens.

![](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>Als u de triomfvisualisatie van het Project door duur in plaats van door geplande uren bekijkt, toont deze legenda een verdeling van gewerkte dagen voor elke schaduw van blauw.\
>![](assets/project-treemap-days-worked.png)>

Aan de hand van deze informatie kunt u bepalen:

* De prioriteit van zaken die tijdens de geselecteerde datumwaaier worden gewerkt.
* Aan welke teams besteden we tijd.
* Als teams zich richten op de juiste dingen.
* Wanneer een specifiek project wordt geklikt, hoeveel het werkingsgebied van een project in die tijdspanne veranderde.

Ga voor meer informatie over de beste gegevens voor deze visualisatie naar [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

## De webstream van het project visualiseren

1. Klik op het pictogram Hoofdmenu ![](assets/main-menu-icon-16x12.png)selecteert u vervolgens **Analyse**.
1. (Optioneel) Als u een ander datumbereik wilt gebruiken, selecteert u nieuwe begin- en einddatums in het filter voor het datumbereik.

   ![](assets/filters-select-date-range-350x344.png)

   Voor informatie over het gebruik van het filter Datumbereik raadpleegt u [Filters toepassen in uitgebreide analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Voorwaardelijk) als u de reeks van projectgegevens moet beperken, selecteer en pas de filters toe die u wilt gebruiken.

   Zie voor meer informatie over het toevoegen van filters in Verbeterde analysemogelijkheden [Filters toepassen in uitgebreide analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nadat u filters hebt toegevoegd, worden er gegevens voor maximaal 50 projecten weergegeven en blijven de filters actief, zelfs nadat u de pagina hebt verlaten of zich hebt afgemeld bij Workfront.

1. (Optioneel) Als u de sortering van de projecten wilt wijzigen, klikt u op de knop **Sorteren op** in de rechterbovenhoek van de projectremap-visualisatie en selecteert u vervolgens een nieuwe sorteeroptie:

   * **A - Z**
   * **Z - A**
   * **Geplande voltooiingsdatum**
   * **Geplande begindatum**

   Alle andere visualisaties op de pagina worden bijgewerkt zodat deze overeenkomen met de geselecteerde sorteervolgorde.

1. (Voorwaardelijk) als er meer dan 50 projecten in uw gegevensreeks zijn, gebruik de pijlen in de bodem-linkerhoek van visualisatie om van één groep van 50 projecten aan volgende te navigeren.

   Alle andere visualisaties op de pagina worden bijgewerkt zodat deze overeenkomen met de geselecteerde pagina.

   ![](assets/pagination-350x118.png)

1. (Optioneel) De weergave wijzigen vanuit **geplande uren** tot **duur**.

   Geplande uren zijn standaard geselecteerd.

1. Beweeg over een project om de projectvoorwaarde, evenals het aantal geplande uren, het aantal voltooide uren in totaal, en het gemiddelde aantal uren aan het project per dag te zien.

   ![](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >Als u **duur** bekijken, zult u de volgende duurdetails zien:
   >
   >* **Geplande tijdlijn**: Het aantal dagen dat is gepland om het project te voltooien.
   >* **Dagen bewerkt**: De geplande duur voor elke taak die werd voltooid binnen het datumbereik dat aan de bovenkant is geselecteerd, gedeeld door het aantal uren in een dag.
   >   
   >![](assets/duration-treemap-350x159.png)
   >
   >Voor meer informatie over duur, zie de sectie &quot;mening van de Duur&quot;in [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

1. (Optioneel) Als u de visualisatiegegevens wilt exporteren, klikt u op **Exportpictogram** ![](assets/export.png) in de rechterbovenhoek van de visualisatie selecteert u de exportindeling:

   * **Diagram (PNG)**
   * **Gegevenstabel (XSLX)**

1. Klik een project om de Indruk en Taken in vluchtvisualisaties te openen om een dieper inzicht van te krijgen hoe de taken en uren-of dagen-bijgedragen aan de grootte van een project.

Voor meer informatie over de Burndown visualisatie, zie [Bekijk de Burndown-visualisatie in de uitgebreide analyse](../enhanced-analytics/burndown-overview.md). Voor meer informatie over de Taken in vluchtvisualisatie, zie [De taken tijdens de visualisatie van de vlucht bekijken in Verbeterde analyse](../enhanced-analytics/tasks-in-flight-overview.md).

