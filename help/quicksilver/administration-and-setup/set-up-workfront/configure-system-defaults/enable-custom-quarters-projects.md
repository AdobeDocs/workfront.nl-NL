---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Aangepaste kwartalen inschakelen voor projecten
description: Voor rapportagedoeleinden kunt u aangepaste kwartalen maken als de kwartalen van uw organisatie zijn gebaseerd op andere criteria dan kalenderdatums (zoals werkdagen of winkeldagen).
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Aangepaste kwartalen inschakelen voor projecten

Voor rapportagedoeleinden kunt u aangepaste kwartalen maken als de kwartalen van uw organisatie zijn gebaseerd op andere criteria dan kalenderdatums (zoals werkdagen of winkeldagen).

U kunt maximaal acht aangepaste kwartalen configureren voor uw [!DNL Adobe Workfront] systeem.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Stel aangepaste kwartalen in voor uw [!DNL Workfront] systeem

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik op **[!UICONTROL Project Preferences]** > **[!UICONTROL Projects].**

1. In de **[!UICONTROL Timelines]** sectie, selecteert u **[!UICONTROL Enable Custom Quarters]**.

1. Typ een naam voor het aangepaste kwartaal, bijvoorbeeld &quot;Fiscaal Q1 2021&quot;.
1. Selecteer de begin- en einddatum voor het aangepaste kwartaal.

   ![](assets/custom-quarters-nwe.png)

1. (Optioneel) Klik op **[!UICONTROL Add Custom Quarter]** om extra douanekwarten aan het systeem toe te voegen.
1. (Optioneel) Maak een rapporteringselement dat betrekking heeft op de belastingkwartalen.

   **Voorbeeld:** Een filter maken voor een [!UICONTROL project] de geplande afsluitende datum van een project dat naar de aangepaste kwartalen verwijst, vermelden en vermelden.

   ![](assets/example-of-project-filter-with-custom-quarters.png)

   De verwijzingen naar &quot;Dit Kwartaal&quot;, &quot;Volgende Kwartaal&quot; en &quot;Laatste Kwartaal&quot; worden vervangen door nieuwe verwijzingen naar de aangepaste kwartalen.

   Zie voor informatie over rapportageelementen [Elementen rapporteren: filters, weergaven en groepen](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Voor informatie over het maken van filters raadpleegt u [Filters maken of bewerken in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
