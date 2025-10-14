---
navigation-topic: use-lists
title: Het snelle filter toepassen op een lijst
description: U kunt het snelle filter in een lijst van voorwerpen gebruiken om u van slechts punten te helpen de plaats bepalen die voor u belangrijk zijn, zodat kunt u hen snel herzien, bijwerken, of delen met anderen.
feature: Get Started with Workfront
author: Nolan
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 0a2ff1ab802b2bd08cd680376321552a8018cb74
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# Het snelle filter toepassen op een lijst

<!--Audited:11/2024-->

U kunt het snelle filter in een lijst van voorwerpen gebruiken om u van slechts punten te helpen de plaats bepalen die voor u belangrijk zijn, zodat kunt u hen snel herzien, bijwerken, of delen met anderen.

>[!IMPORTANT]
>
>U kunt met behulp van snelle filters zoeken naar items die een zoekwoord bevatten. Of dat item nu fysiek op het scherm is weergegeven of dat item wordt weergegeven nadat u naar de onderkant van de pagina hebt geschoven. Wanneer u de zoekmogelijkheden van uw browser gebruikt, kunt u alleen zoeken naar items die fysiek op het scherm worden weergegeven. Als uw lijst meerdere pagina&#39;s bevat, worden met snelfilters geen items gevonden die zich op pagina&#39;s bevinden die niet worden weergegeven.

Als u een snel filter wilt opslaan, raden we u aan een permanent filter voor uw lijst te maken.\
Voor informatie over hoe te om filters in [!DNL Adobe Workfront] te bouwen, zie het overzicht van artikel [&#x200B; Filters &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Het snelfilter is momenteel beschikbaar in de volgende gebieden


U kunt tijdelijke snelle filters in alle lijsten gebruiken, behalve het volgende:

* Het [!UICONTROL Reports] -gebied
* Documentlijsten en -rapporten
* Meerdere [!UICONTROL Setup] gebieden

  >[!NOTE]
  >
  >Snelle filters zijn beschikbaar in de volgende instellingsgebieden: [!UICONTROL Groups], [!UICONTROL Teams], [!UICONTROL Companies], [!UICONTROL Schedules], [!UICONTROL Layout Templates] en [!UICONTROL Custom Forms] .


Houd rekening met het volgende wanneer u snelle filters toepast op een lijst:

* Met trefwoorden kunt u filteren op elk veld dat in de weergave van de lijst wordt weergegeven. Dit omvat aangepaste velden of complexe velden zoals [!UICONTROL Predecessors] , [!UICONTROL Assignments] , [!UICONTROL Assignment] en [!UICONTROL Status] , [!UICONTROL Approver] en [!UICONTROL Status] , enzovoort.
* Als uw lijst samengevouwen groeperingen heeft, worden zij automatisch uitgebreid wanneer u snelle filters gebruikt. Wanneer u het snelle filter verwijdert, worden groepen weer samengevouwen.
* Groepen behouden de geaggregeerde informatie van de oorspronkelijke lijst, ongeacht de toegepaste snelfilters of wijzigingen die zijn aangebracht in de objecten in de lijst.
* Snelle filters zijn tijdelijk. Als u de groep, weergave, filter of sortering van de lijst wijzigt, worden de snelle filtercriteria verwijderd.
* U kunt een snelfilter niet opslaan. Als u een filter wilt opslaan om het opnieuw te gebruiken, kunt u overwegen een permanent filter voor de lijst te maken.
* Als de lijst meerdere groepen bevat en het filter Snel items in slechts één groep vindt, wordt alleen die groep weergegeven met de gevonden items. Alle andere groepen zijn verborgen.
* In een taak of subtakenlijst wordt de taakhiërarchie verwijderd wanneer de resultaten van de snelle filterweergave.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> 
    <p>Nieuw:</p>
   <ul><li><p>Medewerker of hoger </p></li>
   </ul>

<p>Huidige:</p>
   <ul><li><p>Aanvraag of hoger</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang weergeven tot het gebied in de lijst</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>[!UICONTROL View] machtigingen voor het object in de lijst</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Een snel filter toepassen op een lijst

1. Ga naar een lijst of een rapport dat snelle filters steunt, dan klik het **[!UICONTROL Quick Filter]pictogram** ![&#x200B; Snelle filterpictogram &#x200B;](assets/qs-quick-filter-icon.png) in de toolbar.

   of

   Afhankelijk van uw besturingssysteem of browser en wanneer u een standaard QWERTY-toetsenbord gebruikt, drukt u op de volgende set opdrachten om het snelfilter te starten:

   * ALT+F voor [!DNL Windows] computers
   * ALT/Option+F voor [!DNL Mac] computers

     >[!TIP]
     >
     >Als u op CTRL+F of CMD+F drukt, verschijnt knopinfo naast het snelle filter om u aan deze opdrachten te herinneren. De opdrachten worden ook weergegeven in het zoekvak Snel filter.

1. Voer in het vak **[!UICONTROL Filter page]** het trefwoord in waarop u wilt filteren.

   U kunt elk woord gebruiken dat momenteel wordt weergegeven in de weergave van de lijst.

   >[!NOTE]
   >
   >Als u een woord gebruikt dat op een andere pagina van de lijst zou kunnen tonen, vindt de snelle filter geen resultaten.

   Een lijst met items die voldoen aan de zoekcriteria wordt dynamisch weergegeven in de lijst terwijl u typt en alle andere items worden verborgen. Het trefwoord dat u in de zoekopdracht hebt gebruikt, wordt in alle zelfstandige en complexe velden geel gemarkeerd. Enkele voorbeelden van complexe velden zijn gedeelde kolommen of een van de volgende: [!UICONTROL Assignments] , [!UICONTROL Assignments] en [!UICONTROL Status] , [!UICONTROL Percent Complete] , [!UICONTROL Predecessors] , [!UICONTROL Approvers and Status] , [!UICONTROL Resource Managers] , [!UICONTROL Categories] , [!UICONTROL Condition] , [!UICONTROL Condition Update] , enz.

1. (Optioneel) Als u de items die door het snelfilter worden gevonden, bulksgewijs wilt bewerken:

   1. Selecteer alle of meerdere items in de lijst en klik op **[!UICONTROL Edit]** om de items in bulk te bewerken.
   1. Klik op **[!UICONTROL Save Changes]** nadat u de bewerkingen hebt voltooid.

1. (Facultatief) om de punten uit te voeren die door de snelle filter worden gevonden, selecteer allen of verscheidene punten in de lijst, dan klik het **[!UICONTROL Export]** pictogram ![&#x200B; pictogram van de Uitvoer &#x200B;](assets/export.png).

   ![&#x200B; select_all_projects_with_highlight__1_.png &#x200B;](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >Alleen de items die u hebt gevonden in de zoekopdracht met snel filter worden geëxporteerd naar het bestand dat u hebt geselecteerd. Als u geen items selecteert voordat u de lijst exporteert, wordt de volledige, ongefilterde lijst geëxporteerd.\
   >Voor meer informatie, zie [&#x200B; Uitvoer een lijst &#x200B;](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md).

1. (Optioneel) Als u de gefilterde resultaten wilt wissen, klikt u op het pictogram **[!UICONTROL Quick Filter]** in de rechterbovenhoek van het venster.
of
Vernieuw de pagina.
