---
product-area: projects
navigation-topic: use-the-home-area
title: Items weergeven in het dialoogvenster [!UICONTROL Work List] in het thuisgebied
description: De [!UICONTROL Work List] in de [!UICONTROL Home] worden alle werkitems weergegeven die aan u zijn toegewezen. U kunt bepalen welke items in het dialoogvenster [!UICONTROL Work] Lijst zoals hieronder beschreven.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: 7c624eff8931d206285b6c4d91083f4bf09a88b0
workflow-type: tm+mt
source-wordcount: '1402'
ht-degree: 0%

---

# Items weergeven in het dialoogvenster [!UICONTROL Work List] in het thuisgebied

De [!UICONTROL Work List] in de [!UICONTROL Home] worden alle werkitems weergegeven die aan u zijn toegewezen. U kunt bepalen welke items in het dialoogvenster [!UICONTROL Work] Lijst zoals hieronder beschreven.

>[!NOTE]
>
>Wanneer het omzetten van een kwestie in een taak of een project, wordt de kwestie verwijderd uit het gebied van het Huis van de gebruiker die aan de kwestie wordt toegewezen.
>
>Wanneer het omzetten van een taak in een project, wordt de taak geschrapt en het wordt verwijderd uit het gebied van het Huis van de gebruiker die aan de taak wordt toegewezen.


## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>[!UICONTROL Review] alleen voor goedkeuringen</p> <p>[!UICONTROL Work] of hoger voor alle andere objecten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>[!UICONTROL View] of betere toegang tot Projecten, Taken, Kwesties, en Documenten</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Contribute-machtigingen of hoger voor de taken en problemen waaraan u moet werken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Filteren op [!UICONTROL Work List]

U kunt items filteren in het dialoogvenster [!UICONTROL Work List] om alleen bepaalde typen items weer te geven. U kunt bijvoorbeeld het filter [!UICONTROL Work List] om alleen uitgaven of aanvragen weer te geven.

>[!NOTE]
>
>De filteropties worden opgeslagen in de browser. Als u consequent dezelfde browser gebruikt op dezelfde computer (en de sitegegevens niet wist), veranderen de geselecteerde filters niet. Als u van browser of computer verandert dan keren de filters aan de standaardoptie terug die met alle gedeselecteerde filters is.

1. Klik op de knop **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) in de rechterbovenhoek klikt u op **[!UICONTROL Home]**.
1. Klik op de knop **[!UICONTROL Filter]** ![](assets/filter-nwepng.png) vervolgkeuzelijst.
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
      <td role="rowheader"><strong>[!UICONTROL Tasks Working On]</strong></td> 
      <td> <p>Hiermee geeft u alleen taken weer waaraan u actief werkt. Deze taken zijn toegewezen aan u waarvoor u hebt geklikt [!UICONTROL Work On It] knop.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks Ready to Start]</strong></td> 
      <td> 
       <div> 
        <p>Hiermee geeft u alleen taken weer die u kunt starten. Beide volgende instructies moeten waar zijn:</p> 
        <ul> 
         <li> <p>De taken en hun ouders hebben geen voorgangers of taakbeperkingen die hen beletten om aan te werken.</p> </li> 
         <li> <p>De [!UICONTROL Planned Start Date] van de taken is in het verleden of tot twee weken in de toekomst .</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks Not Ready]</strong></td> 
      <td> 
       <div> 
        <p>Hiermee geeft u alleen taken weer die nog niet kunnen worden gestart. Een van de volgende instructies moet true zijn:</p> 
        <ul> 
         <li> <p>De taken en hun ouders zouden voorgangers of taakbeperkingen kunnen hebben die hen verhinderen om aan worden gewerkt.</p> </li> 
         <li> <p>De taken hebben een [!UICONTROL Planned Start Date] dat is meer dan twee weken in de toekomst .</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Issues Working On]</strong></td> 
      <td> <p>Hiermee geeft u alleen problemen weer waaraan u actief werkt. Dit zijn aan u toegewezen kwesties waarvoor u hebt geklikt [!UICONTROL Work On It] knop.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Issues Requested]</strong></td> 
      <td>Hiermee geeft u alleen problemen weer waaraan u bent toegewezen, maar waarvoor u nog niet op de knop [!UICONTROL Work On It] knop.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Persoonlijk</strong></td> 
      <td>Hiermee geeft u alleen persoonlijke taken weer. Dit zijn taken die u maakt als een [!UICONTROL To Do] taak, zoals beschreven in de sectie <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#creating-a-personal-task">Een persoonlijke taak maken</a> in het artikel <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">Werkitems maken op basis van het tabblad [!UICONTROL Home] gebied</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Approvals]</strong></td> 
      <td> 
       <div> 
        <p>Hiermee geeft u alleen goedkeuringen weer die aan u zijn toegewezen of gedelegeerd en goedkeuringen die u hebt verzonden. Goedkeuringen omvatten goedkeuringen voor werkitems (projecten, taken en kwesties) en goedkeuringen voor documenten, proefdrukken, verzoeken om toegang en tijdkaarten. Raadpleeg de volgende artikelen voor meer informatie over goedkeuringen:</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Goedkeuringen weergeven</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">Goedkeuring van werkzaamheden</a> </p> </li> 
        </ul> 
        <p>Opmerking: goedkeuringen die u hebt ingediend en waarvoor u ook een van de fiatteurs bent, worden twee keer geteld.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Completed]</strong></td> 
      <td> <p>Toont slechts voltooide taken, kwesties, en persoonlijke taken. De voltooide werkvertoningen voor de vorige twee weken en het wordt gegroepeerd in de Lijst van het Werk volgens de week waarin zij werden voltooid. Goedkeuringen zijn niet inbegrepen.</p> <p>Voltooid werk is verborgen in het dialoogvenster [!UICONTROL Work List] tenzij u dit filter selecteert.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* Filteropties zijn gebaseerd op objecten (Taken, Problemen, Goedkeuringen, Persoonlijke taken).
   >* Taken en kwesties worden verder gefilterd door hun staat in verhouding tot onze bereidheid om eraan te werken ([!UICONTROL Working On], [!UICONTROL Ready to Start], [!UICONTROL Not Ready] voor taken, en [!UICONTROL Working On] en [!UICONTROL Requested] voor problemen). U kunt selecteren om taken of problemen in een bepaalde status weer te geven of op Taken of Problemen klikken om alle frames te selecteren en weer te geven.
   >* Er is een afzonderlijk filter voor voltooide items en het bevat zowel taken als problemen. Hieronder vallen geen goedkeuringen. De [!UICONTROL Completed] omvat Persoonlijke taken.
   >* U kunt slechts één frame tegelijk selecteren. U kunt bijvoorbeeld alleen weergeven [!UICONTROL Working On] alleen taken en [!UICONTROL Requested] problemen.
   >* U kunt geen filters toepassen op items die zijn toegewezen aan een van uw teams en deze zijn niet opgenomen in de items die rechtstreeks aan u zijn toegewezen.


1. (Optioneel) De [!UICONTROL Work List], zoals beschreven in de sectie [Groeperen en sorteren op datum, project en prioriteit](#group-and-sort-by-date-project-and-priority) in dit artikel.

## Groep en sorteren op [!UICONTROL Date], [!UICONTROL Project], en [!UICONTROL Priority]

U kunt de [!UICONTROL Work List] door [!UICONTROL Planned Completion Date], [!UICONTROL Commit Date], [!UICONTROL Project], of [!UICONTROL My Priority]. De optie die u kiest, bepaalt hoe items worden gegroepeerd in het dialoogvenster [!UICONTROL Work List].

1. Klik op de knop **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) in de rechterbovenhoek klikt u op **[!UICONTROL Home]**.
1. Klik op de knop **[!UICONTROL Group by]** vervolgkeuzelijst.

   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)

1. Selecteer een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Planned Completion]</strong></td> 
      <td> <p> Items worden in de volgende groepen in het dialoogvenster [!UICONTROL Work List], afhankelijk van hun [!UICONTROL Planned Completion Date] (het aantal items in elke groep wordt tussen haakjes weergegeven naast de titel van de kop):</p> 
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
      <td> <p>Items worden in de volgende groepen in het dialoogvenster [!UICONTROL Work List], afhankelijk van hun [!UICONTROL Planned Start Date] (het aantal items in elke groep wordt tussen haakjes weergegeven naast de titel van de kop):</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL This Week] </p> <p>Deze groepering wordt standaard uitgebreid.</p> </li> 
        <li> <p>[!UICONTROL Next Week]</p> </li> 
        <li> <p>[!UICONTROL Planned], gevolgd door diverse [!UICONTROL Planned Start Dates] (meerdere groepen)</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Commit Date]</strong></td> 
      <td> <p>Items worden in de volgende groepen in het dialoogvenster [!UICONTROL Work List] (het aantal items in elke groep wordt tussen haakjes weergegeven naast de titel van de kop):</p> 
       <ul> 
        <li> <p>[!UICONTROL No Commit Date]</p> </li> 
        <li> <p>[!UICONTROL Committed Next Week]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Project]</strong></td> 
      <td>De punten worden gegroepeerd volgens project, en de projecten verschijnen alfabetisch in [!UICONTROL Work List]. (Het aantal items in elke groep wordt tussen haakjes weergegeven naast de titel van de kop.)</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL My Priority]</strong></td> 
      <td>De items worden in een door u gekozen volgorde weergegeven. Zie voor meer informatie <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">Prioriteit geven aan het werk in de [!UICONTROL Home] gebied</a>.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>De standaardsortering wordt oplopend uitgevoerd. Als u de sortering wijzigt in aflopend, worden de geselecteerde sorteeropties opgeslagen in de browser. Als u consequent dezelfde browser gebruikt op dezelfde computer (en de sitegegevens niet wist), verandert het sorteren niet, maar als u van browser of computer overschakelt, verandert het sorteren in de standaardsortering.

## Te late objecten weergeven

[!DNL Adobe Workfront] gebruikt de volgende data om te bepalen of de het werkverzoeken te laat zijn:

* **Taken**: [!UICONTROL Planned Completion Date]
* **Problemen**: [!UICONTROL Planned Completion Date]
* **Documenten**: [!UICONTROL Submitted date]
* **Timesheets**: [!UICONTROL Submitted date]
* **Goedkeuringen**: [!UICONTROL Submitted date]
* **Goedkeuringen van proefdrukken**: [!UICONTROL Proof deadline]

## Zoeken in de [!UICONTROL Work List]

Wanneer u de opdracht [!UICONTROL Work List], worden alle aan u toegewezen items geretourneerd in de zoekopdracht (zelfs items die momenteel niet op het scherm zijn geladen). Als de [!UICONTROL Show complete] als deze optie is geselecteerd, worden alle items die u de afgelopen twee weken hebt gemarkeerd als voltooid, ook geretourneerd.

Bovendien worden alleen de namen van de werkitems doorzocht (er wordt niet gezocht naar informatie binnen het werkitem en de namen van de projecten waarin het werkitem zich bevindt).

Als u de opdracht [!UICONTROL Work List]:

1. Klik op de knop **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) in de rechterbovenhoek klikt u op **[!UICONTROL Home]**.
1. (Optioneel) Filter het filter [!UICONTROL Work List], zoals beschreven in [Filteren op [!UICONTROL Work List]](#filter-the-work-list) en [Groeperen en sorteren op datum, project en prioriteit](#group-and-sort-by-date-project-and-priority).

1. (Optioneel) Als u een werkitem zoekt dat al is voltooid, moet u de [!UICONTROL Work List] om voltooide items weer te geven voordat u doorzoekt.
1. ![](assets/search-icon-highlighted-home-new-filters-and-sorting-nwe-350x238.png)

1. Typ de naam van het item waarnaar u zoekt.\
   De [!UICONTROL Work List] wordt automatisch gefilterd om items met een overeenkomende naam op te nemen.

## De grootte van de werklijst wijzigen

U kunt de grootte van de [!UICONTROL Work List] zodat het overal tussen ongeveer een kwart van het gebied van het Huis aan ongeveer de helft van [!UICONTROL Home] gebied.

1. Klik op de knop **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) in de rechterbovenhoek klikt u op **[!UICONTROL Home]**.
1. Plaats de muis boven de rechterrand van het dialoogvenster [!UICONTROL Work List]Sleep vervolgens naar links of rechts totdat de werklijst de gewenste grootte heeft.

## Groepen samenvouwen en uitbreiden

Items in het dialoogvenster [!UICONTROL Work List] worden weergegeven binnen groepen. U kunt groepen samenvouwen en uitvouwen om te bepalen hoeveel informatie op de pagina tegelijk wordt weergegeven.

U kunt groepen samenvouwen en uitvouwen in het dialoogvenster [!UICONTROL Work List] om beter te controleren welke informatie zichtbaar is.\
Standaard worden de [!UICONTROL This Week] groeperen wordt uitgebreid en alle andere groepen worden samengevouwen. Wijzigingen die u aanbrengt, worden onthouden wanneer u het gebied Home weer opent.

1. Klik op de knop **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) in de rechterbovenhoek klikt u op **[!UICONTROL Home]**.
1. Klik op de knop **[!UICONTROL Expand]** of **[!UICONTROL Collapse]** pijl naast een groep die u wilt uitvouwen of samenvouwen.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   of\
   Als u alle groepen tegelijk wilt uitvouwen of samenvouwen, klikt u op de knop **[!UICONTROL Expand]** of **[!UICONTROL Collapse]** de pijl naast om het even welke groepering terwijl onderdrukt [!UICONTROL Shift] toets.
