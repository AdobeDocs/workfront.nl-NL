---
navigation-topic: use-lists
title: Aan de slag met lijsten in  [!DNL Adobe Workfront]
description: U kunt lijsten van voorwerpen in  [!DNL Adobe Workfront]  bekijken om informatie over hen, zoals hun begin en vervaldata, gebruikers te krijgen die aan hen, en andere voorwerpen worden toegewezen die met hen worden geassocieerd.
feature: Get Started with Workfront
author: Nolan
exl-id: d4262b8e-bbe0-4ac2-8f1f-5d32541311c8
source-git-commit: 0a2ff1ab802b2bd08cd680376321552a8018cb74
workflow-type: tm+mt
source-wordcount: '1902'
ht-degree: 0%

---

# Aan de slag met lijsten in [!DNL Adobe Workfront]

<!--Audited: 11/2024-->

U kunt lijsten met objecten weergeven in [!DNL Adobe Workfront] voor meer informatie over deze objecten, zoals de begin- en vervaldatum, de gebruikers die eraan zijn toegewezen en andere objecten die eraan zijn gekoppeld.

Hier volgen enkele kenmerken van lijsten in [!DNL Workfront] :

* Lijsten verfrissen zich automatisch om de vijf minuten om informatie bij te werken die andere gebruikers in het systeem elders bijwerken.
* Sommige gebieden in [!DNL Workfront] zijn vooraf geconfigureerd met standaardlijsten met objecten.

  U kunt de meeste van deze vooraf geconfigureerde lijsten aanpassen.

* Een [!DNL Workfront] -beheerder kan aangepaste lijsten maken die op verschillende gebieden van [!DNL Workfront] worden toegepast.

  Voor meer informatie over het creëren van systeem-vlakke lijsten, zie het artikel [&#x200B; creëren, uitgeven, en delen standaardfilters, meningen, en groeperingen &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

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
   <td> <p>Toegang tot filters, weergaven, groepen bewerken </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven of hoger voor een filter, weergave of groep met toegang tot delen </p>  </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old access: 

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Request] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>[!UICONTROL View] or higher access to filters, views, groupings</p> <P>For items in the [!UICONTROL Setup] area, you need administrative access for the item or the [!UICONTROL System Administrator] access level.</P> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level.<br>For information on how a [!DNL Workfront] administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>[!UICONTROL View] or higher permissions with access to share</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.
-->

## Objectlijsten

Hieronder vindt u een aantal objectlijsten die u kunt vinden in [!DNL Workfront] en een aantal gebieden waarin deze standaard worden weergegeven wanneer u rechten hebt om een object te bekijken.

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
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL select] een project &gt;[!UICONTROL Issues]</p> </li> 
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
     <li> <p>[!UICONTROL Portfolios] &gt; [!UICONTROL select a portfolio] &gt; [!UICONTROL Programs] &gt; [!UICONTROL select a program] &gt;[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt; [!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL select] een project &gt; [!UICONTROL Issues] &gt; [!UICONTROL select an issue] &gt; [!UICONTROL Documents]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lijst van tijdbladen</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Timesheet] s &gt; [!UICONTROL All Timesheets]*</p> </li> 
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
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL select a project] &gt; [!UICONTROL Billing Records]</p> </li> 
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
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL select a project] &gt; [!UICONTROL Tasks] &gt; [!UICONTROL select a task] &gt;[!UICONTROL Expenses]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lijst met uurwaarden</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select] een project</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt;[!UICONTROL Hours]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL select] een project &gt; [!UICONTROL Issues] &gt; [!UICONTROL select] een kwestie &gt;[!UICONTROL Hours]</p> </li>
    </ul> </td> 
  </tr>
  <tr> 
   <td>Lijst met aangepaste formulieren</td> 
   <td> 
    <ul> 
     <li>[!UICONTROL Setup] &gt;[!UICONTROL Custom Forms] </li> 
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

U kunt de lijst in het opgegeven gebied niet aanpassen. Een [!DNL Workfront] beheerder kan een aangepaste lijst op systeemniveau bouwen, of u kunt een rapport voor dit voorwerp bouwen als uw toegangsniveau u toegang toestaat om rapporten uit te geven.

## Lijstelementen

Een lijst bevat bepaalde elementen die zijn formaat en de informatie bepalen die toont. U kunt verschillende elementen van de systeemlijst vinden die standaard beschikbaar zijn. U kunt ook aangepaste elementen maken die aan uw behoeften voldoen.

>[!NOTE]
>
>Wanneer u een nieuw filter, een nieuwe weergave of een nieuwe groep in een lijst selecteert, blijft die selectie behouden, zelfs als u zich afmeldt bij [!DNL Workfront] of de browser sluit.

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
   <td> <p>De filters houden onnodige informatie uit een lijst, die op de criteria wordt gebaseerd die u specificeert. </p> <p>Voor meer informatie, zie <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref"> Overzicht van Filters </a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL View]</strong></td> 
   <td> <p>Weergaven definiëren welke velden (kolommen) u op het scherm weergeeft.</p> <p>Zie <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref"> Overzicht van weergaven in [!DNL Adobe Workfront]</a> voor meer informatie.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Grouping]</strong></td> 
   <td> <p>Groepen scheiden de objecten in de lijst in gebieden op basis van de criteria die u opgeeft.</p> <p>De problemen in een lijst kunnen bijvoorbeeld in secties worden weergegeven op basis van status of prioriteit.</p> <p>U kunt maximaal drie lagen groepering in een standaardgroepering hebben, en u kunt een vierde laag toevoegen als u een groepering op tekstwijze vormt.</p> <p>Voor meer informatie over groeperingen, zie <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref"> Overzicht van Groepen in [!DNL Adobe Workfront]</a>.</p> <p>Voor meer informatie over tekstwijze, zie <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref"> Overzicht van de Wijze van de Tekst </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Deze elementen worden standaard boven aan elke lijst weergegeven. Ze zijn vast en bewegen niet als u door de lijst schuift. Plaats de muis boven het pictogram voor elk element om het te identificeren.

![&#x200B; de elementen van de Lijst &#x200B;](assets/nwe-list-elements.png)

U kunt lijstelementen in de volgende gebieden aanpassen en hen met andere gebruikers delen:

* Om het even welk systeem standaardlijst die in de sectie [&#x200B; wordt gevonden wordt begonnen met lijsten in  [!DNL Adobe Workfront]](#default-workfront-lists) in dit artikel
* Elk rapport dat met u wordt gedeeld

De bouwelementen voor lijsten zijn het zelfde als de bouwstenen voor rapporten.

Voor meer informatie over het creëren van en het aanpassen van de bouwselementen van lijsten en rapporten, zie [&#x200B; Meldend elementen: filters, meningen, en groeperingen &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

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
   <td><strong> Inline geeft uit </strong> </td> 
   <td> <p>Objecten en hun gegevens rechtstreeks in de lijst bewerken.</p> <p>Voor meer informatie, zie <a href="../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md" class="MCXref xref"> gealigneerde geef punten in een lijst in [!DNL Adobe Workfront]</a> uit.</p> 
   <p><b>OPMERKING:</b></p>
   <p>Inline bewerken is niet mogelijk in een groep.</p>

</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><strong> Update met [!UICONTROL Summary]</strong> </td> 
   <td> <p>Werk taken en problemen op projectniveau bij met het deelvenster [!UICONTROL Summary] .</p> <p><b>TIP:</b></p> <p>De samenvatting is niet beschikbaar voor alle objecten en is niet beschikbaar in taak- of Issue-rapporten.</p> <p>Voor meer informatie, zie <a href="../../../workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref"> Overzicht van de Samenvatting </a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong> pas lijstvertoning </strong> aan </td> 
   <td> <p>Pas de vormgeving van een lijst, kolomindeling, sorteervolgorde van items of het aantal items dat wordt weergegeven aan.</p> <p><b>OPMERKING:</b></p> <p>Wijzigingen die u aanbrengt in het aantal items dat op een pagina wordt weergegeven, worden ongedaan gemaakt wanneer u zich afmeldt bij [!DNL Workfront] of de browser sluit. Wijzigingen kunnen ook na een periode van 8 uur worden teruggedraaid.</p> <p>Voor meer informatie, zie <a href="../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md" class="MCXref xref"> wijzigen zich hoe een lijstvertoningen </a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong> Snelle filter </strong> </td> 
   <td> <p>Pas een snel filter toe om alleen items te zoeken die voor u van belang zijn, zodat u deze snel kunt bekijken, bijwerken of met anderen kunt delen.</p> <p><b>BELANGRIJK:</b></p> <p> U kunt zoeken naar items die een zoekwoord bevatten met behulp van het snelfilter, of dat item zichtbaar is op het scherm of wordt weergegeven nadat u naar de onderkant van de pagina hebt geschoven. Wanneer u de zoekmogelijkheden van uw browser gebruikt, kunt u alleen items vinden die al op het scherm zichtbaar zijn. Als uw lijst meerdere pagina's bevat, worden met snelfilters alleen de items op de huidige pagina gevonden.</p> <p>Voor meer informatie, zie <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref"> de snelle filter op een lijst </a> toepassen.</p> </td> 
  </tr> 
  <tr> 
   <td><strong> Uitvoer </strong> </td> 
   <td> <p>Een lijst met objecten exporteren uit [!DNL Workfront] . Als een lijst meer dan 2000 items bevat, is het exporteren van de lijst de enige manier om alle items op één pagina te bekijken.</p> <p>Voor meer informatie over het uitvoeren van een lijst, zie <a href="../../../workfront-basics/navigate-workfront/use-lists/export-lists.md" class="MCXref xref"> Uitvoer een lijst </a>. Voor meer informatie over de uitvoerformaten en grenzen, zie <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref"> Gegevens van de Uitvoer </a>.</p> </td> 
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
   <td>Exporteer de lijst naar PDF, Excel of bestanden met tabs als scheidingsteken.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-agile-icon-in-new-toolbar-task-list.png"> </td> 
   <td>[!UICONTROL Agile View]</td> 
   <td>Geef de lijst weer in de weergave Gelijk.<br> dit is beschikbaar slechts voor taken.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-gantt-chart-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Gantt Chart]</td> 
   <td> <p>Geef de lijst weer in de weergave [!UICONTROL Gantt Chart] .</p> <p>Dit is alleen beschikbaar voor projecten en taken.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-filter-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-filter-in-new-toolbar-with-blue-dot---small.png"> </p> </td> 
   <td>[!UICONTROL Filter] vervolgkeuzemenu</td> 
   <td> <p>Geef een lijst weer met filters en extra opties voor het beheer van filters, waaronder het maken van filters. </p> <p>Op een klein scherm wordt de naam van het filter vervangen door het filterpictogram. Er wordt een blauwe stip weergegeven op het pictogram Filter wanneer u een ander filter toepast dan "[!UICONTROL All]".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-view-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-view-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>[!UICONTROL View] vervolgkeuzemenu</td> 
   <td> <p>Geef een lijst weer met weergaven en extra opties voor het beheren van weergaven, waaronder het maken van weergaven. </p> <p>Op een klein scherm wordt de weergavenaam vervangen door het pictogram [!UICONTROL view] . Er wordt een blauwe stip weergegeven op het pictogram [!UICONTROL View] wanneer u een andere weergave dan "[!UICONTROL Standard]" toepast.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-grouping-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-grouping-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>[!UICONTROL Grouping] vervolgkeuzemenu</td> 
   <td> <p>Geef een lijst weer met groepen en extra opties voor het beheer van groepen, waaronder het maken van groepen. </p> <p>Op een klein scherm wordt de naam van de groepering vervangen door het pictogram [!UICONTROL grouping] . Er wordt een blauwe stip weergegeven op het pictogram [!UICONTROL Grouping] wanneer u een andere groepering toepast dan "[!UICONTROL Nothing]".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-autosave-icon-in-new-toolbar-for-tasks.png"> </td> 
   <td> <p>[!UICONTROL Plan mode]</p> </td> 
   <td> <p>Kies of u de wijzigingen die u in een takenlijst aanbrengt, automatisch of handmatig wilt opslaan. </p> <p>Voor informatie over het uitgeven van taken in een lijst, zie <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref"> taken in een lijst </a> uitgeven. </p> <p>Dit is alleen beschikbaar voor taken.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/summary-panel-icon.png"> </td> 
   <td>[!UICONTROL Summary]</td> 
   <td> <p>Het vak [!UICONTROL Summary] voor het geselecteerde item weergeven of verbergen.</p> <p>Dit is alleen beschikbaar voor taken en problemen.</p> <p>Voor informatie over het [!UICONTROL Summary] paneel, zie <a href="/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref"> Overzicht van de Samenvatting </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/remove-icon---x-in-circle.png"> </td> 
   <td>[!UICONTROL Remove]</td> 
   <td>Verwijder iets uit de lijst. Bijvoorbeeld, als groepsbeheerder die groep of subgroeplidmaatschap beheren, verwijder een groepslid zoals die in <a href="/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md" class="MCXref xref"> wordt verklaard Mening en beheer het lidmaatschap van een groep </a>.</td> 
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
   <th><strong> Functionaliteit </strong> </th> 
   <th><strong> Lijst </strong> </th> 
   <th><strong> Rapport </strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Iedereen kan ze maken</p> </td> 
   <td><span> ✓* </span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Alleen een [!DNL Workfront] beheerder en gebruikers met een [!UICONTROL Plan] -licentie kunnen deze maken</p> </td> 
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
   <td> <p>U kunt exporteren naar de indelingen .pdf, [!DNL Excel] en Door tabs gescheiden</p> </td> 
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

U moet toegang hebben tot filters, weergaven en groepen om deze te kunnen maken. Voor meer informatie, zie [&#x200B; toegang van de Verlening tot filters, meningen, en groeperingen &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

U moet toegang hebben tot filters, weergaven en groepen, maar ook tot rapporten, dashboards en kalenders om deze te kunnen maken. Voor meer informatie, zie [&#x200B; toegang van de Verlening tot rapporten, dashboards, en kalenders &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

U kunt lijsten voor rapporten aanpassen die op een dashboard worden geplaatst slechts als de schepper van het rapport de lijstelementen heeft gevormd om op het dashboard zichtbaar te zijn.

>[!NOTE]
>
>U kunt geen lijst aan een dashboard toevoegen zonder eerst een rapport te creëren en het toe te voegen aan het dashboard.

Voor meer informatie over de bouw van een rapport, zie [&#x200B; een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren. Voor informatie over het creëren van douanesecties, zie [&#x200B; douanetabellen of secties &#x200B;](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md) creëren.

## Het verschil tussen de bijgewerkte en de oudere lijsten

[!DNL Workfront] bevat twee typen lijsten:

* Oudere lijsten

  ![&#x200B; Blauwe groeperingen &#x200B;](assets/legacy-list-screen-shot-blue-groupings-350x101.png)

* Bijgewerkte lijsten

  ![&#x200B; Grijze groeperingen &#x200B;](assets/updated-list-screen-shot-gray-groupings-350x71.png)

In de volgende tabel ziet u een aantal verschillen tussen de verouderde en bijgewerkte lijsten in [!DNL Workfront] :

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
  <td> <p>Vertoning <strong> 100 </strong> punten door gebrek</p> </td> 
   <td> <p>Toon <strong> allen </strong> of tot <strong> 2000 </strong> punten door gebrek</p> </td> 
  </tr> 
  <tr> 
   <td> <p>CTRL+F gebruiken om items in een lijst te zoeken</p> </td> 
   <td> <p>Gebruik snelle filters om snel informatie in een grote lijst te zoeken</p> <p>Voor informatie over het gebruiken van snelle filters in lijsten, zie <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref"> de snelle filter op een lijst </a> toepassen.</p> </td> 
  </tr> 
  <tr> 
   <td>U kunt aangepaste velden met tekstopmaak niet inline bewerken.</td> 
   <td> <p>Tekst in aangepaste velden met opmaak kan worden geconfigureerd om vette, cursieve, onderstreepte, opsommingstekens, nummering, hyperlinks en blokaanhalingstekens toe te staan.</p> <p>Voor meer informatie, zie <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md"> een douaneformulier </a> creëren.</p> </td> 
  </tr> 
  <tr> 
   <td>Met voorwaardelijke opmaak kunt u de tekstkleur van koppelingen in een lijst wijzigen</td> 
   <td>Kan tekstkleurwijzigingen niet toepassen op koppelingen in een lijst</td> 
  </tr> 
 </tbody> 
</table>
