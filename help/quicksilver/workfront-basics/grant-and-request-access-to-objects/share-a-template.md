---
title: Een sjabloon delen
product-area: templates
navigation-topic: grant-and-request-access-to-objects
description: Als beheerder van Adobe Workfront, kunt u gebruikers toegang tot mening verlenen of malplaatjes uitgeven wanneer u hun toegangsniveau toewijst. Een gebruiker moet een licentie voor een abonnement hebben om toegang te hebben tot Sjablonen bewerken.
author: Courtney
feature: Get Started with Workfront
exl-id: 19fb0de5-7db5-42a9-9f33-a4570acfeef8
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# Een sjabloon delen

Als beheerder van Adobe Workfront, kunt u gebruikers toegang tot mening verlenen of malplaatjes uitgeven wanneer u hun toegangsniveau toewijst. Een gebruiker moet een licentie voor een abonnement hebben om toegang te hebben tot Sjablonen bewerken.

Voor meer informatie over het verlenen van toegang tot malplaatjes, zie [ Toegang van de Verlening tot malplaatjes ](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

Samen met het toegangsniveau dat u verleent, kan een gebruiker toestemmingen om specifieke malplaatjes van andere gebruikers ook te bekijken of te beheren die hen delen.

>[!NOTE]
>
>De niveaus van de toestemming werken binnen de niveaus van de Toegang. Een gebruiker kan bijvoorbeeld geen machtigingen ontvangen om een sjabloon te beheren als het toegangsniveau van de gebruiker alleen sjablonen toestaat.

Machtigingen gelden specifiek voor één item in Workfront en definiëren welke handelingen u op dat item kunt uitvoeren.

## Overwegingen bij het delen van een sjabloon

* Naast de overwegingen hieronder, zie ook [ Overzicht van het delen van toestemmingen op voorwerpen ](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* De maker van een sjabloon en de sjablooneigenaar hebben standaard beheermachtigingen voor de sjabloon. Voor informatie over het aanwijzen van een gebruiker als Eigenaar van het Malplaatje, zie [ projectmalplaatjes ](../../manage-work/projects/create-and-manage-templates/edit-templates.md) uitgeven.
* U kunt het volgende delen bij het delen van een sjabloon:

   * De sjabloon

     Voor meer informatie over hoe te om een malplaatje te delen, zie [ het projectmalplaatjes van het Aandeel ](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

     U kunt de volgende machtigingen aan een sjabloon verlenen:

      * Weergave
      * Beheren

   * De toekomstige projecten die gebruikend het malplaatje worden gecreeerd. U kunt de zelfde niveaus van toestemmingen aan projecten geven die van een malplaatje worden gecreeerd zoals u een individueel project.

     Voor informatie over hoe te om een project van een malplaatje op het malplaatjeniveau te delen, zie [ het projectmalplaatjes van het Aandeel ](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* Wanneer u een malplaatje of een project deelt dat van het malplaatje wordt gecreeerd, erven de gebruikers de zelfde toestemmingen aan alle kindvoorwerpen verbonden aan het malplaatje of het project, door gebrek.

  Zie voor meer informatie over de hiërarchie van objecten in Workfront   [ Begrijp voorwerpen in Adobe Workfront ](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* Wanneer u een malplaatje deelt, erven alle malplaatjetaken en documenten, evenals de kwesties op het toekomstige project dat van het malplaatje wordt gecreeerd de zelfde toestemmingen, tenzij anders gespecificeerd.

  Voor informatie over het beheren van de toegang tot malplaatjetaken en kwesties op het project dat op de toestemmingen van een gebruiker aan het project wordt gebaseerd, zie de [ sectie van de Toegang ](../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) in artikel [ projectmalplaatjes ](../../manage-work/projects/create-and-manage-templates/edit-templates.md) uitgeven.

* De Workfront-beheerder kan opgeven of documenten machtigingen van hogere objecten moeten overnemen op het toegangsniveau van de gebruiker. Voor meer informatie over het beperken van geërfte toestemmingen op documenten, zie [ tot douanetoegangsniveaus ](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.

* U kunt sjabloontaken niet afzonderlijk delen. Door een sjabloon te delen, worden ook de sjabloontaken gedeeld. Het delen van het project van het malplaatje deelt ook de toekomstige projecttaken.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Share a template</h2>
<p>(NOTE: drafted because this is also linked above: Share project templates >> which is an article in the Manage Work section>> Templates)  </p>
<ol>
<li value="1"> <p>Go to the template you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Template Sharing</strong>.<br>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Template</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing the name of a user, group, team, job role, or company that you want to share the template with in the <strong>Give template access to</strong> or <strong>Edit template access for</strong> fields.</p> <p>Select them when they appear in the list.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant:<br>
<ul>
<li><p><strong>View it</strong>: Users with these permissions are able to view the template and create a project using it, or attach it to an existing project.</p><p><img src="assets/template-permissions-350x197.png" alt="template_permissions.png" style="width: 350;height: 197;"></p></li>
<li><strong>Manage it</strong>: Users with these permissions are able to edit or delete the template.</li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions.</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<h2>Share a project at the template level</h2>
<p>You can share the future projects that are created using a template with users at the template level.</p>
<ol>
<li value="1"> <p>Go to the template whose future projects you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Project Sharing</strong>.</p> <p>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Project</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has project permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing and then select the name of a user, group, team, job role, or company with whom you want to share future projects created from the template in the <strong>Give project access to</strong> or <strong>Edit template access for</strong> fields.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant.<br>Select from the following:<br>
<ul>
<li><strong>No access</strong>: You can specify which users will not have any access to the template.<br>This option is available only when bulk sharing projects from templates.  </li>
<li><strong>View</strong>: Users with these permissions can view projects created from the template.</li>
<li><strong>Contribute</strong>: Users with these permissions can contribute to projects created from the template  </li>
<li><strong>Manage</strong>: Users with these permissions can manage or delete projects created from this template.<br><img src="assets/share-project-from-template-350x268.png" alt="share_project_from_template.png" style="width: 350;height: 268;"></li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions. </li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Geavanceerde instellingen voor het delen van sjablonen

In de volgende tabel wordt weergegeven welke machtigingen u gebruikers kunt verlenen wanneer u hen toestaat een sjabloon te bekijken of te beheren. Voor de instructies bij het delen van een malplaatje, zie de sectie [ een malplaatje ](../../manage-work/projects/create-and-manage-templates/share-project-template.md#share) in het artikel [ het projectmalplaatjes van het Aandeel ](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Handelingen</th> 
   <th>Beheren</th> 
   <th>Weergave</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Kopiëren</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Verwijderen</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Sjabloondetails bewerken</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Sjabloon weergeven</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Delen</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Delen in het hele systeem</td> 
   <td>  </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Documenten toevoegen</p> <p>Tip: Soms voegen mensen documenten toe aan een projectsjabloon terwijl ze denken dat ze ze aan een project toevoegen. U kunt dit voor uw ontvangers verhinderen door dit het plaatsen onbruikbaar te maken.</p> </td> 
   <td>  </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

Om de toestemmingen te begrijpen u gebruikers aan projecten verleent die van een malplaatje worden gecreeerd, zie [ een project in Adobe Workfront ](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md) delen.
