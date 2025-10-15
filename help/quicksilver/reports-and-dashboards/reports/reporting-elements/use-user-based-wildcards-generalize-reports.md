---
product-area: reporting
navigation-topic: reporting-elements
title: Gebruik op gebruiker gebaseerde jokertekens om rapporten te generaliseren
description: U kunt een rapport generaliseren door vervangingen in plaats van specifieke informatie te gebruiken wanneer het bouwen van bepaalde rapporteringselementen.
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Gebruik op gebruiker gebaseerde jokertekens om rapporten te generaliseren

<!-- Audited: 11/2024 -->

U kunt een rapport generaliseren door vervangingen in plaats van specifieke informatie te gebruiken wanneer het bouwen van bepaalde rapporteringselementen. Als u bijvoorbeeld een rapport wilt maken waarin de taken worden weergegeven die aan een bepaalde gebruiker zijn toegewezen, kunt u de naam van de gebruiker gebruiken in het veld Toegewezen aan van het filter. Nochtans, als u een rapport wilt tot stand brengen dat taken toont die aan de het programma geopende gebruiker worden toegewezen, ongeacht wie die gebruiker is, kunt u een vervanging gebruiken die erop wijst dat wanneer iemand het rapport bekijkt het informatie toont die slechts op hen betrekking heeft. Op deze manier maakt u het rapport één keer, maar omdat u een jokerteken in het filter gebruikt, geeft het elke keer dat iemand anders het leest andere resultaten.

U kunt op gebruiker-gebaseerde vervangingen gebruiken wanneer het bouwen van de volgende rapporteringselementen:

* Filters
* Aangepaste vragen
* Weergaven bij het toevoegen van regels voor kolommen

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</strong></td> 
   <td> 
    <p>Standard</p>
    <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken om rapportelementen in een rapport te bewerken</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
    <td> <p>Rechten beheren aan een rapport om rapportelementen in een rapport te bewerken</p> <p>Machtigingen beheren voor een weergave of filter om deze te bewerken</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

U moet een rapport creëren alvorens u een vervangingsvariabele aan het kunt toevoegen.

Voor instructies bij het creëren van rapporten, zie [ een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md) creëren.

## Procedure

Om een op gebruiker-gebaseerde vervanging in een rapport op te nemen:

1. Ga naar een rapport waarvoor u een op gebruiker-gebaseerde vervanging wilt opnemen.
1. Klik **de Acties van het Rapport**, dan **uitgeven**.

1. Klik de **Filters** tabel.
1. Klik **toevoegen een Regel van de Filter**.
1. Typ de naam van het veld waarop u wilt filteren.\
   U moet velden typen die verwijzen naar het gebruikersobject of informatie over gebruikers.
1. Selecteer **Gelijk** in het drop-down menu voor de filtervariabele.

   >[!TIP]
   >
   >U moet altijd de **Gelijke** filtervariabele selecteren wanneer het werken met vervangingen in Adobe Workfront.

1. In het **Begin typend naam...** doos, type: `$$USER.ID` of `$$USER.name` als u het rapport informatie over de gebruiker wilt tonen die binnen, gebaseerd op hun naam het programma opent. U kunt andere vervangingen opnemen die naar de het programma geopende Groep van de gebruiker, het Team, het Bedrijf, of andere informatie verwijzen.

   Voor een volledige lijst van op gebruiker-gebaseerde vervangingen, zie [ overzicht van de de filtervariabelen van de Vervanging ](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Klik **sparen + Sluiten**.

## Aanvullende informatie

Zie ook:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [ overzicht van de de filtervariabelen van de Verjaring ](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [ creeer of geef filters in Adobe Workfront uit ](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [ Overzicht van Filters ](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [ voeg een herinnering aan een rapport toe ](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Voorwaardelijke opmaak gebruiken in weergaven](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
