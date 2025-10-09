---
title: Een milestone-pad maken
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Als beheerder van Adobe Workfront, kunt u milestone wegen tot stand brengen die dan op om het even welk project in het systeem kunnen worden toegepast. De wijzigingen die u aanbrengt in paden met mijlpalen op dit gebied, zijn van invloed op het hele Workfront-systeem.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: e717e095f1995dbed0232789616d42492156d843
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 0%

---

# Een milestone-pad maken

<!--Audited: 07/2024-->

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

Als beheerder van Adobe Workfront, kunt u milestone wegen tot stand brengen die dan op om het even welk project in het systeem kunnen worden toegepast. De wijzigingen die u aanbrengt in paden met mijlpalen op dit gebied, zijn van invloed op het hele Workfront-systeem.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
   <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p></td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mijlpalen en mijlpaden

U kunt de belangrijkste taken in een project met vooraf bepaalde mijlpalen associëren. Deze functie kan managers en andere belanghebbenden een overzicht op hoog niveau geven van de voortgang van een project.

De som van alle vooraf gedefinieerde mijlpalen wordt een milestone-pad genoemd.

De eerste stap bij het bouwen van een mijlpaden is het identificeren van de mijlpalen en het vaststellen van de mijlpalen. Omdat u een mijlpaden aan veelvoudige projecten kunt associëren, moeten de mijlpaalstappen algemene fasen of stadia van om het even welk project zijn.

Voor meer informatie over hoe u een milestone weg met een project en een mijlpaal met een taak kunt associëren, zie [ Geassocieerde mijlpalen met taken ](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

## Een milestone-pad maken

{{step-1-to-setup}}

1. Klik **Processen** > **Mijlsteenwegen**.
1. Klik **Nieuwe Weg van de Mijlpaal.**

   Het vak Nieuw milestone-pad wordt geopend.

   ![ Nieuwe de wegdoos van de mijlpaal ](assets/new-milestone-path-box.png)

1. Klik **BasisInfo** in het linkerpaneel.

   Werk de volgende gegevens bij:

   <table style="table-layout:auto">
    <tr>
      <td>Padnaam mijlpaal</td>
       <td>Voer een naam in voor het milestone-pad.</td>
    </tr>
    <tr>
      <td>Beschrijving</td>
      <td>Voer een beschrijving in om het pad van de mijlpaal te definiëren.</td>
    </tr>
    <tr>
       <td>Is actief</td>
      <td>Schakel dit selectievakje in als u het milestone-pad actief wilt maken. Andere gebruikers kunnen dit pad vinden en het aan projecten koppelen wanneer ze projecten maken of bewerken. Niet-actieve mijlpaden kunnen niet aan projecten worden gekoppeld. Dit is standaard ingeschakeld.</td>
    </tr>
    <tr>
      <td>Groepen</td>
      <td>Selecteer de groepen die worden vermeld om gebruikers in deze groepen toe te staan om deze mijlpaden op hun projecten te zien en toe te passen. De thuisgroep van de gebruiker die het milestone-pad invoert, is standaard geselecteerd.</td>
    </tr>
   </table>

1. Klik **Mijlpalen** in het linkerpaneel.

1. Klik **Nieuwe rij** om mijlpalen aan de weg toe te voegen.
1. Werk de volgende gegevens bij:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Naam</td> 
      <td>Typ beschrijvende namen voor elke mijlpaal.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschrijving</td> 
      <td>Typ een beschrijving voor de mijlpaal.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kleur</td> 
      <td> <p>Kies een kleur die u aan uw mijlpaal wilt koppelen. </p> <p>Als u geen kleur kiest, kiest het systeem de laatste kleur die in een milestone-pad wordt gebruikt. We raden u aan voor elke mijlpaal een unieke kleur te kiezen. De kleur wordt gebruikt voor visuele en rapportagedoeleinden.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Sleep elke mijlpaal om deze opnieuw te rangschikken.
1. Klik **creëren Weg van de Mijlpaal** om uw veranderingen te bewaren.

   Uw milestone-pad kan aan een project worden gekoppeld.

   Voor meer informatie over hoe te om milestone wegen aan projecten en mijlpalen aan taken te associëren, zie [ mijlpalen met taken ](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md) associëren.

1. (Facultatief) van de lijst van de Wegen van de Mijlsteen, selecteer één mijlpaal, dan klik **pictogram** uitgeven pictogram ![ om de milestone weg te openen en zijn informatie uit te geven.](assets/edit-icon.png)
1. (Facultatief) klik het **pictogram van de Uitvoer van de Uitvoer** ![, dan uitgezocht van de volgende formaten om de lijst van de milestone weg naar een dossier uit te voeren:](assets/export-icon.png)

   * PDF
   * Excel
   * Excel (xlsx)
   * Door tabs gescheiden

1. (Facultatief) selecteer één of verscheidene mijlpalen in de milestone lijst, dan klik het **pictogram van de Schrapping** ![ om het te schrappen.](assets/delete-icon.png)
1. Klik **ja, schrap het**.

   De mijlpaal wordt verwijderd en kan niet worden hersteld. Het milestone-pad wordt verwijderd uit elk project dat eerder aan het project is gekoppeld en alle mijlpalen worden verwijderd uit de taken die aan het project zijn gekoppeld.

   Verwijderde mijlpalen kunnen niet worden hersteld.


## Details van mijlpaden weergeven in een projectrapport

U kunt de details van een mijlpaden in een projectrapport bekijken.

U moet een milestone-pad aan een project koppelen voordat u de details in een projectrapport kunt zien.

Voor informatie over het associëren van mijlpaden aan projecten, zie [ projecten ](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md) uitgeven.

{{step1-to-reports}}

1. Klik **Nieuw Rapport**, dan klik **Project**.
1. Klik **toevoegen Kolom**.
1. In **toon in dit kolom** gebied, begin **Weg van de Mijlsteen** te typen, dan klik **Naam van de Weg van de Mijlsteen** wanneer het toont.
1. (Facultatief) klik **Filters** en voeg de volgende filter aan het rapport toe: **identiteitskaart van de Weg van de Mijlpaal van het Project is niet leeg**.

   Het filter zorgt ervoor dat u slechts projecten toont die met een milestone weg in het rapport worden geassocieerd.

1. Klik **sparen + Sluiten**.
1. Voeg een naam voor uw rapport toe, dan klik **van toepassing zijn**.

   De vertoningen van het projectrapport. De mijlpaden verbonden aan elke projectvertoning in de laatste kolom van het rapport.
1. Klik de naam van een milestone weg in de laatste kolom van het rapport.

   De details van het pad van de mijlpaal worden weergegeven.

   ![ de wegdetails van de mijlpaal van projectrapport ](assets/milestone-details-from-project-report.png)

   De detailpagina van het milestone-pad bevat de volgende informatie:

   * Naam, id en beschrijving van milestone-pad
   * Padgroepen van mijlpaal
   * Mijlsteennamen, beschrijvingen, kleuren en kleurenpictogrammen

1. (Optioneel) Klik op **Terug** om terug te gaan naar het projectrapport.



