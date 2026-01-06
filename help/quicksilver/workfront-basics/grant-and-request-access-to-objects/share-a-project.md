---
title: Een project delen
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Uw Adobe Workfront-beheerder kan u toegang verlenen tot weergave- of bewerkingsprojecten wanneer u uw toegangsniveau toewijst. Zie Toegang tot projecten verlenen voor meer informatie.
author: Courtney
feature: Get Started with Workfront
exl-id: eaeedff8-9114-40d9-8cd4-56996edc7dad
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1574'
ht-degree: 0%

---

# Een project delen

<!-- Audited: 1/2024 -->

Uw Adobe Workfront-beheerder kan u toegang verlenen tot weergave- of bewerkingsprojecten wanneer u uw toegangsniveau toewijst. Voor meer informatie, zie [&#x200B; toegang van de Verlening tot projecten &#x200B;](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Samen met het toegangsniveau dat gebruikers worden verleend, kunt u hen toestemmingen aan Mening verlenen, bijdragen, of beheren specifieke projecten die u toegang hebt om te delen.

Machtigingen gelden specifiek voor één item in Workfront en definiëren welke handelingen u op dat item kunt uitvoeren.


## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p> 
   <p>Werk of hoger</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot of hoger weergeven voor de objecten die u wilt delen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen of hoger weergeven voor de objecten die u wilt delen</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het delen van projecten

Naast de overwegingen hieronder, zie ook [&#x200B; Overzicht van het delen van toestemmingen op voorwerpen &#x200B;](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Door gebrek, heeft de schepper van een project toestemmingen om het project te beheren en ook aangewezen als Eigenaar van het Project. Als het project aan een andere eigenaar wordt toegewezen, heeft die gebruiker ook toestemmingen om het project te beheren. Wanneer de projectmaker (of eigenaar) het project met andere gebruikers deelt, verlenen zij bepaalde toestemmingen aan die gebruikers om te controleren wat zij kunnen doen aangezien zij aan het project werken.

  Als een eigenaar van een project echter geen plan- of standaardlicentie heeft, hebben hij of zij geen volledige toegang om het project te beheren. Alleen gebruikers met een licentie voor het abonnement of de standaardlicentie kunnen machtigingen hebben om een project te beheren. Voor meer informatie, zie [&#x200B; hoe de toegangsniveaus en de toestemmingen samen &#x200B;](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) werken.

* U kunt projecten afzonderlijk delen, maar u kunt ook verschillende projecten tegelijk delen. Projecten delen is hetzelfde als andere objecten delen. Voor meer informatie over het delen van punten in Workfront, zie [&#x200B; een voorwerp &#x200B;](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md) delen.
* U kunt de volgende toestemmingen aan een project verlenen:

   * Weergave
   * Beheren
   * Contribute

* Wanneer u een project deelt, erven alle taken, kwesties, en de documenten de zelfde toestemmingen, tenzij anders gespecificeerd.

  Voor informatie over het beheren van de toegang tot taken en kwesties op het project dat op de toestemmingen van een gebruiker aan het project wordt gebaseerd, zie de [&#128279;](../../manage-work/projects/manage-projects/edit-projects.md#access) sectie in het artikel [&#x200B; projecten &#x200B;](../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

  De Workfront-beheerder kan opgeven of documenten machtigingen van hogere objecten moeten overnemen op het toegangsniveau van de gebruiker. Voor meer informatie over het beperken van geërfte toestemmingen op documenten, zie [&#x200B; tot douanetoegangsniveaus &#x200B;](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.

* U kunt geërfte toestemmingen uit een project verwijderen zodat de kindvoorwerpen hen niet zullen erven. Voor meer informatie over het verwijderen van geërfte toestemmingen uit voorwerpen, zie [&#x200B; toestemmingen uit voorwerpen &#x200B;](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md) verwijderen.

## Beperkingen voor verschillende licentietypen

* De gebruikers met een vergunning van de Arbeider hebben geen toestemmingen om projecten te beheren. Voor Workers is Contribute de hoogste machtiging voor delen.
* De gebruikers met een vergunning van het Verzoek kunnen projectinformatie bekijken, maar zij hebben beperkte projecttoegang.
* Een uitzondering op het wijzigen van de status van een project treedt op wanneer een gebruiker met de machtiging Weergeven of Contribute ook wordt opgenomen in een goedkeuringsproces. Zij kunnen het project goedkeuren, dat de status van het project verandert, maar de status is de vooraf bepaalde status voor goedkeuring of voor verwerping.
* Om een project te kunnen kopiëren, moet een gebruiker ook toegang hebben om projecten in hun Niveau van de Toegang tot stand te brengen.

## Manieren om een project te delen {#ways-to-share-a-project}

U kunt een project op de volgende manieren delen:

* Handmatig door een van de volgende handelingen uit te voeren:

   * Gebruikers toevoegen aan het projectteam. Wanneer u gebruikers aan het projectteam toevoegt, verkrijgen zij automatisch de toestemmingen van de Mening aan het project.\
     Voor meer informatie over het toevoegen van gebruikers aan een projectteam, zie de Toevoegende Gebruikers aan een sectie van het Team van het Project in [&#x200B; Overzicht van het Team van het Project &#x200B;](../../manage-work/projects/planning-a-project/project-team-overview.md).
   * Individueel of bulk-delend de projecten wanneer het gebruiken van **het Delen** optie.

* Automatisch door een van de volgende handelingen uit te voeren:

   * Plaats een project in a **Portfolio** of **Programma** dat reeds met anderen wordt gedeeld. Gebruikers krijgen dezelfde machtigingen voor het project als voor het portfolio of programma.\
     Voor informatie over het toevoegen van een project aan a **Portfolio**, zie [&#x200B; projecten aan een portefeuille &#x200B;](../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md) toevoegen.\
     Voor informatie over het toevoegen van een project aan a **Programma**, zie [&#x200B; een project aan een programma &#x200B;](../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md) toevoegen.
Voor informatie over het bekijken van geërfte toestemmingen op een voorwerp, zie [&#x200B; Mening geërfte toestemmingen op voorwerpen &#x200B;](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

   * Voeg entiteiten aan het Delen van het Project op een malplaatje toe dat wordt gebruikt om het project tot stand te brengen. Voor informatie over het delen van projecten van malplaatjes, zie [&#x200B; een malplaatje &#x200B;](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md) delen.
   * Bepaal het malplaatje van de projecttoegang.

     >[!TIP]
     >
     >Wanneer het vastmaken van of het bewaren van een malplaatje, kunt u de het Delen van het Project van het Malplaatje regels ontruimen.

   * Bewerk een project en het bepalen van **wanneer iemand toegang tot dit project** het plaatsen wordt gegeven.  Voor meer informatie, zie [&#x200B; projecten &#x200B;](../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

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
<li value="1">Go to a project whose sharing permissions you want for all projects you create from scratch. (NOTE: drafted because linked above)  </li>
<li value="2"> Click the More menu, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>In the Project Access box that displays, near the upper-right corner, click the gear icon <img src="assets/gear-icon-settings.png">, then click <strong>Set as my project access template</strong>.</p> <p>The entities that are granted permissions on the selected project have the same permissions for all the projects you create from scratch in the future.</p> <p> The project access template overrides the sharing defaults granted to you by the Workfront administrator in your Access Level.<br>For more information about specifying sharing defaults for projects in the Access Level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> </li>
<li value="4">Click <strong>Save</strong>.</li>
</ol>
-->

## Een project delen

{{step1-to-projects}}

1. Voor de **pagina van Projecten**, selecteer het project u van de lijst wilt delen. De projectpagina wordt geopend.

1. Aan het recht van de projectnaam, klik **Aandeel**. Het **de dialoogvakje van de Naam van het Project van het Aandeel []** opent.

   ![&#x200B; het projectknoop van het Aandeel &#x200B;](assets/share-project.png)

1. In het **project van de Verlening toegang tot** gebied, begin typend de naam van de gebruiker, het team, de rol, de groep, of het bedrijf u het project met wilt delen, dan klik de naam wanneer het in de drop-down lijst verschijnt.

   >[!TIP]
   >
   >U kunt een project met actieve gebruikers, teams, rollen, of bedrijven slechts delen.


1. (Facultatief) selecteer **wie toegang** drop-down heeft en het de toegangsniveau van het project selecteert:

   * **slechts kunnen de uitgenodigde mensen toegang hebben:** slechts de gebruikers die aan het project worden uitgenodigd kunnen tot het (Gebrek) toegang hebben.
   * **iedereen in het systeem kan** bekijken: Alle gebruikers in het systeem kunnen het project zonder een uitnodiging bekijken.

1. (Facultatief) om de montages van de projecttoegang automatisch toe te passen u aan alle nieuwe projecten selecteerde, klik het **pictogram van het Gear** Uitgezocht het tandwielpictogram ![, dan controleer de doos gealigneerd met &#x200B;](assets/gear-icon.png) Reeks als mijn malplaatje van de projecttoegang **.**

   >[!NOTE]
   >
   >Het malplaatje van de projecttoegang treedt de het delen gebreken met voeten die aan u door de beheerder van Workfront in uw Niveau van de Toegang worden verleend.\
   >Voor meer informatie over het specificeren van het delen van gebreken voor projecten in het Niveau van de Toegang, zie [&#x200B; Toegang van de Verlening tot projecten &#x200B;](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)

   <!--
   >this note also appears in Understanding Project Permissions-->


1. Klik de drop-down rechts van de naam van de gebruiker en selecteer hun toestemmingsniveau voor dit project:


   * **Mening**: De gebruiker kan het project herzien en delen.
   * **draag** bij: De gebruiker kan updates maken, logboekinformatie, minder belangrijke uitgeven maken, en het project (omvat ook alle toestemmingen van de Mening) delen.
   * **leidt**: De gebruiker heeft volledige toegang tot het project zonder administratieve rechten, die op het toegangsniveau (omvat ook alle toestemmingen van de Mening en van Contribute) worden verleend.

1. (Optioneel) Klik op het pictogram Geavanceerde opties naast het machtigingsniveau dat u hebt toegekend om specifieke machtigingen voor het project te configureren.

   ![&#x200B; gevormde geavanceerde toestemmingsopties &#x200B;](assets/advanced-permission-options.png)

1. (Facultatief) om het project snel te delen gebruikend een verbinding, klik **verbinding van het Exemplaar** en door:sturen het aan de ontvanger.

1. Klik **sparen**.

## Projecten bulksgewijs delen

{{step1-to-projects}}

1. Op de **pagina van Projecten**, selecteer de doos links van elk project u wilt delen, dan klik het **pictogram van het Aandeel** pictogram ![&#x200B; van het Aandeel &#x200B;](assets/share-icon.png) bij de bovenkant van de pagina. Het deelmodaal wordt geopend.

   ![&#x200B; Bulk deelt projecten &#x200B;](assets/bulk-share-icon.png)

1. In het **project van de Verlening toegang tot** gebied, begin typend de naam van de gebruiker, het team, de rol, de groep, of het bedrijf u de projecten met wilt delen, dan klik de naam wanneer het in de drop-down lijst verschijnt.

   >[!TIP]
   >
   >U kunt projecten met actieve gebruikers, teams, rollen, of bedrijven slechts delen.


1. (Facultatief) selecteer **wie toegang** drop-down heeft en het de toegangsniveau van de projecten selecteert:

   * **slechts kunnen de uitgenodigde mensen toegang hebben:** slechts de gebruikers die aan de projecten worden uitgenodigd kunnen tot hen (Gebrek) toegang hebben.
   * **iedereen in het systeem kan** bekijken: Alle gebruikers in het systeem kunnen de projecten zonder een uitnodiging bekijken.


1. Klik de drop-down rechts van de naam van de gebruiker en selecteer hun toestemmingsniveau voor de projecten:

   * **Mening**: De gebruiker kan de projecten herzien en delen.
   * **draag** bij: De gebruiker kan updates maken, logboekinformatie, minder belangrijke uitgeven maken, en de projecten (omvat ook alle toestemmingen van de Mening) delen.
   * **leidt**: De gebruiker heeft volledige toegang tot de projecten zonder administratieve rechten, die op het toegangsniveau (omvat ook alle toestemmingen van de Mening en van Contribute) worden verleend.

1. (Facultatief) klik het geavanceerde optiepictogram naast het toestemmingsniveau u hebt verleend om specifieke toestemmingen op de projecten te vormen.

   ![&#x200B; gevormde geavanceerde toestemmingsopties &#x200B;](assets/advanced-permission-options.png)

1. Klik **sparen**.


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Configure default permissions for a project</h2>
<p>(NOTE: drafted because I added one more way to automatically share the project above in the bullet list and linked it to Edit Projects) </p>
<p>As a project owner, you can configure the default permissions for View, Manage, and Contribute access that are used when sharing  the project with others. When users share a project, the default permissions are used. Users can then adjust the default permissions when sharing the project, as described in <a title="Project Permissions" href="#ways-to-share-a-project" class="MCXref xref">Ways to share a project</a>. </p>
<p>To configure the default permissions that are included with each access level:</p>
<ol>
<li value="1">Go to the project where you want to set the default permissions.</li>
<li value="2"> <p>Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. <img src="assets/edit-icon.png"></p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Click <strong>Access</strong> in the list on the left.</li>
<li value="4"> <p>In the <strong>When someone is given access to this PROJECT</strong> section, select permissions that you want to be available when users are given access to the project via sharing.</p> <p>Ensure that any permissions that you want to include in the selected access level are selected and deselect any permissions that you do not want to include in the selected permissions level.</p> <p>To view which permissions are available for each level, see  <a title="Project Permissions" href="#Understanding_Project_Permissions" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <note type="note">
The
<strong>Delete</strong> access in the
<strong>Manage</strong> permission level determines whether users can  delete the project itself. Users with
<strong>Manage</strong> access to the project can delete tasks and issues within the project regardless of whether this option is selected, if they have
<strong>Manage</strong> permissions to the tasks and issues.  
</note> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## Opties voor projectmachtigingen

De volgende lijst maakt een lijst van de toestemmingen die de gebruikers kunnen verlenen wanneer het delen van een project. Voor meer informatie over de toegangsgebruikers die op hun vergunning worden gebaseerd, zie [&#x200B; toegang van de Verlening tot projecten &#x200B;](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong> Acties </strong> </p> </th> 
   <th> <p><strong> leiden </strong> </p> </th> 
   <th> <p><strong> draagt </strong> bij </p> </th> 
   <th> <p><strong> Mening </strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aangepast formulier toevoegen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aangepaste velden bijwerken</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Een goedkeuringsproces toevoegen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
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
   <td> <p>✓  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Een project maken</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
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
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project kopiëren</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project verwijderen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Geplande datums wijzigen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project delen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Delen in het hele systeem</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
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
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Logboekuren</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Toewijzingen bewerken</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Basislijn beheren</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Risico's beheren*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Financiën beheren*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uitgaven toevoegen/bewerken*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
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
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
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
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projectdetails bewerken</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Personeel bewerken</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
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
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Wachtrij-eigenschappen instellen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>    </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project in een lijst bulksgewijs bewerken</p> </td> 
   <td> <p>✓</p> </td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
 </tbody> 
</table>

&#42; de gebruikers zonder toegang tot financiële gegevens kunnen geen risico en financiën voor projecten beheren, zelfs als zij Edit toegang tot projecten hebben. Voor informatie over toegang tot financiële gegevens, zie [&#x200B; Toegang van de Verlening tot financiële gegevens &#x200B;](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
