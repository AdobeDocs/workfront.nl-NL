---
navigation-topic: use-lists
title: Aan de slag met lijsten in [!DNL Adobe Workfront]
description: U kunt lijsten met objecten weergeven in [!DNL Adobe Workfront] om informatie over hen, zoals hun begin en vervaldata, gebruikers te krijgen die aan hen worden toegewezen, en andere voorwerpen die met hen worden geassocieerd.
feature: Get Started with Workfront
author: Lisa
exl-id: d4262b8e-bbe0-4ac2-8f1f-5d32541311c8
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1996'
ht-degree: 0%

---

# Aan de slag met lijsten in [!DNL Adobe Workfront]

<!--
{{highlighted-preview}}
-->

U kunt lijsten met objecten weergeven in [!DNL Adobe Workfront] om informatie over hen, zoals hun begin en vervaldata, gebruikers te krijgen die aan hen worden toegewezen, en andere voorwerpen die met hen worden geassocieerd.

Hier volgen enkele kenmerken van lijsten in [!DNL Workfront]:

* Lijsten verfrissen zich automatisch om de vijf minuten om informatie bij te werken die andere gebruikers in het systeem elders bijwerken.
* Sommige gebieden in [!DNL Workfront] vooraf geconfigureerd zijn met standaardlijsten met objecten.

  U kunt de meeste van deze vooraf geconfigureerde lijsten aanpassen.

* A [!DNL Workfront] de beheerder kan douanelijsten tot stand brengen om op diverse gebieden van toepassing te zijn [!DNL Workfront].

  Raadpleeg het artikel voor meer informatie over het maken van systeemlijsten [Standaardfilters, weergaven en groepen maken, bewerken en delen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>[!UICONTROL Request] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>[!UICONTROL View] of meer toegang tot filters, weergaven, groepen</p> <P>Voor items in het dialoogvenster [!UICONTROL Setup] gebied, hebt u administratieve toegang voor het punt of het [!UICONTROL System Administrator] toegangsniveau.</P> <p>Opmerking: als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen.<br>Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>[!UICONTROL View] of hogere machtigingen met toegang tot delen</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td>
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

## Objectlijsten

Hieronder vindt u een aantal objectlijsten die u kunt vinden in [!DNL Workfront] en sommige gebieden waar ze standaard worden weergegeven wanneer u rechten hebt om een object te bekijken.

>[!NOTE]
>
>* Deze lijst is niet uitgebreid. Elk van deze objecten lijsten kan ook op een rapport of een dashboard verschijnen. Bijvoorbeeld, toont een rapport van het Project of een dashboard dat een rapport van het Project bevat ook een lijst van projecten.
>* In deze lijst betekent &quot;selecteren&quot; dat u op de naam van het item moet klikken en niet op het selectievakje links van de naam.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!DNL Workfront] list</strong></th> 
   <th><strong>Locatie van objectlijst</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Lijst van portefeuilles</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfolios]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lijst van programma's</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL select a portfolio] &gt;[!UICONTROL Programs]</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>[!UICONTROL Programs]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lijst van projecten</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL select a portfolio] &gt;[!UICONTROL Projects]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL select a portfolio] &gt;[!UICONTROL Programs] &gt;[!UICONTROL select a program] &gt;[!UICONTROL Projects]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lijst met taken</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt; [!UICONTROL Tasks]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt;[!UICONTROL Subtasks]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt; [!UICONTROL Predecessors*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lijst met problemen</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL select] een project &gt;[!UICONTROL Issues]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt; [!UICONTROL Issues]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt;[!UICONTROL Subtasks] &gt;[!UICONTROL select a task] &gt; [!UICONTROL Issues]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lijst van verslagen</td> 
   <td> 
    <ul> 
     <li> <p>  [!UICONTROL Reports]  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lijst met dashboards</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Dashboards]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lijst met herhalingen</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Teams] &gt; [!UICONTROL Iterations]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lijst met gebruikers</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Users]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lijst van documenten</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL select a portfolio] &gt; [!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt; [!UICONTROL select a portfolio] &gt;[!UICONTROL Programs] &gt;[!UICONTROL select a program] &gt;[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt; [!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL select] een project &gt; [!UICONTROL Issues] &gt;[!UICONTROL select an issue] &gt; [!UICONTROL Documents]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lijst van tijdbladen</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Timesheet] s &gt; [!UICONTROL All Timesheets]*</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lijst van factureringssnelheden</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Billing Rates*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lijst met factureringsgegevens</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL select a project] &gt; [!UICONTROL Billing Records]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lijst van risico's</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Risks]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lijst van uitgaven</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select] een project &gt;[!UICONTROL Expenses]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt;[!UICONTROL Expenses]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lijst met uurwaarden</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select] een project</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt;[!UICONTROL Hours]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select] een project &gt;[!UICONTROL Issues] &gt;[!UICONTROL select] een uitgave &gt;[!UICONTROL Hours]</p> </li>
    </ul> </td> 
  </tr>
  <tr> 
   <td class="preview">Lijst met aangepaste formulieren</td> 
   <td> 
    <ul> 
     <li class="preview"> <p>[!UICONTROL Setup] &gt;[!UICONTROL Custom Forms]</p>
     <!--Remove the following note box when this goes to Production. Or do this when the Preview highlighting becomes available.-->
     <p><b>OPMERKING</b>: Deze optie is momenteel alleen beschikbaar in de voorvertoningsomgeving</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>Lijst van groepen of subgroepen</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Groups]</p> </li>
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Groups] &gt;[!UICONTROL select the parent group] &gt;[!UICONTROL Subgroups] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lijst van teams</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Teams]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Lijst van ondernemingen</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Companies]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Lijst van dienstregelingen</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Schedules]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Lijst met lay-outsjablonen</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Layout Templates]</p> </li> 
    </ul> </td> 
  </tr>
 </tbody> 
</table>

U kunt de lijst in het opgegeven gebied niet aanpassen. A [!DNL Workfront] de beheerder kan een aangepaste lijst op het systeemniveau bouwen, of u kunt een rapport voor dit voorwerp bouwen als uw toegangsniveau u toegang toestaat om rapporten uit te geven.

## Lijstelementen

Een lijst bevat bepaalde elementen die zijn formaat en de informatie bepalen die toont. U kunt verschillende elementen van de systeemlijst vinden die standaard beschikbaar zijn. U kunt ook aangepaste elementen maken die aan uw behoeften voldoen.

>[!NOTE]
>
>Wanneer u een nieuw filter, een nieuwe weergave of een nieuwe groep in een lijst selecteert, blijft die selectie behouden, ook als u zich afmeldt bij [!DNL Workfront] of sluit uw browser.

Hieronder vindt u de elementen van een lijst:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Element</strong></th> 
   <th><strong>Toelichting</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL Filter]</strong></td> 
   <td> <p>De filters houden onnodige informatie uit een lijst, die op de criteria wordt gebaseerd die u specificeert. </p> <p>Zie voor meer informatie <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Overzicht van filters</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL View]</strong></td> 
   <td> <p>Weergaven definiëren welke velden (kolommen) u op het scherm weergeeft.</p> <p>Zie voor meer informatie <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Overzicht van weergaven in [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Grouping]</strong></td> 
   <td> <p>Groepen scheiden de objecten in de lijst in gebieden op basis van de criteria die u opgeeft.</p> <p>De problemen in een lijst kunnen bijvoorbeeld in secties worden weergegeven op basis van status of prioriteit.</p> <p>U kunt maximaal drie lagen groepering in een standaardgroepering hebben, en u kunt een vierde laag toevoegen als u een groepering op tekstwijze vormt.</p> <p>Zie voor meer informatie over groepen <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Overzicht van groepen in [!DNL Adobe Workfront]</a>.</p> <p>Zie voor meer informatie over de tekstmodus <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">Overzicht van de tekstmodus</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Deze elementen worden standaard boven aan elke lijst weergegeven. Ze zijn vast en bewegen niet als u door de lijst schuift. Plaats de muis boven het pictogram voor elk element om het te identificeren.

![](assets/nwe-list-elements.png)

U kunt lijstelementen in de volgende gebieden aanpassen en hen met andere gebruikers delen:

* Elke standaardsysteemlijst gevonden in de sectie [Aan de slag met lijsten in [!DNL Adobe Workfront]](#default-workfront-lists) in dit artikel
* Elk rapport dat met u wordt gedeeld

De bouwelementen voor lijsten zijn het zelfde als de bouwstenen voor rapporten.

Voor meer informatie over het creëren van en het aanpassen van de bouwelementen van lijsten en rapporten, zie [Elementen rapporteren: filters, weergaven en groepen](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Handelingen weergeven

U kunt de volgende handelingen in een lijst uitvoeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Handeling</strong></th> 
   <th><strong>Informatie</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Inline bewerken</strong> </td> 
   <td> <p>Objecten en hun gegevens rechtstreeks in de lijst bewerken.</p> <p>Zie voor meer informatie <a href="../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md" class="MCXref xref">Items inline bewerken in een lijst in [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><strong>Bijwerken met de [!UICONTROL Summary]</strong> </td> 
   <td> <p>Werk taken en kwesties op projectniveau bij gebruikend [!UICONTROL Summary] deelvenster.</p> <p>Tip: de samenvatting is niet beschikbaar voor alle objecten en is niet beschikbaar in taak- of Issue-rapporten.</p> <p>Zie voor meer informatie <a href="../../../workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Overzicht van samenvattingen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>De lijstweergave aanpassen</strong> </td> 
   <td> <p>Pas de vormgeving van een lijst, kolomindeling, sorteervolgorde van items of het aantal items dat wordt weergegeven aan.</p> <p>Opmerking: wijzigingen die u aanbrengt in het aantal items dat op een pagina wordt weergegeven, worden teruggezet wanneer u zich afmeldt bij [!DNL Workfront] of sluit uw browser. Wijzigingen kunnen ook na een periode van 8 uur worden teruggedraaid.</p> <p>Zie voor meer informatie <a href="../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md" class="MCXref xref">De weergave van een lijst wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Snel filter</strong> </td> 
   <td> <p>Pas een snel filter toe om alleen items te zoeken die voor u van belang zijn, zodat u deze snel kunt bekijken, bijwerken of met anderen kunt delen.</p> <p>Belangrijk: u kunt items zoeken die een zoekwoord bevatten met behulp van het snelfilter. Hiermee kunt u zien of dat item zichtbaar is op het scherm of dat het wordt weergegeven nadat u naar de onderkant van de pagina hebt geschoven. Wanneer u de zoekmogelijkheden van uw browser gebruikt, kunt u alleen items vinden die al op het scherm zichtbaar zijn. Als uw lijst meerdere pagina's bevat, worden met snelfilters alleen de items op de huidige pagina gevonden.</p> <p>Zie voor meer informatie <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Het snelle filter toepassen op een lijst</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Exporteren</strong> </td> 
   <td> <p>Een lijst met objecten exporteren uit [!DNL Workfront]. Als een lijst meer dan 2000 items bevat, is het exporteren van de lijst de enige manier om alle items op één pagina te bekijken.</p> <p>Zie voor meer informatie over het exporteren van een lijst <a href="../../../workfront-basics/navigate-workfront/use-lists/export-lists.md" class="MCXref xref">Een lijst exporteren</a>. Voor meer informatie over exportindelingen en -beperkingen raadpleegt u <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Gegevens exporteren</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Lijst, werkbalk

In de volgende tabel staan veel van de pictogrammen die beschikbaar zijn op de werkbalk en wordt aangegeven wat er gebeurt wanneer u erop klikt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Pictogram</strong></td> 
   <td><strong>Beschrijving</strong></td> 
   <td><strong>Bij klikken</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/add-icon-plus-in-circle.png"> </td> 
   <td>[!UICONTROL Add item or user]</td> 
   <td>Open meer opties, zoals het toevoegen van een nieuw item of een nieuwe gebruiker.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-above-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Insert task above]</td> 
   <td> <p>Voeg een taak in boven de geselecteerde taak.</p> <p>Dit is alleen beschikbaar voor taken. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-below-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Insert task below]</td> 
   <td> <p>Voeg een taak in onder de geselecteerde taak.</p> <p>Dit is alleen beschikbaar voor taken. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/edit-icon.png"> </td> 
   <td>[!UICONTROL Edit]</td> 
   <td>Het geselecteerde item bewerken.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/copy-icon.png"> </td> 
   <td>[!UICONTROL Copy]</td> 
   <td>Kopieer het geselecteerde item.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/delete.png"> </td> 
   <td>[!UICONTROL Delete]</td> 
   <td>Verwijder het geselecteerde item.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-add-to-iteration-icon-in-new-toolbar-for-issues.png"> </td> 
   <td>[!UICONTROL Add to]</td> 
   <td> <p>Open het dialoogvenster om de geselecteerde uitgave aan een herhaling toe te voegen.</p> <p>Dit is alleen beschikbaar voor problemen.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/share-icon.png"> </td> 
   <td>[!UICONTROL Share]</td> 
   <td>Deel het geselecteerde item.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-indent-outdent-tasks-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Indent and outdent tasks] </td> 
   <td> <p>De geselecteerde taak laten inspringen of uitspringen. </p> <p>Dit is alleen beschikbaar voor taken. </p> </td> 
  </tr> 
  <tr> 
   <td><img src="assets/more-icon.png"></a> </td> 
   <td>[!UICONTROL More]</td> 
   <td>Open aanvullende opties voor het geselecteerde item.</td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/search-icon.png"> </p> </td> 
   <td> <p>[!UICONTROL Quick filter] </p> </td> 
   <td> <p>Open het snelle vakje van de filteronderzoek voor het vinden van punten in de getoonde lijst.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/export.png"> </td> 
   <td>[!UICONTROL Export]</td> 
   <td>Exporteer de lijst naar PDF-, Excel- of tabgescheiden bestanden.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-agile-icon-in-new-toolbar-task-list.png"> </td> 
   <td>[!UICONTROL Agile View]</td> 
   <td>Geef de lijst weer in de weergave Gelijk.<br>Dit is alleen beschikbaar voor taken.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-gantt-chart-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Gantt Chart]</td> 
   <td> <p>De lijst weergeven in het dialoogvenster [!UICONTROL Gantt Chart] weergeven.</p> <p>Dit is alleen beschikbaar voor projecten en taken.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-filter-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-filter-in-new-toolbar-with-blue-dot---small.png"> </p> </td> 
   <td>[!UICONTROL Filter] vervolgkeuzemenu</td> 
   <td> <p>Geef een lijst weer met filters en extra opties voor het beheer van filters, waaronder het maken van filters. </p> <p>Op een klein scherm wordt de naam van het filter vervangen door het filterpictogram. Er wordt een blauwe stip weergegeven op het pictogram Filter wanneer u een ander filter dan "[!UICONTROL All]."</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-view-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-view-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>[!UICONTROL View] vervolgkeuzemenu</td> 
   <td> <p>Geef een lijst weer met weergaven en extra opties voor het beheren van weergaven, waaronder het maken van weergaven. </p> <p>Op een klein scherm wordt de naam van de Mening vervangen door [!UICONTROL view] pictogram. Er wordt een blauwe stip weergegeven op het tabblad [!UICONTROL View] pictogram wanneer u een andere weergave dan "[!UICONTROL Standard]."</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-grouping-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-grouping-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>[!UICONTROL Grouping] vervolgkeuzemenu</td> 
   <td> <p>Geef een lijst weer met groepen en extra opties voor het beheer van groepen, waaronder het maken van groepen. </p> <p>Op een klein scherm wordt de naam van de Groepering vervangen door [!UICONTROL grouping] pictogram. Er wordt een blauwe stip weergegeven op het tabblad [!UICONTROL Grouping] pictogram wanneer u een andere groepering toepast dan "[!UICONTROL Nothing]."</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-autosave-icon-in-new-toolbar-for-tasks.png"> </td> 
   <td> <p>[!UICONTROL Plan mode]</p> </td> 
   <td> <p>Kies of u de wijzigingen die u in een takenlijst aanbrengt, automatisch of handmatig wilt opslaan. </p> <p>Voor informatie over het bewerken van taken in een lijst raadpleegt u <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Taken in een lijst bewerken</a>. </p> <p>Dit is alleen beschikbaar voor taken.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/summary-panel-icon.png"> </td> 
   <td>[!UICONTROL Summary]</td> 
   <td> <p>De opdracht weergeven of verbergen [!UICONTROL Summary] voor het geselecteerde item.</p> <p>Dit is alleen beschikbaar voor taken en problemen.</p> <p>Voor informatie over de [!UICONTROL Summary] in het nieuwe [!DNL Adobe Workfront] ervaring, zie <a href="/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Overzicht van samenvattingen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/remove-icon---x-in-circle.png"> </td> 
   <td>[!UICONTROL Remove]</td> 
   <td>Verwijder iets uit de lijst. Als een groepsbeheerder bijvoorbeeld groepslidmaatschappen of subgroepslidmaatschappen beheert, verwijdert u een groepslid zoals uitgelegd in <a href="/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md" class="MCXref xref">De groepslidmaatschappen weergeven en beheren</a>.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/comment-icon.png"> </td> 
   <td>[!UICONTROL Comment] /[!UICONTROL Update]</td> 
   <td> <p>Typ een opmerking of update.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Het verschil tussen lijsten en rapporten

Zowel lijsten als rapporten zijn rasters die informatie over een type object bevatten.

In de volgende tabel worden de overeenkomsten en verschillen tussen lijsten en rapporten beschreven:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Functionaliteit</strong> </th> 
   <th><strong>Lijst</strong> </th> 
   <th><strong>Rapport</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Iedereen kan ze maken</p> </td> 
   <td><span>✓*</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Alleen een [!DNL Workfront] beheerder en gebruikers met een [!UICONTROL Plan] licentie kan ze maken</p> </td> 
   <td> </td> 
   <td>✓**</td> 
  </tr> 
  <tr> 
   <td> <p>Een standaardset is beschikbaar via [!DNL Workfront]</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Aanpasbaar in de standaardmodus</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Aanpasbaar in tekstmodus</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>U kunt deze delen met andere gebruikers</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>U kunt ze op het hele systeem delen</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>U kunt ze buiten het systeem delen</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>U kunt exporteren naar .pdf, [!DNL Excel]en Door tabs gescheiden indelingen</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>U kunt ze plannen voor levering in een e-mail</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>U kunt een lay-outsjabloon toevoegen</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>U kunt ze toevoegen aan aangepaste secties </p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>U kunt ze toevoegen aan een dashboard</p> </td> 
   <td> ✓** </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>U kunt herinneringen gebruiken om aan te passen wat zij tonen</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>U kunt ze in een grafiek weergeven</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>U kunt objecten daarin inline bewerken</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

U moet toegang hebben tot filters, weergaven en groepen om deze te kunnen maken. Zie voor meer informatie [Toegang verlenen tot filters, weergaven en groepen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

U moet toegang hebben tot filters, weergaven en groepen, maar ook tot rapporten, dashboards en kalenders om deze te kunnen maken. Zie voor meer informatie [Toegang verlenen tot rapporten, dashboards en kalenders](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

U kunt lijsten voor rapporten aanpassen die op een dashboard worden geplaatst slechts als de schepper van het rapport de lijstelementen heeft gevormd om op het dashboard zichtbaar te zijn.

>[!NOTE]
>
>U kunt geen lijst aan een dashboard toevoegen zonder eerst een rapport te creëren en het toe te voegen aan het dashboard.

Ga voor meer informatie over het samenstellen van een rapport naar [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Zie voor informatie over het maken van aangepaste secties [Aangepaste tabbladen of secties maken](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

## Het verschil tussen de bijgewerkte en de oudere lijsten

Er zijn twee soorten lijsten in [!DNL Workfront]:

* Oudere lijsten

  ![](assets/legacy-list-screen-shot-blue-groupings-350x101.png)

* Bijgewerkte lijsten

  ![](assets/updated-list-screen-shot-gray-groupings-350x71.png)

Beide typen lijsten worden weergegeven in het dialoogvenster [!DNL Adobe Workfront].

Alle lijsten en rapporten in het dialoogvenster [!DNL Adobe Workfront] zijn bijgewerkte lijsten, met uitzondering van:

* Lijsten in het dialoogvenster [!UICONTROL Setup] gebied
* Lijsten in het dialoogvenster [!UICONTROL Reports] gebied

In de volgende tabel ziet u enkele verschillen tussen de verouderde en bijgewerkte lijsten in [!DNL Workfront]:

<!--
<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> [Legacy does not equal Classic. Legacy lists appear in NWE and Classic. Updated lists appear in NWE and Classic.]</span>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Oudere lijsten</b></td> 
   <td><b>Bijgewerkte lijsten</b></td> 
  </tr> 
  <tr> 
   <td> <p>Oudere lettertypen, kolomkoppen, kleurenschema voor blauwe groepering</p> </td> 
   <td> <p>Bijgewerkte lettertypen, kolomkoppen, kleurschema voor grijstinten</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Langzamere inline bewerking</p> </td> 
   <td> <p>Sneller inline bewerken</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Weergave <strong>100</strong> standaard items</p> </td> 
   <td> <p>Weergave <strong>Alles</strong> of tot <strong>2000</strong> standaard items</p> </td> 
  </tr> 
  <tr> 
   <td> <p>CTRL+F gebruiken om items in een lijst te zoeken</p> </td> 
   <td> <p>Gebruik snelle filters om snel informatie in een grote lijst te zoeken</p> <p>Voor informatie over het gebruik van snelle filters in lijsten raadpleegt u <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Het snelle filter toepassen op een lijst</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>U kunt aangepaste velden met tekstopmaak niet inline bewerken.</td> 
   <td> <p>Tekst in aangepaste velden met opmaak kan worden geconfigureerd om vette, cursieve, onderstreepte, opsommingstekens, nummering, hyperlinks en blokaanhalingstekens toe te staan.</p> <p>Zie voor meer informatie <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Een aangepast formulier maken of bewerken</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Met voorwaardelijke opmaak kunt u de tekstkleur van koppelingen in een lijst wijzigen</td> 
   <td>Kan tekstkleurwijzigingen niet toepassen op koppelingen in een lijst</td> 
  </tr> 
 </tbody> 
</table>
