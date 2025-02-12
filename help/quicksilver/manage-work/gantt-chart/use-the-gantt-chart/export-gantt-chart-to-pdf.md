---
navigation-topic: use-the-gantt-chart
title: Gantt-diagram exporteren naar PDF
description: U kunt het Gantt-diagram exporteren naar een PDF. Nadat u het Gantt-diagram naar PDF hebt geëxporteerd, kunt u het afdrukken of als bijlage aan een e-mailbericht toevoegen om het met andere gebruikers te delen.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# [!UICONTROL Gantt Chart] exporteren naar PDF

<!--Audited: 09/2024-->

U kunt de [!UICONTROL Gantt chart] naar een PDF exporteren.

Nadat u de [!UICONTROL Gantt chart] naar PDF hebt geëxporteerd, kunt u deze afdrukken of als bijlage aan een e-mailbericht toevoegen om deze met andere gebruikers te delen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben om de stappen in dit artikel te volgen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] plan*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] licentie*</td> 
   <td> <p>Nieuw:[!UICONTROL Light] of hoger</p>
   <p>Huidig:[!UICONTROL Review] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>[!UICONTROL View] of betere toegang tot Projecten en Taken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>[!UICONTROL View] of een betere toegang tot het project</p> </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## De [!UICONTROL Gantt chart] exporteren

1. Heb toegang tot [!UICONTROL Gantt chart] dat u naar PDF wilt uitvoeren, zoals die in [ wordt beschreven begonnen met [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Zorg ervoor dat u de [!UICONTROL Gantt chart] zodanig hebt geconfigureerd dat de juiste informatie wordt weergegeven voordat u deze exporteert.

   >[!NOTE]
   >
   >Als u [!UICONTROL Gantt chart] uit een lijst van projecten uitvoert, bevat het dossier van PDF enkel de projecten in de lijst, niet de taken op elk project. Als u een lijst van taken wilt uitvoeren, kunt u dit van het project doen zij met, of door een taakrapport te bouwen en de resultaten van het rapport in [!UICONTROL Gantt View] te tonen worden geassocieerd.

   Configureer een van de volgende gegevens:

   * Klik de **Filters**, **Mening**, en **Groepering** pictogrammen boven [!UICONTROL Gantt chart] en voeg of geef de bestaande filter, mening toe uit, of groepering die op de lijst van punten in [!UICONTROL Gantt chart] wordt toegepast.

     Alle filters en groepen die in de lijstweergave zijn geselecteerd, blijven behouden wanneer de [!UICONTROL Gantt chart] wordt weergegeven. Weergaven worden alleen weerspiegeld in de geëxporteerde [!UICONTROL Gantt chart] pagina in de lijst die naast de [!UICONTROL Gantt chart] op de eerste pagina wordt weergegeven. Weergaven worden niet weergegeven op de [!UICONTROL Gantt chart] zelf.

     >[!TIP]
     >
     >Als u meer ruimte voor de [!UICONTROL Gantt chart] zelf wilt toestaan, past u een weergave toe die zo weinig mogelijk kolommen bevat.

   * Selecteer de **Schakelaar aan Geprojecteerde Datums** optie om Geprojecteerde eerder dan Geplande Datums te bekijken. Standaard worden Geplande datums weergegeven.

   * Klik het **pictogram van Montages ![ pictogram van Montages ](assets/settings-icon.png) in de hoger-juiste hoek van de grafiek van Gantt en selecteer welke informatie u in de grafiek van Gantt wilt bekijken.** Zodra deze optie is geselecteerd, wordt deze informatie opgenomen in het geëxporteerde Gantt PDF-bestand.

     Selecteer een van de volgende opties:

      * Werkelijke datums
      * Toewijzingen
      * Basislijn
      * Vastlegdatum
      * % voltooid
      * Kritiek pad
      * Mijlsteendiamanten
      * Mijlsteenlijnen
      * Predecessors
      * Voortgangsstatus
      * Geplande data

     Zie voor meer informatie   [ vormt hoe de informatievertoningen op [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > Toewijzingen worden niet weergegeven op de [!UICONTROL Gantt chart] wanneer de [!UICONTROL Gantt chart] wordt geëxporteerd naar PDF. Wanneer [!UICONTROL Gantt chart] naar PDF wordt geëxporteerd, worden toewijzingen alleen weergegeven in de lijstweergave.

   * De tijdsperiode die wordt weergegeven op de [!UICONTROL Gantt chart] .

     Voor meer informatie, zie [ het Bekijken van Informatie in [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

     De manier waarop de periode in het exportbestand wordt weergegeven, hangt af van het feit of u **[!UICONTROL What I see]** of **[!UICONTROL Multiple pages]** in een latere stap selecteert.

1. (Optioneel) Als u alleen bepaalde taken in de geëxporteerde PDF wilt opnemen, selecteert u de taken die u wilt opnemen.

   Als u geen taken selecteert, worden alle taken opgenomen in de geëxporteerde PDF.

   Als u bijvoorbeeld [!UICONTROL Gantt chart] weergeeft voor een project dat 50 taken bevat, maar u wilt slechts 10 taken weergeven voor het geëxporteerde project [!UICONTROL Gantt chart] , selecteert u de 10 taken die u wilt weergeven.

1. Klik het pictogram van de printer ![ Printer ](assets/printer-icon.png) in de hoger-juiste hoek van de grafiek van Gantt.
Het dialoogvenster **[!UICONTROL Export to PDF]** wordt weergegeven.

   ![ export_gantt_UI.png ](assets/exported-gantt-ui-350x225.png)

1. In de **sectie van de Uitvoer**, selecteer van de volgende opties om erop te wijzen of u slechts wilt uitvoeren wat u of het volledige [!UICONTROL Gantt chart] ziet:

   * **[!UICONTROL What I see]:** exporteert alle taken (inclusief eventuele subtaken) die op het scherm worden weergegeven voordat maximaal 500 items worden geëxporteerd. (Dit wordt niet weergegeven in de sectie **[!UICONTROL Preview]** . De sectie [!UICONTROL Preview] bevat alleen voorbeeldgegevens.)

     Subtaken worden opgenomen in de geëxporteerde PDF, zelfs als de bovenliggende taak is samengevouwen en de subtaken niet zichtbaar zijn. Als u alleen bovenliggende taken wilt opnemen, selecteert u de bovenliggende taken die u wilt opnemen en schakelt u de subtaken uit.

     >[!TIP]
     >
     >U kunt het **[!UICONTROL Zoom To]** drop-down menu of het schuif gebruiken om slechts een gedeelte van [!UICONTROL Gantt chart] te tonen, zoals die in [ wordt beschreven het Bekijken Informatie in [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).


   * **[!UICONTROL Multiple pages]:** exporteert de volledige [!UICONTROL Gantt chart] , zelfs de items die niet zichtbaar zijn op het huidige scherm, tot maximaal 500 items.

     >[!NOTE]
     >
     >* U kunt het **[!UICONTROL Zoom To]** drop-down menu of het schuif hulpmiddel gebruiken om te bepalen hoeveel informatie op elke pagina wordt getoond, zoals die in [ wordt beschreven vormt hoe de informatie over [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md) toont. Selecteer een gedetailleerdere optie als u meer te exporteren pagina&#39;s wilt weergeven of selecteer een minder korrelige optie als u minder te exporteren pagina&#39;s wilt weergeven.
     >
     >* Als u een [!UICONTROL Gantt chart] wilt exporteren die meer dan 500 items bevat, past u een filter op de lijst toe voordat u de [!UICONTROL Gantt chart] weergeeft, zodat er minder dan 500 items of 250 pagina&#39;s worden weergegeven. Voor informatie over hoe te om een filter toe te passen, zie [ Overzicht van Filters ](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >* U kunt het volledige Gantt-diagram niet in de volgende omstandigheden exporteren:
     >   
     >   * Als het meer dan 250 pagina&#39;s beslaat
     >   * Als het meer dan 500 items bevat


1. Als de PDF wordt afgedrukt nadat deze is geëxporteerd naar PDF, selecteert u in de vervolgkeuzelijst **[!UICONTROL Page Size]** het papierformaat waarnaar u wilt afdrukken.
U kunt uit de volgende opties selecteren:

   * **[!UICONTROL Letter]**
   * **[!UICONTROL Legal]**
   * **[!UICONTROL Ledger]**
   * **[!UICONTROL A1]**
   * **[!UICONTROL A2]**
   * **[!UICONTROL A3]** (alleen beschikbaar voor bepaalde talen)
   * **[!UICONTROL A4]**
1. Selecteer in de sectie **[!UICONTROL Page Orientation]** of u de PDF wilt exporteren in de afdrukstand Liggend of Staand.
1. Selecteer **[!UICONTROL Show Legend]** als u de Legenda wilt opnemen in uw geëxporteerde PDF.
1. Klik op **[!UICONTROL Export]**.

   De PDF van [!UICONTROL Gantt chart] wordt gemaakt en gedownload naar uw computer.

   U ziet de legenda onder aan het geëxporteerde bestand. Hierin worden alleen de opties beschreven die u in uw [!UICONTROL Gantt chart] hebt ingeschakeld en die beschikbaar zijn in uw takenlijst.

   De mijlpalen worden bijvoorbeeld alleen in de legenda weergegeven als u ten minste één taak hebt die aan een mijlpaal is gekoppeld.

   ![ gantt_chart_with_updated__limited__legend.png ](assets/gantt-chart-with-updated--limited--legend-350x271.png)
