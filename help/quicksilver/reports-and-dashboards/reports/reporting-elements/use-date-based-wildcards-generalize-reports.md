---
product-area: reporting
navigation-topic: reporting-elements
title: Gebruik op datum gebaseerde jokertekens om rapporten te generaliseren
description: U kunt een rapport generaliseren door vervangingen in plaats van specifieke informatie te gebruiken wanneer het bouwen van bepaalde rapporteringselementen.
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# Gebruik op datum gebaseerde jokertekens om rapporten te generaliseren

U kunt een rapport generaliseren door vervangingen in plaats van specifieke informatie te gebruiken wanneer het bouwen van bepaalde rapporteringselementen.

Als u bijvoorbeeld een rapport wilt maken waarin de taken worden weergegeven met een specifieke geplande begindatum, kunt u de datumkiezer voor de kalenderdatum in een filter gebruiken om een specifieke datum te selecteren. Nochtans, als u een rapport wilt tot stand brengen dat taken toont die de Geplande Datum van het Begin binnen een bepaald tijdsbestek van de datum hebben wanneer het rapport wordt betreden, kunt u een vervanging gebruiken die erop wijst dat wanneer iemand het rapport bekijkt het informatie voor een timeframe relevant voor het ogenblik toont wanneer zij het rapport bekijken.

Bijvoorbeeld in de afgelopen week, in het afgelopen jaar, in de komende twee weken, enz. Op deze manier maakt u het rapport één keer, maar omdat u een jokerteken in het filter gebruikt, geeft het elke keer dat iemand het leest andere resultaten omdat het zich aanpast aan de dag waarop het rapport wordt uitgevoerd.

U kunt op datum gebaseerde vervangingen gebruiken wanneer het bouwen van de volgende rapporteringselementen:

* Filters
* Aangepaste vragen
* Weergaven bij het toevoegen van regels voor kolommen

## Toegangsvereisten

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken om rapportelementen in een rapport te bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>De toestemmingen van het beheer aan een rapport om rapporteringselementen in een rapport uit te geven</p> <p>Machtigingen beheren voor een weergave of filter om deze te bewerken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

U moet een rapport maken voordat u jokertekenvariabelen eraan kunt toevoegen.

Voor informatie over het maken van een rapport raadpleegt u [Een rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Hoe kan ik-stappen

Om op datum-gebaseerde vervanging in een rapport op te nemen:

1. Ga naar een rapport waarvoor u op datum-gebaseerde vervanging wilt opnemen.
1. Klikken **Handelingen rapporteren** vervolgens **Bewerken**.

1. Klik op de knop **Filters** tab.
1. Klikken **Filterregel toevoegen**.
1. Typ de naam van het veld waarop u wilt filteren.\
   U moet velden typen die naar een datum verwijzen.
1. Selecteren **Gelijk** in het vervolgkeuzemenu voor de filtervariabele.

   >[!TIP]
   >
   >U moet altijd de **Gelijk** filtervariabele bij het werken met jokertekens in Adobe Workfront.

1. In de **Naam beginnen te typen...** vak, type: `$$TODAY` als u informatie over iets wilt tonen dat de zelfde dag voorkomt dat het rapport in werking wordt gesteld.

   of

   Type `$$NOW` als u informatie over iets wilt tonen dat op de zelfde datum en tijd voorkomt dat het rapport in werking wordt gesteld.

   Deze datum is altijd verschillend, aangezien het met de datum verandert het rapport eigenlijk door een gebruiker wordt bekeken. de informatie in het verslag verschilt dus van dag tot dag .

1. (Optioneel) Als u informatie wilt weergeven die optreedt binnen een tijdsbestek na de datum waarop het rapport wordt uitgevoerd, typt u `$$TODAY+1w` om informatie in de volgende week weer te geven, of `$$TODAY+2m` om informatie in de komende twee maanden weer te geven. U kunt ook tijdframes voor kwartalen, uren, dagen of jaren aangeven.
1. (Optioneel) Als u informatie wilt weergeven over iets dat zich heeft voorgedaan binnen een tijdsbestek vóór de datum waarop het rapport wordt uitgevoerd, typt u `$$TODAY-1w` om informatie van de vorige week weer te geven, of `$$TODAY-2m` om informatie van de voorafgaande twee maanden weer te geven. U kunt ook tijdframes voor kwartalen, uren, dagen of jaren aangeven.

   Raadpleeg het artikel voor een volledige lijst met kenmerken, kwalificaties en operatoren die u kunt gebruiken in op datums gebaseerde jokertekens [Variabelen van jokerfilter](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/video-date-based-wildcard-in-task-filter-350x81.png)

1. Klikken **Opslaan + Sluiten**.

## Aanvullende informatie

Zie ook:

* [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program)
* [Variabelen van jokerfilter](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Filters maken of bewerken in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Een vraag toevoegen aan een rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Voorwaardelijke opmaak gebruiken in weergaven](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
