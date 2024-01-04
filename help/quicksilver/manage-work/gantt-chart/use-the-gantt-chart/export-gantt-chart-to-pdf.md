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

# Exporteer de [!UICONTROL Gantt Chart] naar PDF

U kunt de opdracht [!UICONTROL Gantt chart] naar een PDF.

Nadat u het dialoogvenster [!UICONTROL Gantt chart] om te PDF, kunt u het drukken of aan een e-mail, vastmaken om het met andere gebruikers te delen.

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
   <td> <p>[!UICONTROL View] of betere toegang tot Projecten en Taken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>[!UICONTROL View] of een betere toegang tot het project</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Exporteer de [!UICONTROL Gantt chart]

1. Toegang krijgen tot de [!UICONTROL Gantt chart] die u naar PDF wilt exporteren, zoals beschreven in [Aan de slag met de [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Zorg ervoor dat u de [!UICONTROL Gantt chart] om de juiste informatie weer te geven voordat u deze exporteert.

   >[!NOTE]
   >
   >Als u het dialoogvenster [!UICONTROL Gantt chart] uit een lijst van projecten, bevat het dossier van de PDF enkel de projecten in de lijst, niet de taken op elk project. Als u een lijst van taken wilt uitvoeren, kunt u dit van het project doen zij met worden geassocieerd, of door een taakrapport te bouwen en de resultaten van het rapport in te tonen [!UICONTROL Gantt View].

   U kunt de volgende informatie vormen:

   * Filters, Weergaven en Groepen naar wens in de takenlijst. Alle filters en groepen die in de lijstweergave zijn geselecteerd, blijven behouden wanneer de [!UICONTROL Gantt chart]. Weergaven worden weerspiegeld in het geëxporteerde [!UICONTROL Gantt chart] alleen in de lijst die wordt weergegeven naast de [!UICONTROL Gantt chart] op de eerste pagina. Weergaven worden niet weergegeven op de [!UICONTROL Gantt chart] zelf.

     >[!TIP]
     >
     >Meer ruimte voor de [!UICONTROL Gantt chart] Pas zelf een weergave toe die zo weinig mogelijk kolommen bevat.

   * Configuratieopties op de knop [!UICONTROL Gantt chart]. U kunt bijvoorbeeld mijlpalen, datums, [!UICONTROL baselines], of [!UICONTROL percent complete] om op [!UICONTROL Gantt chart].

     Zie voor meer informatie   [Configureer hoe informatie wordt weergegeven op het tabblad [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > Toewijzingen worden niet weergegeven op de [!UICONTROL Gantt chart] wanneer de [!UICONTROL Gantt chart] wordt geëxporteerd naar PDF. Wanneer de [!UICONTROL Gantt chart] wordt geëxporteerd naar PDF, worden toewijzingen alleen weergegeven in de lijstweergave.

   * De tijdsperiode die wordt weergegeven op de [!UICONTROL Gantt chart].\

     Zie voor meer informatie [Informatie weergeven in het dialoogvenster [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

     De manier waarop de periode in het exportbestand wordt weergegeven, hangt af van de vraag of u **[!UICONTROL What I see]** of **[!UICONTROL Multiple pages]** in een latere stap.

1. (Optioneel) Als u alleen bepaalde taken in de geëxporteerde PDF wilt opnemen, selecteert u de taken die u wilt opnemen.

   Als u geen taken selecteert, worden alle taken opgenomen in de geëxporteerde PDF.

   Als u bijvoorbeeld het dialoogvenster [!UICONTROL Gantt chart] voor een project dat 50 taken bevat, maar u wilt slechts 10 taken tonen op uitgevoerd [!UICONTROL Gantt chart]Selecteer de tien taken die u wilt weergeven.

1. Klik op het printerpictogram.\
   De **[!UICONTROL Export to PDF]** wordt weergegeven.\
   ![export_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. Selecteer of u alleen wilt exporteren wat u ziet of het gehele [!UICONTROL Gantt chart]:

   * **[!UICONTROL What I see]:** Exporteert alle taken (inclusief eventuele subtaken) die op het scherm worden weergegeven voordat u maximaal 500 items exporteert. (Dit is niet wat wordt weergegeven in het dialoogvenster **[!UICONTROL Preview]** de [!UICONTROL Preview] -sectie bevat alleen voorbeeldgegevens.)

     Subtaken worden opgenomen in de geëxporteerde PDF, zelfs als de bovenliggende taak is samengevouwen en de subtaken niet zichtbaar zijn. Als u alleen bovenliggende taken wilt opnemen, selecteert u de bovenliggende taken die u wilt opnemen en schakelt u de subtaken uit.

     U kunt de **[!UICONTROL Zoom To]** een vervolgkeuzemenu of het gereedschap Schuifregelaar om slechts een gedeelte van het [!UICONTROL Gantt chart], zoals beschreven in [Informatie weergeven in het dialoogvenster [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) .

   * **[!UICONTROL Multiple pages]:** Hiermee exporteert u de gehele [!UICONTROL Gantt chart], zelfs als dit niet zichtbaar is op het huidige scherm, maximaal 500 items.\

     U kunt de **[!UICONTROL Zoom To]** vervolgkeuzemenu of het gereedschap Schuifregelaar om te bepalen hoeveel informatie op elke pagina wordt weergegeven, zoals beschreven in [Configureer hoe informatie wordt weergegeven op het tabblad [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). Selecteer een gedetailleerdere optie als u meer te exporteren pagina&#39;s wilt weergeven of selecteer een minder korrelige optie als u minder te exporteren pagina&#39;s wilt weergeven.

     >[!NOTE]
     >
     >Als u een [!UICONTROL Gantt chart] die meer dan 500 items bevat, past u een filter toe op de lijst voordat u de [!UICONTROL Gantt chart] zodat er minder dan 500 items of 250 pagina&#39;s worden weergegeven. Voor informatie over het toepassen van een filter raadpleegt u  [Overzicht van filters](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >U kunt het volledige Gantt-diagram niet in de volgende omstandigheden exporteren:
     >
     >   
     >   
     >   * Als het meer dan 250 pagina&#39;s beslaat
     >   * Als het meer dan 500 items bevat




1. Als de PDF wordt afgedrukt nadat deze is geëxporteerd naar PDF, kunt u in het dialoogvenster **[!UICONTROL Page Size]** selecteert u de papiergrootte waarnaar u wilt afdrukken.\
   U kunt **[!UICONTROL Letter]**, **[!UICONTROL Legal]**, **[!UICONTROL Ledger]**, **[!UICONTROL A1]**, **[!UICONTROL A2]**, **[!UICONTROL A3]** (alleen beschikbaar voor bepaalde talen), of **[!UICONTROL A4]**.
1. In de **[!UICONTROL Page Orientation]** selecteert u of u de PDF wilt exporteren in liggende of staande richting.
1. Selecteren **[!UICONTROL Show Legend]** als u de Legenda wilt opnemen in uw geëxporteerde PDF.
1. Klik op **[!UICONTROL Export]**.

   De pdf van de [!UICONTROL Gantt chart] wordt gemaakt en naar uw computer gedownload.

   U ziet de legenda onder aan het geëxporteerde bestand. Hierin worden alleen de opties uitgelegd die u in uw [!UICONTROL Gantt chart] en die beschikbaar zijn in uw takenlijst.

   De mijlpalen worden bijvoorbeeld alleen in de legenda weergegeven als u ten minste één taak hebt die aan een mijlpaal is gekoppeld.

   ![gantt_chart_with_updated__limited_legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
