---
navigation-topic: use-the-gantt-chart
title: De Gantt-grafiek exporteren naar PDF
description: U kunt het Gantt-diagram exporteren naar een PDF.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 0%

---

# [!UICONTROL Gantt Chart] exporteren naar PDF

U kunt de [!UICONTROL Gantt chart] naar een PDF exporteren.

Nadat u de [!UICONTROL Gantt chart] naar PDF hebt geëxporteerd, kunt u deze afdrukken of als bijlage aan een e-mailbericht toevoegen om deze met andere gebruikers te delen.

## Toegangsvereisten

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
   <td> <p>[!UICONTROL Review] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>[!UICONTROL View] of betere toegang tot Projecten en Taken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de [!DNL Workfront] -beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>[!UICONTROL View] of een betere toegang tot het project</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## De [!UICONTROL Gantt chart] exporteren

1. Heb toegang tot [!UICONTROL Gantt chart] dat u naar PDF wilt uitvoeren, zoals die in [ wordt beschreven begonnen met [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Zorg ervoor dat u de [!UICONTROL Gantt chart] zodanig hebt geconfigureerd dat de juiste informatie wordt weergegeven voordat u deze exporteert.

   >[!NOTE]
   >
   >Als u [!UICONTROL Gantt chart] van een lijst van projecten uitvoert, bevat het dossier van de PDF enkel de projecten in de lijst, niet de taken op elk project. Als u een lijst van taken wilt uitvoeren, kunt u dit van het project doen zij met, of door een taakrapport te bouwen en de resultaten van het rapport in [!UICONTROL Gantt View] te tonen worden geassocieerd.

   U kunt de volgende informatie vormen:

   * Filters, Weergaven en Groepen naar wens in de takenlijst. Alle filters en groepen die in de lijstweergave zijn geselecteerd, blijven behouden wanneer de [!UICONTROL Gantt chart] wordt weergegeven. Weergaven worden alleen weerspiegeld in de geëxporteerde [!UICONTROL Gantt chart] pagina in de lijst die naast de [!UICONTROL Gantt chart] op de eerste pagina wordt weergegeven. Weergaven worden niet weergegeven op de [!UICONTROL Gantt chart] zelf.

     >[!TIP]
     >
     >Als u meer ruimte voor de [!UICONTROL Gantt chart] zelf wilt toestaan, past u een weergave toe die zo weinig mogelijk kolommen bevat.

   * Configuratieopties op de [!UICONTROL Gantt chart] . U kunt bijvoorbeeld instellen dat mijlpalen, datums, [!UICONTROL baselines] of [!UICONTROL percent complete] worden weergegeven op de [!UICONTROL Gantt chart] .

     Zie voor meer informatie   [ vormt hoe de informatievertoningen op [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > Toewijzingen worden niet weergegeven op de [!UICONTROL Gantt chart] wanneer de [!UICONTROL Gantt chart] wordt geëxporteerd naar PDF. Wanneer [!UICONTROL Gantt chart] naar PDF wordt geëxporteerd, worden toewijzingen alleen weergegeven in de lijstweergave.

   * De tijdsperiode die wordt weergegeven op de [!UICONTROL Gantt chart]\.

     Voor meer informatie, zie [ het Bekijken van Informatie in [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

     De manier waarop de periode in het exportbestand wordt weergegeven, hangt af van het feit of u **[!UICONTROL What I see]** of **[!UICONTROL Multiple pages]** in een latere stap selecteert.

1. (Optioneel) Als u alleen bepaalde taken in de geëxporteerde PDF wilt opnemen, selecteert u de taken die u wilt opnemen.

   Als u geen taken selecteert, worden alle taken opgenomen in de geëxporteerde PDF.

   Als u bijvoorbeeld [!UICONTROL Gantt chart] weergeeft voor een project dat 50 taken bevat, maar u wilt slechts 10 taken weergeven voor het geëxporteerde project [!UICONTROL Gantt chart] , selecteert u de 10 taken die u wilt weergeven.

1. Klik op het printerpictogram.\
   Het dialoogvenster **[!UICONTROL Export to PDF]** wordt weergegeven.\
   ![ export_gantt_UI.png ](assets/exported-gantt-ui-350x225.png)

1. Selecteer of u alleen wilt exporteren wat u ziet of de volledige [!UICONTROL Gantt chart] :

   * **[!UICONTROL What I see]:** exporteert alle taken (inclusief eventuele subtaken) die op het scherm worden weergegeven voordat maximaal 500 items worden geëxporteerd. (Dit wordt niet weergegeven in de sectie **[!UICONTROL Preview]** . De sectie [!UICONTROL Preview] bevat alleen voorbeeldgegevens.)

     Subtaken worden opgenomen in de geëxporteerde PDF, zelfs als de bovenliggende taak is samengevouwen en de subtaken niet zichtbaar zijn. Als u alleen bovenliggende taken wilt opnemen, selecteert u de bovenliggende taken die u wilt opnemen en schakelt u de subtaken uit.

     Met het vervolgkeuzemenu **[!UICONTROL Zoom To]** of de schuifregelaar kunt u slechts een gedeelte van de [!UICONTROL Gantt chart] -afbeelding weergeven, zoals wordt beschreven in [ Informatie weergeven in [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) .

   * **[!UICONTROL Multiple pages]:** exporteert het gehele bestand [!UICONTROL Gantt chart] , zelfs het item dat niet zichtbaar is op het huidige scherm, tot 500 items.\

     U kunt het **[!UICONTROL Zoom To]** drop-down menu of het schuif hulpmiddel gebruiken om te bepalen hoeveel informatie op elke pagina wordt getoond, zoals die in [ wordt beschreven vormt hoe de informatie over [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md) toont. Selecteer een gedetailleerdere optie als u meer te exporteren pagina&#39;s wilt weergeven of selecteer een minder korrelige optie als u minder te exporteren pagina&#39;s wilt weergeven.

     >[!NOTE]
     >
     >Als u een [!UICONTROL Gantt chart] wilt exporteren die meer dan 500 items bevat, past u een filter op de lijst toe voordat u de [!UICONTROL Gantt chart] weergeeft, zodat er minder dan 500 items of 250 pagina&#39;s worden weergegeven. Voor informatie over hoe te om een filter toe te passen, zie [ Overzicht van Filters ](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >U kunt het volledige Gantt-diagram niet in de volgende omstandigheden exporteren:
     >
     >   
     >   
     >   * Als het meer dan 250 pagina&#39;s beslaat
     >   * Als het meer dan 500 items bevat




1. Als de PDF wordt afgedrukt nadat deze naar PDF is geëxporteerd, selecteert u in de vervolgkeuzelijst **[!UICONTROL Page Size]** het papierformaat waarnaar u wilt afdrukken.\
   U kunt **[!UICONTROL Letter]**, **[!UICONTROL Legal]**, **[!UICONTROL Ledger]**, **[!UICONTROL A1]**, **[!UICONTROL A2]**, **[!UICONTROL A3]** (alleen beschikbaar voor bepaalde talen) of **[!UICONTROL A4]** selecteren.
1. Selecteer in de sectie **[!UICONTROL Page Orientation]** of u de PDF wilt exporteren in de afdrukstand Liggend of Staand.
1. Selecteer **[!UICONTROL Show Legend]** als u de Legenda wilt opnemen in uw geëxporteerde PDF.
1. Klik op **[!UICONTROL Export]**.

   De PDF van [!UICONTROL Gantt chart] wordt gemaakt en gedownload naar uw computer.

   U ziet de legenda onder aan het geëxporteerde bestand. Hierin worden alleen de opties beschreven die u in uw [!UICONTROL Gantt chart] hebt ingeschakeld en die beschikbaar zijn in uw takenlijst.

   De mijlpalen worden bijvoorbeeld alleen in de legenda weergegeven als u ten minste één taak hebt die aan een mijlpaal is gekoppeld.

   ![ gantt_chart_with_updated__limited__legend.png ](assets/gantt-chart-with-updated--limited--legend-350x271.png)
