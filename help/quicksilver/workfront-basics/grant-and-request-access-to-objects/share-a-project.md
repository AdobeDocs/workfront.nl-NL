---
title: Een project delen in Adobe Workfront
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Uw Adobe Workfront-beheerder kan u toegang verlenen tot weergave- of bewerkingsprojecten wanneer u uw toegangsniveau toewijst. Zie Toegang tot projecten verlenen voor meer informatie.
author: Alina
feature: Get Started with Workfront
exl-id: eaeedff8-9114-40d9-8cd4-56996edc7dad
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 0%

---

# Een project delen in Adobe Workfront

<!-- Audited: 1/2024 -->

Uw Adobe Workfront-beheerder kan u toegang verlenen tot weergave- of bewerkingsprojecten wanneer u uw toegangsniveau toewijst. Voor meer informatie, zie [ toegang van de Verlening tot projecten ](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Samen met het toegangsniveau dat de gebruikers worden verleend, kunt u hen toestemmingen aan Mening, Contribute, of beheer specifieke projecten ook verlenen die u toegang hebt om te delen.

Machtigingen gelden specifiek voor één item in Workfront en definiëren welke handelingen u op dat item kunt uitvoeren.

## Overwegingen bij het delen van projecten

Naast de overwegingen hieronder, zie ook [ Overzicht van het delen van toestemmingen op voorwerpen ](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Door gebrek, heeft de schepper van een project toestemmingen om het project te beheren en ook aangewezen als Eigenaar van het Project. Als het project aan een andere eigenaar wordt toegewezen, heeft die gebruiker ook toestemmingen om het project te beheren. Wanneer de projectmaker (of eigenaar) het project met andere gebruikers deelt, verlenen zij bepaalde toestemmingen aan die gebruikers om te controleren wat zij kunnen doen aangezien zij aan het project werken.

  Als de eigenaar van een project echter geen Planner-licentie heeft, hebben deze geen volledige toegang om het project te beheren. Slechts kan een gebruiker met een vergunning van het Plan toestemmingen hebben om een project te beheren. Voor meer informatie, zie [ hoe de toegangsniveaus en de toestemmingen samen ](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) werken.

* U kunt projecten afzonderlijk delen, maar u kunt ook verschillende projecten tegelijk delen. Projecten delen is hetzelfde als andere objecten delen. Voor meer informatie over het delen van punten in Workfront, zie [ een voorwerp ](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md) delen.
* U kunt de volgende toestemmingen aan een project verlenen:

   * Weergave
   * Beheren
   * Contribute

     ![](assets/view-on-projects-190x207.png) ![](assets/contribute-on-projects-159x243.png) ![](assets/manage-on-projects-178x230.png)

* Wanneer u een project deelt, erven alle taken, kwesties, en de documenten de zelfde toestemmingen, tenzij anders gespecificeerd.

  Voor informatie over het beheren van de toegang tot taken en kwesties op het project dat op de toestemmingen van een gebruiker aan het project wordt gebaseerd, zie de [](../../manage-work/projects/manage-projects/edit-projects.md#access) sectie in het artikel [ projecten ](../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

  De Workfront-beheerder kan opgeven of documenten machtigingen van hogere objecten moeten overnemen op het toegangsniveau van de gebruiker. Voor meer informatie over het beperken van geërfte toestemmingen op documenten, zie [ tot douanetoegangsniveaus ](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.

* U kunt geërfte toestemmingen uit een project verwijderen zodat de kindvoorwerpen hen niet zullen erven. Voor meer informatie over het verwijderen van geërfte toestemmingen uit voorwerpen, zie [ toestemmingen uit voorwerpen ](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md) verwijderen.

## Manieren om een project te delen {#ways-to-share-a-project}

U kunt een project op de volgende manieren delen:

* Handmatig door een van de volgende handelingen uit te voeren:

   * Gebruikers toevoegen aan het projectteam. Wanneer u gebruikers aan het projectteam toevoegt, verkrijgen zij automatisch de toestemmingen van de Mening aan het project.\
     Voor meer informatie over het toevoegen van gebruikers aan een projectteam, zie de &quot;Toevoegende Gebruikers aan een sectie van het Team van het Project&quot;in [ overzicht van het Team van het Project ](../../manage-work/projects/planning-a-project/project-team-overview.md).
   * Individueel of bulk-delend de projecten wanneer het gebruiken van **het Delen** optie.

     Het delen van een project is vergelijkbaar met het delen van alle andere objecten in Adobe Workfront.

     Voor informatie over het delen van voorwerpen in Workfront, zie [ een voorwerp ](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md) delen.

* Automatisch, door één van het volgende te doen:

   * Plaats een project in a **Portfolio** of **Programma** dat reeds met anderen wordt gedeeld. Gebruikers krijgen dezelfde machtigingen voor het project als voor het portfolio of programma.\
     Voor informatie over het toevoegen van een project aan a **Portfolio**, zie [ projecten aan een portefeuille ](../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md) toevoegen.\
     Voor informatie over het toevoegen van een project aan a **Programma**, zie [ een project aan een programma ](../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md) toevoegen.

     Voor informatie over het bekijken van geërfte toestemmingen op een voorwerp, zie [ Mening geërfte toestemmingen op voorwerpen ](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

   * Voeg entiteiten aan het Delen van het Project op een malplaatje toe dat wordt gebruikt om het project tot stand te brengen. Voor informatie over het delen van projecten van malplaatjes, zie [ een malplaatje ](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md) delen.
   * Bepaal het malplaatje van de projecttoegang.

     Om het malplaatje van de projecttoegang te bepalen, zie [ een voorwerp ](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md) delen.

     >[!TIP]
     >
     >Wanneer het vastmaken van of het bewaren van een malplaatje, kunt u de het Delen van het Project van het Malplaatje regels ontruimen.

   * Bewerk een project en het bepalen van **wanneer iemand toegang tot dit project** het plaatsen wordt gegeven. Voor meer informatie, zie [ projecten ](../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because I created new article and linked it above) </p>
<p>To view what users have inherited the access on the project from a portfolio or a program, do the following:</p>
<ol style="list-style-type: lower-alpha;">
<li value="1">Go to a project whose sharing permissions you want to view. </li>
<li value="2"> Click the <strong>More</strong> menu <img src="assets/more-icon.png">, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>Expand the <strong>Inherited Permissions</strong> list. </p> <p>This list displays the names of users that have access to either the portfolio or the program that the project belongs to and also have permissions to the project. </p>  </li>
</ol>
</div>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a project whose sharing permissions you want for all projects you create from scratch. (NOTE: drafted because linked above)&nbsp;</li>
<li value="2"> Click the More menu, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>In the Project Access box that displays, near the upper-right corner, click the gear icon <img src="assets/gear-icon-settings.png">, then click <strong>Set as my project access template</strong>.</p> <p>The entities that are granted permissions on the selected project have the same permissions for all the projects you create from scratch in the future.</p> <p> The project access template overrides the sharing defaults granted to you by the Workfront administrator in your Access Level.<br>For more information about specifying sharing defaults for projects in the Access Level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> </li>
<li value="4">Click <strong>Save</strong>.</li>
</ol>
-->

## Beperkingen voor verschillende licentietypen

* De gebruikers met een vergunning van de Arbeider hebben geen toestemmingen om projecten te beheren. Voor Workers is Contribute de hoogste machtiging voor delen.
* De gebruikers met een vergunning van het Verzoek kunnen projectinformatie bekijken, maar zij hebben beperkte projecttoegang.
* Een uitzondering op het wijzigen van de status van een project treedt op wanneer een gebruiker met de machtiging Weergeven of Contribute ook is opgenomen in een goedkeuringsproces. Zij kunnen het project goedkeuren, dat de status van het project verandert, maar de status is de vooraf bepaalde status voor goedkeuring of voor verwerping.
* Om een project te kunnen kopiëren, moet een gebruiker ook toegang hebben om projecten in hun Niveau van de Toegang tot stand te brengen.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Configure default permissions for a project</h2>
<p>(NOTE: drafted because I added one more way to automatically share the project above in the bullet list and linked it to Edit Projects) </p>
<p>As a project owner, you can configure the default permissions for View, Manage, and Contribute access that are used when sharing&nbsp;the project with others. When users share a project, the default permissions are used. Users can then adjust the default permissions when sharing the project, as described in <a title="Project Permissions" href="#ways-to-share-a-project" class="MCXref xref">Ways to share a project</a>. </p>
<p>To configure the default permissions that are included with each access level:</p>
<ol>
<li value="1">Go to the project where you want to set the default permissions.</li>
<li value="2"> <p>Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. <img src="assets/edit-icon.png"></p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Click <strong>Access</strong> in the list on the left.</li>
<li value="4"> <p>In the <strong>When someone is given access to this PROJECT</strong> section, select permissions that you want to be available when users are given access to the project via sharing.</p> <p>Ensure that any permissions that you want to include in the selected access level are selected and deselect any permissions that you do not want to include in the selected permissions level.</p> <p>To view which permissions are available for each level, see&nbsp;<a title="Project Permissions" href="#Understanding_Project_Permissions" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <note type="note">
The
<strong>Delete</strong> access in the
<strong>Manage</strong> permission level determines whether users can&nbsp;delete the project itself. Users with
<strong>Manage</strong> access to the project can delete tasks and issues within the project regardless of whether this option is selected, if they have
<strong>Manage</strong> permissions to the tasks and issues.&nbsp;
</note> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## Opties voor projectmachtigingen

De volgende lijst maakt een lijst van de toestemmingen die de gebruikers kunnen verlenen wanneer het delen van een project. Voor meer informatie over de toegangsgebruikers die op hun vergunning worden gebaseerd, zie [ toegang van de Verlening tot projecten ](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong> Acties </strong> </p> </th> 
   <th> <p><strong> leiden </strong> </p> </th> 
   <th> <p><strong> Contribute </strong> </p> </th> 
   <th> <p><strong> Mening </strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aangepast formulier toevoegen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aangepaste velden bijwerken</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Een goedkeuringsproces toevoegen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Een project goedkeuren</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uren goedkeuren</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓ </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Een project maken</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Document(en) toevoegen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Probleem(en) toevoegen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak/taken toevoegen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project kopiëren</p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project verwijderen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Geplande datums wijzigen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project delen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Delen in het hele systeem</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project weergeven</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Updates/opmerkingen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Status wijzigen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Logboekuren</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Toewijzingen bewerken</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Basislijn beheren</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Risico's beheren*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Financiën beheren*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uitgaven toevoegen/bewerken*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Financiën weergeven*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Sjabloon koppelen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Opslaan als sjabloon</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Zakelijke kwestie toevoegen/bewerken</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projectdetails bewerken</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Personeel bewerken</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Exporteren naar MS-project</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Financiën/ Tijdlijn opnieuw berekenen*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Wachtrij-eigenschappen instellen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project in een lijst bulksgewijs bewerken</p> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; de gebruikers zonder toegang tot financiële gegevens kunnen geen risico en financiën voor projecten beheren, zelfs als zij Edit toegang tot projecten hebben. Voor informatie over toegang tot financiële gegevens, zie [ Toegang van de Verlening tot financiële gegevens ](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
