---
product-area: reporting
navigation-topic: reporting-elements
title: Een filter, weergave of groep delen
description: U kunt filters, weergaven en groeperingen delen die u kunt bekijken met andere gebruikers.
author: Nolan
feature: Reports and Dashboards
exl-id: 63a6db90-d52c-4147-a442-7904ef9e9d49
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '1178'
ht-degree: 0%

---

# Een filter, weergave of groep delen

<!-- Audited: 11/2024 -->

<!--(NOTE: CONSIDER SPLITTING THIS in three articles for each reporting element?)
(NOTE: This is linked from the TOC article in WF Basics > permissions section)-->

Uw Adobe Workfront-beheerder verleent gebruikers toegang tot weergave- of bewerkingsobjecten wanneer zij toegangsniveaus toewijzen. Voor meer informatie over het verlenen van toegang tot voorwerpen, zie [&#x200B; tot douanetoegangsniveaus &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.

Samen met het toegangsniveau dat de gebruikers worden verleend, kunt u hen toestemmingen ook verlenen om specifieke voorwerpen te bekijken of uit te geven die u creeerde of toegang om hebt te delen. Voor meer informatie over toegangsniveaus en toestemmingen, zie [&#x200B; hoe de toegangsniveaus en de toestemmingen samen &#x200B;](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) werken.

U kunt filters, weergaven en groeperingen delen die u kunt bekijken met andere gebruikers.

Wanneer een filter, weergave of groep met u wordt gedeeld, kunt u dat filter, die weergave of die groep toepassen op uw lijsten. Afhankelijk van de toegang die aan u wordt verleend, zou u het kunnen kunnen wijzigen en het met andere gebruikers delen.

Zie de volgende artikelen voor informatie over het maken van een filter, weergave of groepering:

* [&#x200B; Overzicht van Filters &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [&#x200B; Overzicht van meningen in Adobe Workfront &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Overzicht van groepen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-abonnement*</strong></td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie*</strong></td> 
   <td> 
      <p>Nieuw:</p>
         <ul>
         <li><p>Medewerker of hoger</p></li>
         </ul>
      <p>Huidige:</p>
         <ul>
         <li><p>Aanvraag of hoger</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>Toegang tot filters, weergaven, groepen weergeven of vergroten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td><p>Machtigingen weergeven of hoger met toegang voor delen naar een weergave, filter of groep</p></td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een filter, weergave of groep delen

<!--(NOTE: when the beta filters/ groupings come out either consider splitting this in different kinds of FVGs or splitting this article in FVGs for showing sharing on each one of them??)-->

Het delen van filters in geselecteerde lijsten is anders, afhankelijk van de interface die u gebruikt om het filter te delen: standaard of verouderd. Voor informatie over de types van filter-bouwt interfaces, zie [&#x200B; filters in Adobe Workfront &#x200B;](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md) creëren of uitgeven.

U kunt weergaven en groepen alleen delen in de oudere interface.

### Filters delen met de standaardbuilderinterface

U kunt een filter in de standaardinterface van lijsten van projecten, taken, kwesties, portefeuilles, programma&#39;s, gebruikers, malplaatjes, of groepen delen. De standaard builderinterface voor filters is niet beschikbaar voor andere objecten of voor weergaven of groepen.

Een filter delen met de standaardbuilderinterface:

1. Ga naar een lijst met projecten, taken of problemen.
1. Klik het **pictogram van de Filter** pictogram ![&#x200B; van de Filter &#x200B;](assets/filter-nwepng.png).

   ![&#x200B; Standaard filterbouwer &#x200B;](assets/new-filters-all-filter-types.png)

1. Bekijk de volgende lijsten met filters:

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>Favoriet</strong></td>
   <td>Filters die u als favorieten hebt gemarkeerd. Wanneer u een filter favoriete, wordt de originele plaats getoond onder de filternaam, en het wordt verborgen van de originele lijst tenzij u het als favoriet verwijdert.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Opgeslagen</strong></td>
   <td>Filters die u zelf hebt gemaakt en opgeslagen. In deze lijst worden standaard opgeslagen filters weergegeven in de volgorde van de laatst opgeslagen filters, maar u kunt de filternamen slepen om de lijst handmatig opnieuw te rangschikken.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Standaardwaarden systeem</strong></td>
   <td>De standaardfilters van het systeem van Workfront, evenals filters die de beheerder van Workfront aan uw lijst van filters, of op het systeemniveau of in uw lay-outmalplaatje toevoegde.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Gedeeld met mij</strong></td>
   <td>Filters die anderen met u hebben gemaakt en gedeeld of die op het hele systeem worden gedeeld.</td>
   </tr>
   </tbody>
   </table>

1. Beweeg over een filter u toegang tot minstens mening en aandeel hebt, dan klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-icon-spectrum.png), dan klik **Aandeel**.

   ![&#x200B; Meer menuopties &#x200B;](assets/new-filters-more-menu-options-with-delete.png)

   Het dialoogvenster Filter delen wordt weergegeven.

1. Begin de namen van gebruikers, teams, rollen, groepen, of bedrijven te typen die u met in **wilt delen geef toegang tot** gebied.

   ![&#x200B; het delen van de Filter doos &#x200B;](assets/new-filters-share-filter.png)

1. (Facultatief) klik de juist-richt pijl naast de naam van een entiteit om hun toestemmingen aan de filter uit te geven, dan of toelaten de **Mening** of **leiden** optie. **Mening** is het gebrek.

   ![&#x200B; het Delen toestemmingen &#x200B;](assets/new-filters-sharing-permissions.png)

1. (Optioneel) Schakel de aanvullende machtigingen voor een entiteit in of uit door een van de volgende handelingen uit te voeren:

   1. Klik **Mening** en maak de **optie van het Aandeel** onbruikbaar. Deze optie is standaard ingeschakeld.
   1. Klik **leiden** en maak of het **Aandeel** of de **Schrapping** optie onbruikbaar. Deze zijn standaard ingeschakeld.

      >[!NOTE]
      >
      >Als u de optie Beheren inschakelt met de optie Verwijderen, kunnen deze gebruikers het filter van alle gebruikers verwijderen, ook al hebben zij geen eigenaar van het filter.

   >[!TIP]
   >
   >Gebruikers kunnen geen hogere machtigingen ontvangen dan hun toegangsniveau. Als zij geen toegang tot Edit filters in hun toegangsniveau hebben, kunnen zij geen toestemmingen ontvangen om een filter te beheren. Workfront schakelt de optie Beheren voor deze gebruikers uit en de optie is grijs.

1. Klik **Aandeel**. Het filter wordt gedeeld met de entiteiten u specificeerde.

   >[!TIP]
   >
   >Delen met groepen geeft machtigingen aan het filter voor de leden van de groep en voor alle subgroepen.

   De filters u vertoning in **deelde met me** sectie van het filterpaneel voor die entiteiten.

   ![&#x200B; Filters die met me worden gedeeld &#x200B;](assets/new-filters-shared-with-me.png)

### De filters, de meningen, en de groeperingen van het aandeel gebruikend de erfenisinterface

Het delen van filters, weergaven en groepen in de oudere interface is identiek.

1. Ga naar een lijst met objecten of een rapport.
1. (Voorwaardelijk) van een lijst, klik de **Filter**, **Mening**, of **Groeperend** pictogram, dan over de filter, de mening, of het groeperen u wilt delen, klik het **Meer** pictogram ![&#x200B; Meer pictogram &#x200B;](assets/more-icon.png), dan **Aandeel**.

   Van een rapport, klik de **Filter**, **Mening**, of **het Groeperen** drop-down menu, dan selecteren de filter, de mening, of het groeperen u wilt delen.

1. (Voorwaardelijk) als het delen van een rapport, klik de **Filter**, **Mening**, of **het drop-down menu van de Groepering** opnieuw, dan klik de Filter van het Aandeel **,** Mening van het Aandeel **, of** Groepering van het Aandeel **.**\
   De **Toegang van de Filter**, **Toegang van de Mening**, of **de vertoningen van de de dialoogdoos van de Toegang van de Groepering**.

   ![&#x200B; filter van het Aandeel &#x200B;](assets/share-filter-people-box-nwe-350x458.png)

1. Voer een van de volgende twee handelingen uit, afhankelijk van wie u wilt delen:

   **om met individuele gebruikers, teams, rollen, groepen, of bedrijven te delen:** op het verstrekte gebied, begin typend de naam van de gebruiker, het team, de rol, de groep, of het bedrijf u met wilt delen, dan klik de naam wanneer het in de drop-down lijst verschijnt.\
   Herhaal dit proces om toegang met veelvoudige gebruikers, teams, rollen, groepen, of bedrijven te delen.

   >[!TIP]
   >
   >Delen met groepen geeft machtigingen voor het filter, de weergave of de groep aan de leden van de groep en van alle subgroepen.

   **om met alle gebruikers in het systeem te delen:** klik het **pictogram van Montages**, dan klik **maken dit zichtbare systeem-breed**.\
   Uw beheerder moet de optie voor het delen van het hele systeem selecteren om deze optie beschikbaar te maken. Voor meer informatie, zie de artikelen [&#x200B; tot douanetoegangsniveaus &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen en [&#x200B; rapporten, dashboards, en kalenders van het Aandeel &#x200B;](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Voorwaardelijk) als u met individuele gebruikers, teams, rollen, groepen, of bedrijven deelt, klik het drop-down menu om het niveau van toegang te bepalen u wilt verlenen.

   U kunt uit de volgende opties selecteren:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Weergeven</strong></td> 
      <td> <p>Selecteer deze optie als de ontvangers voor delen alleen het gedeelde filter, de gedeelde weergave of de gedeelde groepering mogen gebruiken. Als deze optie is geselecteerd, kunnen ontvangers geen wijzigingen aanbrengen in het gedeelde item.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beheren</strong></td> 
      <td> <p>Selecteer deze optie als de ontvangers voor delen het gedeelde filter, de weergave of de groep mogen gebruiken en wijzigen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Delen</strong></td> 
      <td> <p>Klik <strong> Geavanceerde Montages </strong>, dan selecteren of ontruimen de <strong> optie van het Aandeel </strong>, afhankelijk van of u de ontvangers met anderen wilt kunnen delen.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **sparen**.

   De gebruikers met wie u de filter, de mening, of het groeperen deelde kunnen tot het toegang hebben door de **Filter**, **Mening**, of **Groepering** drop-down menu of pictogram te klikken en neer aan **te scrollen die met me** sectie wordt gedeeld.


