---
title: Overzicht van het type Projectvoorwaarde en Voorwaarde
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: De projectvoorwaarde is een visuele vertegenwoordiging van hoe het project vordert. Het is een te rapporteren variabele die wordt bepaald door het verband tussen de geplande, geplande en geschatte data van het project.
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: e4de185f172b173dcc3ad966afa69ffb3bc479eb
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
   * Automatisch door Adobe Workfront, wanneer het Type van Voorwaarde van het project aan de Status van de Voortgang wordt geplaatst. De status van de voortgang van het project wordt bepaald door de voortgang van de taken van het project. Voor informatie over de Voortgangsstatus van het project, zie [Overzicht van voortgang van project](../../../manage-work/projects/planning-a-project/project-progress-status.md).

  Voor informatie over hoe te om het Type van Voorwaarde van het project bij te werken, zie [Stel het Condition Type van een project in](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md).

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

Nochtans, adviseren wij dat u het Type van Voorwaarde van het project aan de Status van de Voortgang plaatst zodat u een duidelijke aanwijzing kunt hebben van wat de ware vooruitgang van het project is, gebaseerd op de vooruitgang van uw taken. Voor informatie over hoe Workfront de status van voortgang van projecten berekent, raadpleegt u [Overzicht van voortgang van project](../../../manage-work/projects/planning-a-project/project-progress-status.md).

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
   <td> </td> 
  </tr> 
  <tr> 
   <td>Op doel</td> 
   <td>Wanneer de Voortgangsstatus van het project van Op Tijd, de Voorwaarde van het project is <strong>Op doel</strong>. </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risico</td> 
   <td>Wanneer de Voortgangsstatus van het project is <strong>Achter</strong> of <strong>Risico</strong>dan is de voorwaarde van het project <strong>Risico</strong>.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>In problemen</td> 
   <td>Wanneer de Voortgangsstatus van het project is <strong>Late</strong>dan is de voorwaarde van het project <strong>In problemen</strong>. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>De voorwaarden kunnen voor uw milieu worden aangepast, zodat kunt u meer dan drie opties voor Voorwaarde in uw milieu vinden. De namen van de Voorwaarden kunnen verschillen van de hierboven vermelde. Raadpleeg het artikel voor informatie over het aanpassen van Voorwaarden in [Een aangepaste voorwaarde maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Rapport over de Voorwaarde van het Project, de Update van de Voorwaarde van het Project, en de Nota van de Laatste Voorwaarde

In de mening van een projectrapport, kunt u de volgende gebieden met betrekking tot de Voorwaarde van het project tonen:

* **Projectvoorwaarde:** Toont de huidige Voorwaarde van het project.
* **Bijwerken van projectvoorwaarde**: Toont de meest recente update die de projecteigenaar in de updatestroom van het project, samen met de nieuwe Voorwaarde heeft verstrekt.\
  Opmerkingen die zijn gemaakt bij Voorwaarde-updates worden niet weergegeven in het dialoogvenster **Update van voorwaarde** kolom; alleen de hoofdupdate wordt weergegeven.

* **Opmerking laatste voorwaarde**: geeft de laatste update weer die de eigenaar van het object op een object heeft ingevoerd. Dit veld is handig om de meest recente activiteit of interactie van de eigenaar van een object weer te geven.\
  De **Opmerking laatste voorwaarde** is leeg als de notitietekst van de laatste notitie van een object is verwijderd. Wanneer een nieuwe notitie op het object wordt ingevoerd, wordt deze de laatste notitie en wordt deze opnieuw weergegeven in de kolom.

Raadpleeg het artikel voor informatie over het maken van een rapport [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
