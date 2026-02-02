---
product-area: projects
navigation-topic: manage-tasks
title: Taken kopiëren en dupliceren
description: U kunt een taak van een project aan een ander project kopiëren, of u kunt een taak binnen het zelfde project dupliceren.
author: Alina
feature: Work Management
exl-id: daf89062-cf58-4c39-83ff-727d969a9630
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '1744'
ht-degree: 0%

---

# Taken kopiëren en dupliceren

U kunt een taak van een project aan een ander project kopiëren, of u kunt een taak binnen het zelfde project dupliceren.

U kunt een of meer taken of bovenliggende taken tegelijk kopiëren of dupliceren.

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
   <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot taken en projecten bewerken</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een taak beheren</p> <p>Contribute of hoger machtigingen voor het project</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a task</p> <p>Contribute or higher permissions to the project</p> 
   <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Overwegingen bij het kopiëren van taken

Houd rekening met het volgende wanneer u een taak kopieert:

* Wanneer u een taak van één project aan een ander kopieert, zouden de taakdata kunnen worden herberekend. Bij de herberekening wordt rekening gehouden met het tijdschema dat voor het nieuwe project wordt gebruikt en met het tijdschema voor het project op basis van informatie.
* Aangepaste formulieren worden samen met de taak gekopieerd. De gegevens in de aangepaste velden worden alleen naar de gekopieerde taken overgedragen wanneer u Aangepaste gegevens kopieert wanneer u deze taak kopieert.
* U kunt bepaalde onderdelen die aan de taak zijn gekoppeld tijdens het kopiëren naar de gekopieerde taak kopiëren. De volgende objecten worden echter standaard niet overgedragen naar de gekopieerde taak:
   * Problemen
   * Aangemeld aantal uren
   * Opmerkingen van gebruikers <!--not sure about this, enable only if requested by users and verified by Product: System activity comments transfer to the new task if they relate to information that you specifically select to be copied. For example, if you select to copy Expenses to the new task, system comments that identify adding expenses to the task will transfer to the copied task. -->
* De volgende items worden standaard naar de gekopieerde taak verplaatst:

   * De mijlpalen worden overgebracht naar de gekopieerde taak en uit de originele taak verwijderd.
   * Subtaken worden overgedragen naar de nieuwe taak.

* U kunt één taak tegelijk kopiëren of meerdere taken tegelijk wanneer u taken in een lijst bewerkt.

## Taken in een lijst kopiëren {#copy-tasks-in-a-list}

1. Ga naar het project dat de taak of de taken bevat die u wilt kopiëren.

   of

   Ga naar een taakrapport.

1. (Voorwaardelijk) klik **Taken** in het linkerpaneel, als u het project opende dat de taken bevat.
1. Klik de **pictogram van de Wijze van het Plan** van de Lijst of sparen wijzepictogram ![, en zorg ervoor dat de ](assets/qs-list-mode-or-save-mode-icon-small.png) Autosave **optie wordt toegelaten.**

   ![ Autosave pictogram op en benadrukte ](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >U kunt taken alleen in een lijst kopiëren wanneer u uw wijzigingen automatisch opslaat. Voor informatie over besparingsopties wanneer het uitgeven van taken, zie [ taken in een lijst ](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md) uitgeven.

1. Selecteer de taak of taken die u wilt kopiëren en voer een van de volgende handelingen uit:

   * Klik het **Meer menu** bij de bovenkant van de taaklijst, dan klik **Exemplaar aan**.
   * Klik de geselecteerde taken met de rechtermuisknop aan, dan klik **Exemplaar aan**.
   * Wanneer het selecteren van één taak, klik **Meer** menu ![ Meer pictogram op taaklijst ](assets/more-icon-task-list.png) naast de taaknaam in de lijst, dan klik **Exemplaar aan**.

   ![ taak van het Exemplaar in lijst ](assets/copy-task-in-list-nwe-350x131.png)

1. Ga met het kopiëren van de taak voort, zoals die in de sectie [ wordt beschreven Kopieer een taak op het taakniveau ](#copy-a-task-at-the-task-level) die met Stap 4 begint.

   <!--
      (NOTE: is this still accurate?!)
   -->

## Een taak kopiëren op taakniveau {#copy-a-task-at-the-task-level}

Naast het kopiëren van taken in een lijst met taken kunt u ook een taak kopiëren nadat u deze hebt geopend.

1. Zoek naar een taak in je Workfront-systeem.
1. Klik op de naam van de taak om deze te openen.
1. Klik **Meer** drop-down menu ![ Meer menu ](assets/qs-more-menu.png) naast de naam van de taak, dan klik **Exemplaar aan**.

   ![ het Exemplaar van de Taak aan optie op het taakniveau ](assets/taskcopy-to-at-the-task-level-nwe-350x200.png)

   Het vak Taak kopiëren wordt weergegeven.

1. (Facultatief) werk de **Naam van de Taak** bij.

   >[!TIP]
   >
   >Dit veld is grijs en kan niet worden bewerkt als u ervoor kiest meerdere taken in een lijst te kopiëren. U kunt de muisaanwijzer boven het veld Taaknaam en een lijst met alle geselecteerde taken weergeven.
   >
   >![ taak van het Exemplaar in een veelvoudige takendoos ](assets/copy-task-multiple-tasks-box-with-list-of-task-names-nwe-350x130.png)

1. Typ de naam van het **Project van de Bestemming** waar u de taak in het **Uitgezochte gebied van het Project van de Bestemming** wilt kopiëren.

   >[!TIP]
   >
   >* De naam van het project is hoofdlettergevoelig.
   >* U kunt ook het Referentienummer typen of de id van het project invoeren. Hierdoor kunt u projecten met identieke namen beter van elkaar onderscheiden.
   >* Er worden slechts 100 projecten weergegeven in de lijst.

   De huidige projectnaam wordt standaard weergegeven. Als u de taak binnen het zelfde project wilt kopiëren, verlaat dit gebied onveranderd.

1. (Voorwaardelijk) klik **verzoektoegang** om toegang tot het project te verzoeken, als u geen toegang tot het geselecteerde project hebt.
1. (Voorwaardelijk) blijf de taak aan het geselecteerde bestemmingsproject kopiëren zonder toegang te vragen als u toegang hebt om taken aan één van de taken op het bestemmingsproject toe te voegen.

   ![ toegang van het de taakverzoek van het Exemplaar van project ](assets/copy-task-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >De gelijkaardige berichten tonen als het geselecteerde project in afwachting van goedkeuring, voltooid, of dood is, wanneer de beheerder van Workfront het toevoegen van taken aan deze projecten verhindert. Voor meer informatie, zie [ systeem-brede projectvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

1. Klik **Opties** in het linkerpaneel, dan schrap de taakattributen die u niet met de taak wilt kopiëren. Alle opties zijn standaard geselecteerd.

   >[!TIP]
   >
   >Het selecteren dan het deselecteren van **selecteert allen** deselecteert alle opties.

   Schakel een van de volgende opties uit als u deze niet wilt overbrengen naar de gekopieerde taak. In de volgende tabel wordt beschreven wat er gebeurt wanneer de opties zijn uitgeschakeld:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Restrictie</td> 
      <td> <p>De taakbeperking wordt geplaatst aan zo spoedig mogelijk of zo laat mogelijk gebaseerd op het plaatsen van de Wijze van het projectprogramma.</p> <p> Als deze optie is geselecteerd, wordt de huidige beperking van de taak overgedragen naar de gekopieerde taak. </p> <p>Opmerking: wanneer een taak met datumspecifieke beperkingen naar een ander project wordt verplaatst of gekopieerd en de beperkingsdatums van de taak buiten de datums van het nieuwe project vallen, wordt de taakbeperking zo snel mogelijk of zo laat mogelijk gewijzigd of worden de geplande begin- of einddatums van de projecten aangepast. Sommige voorbeelden van datum-specifieke beperkingen zijn moet beginnen, moet beëindigen, begin niet vroeger dan, begin niet later dan, enz. Voor informatie over taakbeperkingen en hoe de taakbeperkingen of projectdata kunnen worden beïnvloed, zie {het overzicht van de Beperking van de Taak 0} <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref"> en zoek een specifieke beperking.</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Toewijzingen</td> 
      <td> <p>Alle toewijzingen worden uit de taak verwijderd. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Goedkeuringsproces</td> 
      <td>Alle goedkeuringsprocessen worden uit de taak verwijderd.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Voortgang</td> 
      <td>De taakstatus is Nieuw. Anders behoudt de gekopieerde taak de status van de bestaande taak.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Financiële informatie</td> 
      <td>De financiële informatie van de taak wordt verwijderd.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alle voorgangers</td> 
      <td> <p>Dit betekent dat de afhankelijkheden niet worden overgedragen naar de gekopieerde taken. </p> <p>Als deze optie is geselecteerd, blijven de voorgangers in de groep gekopieerde taken behouden en worden de andere taken verwijderd.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenten</td> 
      <td> <p>De aan de taak gekoppelde documenten worden niet naar de gekopieerde taak overgebracht. Dit zijn versies, proefdrukken en gekoppelde documenten.</p> <p>Dit omvat geen documentgoedkeuringen. Documentgoedkeuringen kunnen nooit worden gekopieerd wanneer een taak wordt gekopieerd.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Herinneringsmeldingen</td> 
      <td>De taakherinneringen worden niet overgedragen naar de gekopieerde taak. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uitgaven</td> 
      <td>De uitgaven die op de taak worden geregistreerd brengen niet naar de gekopieerde taak over. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Machtigingen</td> 
      <td>Workfront verwijdert de namen van alle entiteiten die worden weergegeven in de lijst voor delen van de taak. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aangepaste gegevens</td> 
      <td> <p>De waarden voor de aangepaste velden worden gewist en de aangepaste formulieren worden overgebracht naar de gekopieerde taak. </p> <p>Als deze optie is geselecteerd, worden zowel de formulieren als de waarden voor de aangepaste velden overgebracht naar de gekopieerde taak. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatief) klik **Uitgezochte Ouder** in het linkerpaneel, dan selecteer de taak in het bestemmingsproject dat u de ouder van de gekopieerde taak wilt worden.

   >[!TIP]
   >
   >Wanneer u selecteert om meerdere taken in een lijst te kopiëren, worden alle geselecteerde taken de onderliggende taken van het geselecteerde bovenliggende element.

   Voer een van de volgende handelingen uit om een bovenliggend element te selecteren:

   * In de taaklijst, selecteer één van de ouders in het projectplan.
   * Klik het pictogram van het onderzoekspictogram ![ Onderzoek ](assets/search-icon.png) en onderzoek naar een oudertaak door naam.

   De taak wordt weergegeven in de lijst.

   ![ Uitgezochte oudertaak wanneer het bewegen van een taak met onderzoeksfunctionaliteit ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Selecteer het keuzerondje voor het bovenliggende element nadat u het hebt gevonden.

   Als u geen oudertaak selecteert, worden de taken gekopieerd als belangrijkste taken eerder dan subtaken en zij worden geplaatst aan het eind van de taaklijst op het bestemmingsproject.

1. Klik **taak van het Exemplaar**

   of

   Klik **de taken van het Exemplaar** wanneer u veelvoudige taken in een lijst selecteert.
De gekopieerde taken zijn nu op het gespecificeerde project en of subtaken aan de geselecteerde oudertaak, of de laatste taken op het project.

## Taken dupliceren

U kunt een taak snel dupliceren in een takenlijst als u een identieke taak nodig hebt voor hetzelfde project.

* [ Overwegingen voor het dupliceren van taken ](#considerations-for-duplicating-tasks)
* [Taken dupliceren](#duplicate-tasks)

### Overwegingen bij het dupliceren van taken {#considerations-for-duplicating-tasks}

* U kunt een taak alleen in een takenlijst dupliceren wanneer de lijst op taaknummer wordt gesorteerd.
* De nieuwe taak krijgt dezelfde naam als de oorspronkelijke taak.
* U kunt niet selecteren welke informatie aan de nieuwe taak wordt gedupliceerd. Bijna alle informatie van de originele taak zal naar de gedupliceerde taak, met inbegrip van ouderverhouding, door gebrek worden overgebracht.
* De volgende punten worden niet overgebracht naar de nieuwe taak:

   * Aangemeld aantal uren
   * Notities
   * Problemen
   * Alleen de voorgangers die zich in dezelfde groep gekopieerde taken bevinden, worden ook gekopieerd met hun opvolgertaken.

     **VOORBEELD**

     Bijvoorbeeld, als u Taak 2 en zijn voorganger, Taak 1, tezelfdertijd kopieert, dan hebt u een exemplaar van Taak 2 en een exemplaar van Taak 1. Het exemplaar van Taak 1 zal voorganger van het exemplaar van Taak 2 zijn. Maar als u enkel Taak 2 kopieert zonder zijn voorganger te kopiëren, dan zal zijn exemplaar geen voorganger hebben.

* Wanneer u een bovenliggende taak dupliceert, worden alle onderliggende taken ook gedupliceerd, zelfs wanneer de onderliggende taken niet zijn geselecteerd.
* U kunt een of meerdere taken tegelijk dupliceren.

  U kunt echter niet meerdere taken tegelijk dupliceren die niet opeenvolgend zijn.

* Mijlpalen worden verplaatst naar de nieuwe taak en uit de oorspronkelijke taak verwijderd.

### Taken dupliceren

1. Ga naar het project dat de taak of de taken bevat die u wilt dupliceren.
1. Klik **Taken** in het linkerpaneel.
1. Voer een van de volgende handelingen uit:

   * (Voorwaardelijk) klik de **pictogram van de Wijze van het Plan** van de Lijst of sparen wijze kleine pictogram ![ en zorg ervoor de ](assets/qs-list-mode-or-save-mode-icon-small.png) Autosave **optie wordt toegelaten, selecteer de taken u wilt dupliceren, dan het** Meer menu **** Meer menu ![ > ](assets/qs-more-menu-29x11.png) dupliceren **klikken.**

     ![ Dubbele taken in het punt van het lijstmenu ](assets/duplicate-tasks-in-list-nwe-350x196.png)

   * (Voorwaardelijk) klik de **pictogram van de Wijze van het Plan** van de Lijst of sparen wijze kleine pictogram ![ > ](assets/qs-list-mode-or-save-mode-icon-small.png) Handboek sparen **>** Standaard **of** Chronologie Planning **, dan doe het volgende:**

      1. Selecteer de taak of de taken u, **dupliceren** wilt dupliceren en klikken.
      1. (Facultatief) klik **ongedaan maken** om uw veranderingen om te keren en niet de taken te dupliceren.
      1. (Facultatief en voorwaardelijk) klik **opnieuw** als u eerder **** had geklikt ongedaan maken, om de veranderingen te houden en de taken te dupliceren.

      1. Klik **sparen** om uw veranderingen te bewaren.

         De taken worden gedupliceerd en aan het zelfde project toegevoegd zoals de originele taken.
