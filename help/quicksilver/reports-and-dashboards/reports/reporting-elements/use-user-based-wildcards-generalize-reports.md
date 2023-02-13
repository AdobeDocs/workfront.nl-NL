---
product-area: reporting
navigation-topic: reporting-elements
title: Gebruik op gebruiker gebaseerde jokertekens om rapporten te generaliseren
description: U kunt een rapport generaliseren door vervangingen in plaats van specifieke informatie te gebruiken wanneer het bouwen van bepaalde rapporteringselementen.
author: Lisa
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# Gebruik op gebruiker gebaseerde jokertekens om rapporten te generaliseren

U kunt een rapport generaliseren door vervangingen in plaats van specifieke informatie te gebruiken wanneer het bouwen van bepaalde rapporteringselementen. Als u bijvoorbeeld een rapport wilt maken waarin de taken worden weergegeven die aan een bepaalde gebruiker zijn toegewezen, kunt u de naam van de gebruiker gebruiken in het veld Toegewezen aan van het filter. Nochtans, als u een rapport wilt tot stand brengen dat taken toont die aan de het programma geopende gebruiker worden toegewezen, ongeacht wie die gebruiker is, kunt u een vervanging gebruiken die erop wijst dat wanneer iemand het rapport bekijkt het informatie toont die slechts op hen betrekking heeft. Op deze manier maakt u het rapport één keer, maar omdat u een jokerteken in het filter gebruikt, geeft het elke keer dat iemand anders het leest andere resultaten.

U kunt op gebruiker-gebaseerde vervangingen gebruiken wanneer het bouwen van de volgende rapporteringselementen:

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

U moet een rapport creëren alvorens u een vervangingsvariabele aan het kunt toevoegen.

Voor instructies over het maken van rapporten raadpleegt u [Een rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Hoe kan ik-stappen

Om een op gebruiker-gebaseerde vervanging in een rapport op te nemen:

1. Ga naar een rapport waarvoor u een op gebruiker-gebaseerde vervanging wilt opnemen.
1. Klikken **Handelingen rapporteren** vervolgens **Bewerken**.

1. Klik op de knop **Filters** tab.
1. Klikken **Filterregel toevoegen**.
1. Typ de naam van het veld waarop u wilt filteren.\
   U moet velden typen die verwijzen naar het gebruikersobject of informatie over gebruikers.
1. Selecteren **Gelijk** in het vervolgkeuzemenu voor de filtervariabele.

   >[!TIP]
   >
   >U moet altijd de **Gelijk** filtervariabele bij het werken met jokertekens in Adobe Workfront.

1. In de **Naam beginnen te typen...** vak, type: `$$USER.ID` of `$$USER.name` als u het rapport informatie over de gebruiker wilt tonen die zich binnen, gebaseerd op hun naam aanmeldt. U kunt andere vervangingen opnemen die naar de het programma geopende Groep van de gebruiker, het Team, het Bedrijf, of andere informatie verwijzen.

   Voor een volledige lijst van op gebruiker-gebaseerde vervangingen, zie [Variabelen van jokerfilter](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/user-based-wildcard-in-project-filter-350x74.png)

1. Klikken **Opslaan + Sluiten**.

## Aanvullende informatie

Zie ook:

* [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program)
* [Variabelen van jokerfilter](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Filters maken of bewerken in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Overzicht van filters in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Een vraag toevoegen aan een rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Voorwaardelijke opmaak gebruiken in weergaven](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
