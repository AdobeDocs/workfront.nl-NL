---
product-area: projects
navigation-topic: manage-projects
title: Een project kopiëren
description: U kunt een project kopiëren in plaats van er zelf een te maken. U kunt slechts één project tegelijk kopiëren. U kunt projecten niet bulksgewijs kopiëren.
author: Alina
feature: Projects, Work Management
role: User
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 0%

---

# Een project kopiëren

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

U kunt een project kopiëren in plaats van er zelf een te maken. U kunt slechts één project tegelijk kopiëren. U kunt projecten niet bulksgewijs kopiëren.

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
>* Portfolio en programma
>* Scorecard
>* Standaardgegevens taak (goedkeuringsproces standaardtaak, Standaard aangepaste Forms taak)
>
> De datums van de oorspronkelijke taken van de projecten worden gekopieerd naar het nieuwe project. U moet de begin- of voltooiingsdatum van het project (afhankelijk van de planningsmodus) wijzigen om de datums van de taken bij te werken. De beperkingen van de taak zouden u kunnen verhinderen de data op het project te veranderen.

## Toegangsvereisten

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>View permissions or higher to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-abonnement*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-licentie*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraties op toegangsniveau*</strong> </td> 
   <td> <p>Toegang tot projecten bewerken met de mogelijkheid om <span>en kopiëren</span> projecten</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objectmachtigingen</strong> </p> </td> 
   <td> <p>Machtigingen of hoger weergeven voor het project</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Eén project kopiëren

Het kopiëren van een project kopieert ook sommige informatie van het originele project aan het nieuwe project. U kunt ook opgeven welke items tijdens het kopiëren niet naar het nieuwe project moeten worden gekopieerd.

Een project kopiëren:

1. Ga naar het project dat u wilt kopiëren en klik **Meer** pictogram ![](assets/qs-more-menu.png) rechts van de projectnaam

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   of

   Ga naar een projectlijst of rapport en selecteer een project, dan klik **Meer** pictogram ![](assets/qs-more-menu.png) boven aan de lijst.

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. Klikken **Kopiëren**.

1. Werk de naam van het nieuwe project bij.

   Standaard is de nieuwe naam **Kopie van `<Original project name>`.**

   ![](assets/copy-project-box-nwe-350x276.png)

1. Selecteer **Status** voor het nieuwe project.

   Standaard worden de **Status** komt overeen met die van het oorspronkelijke project.

1. (Optioneel) Schakel de items uit die u niet naar het nieuwe project wilt kopiëren. In de volgende tabel wordt beschreven wat er gebeurt wanneer u de selectie van de items opheft:


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alles selecteren</td> 
      <td> <p>Hiermee selecteert u alle opties en wist u alle velden en objecten die in het nieuwe project worden vermeld.</p> <p><b>TIP</b>

   Selectie opheffen <strong>Alles selecteren</strong> deselecteert alle items. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Toewijzingen</td> 
      <td>Hiermee worden alle project- en taaktoewijzingen verwijderd</td> 
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
       </ul> <p><b>OPMERKING</b>

   De aangepaste formulieren blijven gekoppeld aan de taken, uitgaven, documenten en het project, maar de informatie in de aangepaste velden van de formulieren wordt niet naar het nieuwe project gekopieerd. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Documenten</td> 
      <td> <p>Hiermee verwijdert u alle gegevens op het documenttabblad, inclusief documentversies, gekoppelde documenten en mappen.</p> <p>Standaard kunnen proefdrukken en goedkeuringen van documenten niet naar een ander project worden gekopieerd. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alle voorgangers</td> 
      <td> <p>Verwijdert alle voorgangersverhoudingen tussen de taken op het project. </p> <p><b>TIP</b>

   Predecessors voor meerdere projecten brengen nooit over naar het nieuwe project, ongeacht of dit is geselecteerd of niet. </p> </td>
   </tr>

<tr> 
      <td role="rowheader">Geforceerde uren</td> 
      <td> <p>Verwijdert de uren die in het gebied van de Planning van het Middel van het BedrijfsGeval van het project in de begroting worden opgenomen uit het gekopieerde project.</p>

<b>OPMERKING</b>

De uren die in de begroting zijn opgenomen met de Scenario Planner worden nooit naar het nieuwe project gekopieerd omdat het nieuwe project niet gekoppeld is aan een initiatief in de Scenario Planner. Zie voor meer informatie <a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">De middelen van de begroting in BedrijfsGeval die Scenario Planner gebruiken</a>
</tr></td>
    <tr> 
      <td role="rowheader">Financiële informatie</td> 
      <td> <p>Hiermee verwijdert u de informatie in de volgende gebieden: </p> 
       <ul> 
        <li>Subtabblad Financiën van het project</li> 
        <li> Gepland voordeel in de bedrijfscase</li> 
        <li>Financiële informatie uit alle taken<br></li> 
       </ul> <p>Voor meer informatie over het subtabblad Projectfinanciering raadpleegt u <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">Informatie beheren in het gebied Projectfinanciering</a>.</p> </td> 
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

1. Klikken **Kopiëren** om een kopie van het project te maken.

   Dit leidt tot een nieuw project dat aan het project gelijkaardig is u kopieerde.

   U kunt wijzigingen aanbrengen in het nieuwe gekopieerde project, zoals taaktoewijzingen controleren of tijdlijnen aanpassen.
