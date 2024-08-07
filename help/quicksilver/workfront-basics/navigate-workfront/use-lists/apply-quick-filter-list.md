---
navigation-topic: use-lists
title: Het snelle filter toepassen op een lijst
description: U kunt het snelle filter in een lijst van voorwerpen gebruiken om u van slechts punten te helpen de plaats bepalen die voor u belangrijk zijn, zodat kunt u hen snel herzien, bijwerken, of delen met anderen.
feature: Get Started with Workfront
author: Lisa
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 0%

---

# Het snelle filter toepassen op een lijst

<!--
{{highlighted-preview}}
-->

U kunt het snelle filter in een lijst van voorwerpen gebruiken om u van slechts punten te helpen de plaats bepalen die voor u belangrijk zijn, zodat kunt u hen snel herzien, bijwerken, of delen met anderen.

>[!IMPORTANT]
>
>U kunt met behulp van snelle filters zoeken naar items die een zoekwoord bevatten. Of dat item nu fysiek op het scherm is weergegeven of dat item wordt weergegeven nadat u naar de onderkant van de pagina hebt geschoven. Wanneer u de zoekmogelijkheden van uw browser gebruikt, kunt u alleen zoeken naar items die fysiek op het scherm worden weergegeven. Als uw lijst meerdere pagina&#39;s bevat, worden met snelfilters geen items gevonden die zich op pagina&#39;s bevinden die niet worden weergegeven.

Als u een snel filter wilt opslaan, raden we u aan een permanent filter voor uw lijst te maken.\
Voor informatie over hoe te om filters in [!DNL Adobe Workfront] te bouwen, zie het overzicht van artikel [ Filters ](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

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

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] plan*</b></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] licentie*</b></td> 
   <td> <p>[!UICONTROL Request] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>Configuraties op toegangsniveau*</b></td> 
   <td> <p>Toegang weergeven tot het gebied in de lijst</p> <p>Als u bijvoorbeeld een snel filter wilt toepassen op een project, hebt u [!UICONTROL View] toegang tot projecten nodig.</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de [!DNL Workfront] -beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld.<br> voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>Objectmachtigingen</b></td> 
   <td> <p>[!UICONTROL View]</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## Een snel filter toepassen op een lijst

1. Ga naar een lijst of een rapport dat snelle filters steunt, dan klik het **[!UICONTROL Quick Filter]pictogram** ![](assets/qs-quick-filter-icon.png) in de toolbar.

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

1. (Optioneel) Als u de items die door het snelfilter worden gevonden, wilt exporteren, selecteert u alle of meerdere items in de lijst en klikt u op **[!UICONTROL Export]** .

   ![ select_all_projects_with_highlight__1_.png ](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >Alleen de items die u hebt gevonden in de zoekopdracht met snel filter worden geëxporteerd naar het bestand dat u hebt geselecteerd. Als u geen items selecteert voordat u de lijst exporteert, wordt de volledige, ongefilterde lijst geëxporteerd.\
   >Voor meer informatie, zie [ Uitvoer een lijst ](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md).

1. (Optioneel) Als u de gefilterde resultaten wilt wissen, klikt u op het pictogram **[!UICONTROL Quick Filter]** in de rechterbovenhoek van het venster.\
   of\
   Vernieuw de pagina.
