---
product-area: documents
navigation-topic: approvals
title: Een sjabloon voor een goedkeuringswerkstroom maken voor documenten
description: U kunt goedkeuringssjablonen maken om het goedkeuringsproces te stroomlijnen.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
source-git-commit: 6d6ac026bb2aa10ba3e678fb7e0f32dc95d0405f
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Een sjabloon voor een goedkeuringswerkstroom maken voor documenten

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Het is beschikbaar slechts in het milieu van de Sandbox van de Voorproef.</span>

In het gedeelte Workfront Setup kunnen gebruikers met een standaardlicentie herbruikbare goedkeuringssjablonen maken. Zodra gecreeerd, kunnen de Malplaatjes van de Goedkeuring op activa in het gebied van Documenten van een project, een taak, of een kwestie worden toegepast.

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
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p> 
   <p>Plan</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++




## Een goedkeuringssjabloon maken in uw productieomgeving

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Overzicht en Goedkeuring** > **Malplaatjes van de Goedkeuring**.
1. Klik **Nieuw Malplaatje** op de rechterkant van de pagina.
1. Geef de volgende informatie op:

   | Sjabloonnaam | Typ een naam voor deze sjabloon. |
   |----------------------------|---|
   | **(Optioneel) Tijdlijn** | Voer de tijdlijn in dagen in. De deadline voor goedkeuring wordt berekend vanuit dit veld zodra de sjabloon op een actief wordt toegepast. |
   | **voegt fiatteurs of recensenten** toe | Typ de naam van gebruikers of teams en wijs deze vervolgens aan als controleur of fiatteur. |

1. Klik **sparen**.



<div class="preview">

## Een goedkeuringssjabloon maken in uw voorvertoningsomgeving

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

Zodra het malplaatje wordt gecreeerd, kan het op documenten in het gebied van Documenten van een project, een taak, of een kwestie worden toegepast om het formele overzicht en goedkeuringsproces in Workfront te beginnen.

</div>


<!-- Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)-->
