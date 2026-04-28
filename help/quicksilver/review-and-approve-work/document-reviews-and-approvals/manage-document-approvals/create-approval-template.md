---
product-area: documents
navigation-topic: approvals
title: Een sjabloon voor een goedkeuringswerkstroom maken voor documenten
description: U kunt goedkeuringssjablonen maken om het goedkeuringsproces te stroomlijnen.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 02d2b8fce60b469b8ea16c4302035371bed04175
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# Een sjabloon voor een goedkeuringswerkstroom maken voor documenten

In het gedeelte Workfront Setup kunnen gebruikers met een standaardlicentie herbruikbare goedkeuringssjablonen maken. Nadat u de goedkeuringssjablonen hebt gemaakt, kunt u deze toepassen op elementen in het gebied Documenten van een object.
>[!IMPORTANT]
>
>De inhoud van dit artikel verwijst naar de functionaliteit voor bijgewerkte documentgoedkeuring die alleen beschikbaar is voor specifieke accounts. Voor informatie over standaardgoedkeuringsprocessen, zie de artikelen die in [&#x200B; worden vermeld goedkeuringen van het Werk &#x200B;](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td><p>Elk Workfront-pakket om goedkeuringen te beheren met behulp van verouderde Workfront-opslag</p>
<p>Elk workflowpakket om goedkeuringen te beheren met behulp van Adobe Enterprise Storage</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standaard</p> 
   <p>Plan</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++
ß

## Een goedkeuringssjabloon maken

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Overzicht en Goedkeuring** > **Malplaatjes van de Goedkeuring**.
1. Klik **Nieuw Malplaatje** op de rechterkant van de pagina.

1. Vul de volgende gegevens in:

   <table>
     <tr>
   <td><strong>Sjabloonnaam</strong></td>
   <td>Voeg een sjabloonnaam toe. </td>
   </tr>
   <tr>
   <td><strong>Werkgebiednaam</strong></td>
   <td>Voeg een werkgebiednaam toe. U kunt de naam in iets beschrijvender veranderen, zoals <em> Eerste Overzicht </em> of <em> Definitieve Goedkeuring </em>.</td>
   </tr>
   <tr>
   <td><strong>Namen of e-mails toevoegen</strong></td>
   <td>Typ een gebruiker- of teamnaam die u als fiatteur of revisor wilt toevoegen. Als u alleen revisoren hebt, worden deze op de hoogte gesteld en hebben ze de mogelijkheid de revisie te voltooien, maar er wordt geen beslissing vereist of genomen.</td>
   </tr>
   <tr>
   <td><strong>Eén beslissing vereist (facultatief)</strong></td>
   <td>De eerste persoon die een besluit neemt, voltooit het stadium.</td>
   </tr>
   <tr>
   <td><strong>Werkdagen tot vervaldatum</strong></td>
   <td>Kies hoeveel werkdagen tot de goedkeuring moet worden uitgevoerd nadat een fase is geactiveerd.</td>
   </tr>
   </table>

1. (Optioneel) Herhaal de vorige stap om zo nodig extra stappen toe te voegen.

   >[!NOTE]
   >
   >Als u meerdere fasen toevoegt, gaat de goedkeuringswerkstroom verder in de volgorde waarin de fasen worden weergegeven. Wanneer alle vereiste beslissingen worden genomen, begint de volgende fase en wordt de vorige fase vergrendeld.

   ![&#x200B; de details van het Document &#x200B;](assets/new-stage.png)

1. Klik **sparen**.

Nadat de sjabloon is gemaakt, kan deze worden toegepast op documenten in het gebied Documenten van een object om het formele beoordelings- en goedkeuringsproces in Workfront te starten.



<!--
 Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)
-->
