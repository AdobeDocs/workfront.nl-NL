---
product-area: reporting
navigation-topic: reporting-elements
title: Een filter, weergave of groep delen
description: U kunt filters, weergaven en groeperingen delen die u kunt bekijken met andere gebruikers.
author: Lisa
feature: Reports and Dashboards
exl-id: 63a6db90-d52c-4147-a442-7904ef9e9d49
source-git-commit: b56e6591c7da166bd1548420b562b838cc7fe0f2
workflow-type: tm+mt
source-wordcount: '1362'
ht-degree: 0%

---

# Een filter, weergave of groep delen

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: CONSIDER SPLITTING THIS in three articles for each reporting element?)</p>
<p>(NOTE: This is linked from the TOC article in WF Basics > permissions section)&nbsp;</p>
</div>
-->

<span class="preview">In de voorvertoningsomgeving is de verbeterde filterervaring (voorheen &quot;bèta&quot; genoemd) nu de standaardinstelling. Deze verbeterde filters zijn nu &#39;standaard&#39; en de oudere filterervaring is &#39;verouderd&#39;.</span>

Uw Adobe Workfront-beheerder verleent gebruikers toegang tot weergave- of bewerkingsobjecten wanneer zij toegangsniveaus toewijzen. Ga voor meer informatie over het verlenen van toegang tot objecten naar [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Samen met het toegangsniveau dat de gebruikers worden verleend, kunt u hen toestemmingen ook verlenen om specifieke voorwerpen te bekijken of uit te geven die u creeerde of toegang om hebt te delen. Voor meer informatie over toegangsniveaus en toestemmingen, zie [Hoe de toegangsniveaus en de toestemmingen samenwerken](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

U kunt filters, weergaven en groeperingen delen die u kunt bekijken met andere gebruikers.

Wanneer een filter, weergave of groep met u wordt gedeeld, kunt u dat filter, die weergave of die groep toepassen op uw lijsten. Afhankelijk van de toegang die aan u wordt verleend, zou u het kunnen kunnen wijzigen en het met andere gebruikers delen.

Zie de volgende artikelen voor informatie over het maken van een filter, weergave of groepering:

* [Overzicht van filters in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Overzicht van weergaven in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Overzicht van groepen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

## Toegangsvereisten

U moet het volgende hebben:

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
   <td> <p>Aanvraag of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>Toegang tot filters, weergaven, groepen weergeven of vergroten</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Machtigingen weergeven of hoger met toegang voor delen naar een weergave, filter of groep</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Een filter, weergave of groep delen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when the beta filters/ groupings come out either consider splitting this in different kinds of FVGs or splitting this article in FVGs for showing sharing on each one of them??)</p>
-->

U kunt filters in uitgezochte lijsten delen gebruikend de volgende interfaces:

* Standaardinterface
* Bètabuilder-interface

Het delen van filters in geselecteerde lijsten is anders, afhankelijk van de interface waarvan u het filter gebruikt om te delen. Voor informatie over de types van filter-bouwt interfaces, zie [Filters maken of bewerken in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

U kunt weergaven en groepen alleen delen in de standaardinterface.

* [Filters, weergaven en groepen delen via de standaardinterface](#share-with-standard-interface)
* [Filters delen via de bètabuilderinterface](#share-with-beta-builder-interface)

### Filters, weergaven en groepen delen via de standaardinterface {#share-with-standard-interface}

Het delen van filters, weergaven en groepen in de standaardinterface is identiek.

1. Ga naar een lijst met objecten of een rapport.
1. (Voorwaardelijk) Klik in een lijst op de knop **Filter**, **Weergave**, of **Groepering** klikt u op de knop **Meer** pictogram ![Meer pictogram](assets/more-icon.png)vervolgens **Delen**.

   Klik in een rapport op de knop **Filter**, **Weergave**, of **Groepering** selecteert u vervolgens het filter, de weergave of de groep die u wilt delen.

1. (Voorwaardelijk) Als u wilt delen via een rapport, klikt u op de knop **Filter**, **Weergave**, of **Groepering** vervolgkeuzemenu nogmaals, en klik vervolgens op **Filter delen**, **Weergave delen**, of **Groepering delen**.\
   De **Filtertoegang**, **Toegang weergeven**, of **Toegang groeperen** wordt weergegeven.

   ![Delen, filter](assets/share-filter-people-box-nwe-350x458.png)

1. Voer een van de volgende twee handelingen uit, afhankelijk van wie u wilt delen:

   **Om met individuele gebruikers, teams, rollen, groepen, of bedrijven te delen:** Typ in het opgegeven veld de naam van de gebruiker, het team, de rol, de groep of het bedrijf waarmee u wilt delen. Klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.\
   Herhaal dit proces om toegang met veelvoudige gebruikers, teams, rollen, groepen, of bedrijven te delen.

   >[!TIP]
   >
   >Delen met groepen geeft machtigingen voor het filter, de weergave of de groep aan de leden van de groep en van alle subgroepen.


   **Met alle gebruikers in het systeem delen:** Klik op de knop **Instellingen** pictogram, klik vervolgens op **Dit voor het hele systeem zichtbaar maken**.\
   Uw beheerder moet de optie voor het delen van het hele systeem selecteren om deze optie beschikbaar te maken. Zie de artikelen voor meer informatie [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) en [Rapporten, dashboards en kalenders delen](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

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
      <td> <p>Klikken <strong>Geavanceerde instellingen</strong>selecteert of wist vervolgens de <strong>Delen</strong> afhankelijk van de vraag of de ontvangers met anderen mogen delen.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Opslaan**.

   Gebruikers met wie u het filter, de weergave of de groep hebt gedeeld, hebben toegang tot het filter door op de knop **Filter**, **Weergave**, of **Groepering** vervolgkeuzemenu of pictogram en omlaag schuiven naar de **Gedeeld met mij** sectie.

### Filters delen via de bètabuilderinterface {#share-with-beta-builder-interface}

Wanneer het delen van filters van lijsten van projecten, taken, of kwesties, kunt u hen delen gebruikend de bèta bouwerinterface in plaats van de standaardinterface.

De bètabuilderinterface is niet beschikbaar voor andere objecten in Workfront.

U kunt geen filters in de interface bouwen van de bètaaannemer wanneer het bouwen van rapporten.

Een filter delen met behulp van de bètabuilderinterface:

1. Ga naar een lijst met projecten, taken of problemen.
1. Klik op de knop **Filter** pictogram ![Filterpictogram](assets/filter-nwepng.png)en stelt vervolgens de **Bètainstelling** ![Bètainstelling](assets/beta-toggle-white-on-existing-filters.png) om toegang te krijgen tot de bètabuilder. Deze optie is standaard uitgeschakeld.

   Ga vervolgens, indien nodig, akkoord met de bètaovereenkomst.

   Hiermee opent u de interface van de bètafilterbuilder.

   >[!TIP]
   >
   >De kopbal van de bouwerinterface verandert in blauw wanneer u bèta bouwer toelaat. Nadat u de bètabuilderinterface hebt ingeschakeld, houdt Workfront deze ingeschakeld voor alle gebieden waar deze beschikbaar is.

   ![Bètafilterbuilder](assets/new-filters-all-filter-types.png)

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
   <td>Filters die u zelf hebt gemaakt en opgeslagen.</td>
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

1. Als u de muisaanwijzer boven een filter houdt, hebt u toegang tot minstens de volgende opties: **Meer** menu ![Het menu Meer](assets/more-icon-spectrum.png)en klik vervolgens op **Delen**.

   ![Meer menuopties](assets/new-filters-more-menu-options-with-delete.png)

   Het dialoogvenster Filter delen wordt weergegeven.

1. Schakel de instelling voor het gehele systeem weergeven in. Dit geeft iedereen in Workfront toestemming om het filter te bekijken.

   >[!IMPORTANT]
   >
   >Wees voorzichtig met deze instelling. Door veel filters voor alle gebruikers toe te voegen, wordt de filterervaring overzichtelijk en worden filters moeilijker te vinden.

   Of typ de namen van gebruikers, teams, rollen, groepen of bedrijven waarmee u wilt delen in de **Toegang verlenen aan** veld.

   ![Filter delen, vak](assets/new-filters-share-filter.png)

1. (Optioneel) Klik op de pijl naar rechts naast de naam van een entiteit om de machtigingen voor het filter te bewerken en schakel vervolgens de optie **Weergave** of **Beheren** optie. **Weergave** is de standaardwaarde.

   ![Machtigingen delen](assets/new-filters-sharing-permissions.png)

1. (Optioneel) Schakel de aanvullende machtigingen voor een entiteit in of uit door een van de volgende handelingen uit te voeren:

   1. Klikken **Weergave** en schakelt u de **Delen** optie. Deze optie is standaard ingeschakeld.
   1. Klikken **Beheren** en schakelt u **Delen** of de **Verwijderen** optie. Deze zijn standaard ingeschakeld.

      >[!NOTE]
      >
      >Als u de optie Beheren inschakelt met de optie Verwijderen, kunnen deze gebruikers het filter van alle gebruikers verwijderen, ook al hebben zij geen eigenaar van het filter.
   >[!TIP]
   >
   >Gebruikers kunnen geen hogere machtigingen ontvangen dan hun toegangsniveau. Als zij geen toegang tot Edit filters in hun toegangsniveau hebben, kunnen zij geen toestemmingen ontvangen om een filter te beheren. Workfront schakelt de optie Beheren voor deze gebruikers uit en de optie is grijs.

1. Klikken **Delen**. Het filter wordt gedeeld met de entiteiten u specificeerde.

   >[!TIP]
   >
   >Delen met groepen geeft machtigingen aan het filter voor de leden van de groep en voor alle subgroepen.

   De filters die u in de **Gedeeld met mij** van het filterdeelvenster voor deze entiteiten.

   ![Filters die met mij worden gedeeld](assets/new-filters-shared-with-me.png)

