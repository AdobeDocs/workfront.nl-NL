---
product-area: reporting
navigation-topic: report-usage
title: Rapportgebruik weergeven
description: Rapportgebruik weergeven
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1011'
ht-degree: 0%

---

# Rapportgebruik weergeven

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : *** DO NOT CHANGE, REMOVE, CHANGE LINK, RENAME THIS ARTICLE- IT IS LINKED TO THE PENDO GUIDE FOR THE MAIN REPORTS AREA***)</p>
-->

Als u wilt weten hoe uitgebreid rapporten worden gebruikt in uw systeem, kunt u de volgende informatie weergeven in een lijst met rapporten:

* Laatste 10 gebruikers die het rapport hebben bekeken
* Tellen weergeven binnen een opgegeven tijdsbestek

  >[!NOTE]
  >
  >Adobe Workfront telt per gebruiker per dag één weergave. Als je hetzelfde rapport meerdere keren per dag opent, telt Workfront dit als één weergave voor dat rapport. Als hetzelfde rapport wordt geopend door een andere gebruiker op dezelfde dag, telt Workfront dit als een nieuwe weergave voor de tweede gebruiker.

* Datum van laatste weergave
* Laatst weergegeven door gebruiker
* Een lijst met dashboards die het rapport bevatten\
  Voor meer informatie over het tonen van de naam van de dashboards die de rapporten zouden kunnen worden toegevoegd in een lijst van rapporten, zie het artikel [ begrijpen hoe te om rapporten op een dashboard ](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md) te organiseren.

U kunt een weergave maken voor een lijst met rapporten waarin u deze gegevens kunt weergeven.\
Op sommige van deze velden kunt u een lijst met rapporten filteren.\
Voor meer informatie over welke gebieden u een rapport door kunt filtreren, zie het artikel [ Filter een rapportlijst door gebruiksinformatie ](#filter-a-report-list-by-usage-information).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## De informatie van het rapportgebruik van de vertoning in de Mening van een rapportlijst

1. Klik het **pictogram van het 1} pictogram van het Belangrijkste Menu ![ ](assets/main-menu-icon.png) in de hoger-juiste hoek van Workfront, dan klik** Rapporten **.**

1. Voor de lijst van rapporten, klik het **drop-down menu van de Mening**.
1. (Facultatief) selecteer de **mening van het Gebruik van het 0} Rapport om de gemeenschappelijkste informatie van het rapportgebruik te tonen.**\
   of

1. Klik **Nieuwe Mening** om een douanemening tot stand te brengen.
1. Klik **toevoegen Kolom**.
1. Begin om het even welke volgende gebieden te typen, en hen te selecteren wanneer zij in de lijst onder het **1} voorwerp van het Rapport {verschijnen om hen aan een nieuwe kolom toe te voegen:**

   * **Laatste 10 gebruikers**: Toont de namen van de laatste 10 gebruikers die het rapport bekeken.
   * **Meningen**: Toont het aantal meningen binnen om het even welke volgende tijdkaders:

      * **Deze Maand, Kwartaal, Jaar**
      * **Vorige maand, Kwartaal, Jaar**
      * **Alle Meningen**: Toont een algemene telling voor alle meningen op het rapport

   * **Laatste Bekeken door**: De informatie van vertoningen over de gebruiker die het rapport het laatst bekeken
   * **Laatste Bekeken Datum**: Toont de datum toen het rapport het laatst werd bekeken

1. Klik **sparen Mening**.\
   De gebruiksinformatie over het rapport wordt getoond in de kolommen u aan de mening toevoegde.\
   U kunt een rapport voor het rapportvoorwerp ook bouwen en deze mening in het rapport gebruiken.\
   Voor meer informatie over de bouw van een rapport, zie het artikel [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.\
   U moet Edit toegang tot Rapporten in uw toegangsniveau hebben om een rapport te bouwen.\
   Voor meer informatie over toegang tot rapporten, zie de artikel [ toegang van de Verlening tot rapporten, dashboards, en kalenders ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Een rapportlijst filteren op gebruiksgegevens {#filter-a-report-list-by-usage-information}

1. Klik het **pictogram van het 1} pictogram van het Belangrijkste Menu ![ ](assets/main-menu-icon.png) in de hoger-juiste hoek van Workfront, dan klik** Rapporten **.**
1. Voor de lijst van rapporten, klik het **drop-down menu van de Filter**.
1. Klik **Nieuwe Filter**, dan klik **voegt een Regel van de Filter** toe.
1. Begin om het even welke volgende gebieden te typen, en hen te selecteren wanneer zij in de lijst onder het **1} voorwerp van het Rapport {verschijnen om hen als nieuwe filterregel toe te voegen:**

   * **Meningen**: Toont het aantal meningen binnen om het even welke volgende tijdkaders:

      * **Deze Maand, Kwartaal, Jaar**
      * **Vorige maand, Kwartaal, Jaar**
      * **Alle Meningen**

   * **Laatste Bekeken door**: De informatie van vertoningen over de gebruiker die het rapport het laatst bekeken
   * **Laatste Bekeken Datum**: Toont de datum toen het rapport het laatst werd bekeken

1. Selecteer een bepaling voor uw gebied, dan specificeer een waarde, wanneer ertoe aangezet.\
   ![ de statistieken van de het gebruiksfilter van het Rapport ](assets/qs-report-usage-filter-statistics-350x150.png)

1. Klik **sparen Filter**.\
   Dit toont een lijst van rapporten die de gebruiksinformatie ontmoeten u hebt bepaald.\
   U kunt een rapport voor het rapportvoorwerp ook bouwen en deze filter in het rapport gebruiken.\
   Voor meer informatie over de bouw van een rapport, zie het artikel [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren. U moet Edit toegang tot Rapporten in uw toegangsniveau hebben om een rapport te bouwen.\
   Voor meer informatie over toegang tot rapporten, zie de artikel [ toegang van de Verlening tot rapporten, dashboards, en kalenders ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Uitzonderingen bij het bekijken van gebruiksinformatie van rapporten

>[!IMPORTANT]
>
>De gebruiksinformatie van het rapport is sinds maart 2018 verzameld. Vóór deze datum is geen informatie beschikbaar.

Hieronder volgen enkele uitzonderingen waarmee u rekening moet houden wanneer u werkt met gebruiksgegevens van rapporten:

* Telkens wanneer een rapport op een dashboard of een douanelusje wordt getoond, wordt het geteld als één mening. De gebruiker die dat rapport op zijn dashboard toont wordt getoond als Laatste Mening door: De gebruiker van de Naam, en de datum waarop het dashboard werd getoond wordt getoond als Laatste Bekeken op datum.
* Workfront verzamelt geen gebruiksgegevens voor ingebouwde rapporten.\
  Voor meer informatie over ingebouwde rapporten van Workfront, zie het artikel [ ingebouwde rapporten van Adobe Workfront van het Gebruik ](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

* Workfront verzamelt geen gebruiksgegevens voor geleverde rapporten. Een bezorgd rapport telt niet als één mening.\
  Voor meer informatie over geleverde rapporten, zie het artikel [ de leveringsoverzicht van het Rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

* Wanneer een systeem of groepsbeheerder als een andere gebruiker het programma opent, worden de meningen geteld voor en geassocieerd met het systeem of de groepsbeheerder.
* Workfront verzamelt geen gebruiksinformatie voor rapporten door aangepaste kwartalen. Slechts worden de standaard ingebouwde kwarten van verwijzingen voorzien in de gebieden van het rapportgebruik.
* Workfront verzamelt geen gebruiksinformatie voor rapporten die openbaar worden gedeeld en weergegeven. Wanneer een openbaar rapport door iemand wordt bekeken zonder zich aan te melden bij Workfront, worden de rapportweergaven niet geteld.\
  Voor meer informatie over het delen van rapporten, zie het artikel [ een rapport in Adobe Workfront ](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md) delen.
