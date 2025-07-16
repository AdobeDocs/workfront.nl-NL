---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Aangepaste tekens inschakelen
description: Voor rapportagedoeleinden kunt u aangepaste kwartalen maken als de kwartalen van uw organisatie zijn gebaseerd op andere criteria dan kalenderdatums (zoals werkdagen of winkeldagen).
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
source-git-commit: b27b01e1efacc3fc459cec0a53b2c11cbe5e132b
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# Aangepaste kwarten inschakelen

<!--Audited: 11/2024-->

Voor rapportagedoeleinden kunt u aangepaste kwartalen maken als de kwartalen van uw organisatie zijn gebaseerd op andere criteria dan kalenderdatums (zoals werkdagen of winkeldagen).

Afhankelijk van welke producten uw bedrijf heeft gekocht, kunt u het volgende aantal kwartalen in uw gebied van de Opstelling van Workfront vormen:

* Klanten die alleen [!DNL Workfront] hebben aangeschaft, kunnen maximaal acht aangepaste kwartalen configureren voor hun [!DNL Adobe Workfront] -systeem.
* Klanten die [!DNL Workfront] en [!DNL Workfront Planning] hebben aangeschaft, kunnen maximaal 100 kwartalen configureren voor hun [!DNL Workfront] -systeem. Deze zijn ook beschikbaar in [!DNL Planning] .

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <td><p>Nieuw: [!UICONTROL Standard]</p>
   of
   <p>Huidige: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aangepaste kwarten instellen voor uw [!DNL Workfront] -systeem

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Project Preferences]** > **[!UICONTROL Projects].**

1. Selecteer **[!UICONTROL Timelines]** in de sectie **[!UICONTROL Enable Custom Quarters]** .

1. Typ een naam voor het aangepaste kwartaal, bijvoorbeeld &quot;Fiscaal Q1 2021&quot;.
1. Selecteer de begin- en einddatum voor het aangepaste kwartaal.

   ![ Aangepaste kwarten ](assets/custom-quarters-nwe.png)

1. (Optioneel) Klik op **[!UICONTROL Add Custom Quarter]** om extra aangepaste vierkanten aan het systeem toe te voegen.

   >[!IMPORTANT]
   >
   > Als uw bedrijf [!DNL Workfront Planning] heeft aangeschaft, kunt u uw aangepaste kwartalen niet opslaan als er tussenruimten of overlappingen zijn tussen de kwartalen.
   >![ de kwarten van de Douane met overlappende waarschuwing ](assets/custom-quarters-with-overlap-warning.png)
   >Tussenruimten en overlappingen tussen de kwartalen zijn alleen toegestaan voor [!DNL Workfront] -klanten.

1. (Optioneel en voorwaardelijk) Als uw bedrijf alleen [!DNL Workfront] zonder [!DNL Workfront Planning] heeft aangeschaft, maakt u een rapporteringselement dat naar de fiscale kwartalen verwijst.


   **Voorbeeld:** creeer een filter voor een [!UICONTROL project] lijst en omvat de Geplande Datum van de Voltooiing van een project dat van de douanekwartalen van verwijzingen voorziet.

   ![ filter van het Project met douanekwartalen ](assets/example-of-project-filter-with-custom-quarters.png)

   De verwijzingen naar &quot;Dit Kwartaal&quot;, &quot;Volgende Kwartaal&quot; en &quot;Laatste Kwartaal&quot; worden vervangen door nieuwe verwijzingen naar de aangepaste kwartalen.

   Voor informatie over het melden van elementen, zie [ Rapporterende elementen: filters, meningen, en groeperingen ](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Voor informatie over het creëren van filters, zie [ filters in  [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md) creëren of uitgeven.
1. (Optioneel en voorwaardelijk) Ga naar een pagina met recordtypen en open een tijdlijnweergave als u toegang hebt tot [!DNL Workfront Planning] . In de weergave worden de nieuwe aangepaste kwartalen weergegeven.
Voor informatie, zie [ de chronologiemening ](/help/quicksilver/planning/views/manage-the-timeline-view.md) leiden.
