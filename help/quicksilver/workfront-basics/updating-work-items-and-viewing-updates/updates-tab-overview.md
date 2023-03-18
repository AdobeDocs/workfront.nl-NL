---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Overzicht van de sectie Updates
description: De sectie Updates bevat maximaal 200 van de meest recente updates die in de afgelopen 90 dagen zijn uitgevoerd.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 39647f235c2e131e0ddd5d3b72d2f073387e531e
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# Overzicht van de sectie Updates

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the Updates section of an object. You can access the new design by enabling the commenting Beta. 
Currently, the Beta is available for <span class="preview">issues</span>. 
For more information about the new commenting  experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 

-->

In de sectie Updates van een object worden opmerkingen weergegeven die gebruikers maken over de object- of systeemupdates waarmee wijzigingen in het object worden bijgehouden.

## Overzicht van de sectie Updates

<!--drafted for the commenting beta for issues: 
The information is organized differently in the Updates section, depending on which environment you access it from. 

###  Overview of the current Updates section 
-->

De sectie Updates van een object bevat maximaal 200 van de meest recente updates die in de afgelopen 90 dagen zijn uitgevoerd.

<!--drafted for the commenting beta for issues: 
The current Updates section shows the following information:

************** AND REMOVE THE SENTENCE BELOW WHEN MAKING THIS LIVE:
-->

In de sectie Updates wordt de volgende informatie weergegeven:

* Opmerkingen van gebruikers en antwoorden op deze opmerkingen.
* Systeemupdates die informatieve berichten zijn die Workfront maakt om bepaalde gebeurtenissen op een object op te nemen. U kunt bijvoorbeeld wijzigingen in status, naam of aangepaste velden vastleggen met systeemupdates. Uw Workfront- of groepsbeheerder kan systeemupdates voor uw objecten inschakelen. Zie voor meer informatie [Systeemupdates configureren](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

De sectie Updates wordt weergegeven voor de volgende objecten:

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

<!--drafted for the commenting beta for issues: 
###  Overview of the Updates section in the Beta commenting experience

The Updates section displays information in the following tabs in the Beta commenting experience: 

* **Updates**: Displays comments made by users and replies to those comments. 
* **System Activity**: Displays system updates which are informational messages that Workfront creates to record certain events on an objects. For example, you can capture changes in status, name, or custom fields with system updates. Your Workfront or group administrator can enable system updates for your ojects. For more information, see [Configure system updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Currenlty, you can make comments and reply to updates using the Beta commenting experience on the following objects:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Goals</li> 
     </ul> </td> 
   <td> 
    <ul> 
     <li><span class="preview">Issues</span></li> 
     </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>The commenting experience Beta is the default current experience for goals. You must have an additional license to access Workfront Goals. For information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
-->

## Updates die ook worden weergegeven op objecten met een hogere positie

Zoals getoond in de volgende lijst, verschijnen de antwoorden die op updates over bepaalde voorwerpen worden gemaakt ook op de sectie van Updates van hoger-gerangschikte voorwerpen.

Wanneer u bijvoorbeeld een update toevoegt aan een taak, wordt de update weergegeven in de sectie Updates voor de taak en in de sectie Updates voor het project dat de taak bevat.

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

## Beperkingen van de sectie Updates

### Beperkingen voor gebruikers en teams

U kunt geen updates uitvoeren op teams. De sectie Updates voor teams wordt gevuld met updates die worden ingevoerd voor de volgende objecten:

* Gebruikers
* Timesheets
* Artikelen
* Herhalingen

In de sectie Updates voor gebruikers en teams kunt u de updates weergeven die in de afgelopen 90 dagen zijn ingevoerd.

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
