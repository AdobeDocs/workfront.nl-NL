---
product-area: reporting
navigation-topic: report-usage
title: Rapportgebruik weergeven
description: Rapportgebruik weergeven
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '997'
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
   Zie het artikel voor meer informatie over het weergeven van de naam van de dashboards waarop rapporten kunnen worden toegevoegd in een lijst met rapporten [Begrijp hoe te om rapporten op een dashboard te organiseren](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md).

U kunt een weergave maken voor een lijst met rapporten waarin u deze gegevens kunt weergeven.\
Op sommige van deze velden kunt u een lijst met rapporten filteren.\
Zie het artikel voor meer informatie over de velden waarop u een rapport kunt filteren [Een rapportlijst filteren op gebruiksgegevens](#filter-a-report-list-by-usage-information).

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
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## De informatie van het rapportgebruik van de vertoning in de Mening van een rapportlijst

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Rapporten**.

1. Klik in de lijst met rapporten op de knop **Weergave** vervolgkeuzemenu.
1. (Optioneel) Selecteer de optie **Rapportgebruik** mening om de gemeenschappelijkste informatie van het rapportgebruik te tonen.\
   of

1. Klikken **Nieuwe weergave** om een aangepaste weergave te maken.
1. Klikken **Kolom toevoegen**.
1. Typ een van de volgende velden en selecteer deze als ze in de lijst onder de **Rapport** object om deze aan een nieuwe kolom toe te voegen:

   * **Laatste 10 gebruikers**: Toont de namen van de laatste 10 gebruikers die het rapport bekeken.
   * **Weergaven**: Hiermee geeft u het aantal weergaven weer binnen een van de volgende tijdframes:

      * **Deze maand, kwartaal, jaar**
      * **Vorige maand, kwartaal, jaar**
      * **Alle weergaven**: Toont een algemene telling voor alle meningen op het rapport
   * **Laatst weergegeven door**: De informatie van vertoningen over de gebruiker die het rapport het laatst bekeken
   * **Datum van laatste weergave**: Toont de datum toen het rapport het laatst werd bekeken


1. Klikken **Weergave opslaan**.\
   De gebruiksinformatie over het rapport wordt getoond in de kolommen u aan de mening toevoegde.\
   U kunt een rapport voor het rapportvoorwerp ook bouwen en deze mening in het rapport gebruiken.\
   Raadpleeg het artikel voor meer informatie over het samenstellen van een rapport [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
   U moet Edit toegang tot Rapporten in uw toegangsniveau hebben om een rapport te bouwen.\
   Raadpleeg het artikel voor meer informatie over toegang tot rapporten [Toegang verlenen tot rapporten, dashboards en kalenders](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Een rapportlijst filteren op gebruiksgegevens {#filter-a-report-list-by-usage-information}

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Rapporten**.
1. Klik in de lijst met rapporten op de knop **Filter** vervolgkeuzemenu.
1. Klikken **Nieuw filter** en klik vervolgens op **Filterregel toevoegen**.
1. Typ een van de volgende velden en selecteer deze als ze in de lijst onder de **Rapport** -object om deze als een nieuwe filterregel toe te voegen:

   * **Weergaven**: Hiermee geeft u het aantal weergaven weer binnen een van de volgende tijdframes:

      * **Deze maand, kwartaal, jaar**
      * **Vorige maand, kwartaal, jaar**
      * **Alle weergaven**
   * **Laatst weergegeven door**: De informatie van vertoningen over de gebruiker die het rapport het laatst bekeken
   * **Datum van laatste weergave**: Toont de datum toen het rapport het laatst werd bekeken


1. Selecteer een bepaling voor uw gebied, dan specificeer een waarde, wanneer ertoe aangezet.\
   ![](assets/qs-report-usage-filter-statistics-350x150.png)

1. Klikken **Filter opslaan**.\
   Dit toont een lijst van rapporten die de gebruiksinformatie ontmoeten u hebt bepaald.\
   U kunt een rapport voor het rapportvoorwerp ook bouwen en deze filter in het rapport gebruiken.\
   Raadpleeg het artikel voor meer informatie over het samenstellen van een rapport [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). U moet Edit toegang tot Rapporten in uw toegangsniveau hebben om een rapport te bouwen.\
   Raadpleeg het artikel voor meer informatie over toegang tot rapporten [Toegang verlenen tot rapporten, dashboards en kalenders](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Uitzonderingen bij het bekijken van gebruiksinformatie van rapporten

>[!IMPORTANT]
>
>De gebruiksinformatie van het rapport is sinds maart 2018 verzameld. Vóór deze datum is geen informatie beschikbaar.

Hieronder volgen enkele uitzonderingen waarmee u rekening moet houden wanneer u werkt met gebruiksgegevens van rapporten:

* Telkens wanneer een rapport op een dashboard of een douanelusje wordt getoond, wordt het geteld als één mening. De gebruiker die dat rapport op zijn dashboard toont wordt getoond als Laatste Mening door: De gebruiker van de naam, en de datum waarop het dashboard werd getoond wordt getoond als Laatste Bekeken op datum.
* Workfront verzamelt geen gebruiksgegevens voor ingebouwde rapporten.\
   Raadpleeg het artikel voor meer informatie over ingebouwde Workfront-rapporten [Ingebouwde Adobe Workfront-rapporten gebruiken](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

* Workfront verzamelt geen gebruiksgegevens voor geleverde rapporten. Een bezorgd rapport telt niet als één mening.\
   Raadpleeg het artikel voor meer informatie over geleverde rapporten [Overzicht van levering rapporteren](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

* Wanneer een systeem of groepsbeheerder als een andere gebruiker het programma opent, worden de meningen geteld voor en geassocieerd met het systeem of de groepsbeheerder.
* Workfront verzamelt geen gebruiksinformatie voor rapporten door aangepaste kwartalen. Slechts worden de standaard ingebouwde kwarten van verwijzingen voorzien in de gebieden van het rapportgebruik.
* Workfront verzamelt geen gebruiksinformatie voor rapporten die openbaar worden gedeeld en weergegeven. Wanneer een openbaar rapport door iemand wordt bekeken zonder zich aan te melden bij Workfront, worden de rapportweergaven niet geteld.\
   Zie het artikel voor meer informatie over het delen van rapporten [Een rapport delen in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
