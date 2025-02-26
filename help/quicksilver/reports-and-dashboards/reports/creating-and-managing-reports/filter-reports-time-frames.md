---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Rapporten filteren op tijdframes
description: U kunt een rapport filteren tegen het tijdkader van een datum die op een voorwerp bestaat. Bijvoorbeeld, kunt u een uurrapport voor een bepaald tijdkader van filtreren wanneer de uren waren ingegaan.
author: Nolan
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: e8acdf8f7b3859385237e788dfda34ee62ee11d1
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 0%

---

# Rapporten filteren op tijdframes

<!-- Audited: 11/2024 -->

U kunt een rapport filteren tegen het tijdkader van een datum die op een voorwerp bestaat. Bijvoorbeeld, kunt u een uurrapport voor een bepaald tijdkader van filtreren wanneer de uren waren ingegaan.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p></td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Het rapport moet worden gecreeerd alvorens u zijn resultaten filtreert.

Voor meer informatie bij het creëren van rapporten, zie [ een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md) creëren.

## Een rapport filteren op het tijdframe van een datum {#filter-a-report-by-the-time-frame-of-a-date}

1. Klik het **pictogram van het 1} pictogram van het Belangrijkste Menu ![ ](assets/main-menu-icon.png), dan klik** Meldend **.**

1. Klik **Nieuw Rapport**, dan selecteer het type van rapport u wilt.\
   Bijvoorbeeld, uitgezochte **Rapport van het Uur**.

1. Selecteer de **Filters** tabel.
1. Klik **toevoegen een Regel van de Filter**, dan selecteren **Datum van de Ingang van het Uur**.\
   ![ het Filtreren het rapport van uur door timeframe ](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. Selecteer in het volgende keuzemenu een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Gelijk (hoofdlettergevoelig)</td> 
      <td>Nadat u deze optie hebt geselecteerd, geeft u de datum op waarop de uren zijn ingevoerd.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Niet gelijk (hoofdlettergevoelig)</td> 
      <td>Nadat u deze optie hebt geselecteerd, geeft u de datum op waarop de uren zijn ingevoerd om deze datum uit te sluiten van uw rapport. Het rapport toont uren het programma geopend alle datums, verwacht voor de datum u specificeerde.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Null</td> 
      <td>Selecteer deze optie als u alleen uren wilt weergeven waarop de invoerdatum ontbreekt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Niet null</td> 
      <td>Selecteer deze optie om alleen uren weer te geven waarop de invoerdatum een waarde heeft.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tussen</td> 
      <td>Nadat u deze optie hebt geselecteerd, geeft u een datumbereik op wanneer de uren zijn ingevoerd. Het rapport bevat de uren die tussen de opgegeven datums zijn ingevoerd.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Minder dan</td> 
      <td>Nadat u deze optie hebt geselecteerd, geeft u een datum op vóór welke de uren zijn ingevoerd. Het rapport bevat de uren die vóór de opgegeven datum zijn ingevoerd, exclusief de opgegeven datum.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Minder dan gelijk</td> 
      <td>Nadat u deze optie hebt geselecteerd, geeft u een datum op vóór welke de uren zijn ingevoerd. Het rapport bevat de uren die vóór de opgegeven datum zijn ingevoerd, inclusief de opgegeven datum.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Groter dan</td> 
      <td>Na het selecteren van deze bepaling, specificeer een datum waarna de uren waren ingegaan. Het rapport bevat de uren die na de opgegeven datum zijn ingevoerd, exclusief de opgegeven datum.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Groter dan gelijk</td> 
      <td> <p>Na het selecteren van deze bepaling, specificeer een datum waarna de uren waren ingegaan. Het rapport bevat de uren die na de opgegeven datum zijn ingevoerd, inclusief de opgegeven datum.</p> <p>Selecteer om het even welke ingebouwde bepalingen van het tijdkader, zoals die in <a href="#built-in-time-frame-modifiers" class="MCXref xref"> worden beschreven ingebouwde tijdkaderbepalingen </a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Deze bepalingen zijn beschikbaar voor om het even welk datumgebied in een filter of een herinnering in om het even welk rapport.
1. Klik **sparen + Sluiten**.

## Ingebouwde tijdframewijzigingstoetsen {#built-in-time-frame-modifiers}

Adobe Workfront heeft ingebouwde tijdframemodifiers die u kunt gebruiken zonder een specifieke datum te definiëren.

Deze bepalingen zijn beschikbaar voor om het even welk datumgebied in een filter of een herinnering in om het even welk rapport.

Voor meer informatie over hoe te om een rapport tegen een tijdkader te filtreren verbonden aan een datum, zie de bovengenoemde sectie [ een rapport tegen het tijdkader van een datum ](#filter-a-report-by-the-time-frame-of-a-date) filtreren.

Bijvoorbeeld, als u een uurrapport bouwt en uren ingegaan in een specifiek tijdkader zou willen tonen, kunt u van de volgende ingebouwde opties van de tijdkaderfilter kiezen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Vandaag</td> 
   <td>Hier worden de uren weergegeven waarop de ingangsdatum vandaag staat.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Deze week</td> 
   <td>Hier worden uren weergegeven waarop de ingangsdatum een datum in de huidige week is, waarbij de week op een zondag begint en op een zaterdag eindigt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Volgende week</td> 
   <td>Geeft uren weer waarbij de ingangsdatum een datum is in de week na de huidige week, waarbij de week op zondag begint en op zaterdag eindigt. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Vorige week</td> 
   <td>Geeft uren weer waarbij de ingangsdatum een datum is in de week voorafgaand aan de huidige week, waarbij de week op zondag begint en op zaterdag eindigt. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Deze maand</td> 
   <td>Hier worden uren weergegeven waarop de datum van binnenkomst een datum in de huidige maand is.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Volgende maand</td> 
   <td>Hier worden uren weergegeven waarop de invoerdatum een datum in de maand na de huidige maand is.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Vorige maand</td> 
   <td>Hier worden uren weergegeven waarop de datum van item een datum is in de maand die voorafgaat aan de huidige maand</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dit kwartaal</td> 
   <td> <p>Geeft uren weer waarbij de datum van binnenkomst een datum is in het huidige kwartaal, waarbij kwartalen worden gedefinieerd als:</p> 
    <ul> 
     <li>Eerste kwartaal: 1 januari - 30 maart</li> 
     <li>Tweede kwartaal: 1 april - 30 juni</li> 
     <li>Derde kwartaal: 1 juli - 30 september</li> 
     <li>Vierde kwartaal: 1 oktober - 31 december</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Volgend kwartaal</td> 
   <td>Geeft uren weer waarbij de ingangsdatum een datum is in het kwartaal volgend op het huidige kwartaal, waarbij kwartalen hierboven zijn gedefinieerd.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Laatste kwartier</td> 
   <td> <p>Geeft uren weer waarbij de ingangsdatum een datum is in het kwartaal voorafgaand aan het huidige kwartaal, waarbij kwartalen hierboven zijn gedefinieerd.</p> <p>Opmerking: als uw Workfront-beheerder aangepaste kwartalen voor uw systeem heeft ingeschakeld en gedefinieerd, worden de ingebouwde filters voor kwartalen vervangen door uw aangepaste kwartgegevens. Voor meer informatie over het toelaten van douanekwartalen, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref"> douanekwartalen voor projecten </a> toelaten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dit jaar</td> 
   <td>Geeft uren weer waarbij de ingangsdatum een datum is in het huidige jaar, waarbij het huidige jaar op 1 januari begint en op 31 december eindigt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Afgelopen jaar</td> 
   <td>Hier worden uren weergegeven waarop de datum van binnenkomst een datum in het afgelopen jaar is, waarbij het afgelopen jaar twaalf maanden voor de huidige datum start.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Vorig jaar</td> 
   <td> <p>Geeft uren weer waarbij de datum van binnenkomst een datum is in het laatste jaar, waarbij het laatste jaar begint op 1 januari en eindigt op 31 december van het jaar dat voorafgaat aan het lopende jaar.</p> <p>Opmerking: er is geen ingebouwde tijdsperiode voor het belastingjaar. U kunt een rapport creëren en de informatie door datum filtreren gebruikend een douanebepaling voor de datumwaaier van het fiscale jaar, zoals het in uw organisatie wordt bepaald. Als u een tijdkader voor een belastingjaar op de plaats wilt kiezen, dan zou u een herinnering in plaats van een filter moeten gebruiken. </p> </td> 
  </tr> 
 </tbody> 
</table>
