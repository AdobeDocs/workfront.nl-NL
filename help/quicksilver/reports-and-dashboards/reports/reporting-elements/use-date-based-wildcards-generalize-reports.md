---
product-area: reporting
navigation-topic: reporting-elements
title: Gebruik op datum gebaseerde jokertekens om rapporten te generaliseren
description: U kunt een rapport generaliseren door vervangingen in plaats van specifieke informatie te gebruiken wanneer het bouwen van bepaalde rapporteringselementen.
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# Gebruik op datum gebaseerde jokertekens om rapporten te generaliseren

<!-- Audited: 11/2024 -->

U kunt een rapport generaliseren door vervangingen in plaats van specifieke informatie te gebruiken wanneer het bouwen van bepaalde rapporteringselementen.

Als u bijvoorbeeld een rapport wilt maken waarin de taken worden weergegeven met een specifieke geplande begindatum, kunt u de datumkiezer voor de kalenderdatum in een filter gebruiken om een specifieke datum te selecteren. Nochtans, als u een rapport wilt tot stand brengen dat taken toont die de Geplande Datum van het Begin binnen een bepaald tijdsbestek van de datum hebben wanneer het rapport wordt betreden, kunt u een vervanging gebruiken die erop wijst dat wanneer iemand het rapport bekijkt het informatie voor een timeframe relevant voor het ogenblik toont wanneer zij het rapport bekijken.

Bijvoorbeeld in de afgelopen week, in het afgelopen jaar, in de komende twee weken, enz. Op deze manier maakt u het rapport één keer, maar omdat u een jokerteken in het filter gebruikt, geeft het elke keer dat iemand het leest andere resultaten omdat het zich aanpast aan de dag waarop het rapport wordt uitgevoerd.

U kunt op datum-gebaseerde vervangingen gebruiken wanneer het bouwen van de volgende rapporteringselementen:

* Filters
* Aangepaste vragen
* Weergaven bij het toevoegen van regels voor kolommen

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-abonnement*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie*</strong></td> 
   <td> 
      <p>Nieuw:</p>
         <ul>
         <li><p>Standaard</p></li>
         </ul>
      <p>Huidige:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken om rapportelementen in een rapport te bewerken</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Rechten beheren aan een rapport om rapportelementen in een rapport te bewerken</p> <p>Machtigingen beheren voor een weergave of filter om deze te bewerken</p></td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

U moet een rapport maken voordat u jokertekenvariabelen eraan kunt toevoegen.

Voor informatie bij het creëren van een rapport, zie [ een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md) creëren.

## Procedure

Om op datum-gebaseerde vervanging in een rapport op te nemen:

1. Ga naar een rapport waarvoor u op datum-gebaseerde vervanging wilt opnemen.
1. Klik **de Acties van het Rapport**, dan **uitgeven**.
1. Klik de **Filters** tabel.
1. Klik **toevoegen een Regel van de Filter**.
1. Typ de naam van het veld waarop u wilt filteren.\
   U moet velden typen die naar een datum verwijzen.
1. Selecteer **Gelijk** in het drop-down menu voor de filtervariabele.

   >[!TIP]
   >
   >U moet altijd de **Gelijke** filtervariabele selecteren wanneer het werken met vervangingen in Adobe Workfront.

1. Klik de **Vastgestelde relatieve datum** knevel, dan in het tekstvakje dat type lijkt: `$$TODAY` als u informatie over iets wilt tonen dat de zelfde dag voorkomt dat het rapport in werking wordt gesteld.

   of

   Typ `$$NOW` als u informatie wilt weergeven over iets dat optreedt op dezelfde datum en tijd als het rapport wordt uitgevoerd.

   Deze datum is altijd verschillend, aangezien het met de datum verandert het rapport eigenlijk door een gebruiker wordt bekeken. de informatie in het verslag verschilt dus van dag tot dag .

1. (Optioneel) Als u informatie wilt weergeven die binnen een tijdsbestek na de datum plaatsvindt waarop het rapport wordt uitgevoerd, typt u `$$TODAY+1w` om informatie weer te geven in de volgende week of `$$TODAY+2m` om informatie weer te geven in de volgende twee maanden. U kunt ook tijdframes voor kwartalen, uren, dagen of jaren aangeven.
1. (Optioneel) Als u informatie wilt weergeven over iets dat is opgetreden binnen een tijdsbestek vóór de datum waarop het rapport wordt uitgevoerd, typt u `$$TODAY-1w` om informatie van de vorige week weer te geven of `$$TODAY-2m` om informatie van de vorige twee maanden weer te geven. U kunt ook tijdframes voor kwartalen, uren, dagen of jaren aangeven.

   Voor een volledige lijst van attributen, kwaliteiten, en exploitanten die u in op datum-gebaseerde vervangingen kunt gebruiken, zie het artikel [ overzicht van de de filtervariabelen van de vervanging ](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Klik **sparen + Sluiten**.

## Aanvullende informatie

Zie ook:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [ overzicht van de de filtervariabelen van de Verjaring ](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [ creeer of geef filters in Adobe Workfront uit ](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [ voeg een herinnering aan een rapport toe ](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Voorwaardelijke opmaak gebruiken in weergaven](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
