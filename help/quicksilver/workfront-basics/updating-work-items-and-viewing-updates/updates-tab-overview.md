---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Overzicht van het tabblad Updates
description: Het tabblad Updates bevat maximaal 200 van de meest recente updates die in de afgelopen 90 dagen zijn gemaakt.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 19872953e847921c0fee6d383026641c05012ead
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# Overzicht van het tabblad Updates

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only for a limited number of objects when you opt in to the new commenting experience Beta.</span> -->

<!-- for preview commenting beta: at the release of commenting beta: change the title to: Updates section overview - also update ALL articles from which this is linked-->

Het tabblad Updates bevat maximaal 200 van de meest recente updates die in de afgelopen 90 dagen zijn gemaakt.

U kunt opmerkingen maken en reageren op updates voor de volgende objecten:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Documenten</li> 
     <li>Doelen</li> 
     <li>Problemen</li> 
     <li>Herhalingen</li> 
     <li>Projecten</li> 
     <li>Programma's</li> 
     <li>Portfolio</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Artikelen</li> 
     <li>Taken</li> 
     <li>Sjablonen</li> 
     <li>Sjabloontaken</li> 
     <li>Timesheets</li> 
     <li>Gebruikers</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Updates die ook worden weergegeven op objecten met een hogere positie

Zoals in de volgende tabel wordt getoond, worden antwoorden op updates voor bepaalde objecten ook weergegeven op het tabblad Updates van objecten met een hogere positie.

Wanneer u bijvoorbeeld een update toevoegt aan een taak, wordt de update weergegeven op het tabblad Updates voor de taak en op het tabblad Updates voor het project dat de taak bevat.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Object waar de oorspronkelijke update is toegevoegd</strong> </th> 
   <th> <p><strong>Hoger gerangschikt object waar de oorspronkelijke update ook wordt weergegeven</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Probleem</td> 
   <td>Project</td> 
  </tr> 
  <tr> 
   <td>Taak</td> 
   <td>Project</td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>Programma, Portfolio</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Document </td> 
   <td>Object waaraan het document is gekoppeld, Project </td> 
  </tr> 
  <tr> 
   <td>Programma</td> 
   <td>Portfolio</td> 
  </tr> 
  <tr> 
   <td>Gebruiker</td> 
   <td>Team</td> 
  </tr> 
  <tr> 
   <td>Tijdschema</td> 
   <td>Gebruiker, team</td> 
  </tr> 
  <tr> 
   <td>Sjabloontaak</td> 
   <td>Sjabloon</td> 
  </tr> 
  <tr> 
   <td>Artikel</td> 
   <td>Herhaling, team</td> 
  </tr> 
  <tr> 
   <td>Iteratie</td> 
   <td>Team</td> 
  </tr>

<tr> 
   <td>Doelen</td> 
   <td>Resultaat, activiteit</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>De reacties die aan systeemupdates worden toegevoegd rollen niet omhoog aan het oudervoorwerp. Alleen directe antwoorden op een onderliggend object en antwoorden die aan bestaande updates zijn toegevoegd, worden doorgegeven aan bovenliggende objecten.
>
>Voor informatie over de objecthiërarchie in Adobe Workfront raadpleegt u [Objecten in Adobe Workfront begrijpen](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

<!-- drafted for the new commenting experience for issues in beta: Add this paragraph to the note above: 
><span class="preview"> It is not possible to reply to system updates in the new commenting experience Beta. For more information, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md).</span> -->

## Beperkingen op het tabblad Updates

### Beperkingen voor gebruikers en teams

U kunt geen updates uitvoeren op teams. Het tabblad Updates voor teams wordt gevuld met updates die worden ingevoerd voor de volgende objecten:

* Gebruikers
* Timesheets
* Artikelen
* Herhalingen

Op het tabblad Updates voor gebruikers en teams kunt u de updates weergeven die in de afgelopen 90 dagen zijn ingevoerd.

Als u alle updates wilt zien die op een gebruiker of een team, voorbij de grens van 90 dagen worden gemaakt, kunt u een rapport voor nota&#39;s bouwen. Het rapport zou geen tijdfilter moeten hebben dat alle updates toont die voor gebruikers of teams worden gemaakt. Zie voor meer informatie [Een aangepast rapport maken](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Beperkingen bij het invoeren van opmerkingen namens een andere gebruiker

Adobe Workfront-beheerders en groepsbeheerders kunnen zich aanmelden als andere gebruikers en acties uitvoeren in Workfront, zoals het invoeren van opmerkingen. (Zie voor meer informatie [Aanmelden als een andere gebruiker](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).) Eventuele opmerkingen die namens een andere gebruiker worden gemaakt, worden in de opmerking vermeld.

Een groepsbeheerder kan opmerkingen maken namens een andere persoon, maar kan die opmerking niet verwijderen. Alleen een Adobe Workfront-beheerder kan een opmerking verwijderen die hij namens een andere gebruiker heeft gemaakt.

## Systeemupdates van werkitems weergeven met het rapport Dagboekingang

Het rapport van de Ingang van het Dagboek oppervlakt systeemupdates van het gebied van Updates van projecten, taken, en kwesties.

Met het rapport kunt u zien:

* Aantal statuswijzigingen
* Wanneer een taak of kwestie werd geschrapt
* De manier waarop waarden in belangrijke aangepaste velden tijdens een project zijn gewijzigd
* Welke belangrijke data zijn in de loop van een project gewijzigd
* Indien de prioriteit tijdens een project is gewijzigd
* Als de eigenaar van een project is gewijzigd

Zie voor meer informatie [Rapport over het gebied Updates](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
