---
title: Overzicht van het type Projectvoorwaarde en Voorwaarde
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: De projectvoorwaarde is een visuele vertegenwoordiging van hoe het project vordert. Het is een te rapporteren variabele die wordt bepaald door het verband tussen de geplande, geplande en geschatte data van het project.
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---

# Overzicht van het type Projectvoorwaarde en Voorwaarde

<!-- Audited: 12/2023 -->

De projectvoorwaarde is een visuele vertegenwoordiging van hoe het project vordert. Het is een te rapporteren variabele die wordt bepaald door het verband tussen de geplande, geplande en geschatte data van het project.

## Overzicht van projectvoorwaarde

Overweeg het volgende in het begrip van de Voorwaarde van een project:

* Als projecteigenaar, kunt u beslissen of de Voorwaarde van een project manueel of automatisch wordt geplaatst. De voorwaarde van een project kan op de volgende manieren worden geplaatst:

   * Handmatig door gebruikers die toegang hebben tot het project beheren en wanneer het Condition Type of het project is ingesteld op Handmatig.
   * Automatisch door Adobe Workfront, wanneer het Type van Voorwaarde van het project aan de Status van de Voortgang wordt geplaatst. De status van de voortgang van het project wordt bepaald door de voortgang van de taken van het project. Voor informatie over de Voortgangsstatus van het project, zie [ Overzicht van de Status van de Voortgang van het Project ](../../../manage-work/projects/planning-a-project/project-progress-status.md).

  Voor informatie over hoe te om het Type van Voorwaarde van het project bij te werken, zie [ het Type van Voorwaarde van een project ](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md) plaatsen.

* Wanneer het toestaan van Workfront om de Voorwaarde van het project automatisch te schatten, adviseren wij dat u predecessors op uw taken gebruikt zodat de taakvooruitgang in de daadwerkelijke vooruitgang en de Voortgangsstatus van het project weerspiegelt.
* Als projecteigenaar, kunt u het project veranderen om een Handmatig Type van Voorwaarde in plaats van het gebruiken van de Status van de Voortgang te gebruiken door het Type van Voorwaarde van de Status van de Voortgang in Handboek te veranderen.

  >[!NOTE]
  >
  >Projecten die zich in een van de volgende statussen bevinden, worden altijd gemarkeerd als Op doel, ongeacht de datum van de taken en de voortgang ervan:
  >
  >* Idea
  >* Gevraagd
  >* Goedgekeurd
  >* Geweigerd

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set the Condition Type for a project</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted here and moved it to a separate article: /Content/Manage work/Projects/Manage projects/set-condition-type-for-project.htm)</p>
<ol>
<li value="1">Go to the project for which you want to update the Condition Type. </li>
<li value="2"> <p>  Click the <strong>More</strong> menu <img src="assets/qs-more-menu.png"> to the right of the project name, then click <strong>Edit</strong>.  <br> </p> </li>
<li value="3">In the <strong>Condition Type</strong> field, choose one of the following:
<ul>
<li><p><strong>Manual:</strong> The project owner sets the Condition on the project manually.</p><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In this case, the project owner can update the Condition of the project in the project header, or the Project Details section. </p></li>
<li><p><strong>Progress Status:</strong> Workfront sets the Condition based on the Progress Status of the project. <br></p></li>
</ul></li>
<li value="4">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Hoe Workfront de Projectvoorwaarde bijwerkt op basis van de Voortgangsstatus

Wanneer het Type van Voorwaarde van het project aan Handboek wordt geplaatst, kunt u bepalen wat de Voorwaarde van het project onafhankelijk van de Voortgangsstatus van het project is.

Nochtans, adviseren wij dat u het Type van Voorwaarde van het project aan de Status van de Voortgang plaatst zodat u een duidelijke aanwijzing kunt hebben van wat de ware vooruitgang van het project is, gebaseerd op de vooruitgang van uw taken. Voor informatie over hoe Workfront de Voortgangsstatus van projecten berekent, zie [ Overzicht van de Status van de Voortgang van het Project ](../../../manage-work/projects/planning-a-project/project-progress-status.md).

In dit geval kunnen de waarden voor de projectvoorwaarde als volgt zijn:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Projectvoorwaarde</strong></td> 
   <td><strong>Voortgang van project</strong></td> 
   <td><strong>Workfront Condition Indicator</strong></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Op doel</td> 
   <td>Wanneer de Voortgangsstatus van het project van Op Tijd, de Voorwaarde van het project <strong> op Doel </strong> is. </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risico</td> 
   <td>Wanneer de Voortgangsstatus van het project <strong> Achter </strong> of <strong> bij Risico </strong> is, dan is de Voorwaarde van het project <strong> bij Risico </strong>.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>In problemen</td> 
   <td>Wanneer de Voortgangsstatus van het project <strong> Late </strong> is, dan is de Voorwaarde van het project <strong> in Problemen </strong>. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>De voorwaarden kunnen voor uw milieu worden aangepast, zodat kunt u meer dan drie opties voor Voorwaarde in uw milieu vinden. De namen van de Voorwaarden kunnen verschillen van de hierboven vermelde. Voor informatie over het aanpassen van Voorwaarden in, zie het artikel [ creeer of geef een douanevoorwaarde ](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md) uit.

## Rapport over de Voorwaarde van het Project, de Update van de Voorwaarde van het Project, en de Nota van de Laatste Voorwaarde

In de mening van een projectrapport, kunt u de volgende gebieden met betrekking tot de Voorwaarde van het project tonen:

* **Voorwaarde van het Project:** toont de huidige Voorwaarde van het project.
* **Update van de Voorwaarde van het Project**: Toont de meest recente update die de projecteigenaar in de updatestroom van het project, samen met de nieuwe Voorwaarde heeft verstrekt.\
  De commentaren die op de updates van de Voorwaarde worden gemaakt worden niet getoond in de **kolom van de Update van de Voorwaarde**; slechts wordt de belangrijkste update getoond.

* **Laatste Nota van de Voorwaarde**: Toont de update het laatst ingegaan op een voorwerp door de eigenaar van het voorwerp. Dit veld is handig om de meest recente activiteit of interactie van de eigenaar van een object weer te geven.\
  De **laatste kolom van de Nota van de Voorwaarde** is leeg als de notitietekst van de laatste nota van een voorwerp is geschrapt. Wanneer een nieuwe notitie op het object wordt ingevoerd, wordt deze de laatste notitie en wordt deze opnieuw weergegeven in de kolom.

Voor informatie over hoe te om een rapport tot stand te brengen, zie het artikel [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.
