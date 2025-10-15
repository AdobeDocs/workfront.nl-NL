---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Rapporten filteren op tijdframes
description: U kunt een rapport filteren op het tijdframe van een datum die op een object bestaat. U kunt bijvoorbeeld een uurrapport filteren voor een bepaald tijdsbestek waarin de uren zijn ingevoerd.
author: Courtney
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 0%

---

# Rapporten filteren op tijdframes

<!-- Audited: 4/2025 -->

U kunt een rapport filteren op het tijdframe van een datum die op een object bestaat. U kunt bijvoorbeeld een uurrapport filteren voor een bepaald tijdsbestek waarin de uren zijn ingevoerd.

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
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
      <p>Standard</p>
      <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Het rapport moet worden gecreeerd alvorens u zijn resultaten kunt filtreren.

Voor meer informatie bij het creëren van rapporten, zie [&#x200B; een rapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md) creëren.

## Een rapport filteren op de tijdlijn van een datum {#filter-a-report-by-the-timeframe-of-a-date}

{{step1-to-reports}}

1. In de upper-left hoek, klik **Nieuw Rapport**, dan selecteer het type van rapport u wilt tot stand brengen.

1. Voor de **Nieuwe pagina van het Rapport**, selecteer de **Filters** tabel.

1. Klik **toevoegen een Regel van de Filter**, dan **Uitgezocht een gebied**.

1. In **selecteer een gebied** dialoogdoos, uitgezochte **Uur**, toen **Datum van de Ingang**.
   ![&#x200B; het Filtreren het rapport van uur door timeframe &#x200B;](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. Selecteer een van de volgende opties in het keuzemenu dat wordt weergegeven:

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
      <td> Na het selecteren van deze bepaling, specificeer een datum waarna de uren waren ingegaan. Het rapport bevat de uren die na de opgegeven datum zijn ingevoerd, inclusief de opgegeven datum. </td> 
     </tr>

   <tr> 
      <td role="rowheader">Tussen</td> 
      <td>Nadat u deze optie hebt geselecteerd, geeft u een datumbereik op wanneer de uren zijn ingevoerd. Het rapport bevat de uren die tussen de opgegeven datums zijn ingevoerd.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Null</td> 
      <td>Selecteer deze optie als u alleen uren wilt weergeven waarop de invoerdatum ontbreekt.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Niet null</td> 
      <td>Selecteer deze optie om alleen uren weer te geven waarop de invoerdatum een waarde heeft.</td> 
     </tr>

   </tbody> 
   </table>

1. Klik **sparen + Sluiten**.

## Ingebouwde tijdframewijzigingstoetsen {#built-in-timeframe-modifiers}

Adobe Workfront beschikt over ingebouwde tijdlijnmodifiers die u kunt gebruiken zonder een specifieke datum te definiëren. Deze bepalingen zijn beschikbaar voor om het even welk datumgebied in een filter of een herinnering in om het even welk rapport.

Als u bijvoorbeeld een uurrapport maakt en de uren wilt weergeven die zijn ingevoerd in een bepaald tijdframe, kunt u uit de volgende ingebouwde filteropties voor het tijdframe kiezen:

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
   <td> <p>Geeft uren weer waarbij de ingangsdatum een datum is in het kwartaal voorafgaand aan het huidige kwartaal, waarbij kwartalen hierboven zijn gedefinieerd.</p> <p>Opmerking: als uw Workfront-beheerder aangepaste kwartalen voor uw systeem heeft ingeschakeld en gedefinieerd, worden de ingebouwde filters voor kwartalen vervangen door uw aangepaste kwartgegevens. Voor meer informatie over het toelaten van douanekwartalen, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref"> douanekwarten </a> toelaten.</p> </td> 
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
   <td> <p>Geeft uren weer waarbij de datum van binnenkomst een datum is in het laatste jaar, waarbij het laatste jaar begint op 1 januari en eindigt op 31 december van het jaar dat voorafgaat aan het lopende jaar.</p> <p>Opmerking: er is geen ingebouwde tijdsperiode voor het belastingjaar. U kunt een rapport creëren en de informatie door datum filtreren gebruikend een douanebepaling voor de datumwaaier van het fiscale jaar, zoals het in uw organisatie wordt bepaald. Als u een tijdpad voor een belastingjaar ter plekke wilt kiezen, gebruikt u een vraag in plaats van een filter. </p> </td> 
  </tr> 
 </tbody> 
</table>
