---
product-area: projects
navigation-topic: manage-projects
title: Een project kopiëren
description: U kunt een project kopiëren in plaats van er zelf een te maken. U kunt slechts één project tegelijk kopiëren. U kunt geen projecten in bulk kopiëren.
author: Alina
feature: Projects, Work Management
role: User
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: 93db334537b5ec12dc0c77d51f8b2d83d8348f3d
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 0%

---

# Een project kopiëren

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

<!-- Audited: 5/2025 -->

U kunt een project kopiëren van een bestaand project in plaats van een geheel nieuw project te maken, zodat u tijd bespaart.

Houd er rekening mee dat projecten niet in bulk kunnen worden gekopieerd.

>[!IMPORTANT]
>
>De volgende items worden nooit van een bestaand project naar een nieuw project gekopieerd:
>
>* Problemen
>* Factureringstarieven
>* Factureringsgegevens
>* Notities
>* Uren
>* Predecessors voor meerdere projecten
>* Geforceerde uren
>
>De volgende punten worden altijd gekopieerd van een bestaand project aan nieuwe:
>
>* Taken
>* Sjabloon
>* Risico&#39;s
>* Informatie over wachtrijinstellingen
>* Portfolio en Programma
>* Scorecard
>* Standaardgegevens taak (goedkeuringsproces standaardtaak, Standaard aangepaste Forms taak)
>
> De data van de oorspronkelijke projecttaken worden gekopieerd naar het nieuwe project. U moet de begin- of voltooiingsdatum van het project (afhankelijk van de planningsmodus) wijzigen om de taakdatums bij te werken. De beperkingen van de taak zouden u kunnen verhinderen de data op het project te veranderen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.
U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-pakket</p> </td>  
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-licentie</p> </td> 
   <td> <p>Standard</p> 
   <p>Plan</p>
      </td> 
  </tr> 
     <td>Configuraties op toegangsniveau </td> 
   <td> <p>Toegang tot projecten bewerken met de mogelijkheid projecten te maken en te kopiëren</p> </td> 
  </tr>

<td> <p>Objectmachtigingen </p> </td> 
   <td> <p>Machtigingen of hoger weergeven voor het project</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
 
 <table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license</p> </td> 
   <td> <p>New: Standard </p> 
   <p>Or</p>
   <p>Current: Plan </p>
   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level configurations </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>View permissions or higher to the project</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Overwegingen

* Er geldt een verwerkingslimiet van 5 minuten voor het kopiëren van een project. Als aan het project een groot aantal documenten is gekoppeld en er geen kopie van wordt gemaakt, moet u mogelijk enkele documenten verwijderen en het opnieuw proberen.

## Eén project kopiëren

Het kopiëren van een project kopieert ook sommige informatie van het originele project aan het nieuwe project. U kunt ook opgeven welke items tijdens het kopiëren niet naar het nieuwe project moeten worden gekopieerd.

Een project kopiëren:

{{step1-to-projects}}

1. Selecteer het project dat u van de projectlijst wilt kopiëren, dan klik **Meer** pictogram ![ Meer menu ](assets/more-icon.png) rechts van de projectnaam.

   of

   Ga naar een projectlijst of een rapport en selecteer een project, dan klik het **Meer** pictogram ![ Meer menu ](assets/more-icon.png) bij de bovenkant van de lijst.

1. In **Meer** drop-down menu, klik **Exemplaar**. Het **Exemplaar van [ de dialoogvakje van de Naam van het Project]** verschijnt.

1. (Facultatief) werk de **Naam van het Project** bij. Door gebrek, is de nieuwe naam **Exemplaar van [ Oorspronkelijke projectnaam]**.

   ![ het projectvakje van het Exemplaar ](assets/copy-of-project-box.png)

1. Selecteer a **Status**. Standaard is de status van het oorspronkelijke project geselecteerd.

1. (Optioneel) Schakel de items uit die u niet naar het nieuwe project wilt kopiëren. In de volgende tabel wordt beschreven wat er gebeurt wanneer u de selectie van de items opheft:


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alles selecteren</td> 
      <td> <p>Hiermee selecteert u alle opties en wist u alle velden en objecten die in het nieuwe project worden vermeld. </p>

   <p> Als u deze optie uitschakelt, worden alle items uitgeschakeld. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Toewijzingen</td> 
      <td>Hiermee verwijdert u alle project- en taaktoewijzingen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Voortgang</td> 
      <td>Hiermee verwijdert u de voortgang van alle taken en geeft u deze weer als Nieuw. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aangepaste gegevens</td> 
      <td> <p>Hiermee verwijdert u de informatie uit het aangepaste formulier over het project en de informatie over de aangepaste formulieren die aan de volgende items zijn gekoppeld:</p> 
       <ul> 
        <li>Taken</li> 
        <li>Uitgaven</li> 
        <li> Documenten</li> 
       </ul> 
      <p>De aangepaste formulieren blijven gekoppeld aan de taken, uitgaven, documenten en projecten, maar de gegevens in de aangepaste velden van het formulier worden niet naar het nieuwe project gekopieerd. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenten</td> 
      <td> <p>Hiermee verwijdert u alles op het tabblad Documenten, inclusief documentversies, gekoppelde documenten en mappen.</p> <p>Standaard kunnen proefdrukken en goedkeuringen van documenten niet naar een ander project worden gekopieerd. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alle voorgangers</td> 
      <td> <p>Verwijdert alle voorgangersverhoudingen tussen de taken op het project. </p> <p>

   Predecessors voor meerdere projecten brengen nooit over naar het nieuwe project, ongeacht of dit is geselecteerd of niet. </p> </td>
   </tr>

<tr> 
      <td role="rowheader">Geforceerde uren</td> 
      <td> <p>Verwijdert de uren die in het gebied van de Planning van het Middel van het BedrijfsGeval van het project in de begroting worden opgenomen uit het gekopieerde project.</p> 
    <p>
   De uren die in de begroting zijn opgenomen met de Scenario Planner worden nooit naar het nieuwe project gekopieerd omdat het nieuwe project niet gekoppeld is aan een initiatief in de Scenario Planner. Voor meer informatie, zie {de middelen van de Begroting in het BedrijfsGeval gebruikend de Planner van het Scenario <a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md"></a></p>
   </tr></td>
    <tr> 
      <td role="rowheader">Financiële informatie</td> 
      <td> <p>Hiermee verwijdert u de informatie in de volgende gebieden: </p> 
       <ul> 
        <li>Subtabblad Financiën van het project</li> 
        <li> Gepland voordeel in de bedrijfscase</li> 
        <li>Financiële informatie uit alle taken<br></li> 
       </ul> <p>Voor meer informatie over subtab van de projectfinanciering, zie <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref"> informatie in het gebied van de projectfinanciering beheren </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Goedkeuringsproces</td> 
      <td>Verwijdert alle goedkeuringen verbonden aan de taken of het project. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Herinneringsmeldingen</td> 
      <td> Hiermee verwijdert u de herinneringsmeldingen die aan de taken of het project zijn gekoppeld. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uitgaven</td> 
      <td>Verwijdert uitgaven verbonden aan de taken of het project. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Machtigingen</td> 
      <td> Verwijdert toestemmingen aan alle gebruikers op de taken of het project.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **project van het Exemplaar**. Het gekopieerde project wordt gemaakt.
