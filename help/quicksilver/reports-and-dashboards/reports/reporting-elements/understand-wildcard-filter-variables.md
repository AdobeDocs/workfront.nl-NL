---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Variabelen van jokerfilter
description: Door vervangingen in filters te gebruiken, kunt u een generische gebruiker of een datum in plaats van een specifieke gebruiker of een datum van verwijzingen voorzien. Op deze manier zijn de elementen die u maakt dynamisch en veranderen de resultaten afhankelijk van de context waarin ze worden gebruikt.
author: Nolan
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '1447'
ht-degree: 0%

---

# Variabelen van jokerfilter

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked to the training self-serve promted articles for user-based and date-based widlcards (how-to articles). This serves as the "overview/ reference" article for those articles. Consider renaming this when that is allowed.) </p>
<p>(NOTE: Alina: ***&gt;&gt;Linked in other articles - do not move/ delete.</p>
<p>&gt;&gt;This was included but it is not supported???:</p>
<p>The $$USER.roleIDs variable refers to all the job roles that are associated with the logged-in user. Using this variable, you can&nbsp; items assigned to all of the job roles associated with the logged-in user.</p>
<p>For example, if you want to display tasks assigned to any of the job roles associated with the logged-in user, you can use the following filter rule in a task filter:</p>
<p>AssignedToID Equals $$USER.roleIDs.)</p>
</div>
-->

Adobe Workfront ondersteunt filtervariabelen of jokertekens bij het maken van de volgende elementen:

* Filters in lijsten, rapporten en de Planner van het Middel

   Raadpleeg het artikel voor informatie over Workfront-filters [Overzicht van filters in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Geavanceerde zoekopdrachten

   Zie de sectie voor informatie over geavanceerde zoekopdrachten [Geavanceerd zoeken gebruiken](../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search) in het artikel [Zoeken in Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

* Berekende kolommen in weergaven
* Voorwaardelijke opmaak in weergaven

   Zie het artikel voor informatie over voorwaardelijke opmaak [Voorwaardelijke opmaak gebruiken in weergaven](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

* Berekende aangepaste velden

   >[!NOTE]
   >
   >Variabelen van jokertekenfilters worden niet ondersteund wanneer wordt verwezen naar geneste verzamelingen in een berekende kolom.

   Zie het artikel voor informatie over berekende aangepaste velden en kolommen [Berekende aangepaste velden versus berekende kolommen](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Door vervangingen te gebruiken, kunt u een generische gebruiker of een datum in plaats van een specifieke gebruiker of een datum van verwijzingen voorzien. Op deze manier zijn de elementen die u maakt dynamisch en veranderen de resultaten afhankelijk van de context waarin ze worden gebruikt.

Bijvoorbeeld, wint het filtreren voor $$USER.homeGroupID in een projectrapport slechts projecten verbonden aan de Groep van het Huis van de gebruiker terug die het programma wordt geopend.

In Workfront kunt u op datum gebaseerde of op gebruiker gebaseerde filtervariabelen gebruiken.

## Filtervariabelen voor jokertekens op basis van datum

De op datum-gebaseerde vervangingsopties van Workfront kunnen in combinatie met om het even welk attribuut van de datumfilter worden gebruikt.

Voor informatie over het toevoegen van een op datum gebaseerde vervanging aan een rapport, zie het artikel [Gebruik op datum gebaseerde jokertekens om rapporten te generaliseren](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>Als u een datum- en tijdberekening maakt die geen tijdgedeelte bevat of die de jokertekens $$TODAY of $$NOW gebruikt, gebruikt het systeem de datum volgens de UTC-zone (Coordinated Universal Time), niet volgens uw lokale tijdzone. Dit kan tot een onverwacht datumresultaat leiden.

Kies een van de volgende jokertekens op basis van datum:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$TODAY</strong> </p> </td> 
   <td> <p>Wij adviseren dat u datum-gevoelige filters gebruikend deze vervangingskaart bouwt zodat vermijdt u bouw de filter morgen, volgende week, of volgende maand opnieuw.</p> <p>Als u bijvoorbeeld alle taken wilt weergeven die vóór vandaag verschuldigd zijn, kunt u de volgende regel in een taakfilter gebruiken: <em>Geplande begindatum minder dan $$TODAY</em>.</p> <p>$$TODAY is altijd gelijk aan middernacht voor de huidige dag.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>Dit is vergelijkbaar met de jokerteken $$TODAY, maar inclusief de huidige datum en tijd. $$NOW is gelijk aan de huidige datum en tijd.</p> <p>Bijvoorbeeld, als u alle die uuringangen wilt tonen tot de huidige tijd worden verstrekt, kunt u dit doen door de volgende regel in een uurfilter te gebruiken: <em>Geplande begindatum minder dan $$NOW</em>.</p> <p>Opmerking: Dit jokerteken wordt niet ondersteund in de Resource Planner.</p> </td> 
  </tr> 
 </tbody> 
</table>

U kunt jokertekens combineren met de volgende elementen om verschillende tijdsperioden en verschillende tijdstippen (in de toekomst of in het verleden) aan te geven:

| Attributen |   |
|---|---|
| **q** | kalenderkwartaal |
| **h** | uur |
| **d** | dag |
| **w** | week |
| **m** | maand |
| **y** | jaar |

{style="table-layout:auto"}

| **Kwalificaties** |  |
|---|---|
| **b** | begin van de week (zondag) |
| **e** | einde van de week (zaterdag) |

{style="table-layout:auto"}

| **Operatoren** |  |
|---|---|
| **+** | waarde toevoegen aan jokertekenwaarde |
| **-** | Waarde van jokerteken aftrekken van waarde |

{style="table-layout:auto"}

Bijvoorbeeld de jokerteken `$$TODAYb+2w` verwijst naar &quot;2 weken vanaf het begin van deze week&quot;. Jokerteken *`$$NOW+2h` verwijst naar &quot;over 2 uur.&quot;

## Op gebruikers gebaseerde jokertekenfiltervariabelen

>[!IMPORTANT]
>
>Als een filter of een rapport een op gebruiker-gebaseerde variabele van de vervangingsfilter bevat tonen de resultaten altijd informatie die door de gebruiker wordt gefilterd die momenteel het programma wordt geopend. Wanneer u zulk een filter of rapport met een andere gebruiker deelt, wint het vervanging informatie voor de gebruiker terug die het rapport bekijken. De twee gebruikers zien verschillende resultaten.

Voor informatie over het toevoegen van een op gebruiker-gebaseerde vervanging aan een rapport, zie het artikel [Gebruik op gebruiker gebaseerde jokertekens om rapporten te generaliseren](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Workfront biedt de volgende gebruikersvariabelen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>De meest voorkomende op gebruikers gebaseerde variabele is $$USER.ID. Dit keert altijd identiteitskaart van de het programma geopende gebruiker terug. Dit is identiteitskaart die wordt gebruikt om te identificeren welke gebruiker elk voorwerp en hun werktaken creeerde.</p> <p>Wanneer gebruikt in rapporten, vermindert dit vervangingsaantal het aantal rapporten die u in uw systeem moet creëren. U kunt één rapport tot stand brengen en het met verscheidene gebruikers delen, en de resultaatverandering die op de gebruiker wordt gebaseerd die het programma wordt geopend en het rapport bekijkt.</p> <p>Bijvoorbeeld, om een rapport voor alle kwesties te bouwen die aan de gebruiker worden toegewezen die het programma wordt geopend, kunt u de volgende regel in een uitgevende filter gebruiken: <em>Toegewezen aan id is gelijk aan $$USER.ID</em>.</p> <p>Workfront gebruikt deze variabele in de volgende ingebouwde filters:</p> 
    <ul> 
     <li>Mijn rapporten</li> 
     <li>Mijn projecten</li> 
     <li>Mijn taken</li> 
     <li>Mijn problemen</li> 
     <li>Mijn uren</li> 
    </ul> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.categoryID</strong> </p> </td> 
   <td> <p>De variabele $$USER.categoryID verwijst naar een specifiek aangepast formulier dat is gekoppeld aan de aangemelde gebruiker.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelID</strong> </p> </td> 
   <td> <p>De $$USER.accessLevelID-variabele verwijst naar de id van het toegangsniveau dat aan de aangemelde gebruiker is gekoppeld.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelRank</strong> </p> </td> 
   <td> <p>De variabele $$USER.accessLevelRank verwijst naar de rang van het toegangsniveau verbonden aan het programma geopende gebruiker.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.companyID</strong> </p> </td> 
   <td> <p>De $$USER.companyID-variabele verwijst naar het bedrijf dat is gekoppeld aan de aangemelde gebruiker.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.customerID</strong> </p> </td> 
   <td> <p>De variabele $$USER.customerID verwijst naar de id van de klantenaccount die aan uw omgeving is gekoppeld. Voor uw omgeving is er slechts één mogelijke waarde voor deze variabele en deze wordt doorgaans alleen gebruikt bij het bouwen van integratie via de API.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.firstName</strong> </p> </td> 
   <td> <p>De variabele $$USER.firstName verwijst naar de voornaam van de aangemelde gebruiker.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.lastName</strong> </p> </td> 
   <td> <p>De variabele $$USER.lastName verwijst naar de achternaam van de aangemelde gebruiker.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.name</strong> </p> </td> 
   <td> <p>De variabele $$USER.name verwijst naar de volledige naam van de aangemelde gebruiker.</p> <p>Opmerking:   <p>Deze jokertekenvariabele werkt alleen wanneer u een filter in de tekstmodus wijzigt. U kunt dit jokerteken niet gebruiken in filters die geen tekstmodus ondersteunen. U kunt dit jokerteken bijvoorbeeld niet gebruiken in de filters in de volgende gebieden:</p> 
     <ul> 
      <li> <p>Resource Planner</p> </li> 
      <li> <p>Werklastverdeling</p> </li> 
      <li> <p>Analyse</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>De $$USER.homeGroupID-variabele verwijst naar de id van de Home Group van de aangemelde gebruiker. Als Beheerder van de Groep, kunt u deze variabele gebruiken om slechts voor punten te filtreren die tot de gebruikers in uw Groep van het Huis behoren.</p> <p>Bijvoorbeeld, om alle onvolledige taken op projecten in de financieringsgroep te zien, gebruik de volgende filterregels in een taakfilter:<br><em>Project: Groep-id is gelijk aan $$USER.homeGroupID </em><br><em>Percentage voltooid minder dan 100</em></p> <p>Om alle onvolledige taken te zien die aan individuen in een specifieke groep worden toegewezen die de Groep van het Huis van de het programma geopende gebruiker is, gebruik de volgende filterregels in een taakfilter:</p> <p><em>Toegewezen aan: Groep-id is gelijk aan $$USER.homeGroupID<br>Percentage voltooid minder dan 100</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>De variabele $$USER.otherGroupIDs verwijst naar alle groepen (met inbegrip van de Groep van het Huis) verbonden aan het het programma geopende gebruikersprofiel.</p> <p>De functionaliteit van deze variabele is gelijkaardig aan dat van de $$USER.homeGroupID variabele, behalve de informatie van de resultaatvertoning over de gebruikers die tot om het even welke groepen behoren verbonden aan de het programma geopende gebruiker.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>De $$USER.homeTeamID-variabele verwijst naar de id van het Home Team van de aangemelde gebruiker. Als teammanager, kunt u deze variabele aan filter slechts voor punten gebruiken die tot de gebruikers in uw Team van het Huis behoren.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.teamIDs</strong> </p> </td> 
   <td> <p>De variabele $$USER.teamIDs keert een lijst van alle teams verbonden aan de het programma geopende gebruiker terug.</p> <p>De functionaliteit van deze variabele is gelijkaardig aan dat van de variabele $$USER.homeTeamID, behalve de informatie van de resultaatvertoning over de gebruiker die tot om het even welke die teams behoort in de filter worden geïdentificeerd.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>De $$USER.roleID-variabele verwijst naar de primaire rol van de aangemelde gebruiker. Met deze variabele kunt u taken of problemen rapporteren die zijn toegewezen aan een specifieke taakrol.</p> <p>Bijvoorbeeld, om alle taken te zien die aan de Primaire Rol van de het programma geopende gebruiker worden toegewezen, kunt u de volgende filterregel in een taakfilter gebruiken:</p> <p><em>Taak: Rol-id is gelijk aan $$USER.roleID.</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader">$$USER.roleIDs</td> 
   <td> <p>De variabele $$USER.roleIDs verwijst naar alle baanrollen verbonden aan het programma geopende gebruiker. Gebruikend deze variabele, kunt u over taken of kwesties rapporteren die aan om het even welke baanrollen worden toegewezen verbonden aan het programma geopende gebruiker. </p> <p>Bijvoorbeeld, om alle taken te zien die aan om het even welke rollen worden toegewezen verbonden aan het programma geopende gebruiker, kunt u de volgende filterregel in een taakfilter gebruiken:</p> <p><i>Taak: Rol-id is gelijk aan $$USERID.roleIDs<br></i> </p> <p>Tip: De <i>Taak: Rol-id is gelijk aan $$USERID.roleIDs</i> filterregel bestaat in de ingebouwde filters Niet toegewezen Taken in Mijn Rol en Niet toegewezen Kwesties in Mijn Rol. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Filtervariabelen van wilde kaarten op basis van object

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>De variabele $$OBJCODE verwijst naar het type van een object. </p> 
     <p>Wanneer in een aangepast formulier de geselecteerde objecttypen van het formulier niet compatibel zijn met een veld waarnaar wordt verwezen in een berekend aangepast veld, kunt u met deze jokerkaart voorkomen dat dubbele formulieren voor deze objecttypen worden gemaakt.</p> 
     <p>In het berekende aangepaste veld doet u dit door de jokertekens in een IF-expressie op te nemen, zodat de berekening verschillende waarden kan weergeven voor elk objecttype van het formulier. </p> 
     <p>Zie de sectie voor meer informatie en een voorbeeld <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat" class="MCXref xref">Berekende aangepaste velden in aangepaste formulieren voor meerdere objecten</a> in het artikel <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Berekende gegevens toevoegen aan een aangepast formulier</a>.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
