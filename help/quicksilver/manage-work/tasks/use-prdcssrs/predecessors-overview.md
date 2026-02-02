---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Overzicht van taakvoorgangers
description: Een voorganger is de taak waarvan een andere taak (een opvolger of afhankelijke taak genoemd) afhankelijk is. Adobe Workfront ondersteunt vijf typen afhankelijkheden van voorgangers.
author: Alina
feature: Work Management
exl-id: b2020a50-0921-4ed2-8a34-1a0411992b99
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '1184'
ht-degree: 0%

---

# Overzicht van voorgangers van taken

<!--Audited: 12/2023-->

<!-- 

CONTEXT SENSITIVE HELP article. DO NOT CHANGE THE NAME OF THE ARTICLE/ DO NOT MOVE OR DELETE! -->

Een voorganger is de taak waarvan een andere taak (een opvolger of afhankelijke taak genoemd) afhankelijk is. Adobe Workfront ondersteunt vijf typen afhankelijkheden van voorgangers. Om voorgangsafhankelijkheden te begrijpen, zie [&#x200B; Overzicht van de types van taakgebiedsdeel &#x200B;](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Overzicht van voorgangers

Kennis van de functionaliteit van de voorganger is belangrijk voor het begrijpen van de tijdlijnen in uw projecten.

De voorgangersverhoudingen van de taak bestaan zowel tussen taken binnen één enkel project als tussen taken van verschillende projecten.

In het geval van multi-project afhankelijkheid, kunt u dwars-project predecessors tussen taken van twee verschillende projecten vestigen.

Of de voorganger en opvolgertaken tot het zelfde project of tot twee verschillende projecten behoren, worden de gebiedsdelen en de chronologie van elk project berekend op de zelfde manier.

Wanneer het op predecessors aankomt, wordt de projectchronologie beïnvloed door het volgende:

* Afhankelijkheid van voorgangers
* Lagwaarde en -type\
  Voor meer informatie over zowel gebiedsdeel als de vertragingen, zie [&#x200B; Voorbeelden van voorgangerswaarden in een taaklijst &#x200B;](#examples-of-predecessor-values-in-a-task-list).

  Bijvoorbeeld, als taak A een voorganger is om B in een eindstartverhouding te taken, en taak B heeft een taakbeperking van zo snel mogelijk, dan wijst Workfront taak B een geplande begindatum onmiddellijk na de geplande voltooiingsdatum van taak A toe, ongeacht of voorganger wordt afgedwongen of niet.

Als u relaties met voorgangers wilt begrijpen, moet u begrijpen:

* **Types van Afhankelijkheid:** Predecessors zijn verbonden door diverse gebiedstypes. Voor meer informatie over gebiedsdeeltypes, zie [&#x200B; Overzicht van de types van taakgebiedsdeel &#x200B;](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

* **Uitvoerend een voorganger:** wanneer het afdwingen van een voorganger, kan de opvolgertaak absoluut niet beginnen tot voorganger voltooit. De opvolgertaak wordt weergegeven als onmiddellijk starten nadat de voorganger is voltooid.

  Wanneer de voorganger niet is voltooid (of is gestart) en niet wordt afgedwongen, kan de opvolgertaak worden gestart, maar is de projecttijdlijn nog steeds van invloed op de datums van zowel de voorganger als de opvolgertaken.

  Met een afgedwongen voorganger staat Workfront niet toe dat de opvolgertaak wordt gemarkeerd als Bezig of Voltooid totdat de voorganger is voltooid.

  Workfront staat echter toe dat er uren worden gerapporteerd over de taak.\
  Voor meer informatie bij het afdwingen van predecessors, zie [&#x200B; predecessors &#x200B;](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md) afdwingen.

* **Markeringen:** u kunt lagen in uw gebiedsdelen bouwen die tot een vertraging leiden die na de voltooiing van een voorgangerstaak en vóór de opvolgertaak moet voorkomen kan beginnen. Lags beïnvloeden de tijdlijn van het project.

  Om vertragingstypes te begrijpen, zie [&#x200B; Overzicht van de Types van Lag &#x200B;](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

## Relaties van voorgangers maken

Zie een of meer van de volgende artikelen om voordecessors te maken:

* Om predecessors te vestigen die het lusje van Predecessors van de taak gebruiken, zie [&#x200B; een voorgangersverhouding creëren gebruikend het gebied van Predecessors &#x200B;](../../../manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).
* Om predecessors in een taaklijst te vestigen, zie [&#x200B; een voorgangersverhouding op de taaklijst &#x200B;](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md) creëren.
* Om predecessor verhoudingen te vestigen door taken in een keten te plaatsen, zie [&#x200B; predecessor verhoudingen tot stand brengen door taken &#x200B;](../../../manage-work/tasks/use-prdcssrs/create-predecessors-by-chaining-tasks.md) in een keten te brengen.
* Om dwars-project predecessors te vestigen, zie [&#x200B; tot dwars-project predecessors &#x200B;](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md) leiden.

## De voorgangers van een taak zoeken {#locate-the-predecessors-of-a-task}

Als u de voorgangers van een taak wilt zoeken, voert u een van de volgende handelingen uit:

* Ga naar het project u werkt aan en doe het volgende:

   1. Zoek de taak waarvoor u de voorgangers wilt zoeken en klik op de taak.
   1. Klik **Predecessors** in het linkerpaneel.
   1. De naam van het project dat predecessor is op toont in het **Project** kolom.

      Het getal in de kolom **#** toont het vorige taaknummer. Bijvoorbeeld &quot;6&quot;betekent de zesde taak in het project.

      ![&#x200B; Predecessors sectie van taak &#x200B;](assets/predecessors-area-with-task-header.png)

* Ga naar het project u werkt aan en doe het volgende:

   1. Klik de **Taken** tabel.
   1. Kies de **StandaardMening** bij de bovenkant van de taaklijst.
   1. De **1&rbrace; kolom van Predecessors &lbrace;toont de aantallen van de voorgangertaak.**

      Voor een dwars-projectvoorganger, toont de kolom van Voorgangers het verwijzingsaantal van het project predecessor tot behoort en het aantal van de taak, die door een dubbelpunt wordt gescheiden.

      Het voorgangspictogram wordt groen als de voorganger de markering Voltooid heeft. Dit wijst erop dat de afhankelijke taak klaar voor het werk is.

      Houd de muisaanwijzer boven deze waarde voor meer informatie over de voorganger, het project en de datums.

      ![&#x200B; Details van de Predecessor &#x200B;](assets/predecessor-details-in-task-list.png)

## Voorbeelden van voorgangerswaarden in een takenlijst {#examples-of-predecessor-values-in-a-task-list}

Wanneer u predecessors in een lijst van taken bekijkt, zou u om het even welke volgende types van predecessors met hun respectieve Types van Afhankelijkheid en de bedragen van de Lag kunnen zien:

* **1fs -** het aantal van de voorgangertaak is 1. Het afhankelijkheidstype is Finish-Start. In de projectchronologie, is deze taak gepland om onmiddellijk te beginnen nadat taak 1 wordt gebeëindigd. Desondanks kan het nog worden gemarkeerd als Bezig of Voltooid.
* **1 -** het aantal van de voorgangstaak is 1. Dit is het zelfde als **1fs**, omdat **fs** de standaardvoorgangersverhouding in Workfront is.

* **1fse -** het aantal van de voorgangertaak is 1. Het afhankelijkheidstype is Voltooien-Begin-Geforceerd. In de projectchronologie, toont deze taak zoals aanvang onmiddellijk nadat taak 1 wordt gebeëindigd. Workfront staat niet toe dat het wordt gemarkeerd als Bezig of Voltooid totdat taak 1 is voltooid. Workfront staat echter toe dat er uren worden gerapporteerd over de taak.
* **1fs+3d -** het aantal van de voorgangertaak is 1. Het afhankelijkheidstype is Finish-Start met een vertragingstijd van 3 dagen. In de projectchronologie, toont deze taak als aanvang 3 werkdagen nadat taak 1 wordt gebeëindigd.
* **1fs-3d -** het aantal van de voorgangertaak is 1. Het afhankelijkheidstype is Finish-Start met een vertragingstijd van 3 dagen. In de projectchronologie, toont deze taak als aanvang 3 werkdagen alvorens de voorgangerstaak wordt gebeëindigd.
* **1fs+3de** - het aantal van de voorgangertaak is 1. Het afhankelijkheidstype is Voltooien-Begin-Geforceerd met een vertragingstijd van 3 dagen. In de projectchronologie, toont deze taak als aanvang 3 werkdagen nadat taak 1 wordt gebeëindigd. Workfront staat niet toe dat het wordt gemarkeerd als Bezig of Voltooid totdat Taak 1 is voltooid. Workfront staat echter toe dat er uren worden gerapporteerd over de taak.

  >[!NOTE]
  >
  >U moet de afgedwongen waarde (**e**) aan de Lag, en niet aan predecessor toevoegen.

* **4515:2** Het aantal van de voorgangertaak is 2. - Dit is een Einde aan Begin, niet-afgedwongen gebiedsdeel met predecessor in het project met verwijzingsaantal **4515**.

## Voorgangergegevens weergeven

U kunt voorganger-informatie weergeven in de volgende gebieden van Workfront. Dit omvat informatie over predecessors voor meerdere projecten:

* Op taakniveau, in de sectie Predecessors.

  Voor informatie over het bekijken van voorgangersinformatie in de sectie van Predecessors, zie de sectie [&#x200B; plaats van de voorgangers van een taak &#x200B;](#locate-the-predecessors-of-a-task) in dit artikel.

* In het Gantt-diagram.

  Voor informatie over het tonen van predecessors in de grafiek van Gantt, zie [&#x200B; vormen hoe de informatievertoningen op de Grafiek van Gantt &#x200B;](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

* In een takenlijst.

  Als u informatie wilt bekijken over de voorgangers van uw taken in een takenlijst, kunt u een van de volgende handelingen uitvoeren:

   * Pas de ingebouwde standaardweergave toe in een takenlijst.

     Voor informatie over het bekijken van voorgangersinformatie in de Standaardmening, zie de sectie [&#x200B; plaats van de voorgangers van een taak &#x200B;](#locate-the-predecessors-of-a-task) in dit artikel.

   * Bouw een taakmening of een rapport en voeg de kolom Predecessors aan die mening toe.

     Voor meer informatie over de bouw van een aangepaste mening voor taken met voorgangersinformatie, zie [&#x200B; Mening: voorgangersdetails &#x200B;](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-predecessor-details.md).

* In de taakkopbal wanneer het toegang tot van de taak.

  ![&#x200B; Info van de Predecessor in taakkopbal &#x200B;](assets/qs-predecessor-info-in-task-header-350x141.png)
