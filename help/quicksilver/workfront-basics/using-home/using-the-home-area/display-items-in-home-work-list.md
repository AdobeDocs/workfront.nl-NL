---
product-area: projects
navigation-topic: use-the-home-area
title: Items weergeven in de [!UICONTROL Work List] in het gebied Home
description: In [!UICONTROL Work List] in het [!UICONTROL Home] -gebied worden alle werkitems weergegeven die aan u zijn toegewezen. U kunt bepalen welke items in uw [!UICONTROL Work List] worden weergegeven door filters te gebruiken en uw werkitems te groeperen en te sorteren.
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1558'
ht-degree: 0%

---

# Items weergeven in het [!UICONTROL Work List] gebied in het [!UICONTROL Home] gebied

<!-- Audited: 1/2024 -->


In [!UICONTROL Work List] in het [!UICONTROL Home] -gebied worden alle werkitems weergegeven die aan u zijn toegewezen. U kunt bepalen welke items in uw [!UICONTROL Work List] worden weergegeven door filters te gebruiken en uw werkitems te groeperen en te sorteren.

>[!NOTE]
>
>* Wanneer het omzetten van een kwestie in een taak of een project, wordt de kwestie verwijderd uit het gebied van het Huis van de gebruiker die aan de kwestie wordt toegewezen.
>
>* Wanneer het omzetten van een taak in een project, wordt de taak geschrapt en het wordt verwijderd uit het gebied van het Huis van de gebruiker die aan de taak wordt toegewezen.


## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie</strong></td> 
   <td> <p>Nieuw:</p><ul><li>[!UICONTROL Contributor] alleen voor goedkeuringen</li> <li>[!UICONTROL Standard] of hoger voor alle andere objecten</li> <p>of</p> 
  </ul><p>Huidige:</p><ul><li>[!UICONTROL Review] alleen voor goedkeuringen</li> <li>[!UICONTROL Work] of hoger voor alle andere objecten</li> </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau</strong></td> 
   <td> <p>[!UICONTROL View] of betere toegang tot Projecten, Taken, Kwesties, en Documenten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Contribute-machtigingen of hoger voor de taken en problemen waarmee u moet werken</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filter de [!UICONTROL Work List]

U kunt items filteren in de [!UICONTROL Work List] om alleen bepaalde typen items weer te geven. U kunt bijvoorbeeld de filter [!UICONTROL Work List] filteren om alleen uitgaven of aanvragen weer te geven.

>[!NOTE]
>
>De filteropties worden opgeslagen in de browser. Als u consequent dezelfde browser gebruikt op dezelfde computer (en de sitegegevens niet wist), veranderen de geselecteerde filters niet. Als u van browser of computer verandert dan keren de filters aan de standaardoptie terug, die met alle gedeselecteerde filters is.

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Home]**.
1. Klik op de vervolgkeuzelijst **[!UICONTROL Filter]** ![](assets/filter-nwepng.png) . Als u filters hebt geselecteerd, wordt het aantal geselecteerde filters weergegeven in plaats van het pictogram.
1. Selecteer een van de volgende filteropties om het type items op te geven dat u wilt weergeven:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL All]</strong></td> 
      <td>Hiermee geeft u alle items weer en selecteert u deze. Dit omvat taken, kwesties, goedkeuringen, persoonlijke taken, en voltooide taken en kwesties. </td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks: Working On]</strong></td> 
      <td> <p>Hiermee geeft u alleen taken weer waaraan u actief werkt. Dit zijn taken die aan u zijn toegewezen en waarvoor u op de knop [!UICONTROL Work On It] hebt geklikt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks: Ready to Start]</strong></td> 
      <td> 
       <div> 
        <p>Hiermee geeft u alleen taken weer die u kunt starten. Beide volgende instructies moeten waar zijn:</p> 
        <ul> 
         <li> <p>De taken en hun ouders hebben geen voorgangers of taakbeperkingen die hen beletten om aan te werken.</p> </li> 
         <li> <p>De [!UICONTROL Planned Start Date] van de taken is in het verleden of tot twee weken in de toekomst.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks: Not Ready]</strong></td> 
      <td> 
       <div> 
        <p>Hiermee geeft u alleen taken weer die nog niet kunnen worden gestart. Een van de volgende instructies moet true zijn:</p> 
        <ul> 
         <li> <p>De taken en hun ouders zouden voorgangers of taakbeperkingen kunnen hebben die hen verhinderen om aan worden gewerkt.</p> </li> 
         <li> <p>De taken hebben een [!UICONTROL Planned Start Date] die meer dan twee weken in de toekomst is.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Issues: Working On]</strong></td> 
      <td> <p>Hiermee geeft u alleen problemen weer waaraan u actief werkt. Dit zijn aan u toegewezen problemen waarvoor u op de knop [!UICONTROL Work On It] hebt geklikt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Issues: Requested]</strong></td> 
      <td>Hiermee geeft u alleen problemen weer waaraan u bent toegewezen, maar waarvoor u niet op de knop [!UICONTROL Work On It] hebt geklikt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Persoonlijk</strong></td> 
      <td>Hiermee geeft u alleen persoonlijke taken weer. Dit zijn taken die u als a [!UICONTROL To Do] taak creeert, zoals die in de sectie <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-personal-task"> wordt beschreven creeer een persoonlijke taak </a> in het artikel <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md"> creeert het werkpunten van het [!UICONTROL Home] gebied </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Approvals]</strong></td> 
      <td> 
       <div> 
        <p>Hiermee geeft u alleen goedkeuringen weer die aan u zijn toegewezen of gedelegeerd en goedkeuringen die u hebt verzonden. Goedkeuringen omvatten goedkeuringen voor werkitems (projecten, taken en kwesties) en goedkeuringen voor documenten, proefdrukken, verzoeken om toegang en tijdkaarten. Raadpleeg de volgende artikelen voor meer informatie over goedkeuringen:</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref"> goedkeuringen van de Mening </a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref"> Goedkeuringen van het Werk </a> </p> </li> 
        </ul> 
        <p>Opmerking: goedkeuringen die u hebt ingediend en waarvoor u ook een van de fiatteurs bent, worden twee keer geteld.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Delegated: Delegated by me]</strong></td> 
      <td> 
       <div> 
        <p>Hiermee geeft u alleen werkitems weer die u aan een andere gebruiker hebt gedelegeerd.</p> 
        <p>Voor meer informatie over het delegeren van taken, zie <a href="/help/quicksilver/manage-work/delegate-work/how-to-delegate-work.md#delegate-tasks-and-issues-to-another-user" class="MCXref xref"> de taken en kwesties van de Afgevaardigde aan een andere gebruiker </a>.
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Delegated: Delegated to me]</strong></td> 
      <td> 
       <div> 
        <p>Hiermee geeft u alleen de werkitems weer die tijdelijk aan u zijn gedelegeerd door een andere gebruiker.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Completed]</strong></td> 
      <td> <p>Toont slechts voltooide taken, kwesties, en persoonlijke taken. De voltooide werkvertoningen voor de vorige twee weken en het wordt gegroepeerd in de Lijst van het Werk volgens de week waarin zij werden voltooid. Goedkeuringen zijn niet inbegrepen.</p> <p>Voltooid werk wordt verborgen in [!UICONTROL Work List] tenzij u dit filter selecteert.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* Filteropties zijn gebaseerd op objecten (Taken, Problemen, Goedkeuringen, Persoonlijke taken).
   >* Taken en problemen worden verder gefilterd op basis van hun status in relatie tot onze gereedheid om eraan te werken ( [!UICONTROL Working On] , [!UICONTROL Ready to Start] , [!UICONTROL Not Ready] voor taken en [!UICONTROL Working On] en [!UICONTROL Requested] voor problemen). U kunt selecteren om taken of problemen in een bepaalde status weer te geven of op Taken of Problemen klikken om alle frames te selecteren en weer te geven.
   >* Er is een afzonderlijk filter voor voltooide items en het bevat zowel taken als problemen. Hieronder vallen geen goedkeuringen. Het filter [!UICONTROL Completed] bevat persoonlijke taken.
   >* U kunt ervoor kiezen slechts één frame tegelijk weer te geven. U kunt bijvoorbeeld alleen [!UICONTROL Working On] taken en alleen [!UICONTROL Requested] uitgaven weergeven. U kunt ook meerdere frames tegelijk selecteren.
   >* U kunt geen filters toepassen op items die zijn toegewezen aan een van uw teams en teamtoewijzingen zijn niet opgenomen in de items die rechtstreeks aan u zijn toegewezen.


1. (Facultatief) organiseer verder [!UICONTROL Work List], zoals die in de sectie [ Groep en soort door Datum, Project, en Prioriteit ](#group-and-sort-by-date-project-and-priority) in dit artikel wordt beschreven.

## Groeperen en sorteren op [!UICONTROL Date] , [!UICONTROL Project] en [!UICONTROL Priority]

U kunt de [!UICONTROL Work List] op [!UICONTROL Planned Completion Date] , [!UICONTROL Commit Date] , [!UICONTROL Project] of [!UICONTROL My Priority] groeperen en sorteren. De optie die u kiest, bepaalt hoe items worden gegroepeerd in de [!UICONTROL Work List] .

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Home]**.
1. Klik de **[!UICONTROL Group by]** ![ Groep door ](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/grouping-28x19.png) drop-down menu.

   <!--
   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)
   -->

1. Selecteer een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Planned Completion]</strong></td> 
      <td> <p> De items worden in de volgende groepen in de [!UICONTROL Work List] weergegeven, afhankelijk van [!UICONTROL Planned Completion Date] (het aantal items in elke groep wordt tussen haakjes weergegeven naast de titel van de kop):</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL No Planned Completion Date]</p> </li> 
        <li> <p>[!UICONTROL This Week]</p> <p>Deze groepering wordt standaard uitgebreid.</p> </li> 
        <li> <p>[!UICONTROL Next Week]</p> </li> 
        <li> <p>[!UICONTROL Planned], gevolgd door diverse [!UICONTROL Planned Completion Dates] (meerdere groepen)</p> </li> 
        <li> <p>[!UICONTROL Complete]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Planned Start]</strong></td> 
      <td> <p>De items worden in de volgende groepen in de [!UICONTROL Work List] weergegeven, afhankelijk van [!UICONTROL Planned Start Date] (het aantal items in elke groep wordt tussen haakjes weergegeven naast de titel van de kop):</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL This Week] </p> <p>Deze groepering wordt standaard uitgebreid.</p> </li> 
        <li> <p>[!UICONTROL Next Week]</p> </li> 
        <li> <p>[!UICONTROL Planned], gevolgd door diverse [!UICONTROL Planned Start Dates] (meerdere groepen)</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Commit Date]</strong></td> 
      <td> <p>De items worden in de volgende groepen in de [!UICONTROL Work List] weergegeven (het aantal items in elke groep wordt tussen haakjes naast de titel van de kop weergegeven):</p> 
       <ul> 
        <li> <p>[!UICONTROL No Commit Date]</p> </li> 
        <li> <p>[!UICONTROL Committed Next Week]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Project]</strong></td> 
      <td>De items worden gegroepeerd op project en projecten worden in alfabetische volgorde weergegeven in de [!UICONTROL Work List] . (Het aantal items in elke groep wordt tussen haakjes weergegeven naast de titel van de kop.)</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL My Priority]</strong></td> 
      <td>De items worden in een door u gekozen volgorde weergegeven. Voor meer informatie, zie <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref"> het werk in het [!UICONTROL Home] gebied </a> Prioritize.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>De standaardsortering wordt oplopend uitgevoerd. Als u de sortering wijzigt in aflopend, worden de geselecteerde sorteeropties opgeslagen in de browser. Als u consequent dezelfde browser gebruikt op dezelfde computer (en de sitegegevens niet wist), verandert het sorteren niet, maar als u van browser of computer overschakelt, verandert het sorteren in de standaardsortering.

## Te late objecten weergeven

[!DNL Adobe Workfront] gebruikt de volgende datums om te bepalen of werkverzoeken te laat zijn:

* **Taken**: [!UICONTROL Planned Completion Date]
* **Kwesties**: [!UICONTROL Planned Completion Date]
* **Documenten**: [!UICONTROL Submitted date]
* **Timesheets**: [!UICONTROL Submitted date]
* **goedkeurt**: [!UICONTROL Submitted date]
* **Goedkeuringen van het Bewijs**: [!UICONTROL Proof deadline]

## Zoeken in [!UICONTROL Work List]

Wanneer u de [!UICONTROL Work List] doorzoekt, worden alle aan u toegewezen items in de zoekopdracht geretourneerd (zelfs items die momenteel niet op het scherm zijn geladen). Als de optie [!UICONTROL Show complete] is geselecteerd, worden alle items die u de afgelopen twee weken hebt gemarkeerd als voltooid, ook geretourneerd.

Bovendien worden alleen de namen van de werkitems doorzocht (informatie binnen het werkitem wordt niet doorzocht en ook de namen van de projecten waar het werkitem zich bevindt).

U kunt als volgt de [!UICONTROL Work List] zoeken:

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Home]**.
1. (Facultatief) filter en groepeer [!UICONTROL Work List], zoals die in [ wordt beschreven filter de [!UICONTROL Work List]](#filter-the-work-list) en [ Groep en soort door Datum, Project, en Prioriteit ](#group-and-sort-by-date-project-and-priority).

1. (Optioneel) Als u op zoek bent naar een werkitem dat al is voltooid, moet u de [!UICONTROL Work List] zodanig configureren dat de items worden weergegeven voordat u kunt zoeken.

1. Klik het pictogram van het Onderzoek ![ Onderzoek ](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/search-icon.png).
1. Typ de naam van het item waarnaar u zoekt.\
   Het filter [!UICONTROL Work List] wordt automatisch gefilterd om items met een overeenkomende naam op te nemen.

## De grootte van de werklijst wijzigen

U kunt de grootte van de [!UICONTROL Work List] zodanig wijzigen dat deze overal tussen ongeveer een kwart van het gebied Home verbruikt en ongeveer de helft van het gebied [!UICONTROL Home] .

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Home]**.
1. Plaats de muis boven de rechterrand van de [!UICONTROL Work List] en sleep vervolgens naar links of rechts totdat de werklijst de gewenste grootte heeft.

## Groepen samenvouwen en uitbreiden

Items in de [!UICONTROL Work List] worden weergegeven in groepen. U kunt groepen samenvouwen en uitvouwen om te bepalen hoeveel informatie op de pagina tegelijk wordt weergegeven.

U kunt groepen in de [!UICONTROL Work List] samenvouwen en uitvouwen om beter te bepalen welke informatie zichtbaar is.\
Standaard wordt de [!UICONTROL This Week] -groep uitgevouwen en worden alle andere groepen samengevouwen. Wijzigingen die u aanbrengt, worden onthouden wanneer u het gebied Home weer opent.

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Home]**.
1. Klik op de pijl **[!UICONTROL Expand]** of **[!UICONTROL Collapse]** naast een groep die u wilt uitvouwen of samenvouwen.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   of\
   Als u alle groepen tegelijk wilt uitvouwen of samenvouwen, klikt u op de **[!UICONTROL Expand]** - of **[!UICONTROL Collapse]** -pijl naast een willekeurige groep terwijl u de [!UICONTROL Shift] -toets ingedrukt houdt.
