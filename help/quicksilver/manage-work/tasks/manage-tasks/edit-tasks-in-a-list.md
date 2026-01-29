---
product-area: projects
navigation-topic: manage-tasks
title: Taken in een lijst bewerken
description: U kunt de taakgegevens in een takenlijst bewerken door de velden in de lijst te bewerken. U moet de overzichtsmodus definiëren in een lijst met taken om aan te geven hoe u uw wijzigingen wilt opslaan in Workfront. U kunt uw wijzigingen handmatig of automatisch opslaan.
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: 665e753880be59cf07062d75c66a7be5f2056aa1
workflow-type: tm+mt
source-wordcount: '3233'
ht-degree: 0%

---

# Taken in een lijst bewerken {#edit-tasks-in-a-list}

<!-- Audited: 10/2025 -->

<div class="preview">

De gemarkeerde informatie op deze pagina verwijst naar functionaliteit die nog niet algemeen beschikbaar is. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Dezelfde functies zijn ook beschikbaar in de productieomgeving voor alle klanten vanaf een week na de release Preview.

Voor meer informatie, zie [&#x200B; modernisering van de Interface &#x200B;](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

U kunt de taakgegevens in een takenlijst bewerken door de velden in de lijst te bewerken. Voor informatie over andere manieren om taken uit te geven, zie [&#x200B; taken &#x200B;](../../../manage-work/tasks/manage-tasks/edit-tasks.md) uitgeven.

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
   <td> <p>Standard<p>
   <p>Werk of hoger</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot taken en projecten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute of hoger machtigingen voor de taak en het project</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard<p>
   <p>Current: Work or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to the task and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Overwegingen bij het bewerken van taken in een lijst {#considerations-about-editing-tasks-in-a-list}

Het uitgeven van taken in een lijst is een snelle manier om veranderingen in veelvoudige taken gelijktijdig met een duidelijke mening van aan te brengen hoe uw veranderingen de projectchronologie zouden kunnen beïnvloeden.

Houd rekening met het volgende wanneer u taken in een lijst bewerkt:

* In tegenstelling tot het gebruik van de machtiging Beheren voor de taak wanneer u deze bewerkt in het bewerkingsvak, kunt u een taak in een lijst alleen bewerken met de Contribute-machtigingen voor de taak. Hierdoor kunt u de volgende beperkte informatie voor de taak bewerken:

   * Beschrijving
   * Status
   * Percentage voltooid
   * Aangepaste formuliergegevens

     >[!NOTE]
     >
     >U kunt een taakaangepast veld alleen in een lijst bewerken als u machtigingen hebt om het veld bij te werken.

   * Logboekuren
   * Toewijzingen wijzigen
   * Financiële informatie weergeven
   * Voeg uitgaven, taken of kwesties toe

* U kunt een taak in de volgende lijsten bewerken:

   * De sectie van Taken van het project
   * De subtakensectie van het project
   * Een taakrapport

     >[!NOTE]
     >
     >Standaard slaat Workfront uw wijzigingen in taken automatisch op in de sectie Subtaken of in een taakrapport.

* U kunt bepalen wanneer Workfront de wijzigingen opslaat die u in de taken in een lijst aanbrengt door de overzichtsmodus te definiëren voordat u de taken gaat bewerken.

  U kunt de wijzigingen die u aanbrengt als volgt opslaan tussen Workfront:

   * Automatisch, na elke wijziging
   * Handmatig, slechts nadat u sparen klikt.

  Voor informatie over het vormen wanneer Workfront veranderingen opslaat u aan taken in een lijst aanbrengt, zie [&#x200B; de Wijzig Wijzig Wijzig de Wijze van het Plan alvorens taken in een lijst &#x200B;](#modify-plan-mode-before-editing-tasks-in-a-list) sectie in dit artikel uit te geven.

* Andere gebruikers moeten hun pagina&#39;s vernieuwen voordat ze de updates die u voor een taak maakt, kunnen bekijken.

## Abonnementsmodus wijzigen voordat taken in een lijst worden bewerkt

U kunt bepalen of de wijzigingen die u in taken in een lijst aanbrengt, automatisch worden opgeslagen wanneer deze zich voordoen, of dat u elke wijziging handmatig wilt opslaan. Om dit te doen, moet u de Wijze van het Plan in een lijst van taak wijzigen alvorens de taken uit te geven.

>[!IMPORTANT]
>
>Afhankelijk van of u de taken automatisch of manueel opslaat, zou u de informatie van iemand anders kunnen beschrijven aangezien u taken in een lijst uitgeeft. Voor meer informatie, zie [&#x200B; Overzicht van het bewaren van gezamenlijke veranderingen binnen een taaklijst &#x200B;](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

Wanneer u uw veranderingen in een lijst voor een project opslaat dat of Automatisch of bij Verandering als Type van Update wordt geselecteerd, werkt Workfront de projectchronologie, samen met alle in-project en dwars-projectgebiedsdelen bij. De berekeningen van de Chronologie kunnen lange tijd vergen als het project groot is of als er veel gebiedsdelen zijn. Sommige methoden voor het bewerken van een takenlijst zijn mogelijk sneller dan andere, afhankelijk van de methode die u selecteert om uw wijzigingen op te slaan.

U kunt bepalen wanneer Workfront de wijzigingen opslaat die u in de taken in een lijst aanbrengt. De volgende scenario&#39;s bestaan:

* Workfront kan de wijzigingen na elke update automatisch laten opslaan.

  Voor informatie, zie de sectie [&#x200B; plaats de Wijze van het Plan om veranderingen &#x200B;](#set-the-plan-mode-to-automatically-save-changes) in dit artikel automatisch te bewaren.

* Met de knop Opslaan kunt u zelf bepalen wanneer u meerdere wijzigingen tegelijk toepast.

  Voor informatie, zie de sectie [&#x200B; plaatsen de Wijze van het Plan om veranderingen &#x200B;](#set-the-plan-mode-to-manually-save-changes) in dit artikel manueel te bewaren.

### Stel de overzichtsmodus in om wijzigingen automatisch op te slaan

>[!TIP]
>
>Het opslaan van uw veranderingen en alle projectgebiedsdelen zou langzamer kunnen zijn als uw project meer dan 2000 taken heeft of als het veel gebiedsdelen heeft.

Houd rekening met het volgende wanneer u uw takenlijst automatisch opslaat:

* U kunt een aangepaste weergave toepassen op de takenlijst en alle taakgerelateerde velden bewerken die u kunt bijwerken.
* U kunt automatisch opgeslagen wijzigingen niet ongedaan maken. Dit is de standaardinstelling.
* Wanneer het Type van projectupdate Automatisch of Automatisch en bij Verandering is, herberekent Workfront de chronologie van het project en alle in-project en dwars-projecten gebiedsdelen automatisch na elke verandering. Voor informatie over het Type van projectupdate, zie [&#x200B; het Type van projectupdate &#x200B;](../../../manage-work/projects/manage-projects/select-project-update-type.md) selecteren.

Taken in een lijst bewerken en wijzigingen automatisch opslaan:

{{step1-to-projects}}

1. Voor de **pagina van Projecten**, selecteer een project.
1. In het linkerpaneel, klik de **sectie van Taken**.

1. Klik het **pictogram van de Wijze van het Plan** pictogram van de Wijze van het Plan ![&#x200B; bij de bovenkant van de lijst en zorg ervoor de &#x200B;](assets/plan-mode-icon.png) Autosave **optie wordt geselecteerd.**

   ![&#x200B; laat autosave het plaatsen &#x200B;](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png) toe

1. Bewerk elk veld dat u gemachtigd bent om handmatig bij te werken.

1. (Facultatief) Pers **Escape** om uw veranderingen te annuleren.
1. De pers **gaat** (Vensters) of **Terugkeer** (Mac) op uw toetsenbord in om uw veranderingen in de taken en de projectchronologie te bewaren.
1. (Optioneel) Klik met de rechtermuisknop op een taak die u wilt wijzigen.

   of

   Klik **Meer** menu ![](assets/more-icon-task-list.png) rechts van de taaknaam.

1. (Optioneel) Kies een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Openen op nieuw tabblad</td> 
      <td>Hiermee opent u de taak in een nieuw browsertabblad. </td> 
     </tr> 
          <tr> 
      <td role="rowheader">Taak invoegen boven</td> 
      <td>Hiermee voegt u een taak in boven de geselecteerde taak.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taak invoegen onder</td> 
      <td>Hiermee voegt u een taak in onder de geselecteerde taak</td> 
     </tr>
     <tr> 
      <td role="rowheader">Bewerken</td> 
      <td><p>Hiermee opent u het vak Taak bewerken, waarin u de taak kunt bewerken.</p><p>Voor informatie over het uitgeven van een taak, zie <a href="#edit-tasks-in-a-list" class="MCXref xref"> taken in een lijst </a> uitgeven.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verwijderen</td> 
      <td><p>Hiermee verwijdert u de taak.</p><p>Voor informatie over het schrappen van taken, zie <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref"> de taken van de Schrapping </a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inspringen</td> 
      <td><p>Hiermee wordt de taak op één niveau ingesprongen. </p><p>Deze optie wordt alleen weergegeven bij zelfstandige taken.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uitspringen</td> 
      <td><p>Hiermee wordt de taak één niveau uitgespreid. </p><p>Deze optie wordt alleen weergegeven bij onderliggende taken. </p></td> 
     </tr>  
     <tr> 
      <td role="rowheader">Dupliceren</td> 
      <td><p>Hiermee maakt u een gedupliceerde versie van de taak in hetzelfde project. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kopiëren naar..</td> 
      <td><p>Kopieert de taak naar een ander project.</p><p>Voor informatie over het kopiëren en het dupliceren van taken, zie <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref"> Kopiëren en dupliceren taken </a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verplaatsen naar..</td> 
      <td><p>Verplaatst de taak naar een ander project.</p><p>Voor informatie over het bewegen van taken, zie <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref"> de taken van de Beweging </a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

### Stel de overzichtsmodus in om wijzigingen handmatig op te slaan {#edit-tasks-in-a-list-and-manually-save-changes}

U kunt wijzigingen die u aanbrengt in taken in een lijst handmatig opslaan. Als u wijzigingen op deze manier opslaat, hebt u de flexibiliteit om deze om te keren voordat u ze opslaat.

>[!TIP]
>
>* U kunt wijzigingen die u aanbrengt in taken in een lijst niet omkeren wanneer u deze bewerkt in de sectie Subtaken of in een taakrapport.
>* Er gelden geen beperkingen voor het aantal wijzigingen dat u kunt terugdraaien. U kunt al hen één voor één om keren tot u de originele staat van de taken bereikt.
>

Houd rekening met het volgende wanneer u wijzigingen handmatig opslaat in een takenlijst:

* Als u wijzigingen in de takenlijst handmatig wilt opslaan, hebt u machtigingen nodig om zowel de taken als het project te beheren.
* U kunt het project niet bewerken. De optie om het project te bewerken is uitgeschakeld.
* U kunt geen informatie in de kopbal van het project bijwerken. U kunt alleen het volgende doen wanneer u de wijzigingen handmatig opslaat in de takenlijst:

   * Abonneren op het project.
   * Voeg het project toe aan uw lijst met favorieten.
   * Open een taak door op de naam ervan in de lijst te klikken.

* De taken bulksgewijs bewerken. Het pictogram Bewerken is uitgeschakeld wanneer u meerdere taken selecteert.
* Workfront activeert alleen meldingen over de wijzigingen die u in de taken aanbrengt nadat u de wijzigingen hebt opgeslagen.

Er zijn twee manieren om wijzigingen in taken in een lijst handmatig op te slaan:

* [&#x200B; sparen veranderingen in een taaklijst manueel wanneer u het Handboek sparen de optie Standaard &#x200B;](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option) selecteert
* [Wijzigingen handmatig opslaan in een takenlijst wanneer u de optie Tijdlijnplanning handmatig opslaan selecteert](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### Wijzigingen handmatig opslaan in een takenlijst wanneer u de optie Handmatig opslaan kiest {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>Als uw project meer dan 2000 taken heeft, of als het veel gebiedsdelen heeft, zou het een tijdje kunnen nemen om visueel de veranderingen te identificeren u aan uw taken aanbrengt en hoe deze veranderingen alle projectgebiedsdelen beïnvloeden. In dit geval kan het opslaan van uw wijzigingen langer duren dan u had verwacht.

Houd rekening met het volgende wanneer u taken in een lijst bijwerkt nadat u de optie Standaard handmatig opslaan hebt geselecteerd:

* U kunt een aangepaste weergave toepassen op de takenlijst en alle taakgerelateerde velden bewerken die u in die weergave hebt gemachtigd om te beheren.
* Wanneer het Type van projectupdate Automatisch of Automatisch en bij Verandering is, berekent Workfront de chronologie van het project en alle in-project en dwars-project gebiedsdelen nadat u sparen klikt. Voor informatie over het Type van projectupdate, zie [&#x200B; het Type van projectupdate &#x200B;](../../../manage-work/projects/manage-projects/select-project-update-type.md) selecteren.

Taken in een lijst bewerken wanneer u de optie Handmatig opslaan kiest:

{{step1-to-projects}}

1. Voor de **pagina van Projecten**, selecteer een project.

1. In het linkerpaneel, klik de **sectie van Taken**.

1. Klik het **pictogram van de Wijze van het Plan** pictogram van de Wijze van het Plan ![&#x200B; bij de bovenkant van de lijst.](assets/plan-mode-icon.png)

1. In de **dialoog van de Wijze van het Plan**, uitgezochte **Handboek sparen**, dan klik **Standaard**.

   ![&#x200B; laat handbediende sparen plaatsen &#x200B;](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png) toe

1. Klik **toepassen**. Er wordt een werkbalkinstelling weergegeven met opties voor het ongedaan maken, opnieuw uitvoeren en opslaan van de wijzigingen.

   ![&#x200B; Handmatig sparen toolbar &#x200B;](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Klik in een veld waarvoor u gemachtigd bent om handmatig bij te werken. Het veld wordt bewerkbaar en u kunt de wijzigingen aanbrengen.

1. De pers **gaat** (Vensters) of **Terugkeer** (Mac) op uw toetsenbord in om de veranderingen tijdelijk te bewaren u aanbracht.

1. (Facultatief) klik **ongedaan maken** pictogram ![&#x200B; pictogram &#x200B;](assets/undo-icon-on-task-list.png) om een verandering om te keren en een gebied op zijn originele staat terug te keren.

1. (Facultatief en voorwaardelijk) klik **opnieuw** pictogram ![&#x200B; pictogram &#x200B;](assets/redo-icon-on-task-list.png) om de verandering te herstellen u hebt omgekeerd.

1. (Optioneel) Klik met de rechtermuisknop op een taak die u wilt wijzigen.

   of

   Klik **Meer** menu ![](assets/more-icon-task-list.png).

1. (Optioneel) Kies een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Openen op nieuw tabblad</td> 
      <td>Hiermee opent u de taak in een nieuw browsertabblad. </td> 
     </tr> 
          <tr> 
      <td role="rowheader">Taak invoegen boven</td> 
      <td>Hiermee voegt u een taak in boven de geselecteerde taak.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taak invoegen onder</td> 
      <td>Hiermee voegt u een taak in onder de geselecteerde taak</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verwijderen</td> 
      <td>Voor informatie over het schrappen van taken, zie <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref"> de taken van de Schrapping </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inspringen</td> 
      <td> <p>Hiermee wordt de taak op één niveau ingesprongen. </p> <p>Deze optie wordt alleen weergegeven bij zelfstandige taken.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uitspringen</td> 
      <td> <p>Hiermee wordt de taak één niveau uitgespreid. </p> <p>Deze optie wordt alleen weergegeven bij onderliggende taken. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dupliceren</td> 
      <td> <p>Hiermee maakt u een gedupliceerde versie van de taak in hetzelfde project. </p> <p>Voor informatie over het kopiëren en het dupliceren van taken, zie <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref"> Kopiëren en dupliceren taken </a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront werkt alle in-project en dwars-project gebiedsdelen bij wanneer u veranderingen in de chronologie van taken aanbrengt.
1. Klik **sparen** wanneer u uw taakveranderingen permanent wilt houden en de chronologie van het project bewaren.

#### Wijzigingen handmatig opslaan in een takenlijst wanneer u de optie Tijdlijnplanning handmatig opslaan selecteert {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

Het opslaan van uw veranderingen en alle projectgebiedsdelen is sneller. Dit is niet beschikbaar voor projecten met meer dan 2000 taken.

>[!IMPORTANT]
>
>Wij adviseren dat u deze optie gebruikt wanneer het uitgeven van een grote lijst van taken van meer dan een paar honderd die veel gebiedsdelen hebben. Met deze optie kunt u uw wijzigingen veel sneller visueel identificeren dan met de optie Handmatig opslaan.

Houd rekening met het volgende wanneer u de optie Tijdlijnplanning handmatig opslaan gebruikt in een takenlijst:

* U kunt de optie voor het handmatig opslaan van tijdlijnplanning niet toepassen op projecten met meer dan 2000 taken.
* U kunt geen aangepaste weergave, filter of groep toepassen op de takenlijst. De vervolgkeuzemenu&#39;s Weergave, Filter en Groeperen en het pictogram Gegraveerde weergave zijn uitgeschakeld. De weergave die standaard wordt toegepast, bevat een beperkt aantal velden.
* De chronologie van het project en alle in-projectgebiedsdelen worden automatisch berekend na elke verandering wanneer het Type van projectupdate Automatisch of Automatisch en bij Verandering is.
* Wanneer het Type van projectupdate Automatisch of Automatisch en bij Verandering is, worden de dwars-projectgebiedsdelen berekend nadat u sparen klikt. Voor informatie over het Type van projectupdate, zie [&#x200B; het Type van projectupdate &#x200B;](../../../manage-work/projects/manage-projects/select-project-update-type.md) selecteren.

Taken in een lijst bewerken wanneer u de optie Tijdlijnplanning handmatig opslaan gebruikt:


{{step1-to-projects}}

1. Voor de **pagina van Projecten**, selecteer een project.

1. In het linkerpaneel, klik de **sectie van Taken**.

1. Klik het **pictogram van de Wijze van het Plan** pictogram van de Wijze van het Plan ![&#x200B; bij de bovenkant van de lijst.](assets/plan-mode-icon.png)

1. In de **dialoog van de Wijze van het Plan**, uitgezochte **Handboek sparen**, dan klik **Planning van de Chronologie**.

   ![&#x200B; pas de Planning van de Chronologie het plaatsen &#x200B;](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png) toe

   >[!TIP]
   >
   >De **optie van de Planning van de Tijd** wordt gedimd voor projecten met meer dan 2000 taken.

1. Klik **toepassen**.

   De volgende wijzigingen vinden plaats in de lijst:

   * De vervolgkeuzemenu&#39;s Weergeven, Groeperen en Filter worden verwijderd en de weergave wordt vervangen door de volgende velden:

      * Taaknummer
      * Taaknaam
      * Restrictietype
      * Duur
      * Geplande begindatum
      * Geplande afsluitdatum
      * Predecessors
      * Toewijzingen
      * Status
      * Percentage voltooid

   * Het pictogram van de Gegraveerde weergave wordt verwijderd.
   * Er wordt een werkbalkinstelling weergegeven met opties voor het ongedaan maken, opnieuw uitvoeren en opslaan van de wijzigingen.

     ![&#x200B; Handmatig sparen toolbar &#x200B;](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Bewerk elk veld dat u gemachtigd bent om handmatig bij te werken.

1. De pers **gaat** (Vensters) of **Terugkeer** (Mac) op uw toetsenbord in om de veranderingen tijdelijk te bewaren u aanbracht.
1. (Facultatief) klik **ongedaan maken** pictogram ![&#x200B; pictogram &#x200B;](assets/undo-icon-on-task-list.png) om een verandering om te keren en een gebied op zijn originele staat terug te keren.
1. (Facultatief en voorwaardelijk) klik **opnieuw** pictogram ![&#x200B; pictogram &#x200B;](assets/redo-icon-on-task-list.png) om de verandering op te nemen u hebt omgekeerd.

1. (Optioneel) Klik met de rechtermuisknop op een taak die u wilt wijzigen.

   of

   Klik **Meer** menu ![](assets/more-icon-task-list.png).

1. Selecteer een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Openen op nieuw tabblad</td> 
      <td>Hiermee opent u de taak in een nieuw browsertabblad. </td> 
     </tr> 
          <tr> 
      <td role="rowheader">Taak invoegen boven</td> 
      <td>Hiermee voegt u een taak in boven de geselecteerde taak.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taak invoegen onder</td> 
      <td>Hiermee voegt u een taak in onder de geselecteerde taak</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verwijderen</td> 
      <td>Voor informatie over het schrappen van taken, zie <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref"> de taken van de Schrapping </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inspringen</td> 
      <td> <p>Hiermee wordt de taak op één niveau ingesprongen. </p> <p>Deze optie wordt alleen weergegeven bij zelfstandige taken.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uitspringen</td> 
      <td> <p>Hiermee wordt de taak één niveau uitgespreid. </p> <p>Deze optie wordt alleen weergegeven bij onderliggende taken. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dupliceren</td> 
      <td> <p>Hiermee maakt u een gedupliceerde versie van de taak in hetzelfde project. </p> <p>Voor informatie over het kopiëren en het dupliceren van taken, zie <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref"> Kopiëren en dupliceren taken </a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront werkt alle in-project en dwars-project gebiedsdelen bij wanneer u de chronologie van een taak verandert.
1. Klik **sparen** wanneer u uw taakveranderingen permanent wilt houden en de chronologie van het project bewaren.

## Een taak in een lijst bewerken met Overzicht

{{step1-to-projects}}

1. Voor de **pagina van Projecten**, selecteer een project.

1. In het linkerpaneel, klik de **sectie van Taken**. De lijst van taken op de projectvertoningen.

1. Selecteer de taak u wilt uitgeven, dan klik het **Open Samenvatting** pictogram ![&#x200B; Open Samenvattingspictogram &#x200B;](assets/task-summary-icon.png) in de hoger-juiste hoek van de lijst. Het **Summiere paneel van de Taak** opent.

1. (Optioneel) Typ een update voor de taak in het **gebied van Updates**.
1. Klik op een van de volgende pictogrammen of gebieden om naar de taak te gaan en gegevens op taakniveau te bewerken:

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Documenten</td> 
      <td>Voeg documenten toe aan de taak. </td> 
     </tr> 
          <tr> 
      <td role="rowheader">Aangepaste Forms</td> 
      <td>Voeg aangepaste formulieren toe of verwijder deze of werk gegevens bij op de formulieren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uren</td> 
      <td>Loguren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Goedkeuringen</td> 
      <td>Voeg taakgoedkeuringen toe.</td> 
     </tr> 
     <tr> 
    </tbody> 
   </table>

1. Klik **X** in de hoger-juiste hoek van het paneel om het te sluiten.

## Taken bulksgewijs bewerken

U kunt meerdere taken tegelijk bewerken. Zorg ervoor dat u beheermachtigingen hebt voor de taken die u bulksgewijs selecteert, zodat u deze kunt bewerken.

Het tegelijkertijd bewerken van meerdere taken is afhankelijk van de omgeving die u kiest.

### Grote taken in de productieomgeving bewerken

{{step1-to-projects}}

1. Voor de **pagina van Projecten**, selecteer een project.
1. In het linkerpaneel, klik de **sectie van Taken**.

1. Klik het **pictogram van de Wijze van het Plan** pictogram van de Wijze van het Plan ![&#x200B; bij de bovenkant van de lijst en zorg ervoor de &#x200B;](assets/plan-mode-icon.png) Autosave **optie wordt geselecteerd.**

   ![&#x200B; laat autosave het plaatsen &#x200B;](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png) toe

   >[!IMPORTANT]
   >
   >U kunt taken niet bulksgewijs bewerken wanneer u taken handmatig opslaat.

1. Selecteer meerdere taken in de takenlijst.
1. (Facultatief) klik het **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-icon.png) bij de bovenkant van de taaklijst, toen **Uitdrukkingen** opnieuw berekenen om alle informatie op berekende douanegebieden bij te werken.
1. Klik **uitgeven** pictogram ![&#x200B; uitgeven pictogram &#x200B;](assets/qs-edit-icon.png). Het **geeft de doos van Taken** uit opent in de nieuwe ervaring.

   Het bewerken van de informatie over alle taken is hetzelfde als het bewerken van de informatie over één taak.

   Voor meer informatie over het uitgeven van een taak, zie [&#x200B; taken &#x200B;](../../../manage-work/tasks/manage-tasks/edit-tasks.md) uitgeven.

1. (Voorwaardelijk) Voer in de nieuwe ervaring de volgende handelingen uit:

   1. Geef de informatie op die u wilt wijzigen voor alle taken die u hebt geselecteerd op een van de volgende gebieden:

      * Overzicht
      * Toewijzingen
      * Aangepaste Forms
      * Financiën
      * Instellingen
      * Instellingen
      * Opmerking

      >[!NOTE]
      >
      >* De informatie u op alle geselecteerde taken verandert zal de bestaande informatie over individuele taken met voeten treden, behalve het **gebied van Taken**. Als u een nieuwe toewijzing toevoegt in bulkbewerking, wordt die toewijzing toegevoegd aan alle geselecteerde taken. Als er andere toewijzingen zijn toegewezen aan de geselecteerde taken, blijven deze toegewezen naast de toewijzing die via bulkbewerking wordt toegevoegd.
      >* Als u taakduur wilt bewerken, moeten de geselecteerde taken dezelfde taakbeperking hebben. Anders, bevolkt het **gebied van de Duur** niet.
      >
      >* Alleen actieve aangepaste formulieren worden in de lijst weergegeven. Als de geselecteerde taken geen aangepaste formulieren hebben, worden in deze sectie geen formulieren weergegeven.
      >* U kunt alleen de velden in de formulieren bewerken die zijn gekoppeld aan alle geselecteerde taken en die u kunt bewerken.  Voor informatie over bulk die douaneformulieren uitgeven, zie [&#x200B; douaneformulieren beheren in bijlage aan voorwerpen &#x200B;](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).

   1. Klik **sparen**.
   1. (Facultatief) klik **Schakelaar terug naar oude ervaring** bij de bodem van **geeft de doos van Taken** uit.

1. (Voorwaardelijk) Voer in de oude ervaring de volgende handelingen uit:

   1. Geef de informatie op die u wilt wijzigen voor alle taken die u hebt geselecteerd op een van de volgende gebieden:

      * Overzicht
      * Instellingen
      * Toewijzingen
      * Aangepaste Forms
      * Opmerking

   1. (Facultatief) in de **sectie van Forms van de Douane 0&rbrace;, selecteer de** **optie van de Uitdrukkingen van de Douane opnieuw berekenen om ervoor te zorgen dat alle Berekende Gebieden van de Douane die op de douaneformulieren in bijlage aan de geselecteerde taken zijn bijgewerkt.**
   1. Klik **sparen Veranderingen**. Alle wijzigingen die u hebt aangebracht, zijn nu zichtbaar voor alle geselecteerde taken.

<div class="preview">

### Grote taken in de voorvertoningsomgeving bewerken

{{step1-to-projects}}

1. Voor de **pagina van Projecten**, selecteer een project.
1. In het linkerpaneel, klik de **sectie van Taken**.

1. Klik het **pictogram van de Wijze van het Plan** pictogram van de Wijze van het Plan ![&#x200B; bij de bovenkant van de lijst en zorg ervoor de &#x200B;](assets/plan-mode-icon.png) Autosave **optie wordt geselecteerd.**

   ![&#x200B; laat autosave het plaatsen &#x200B;](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png) toe

   >[!IMPORTANT]
   >
   >U kunt taken niet bulksgewijs bewerken wanneer u taken handmatig opslaat.

1. Selecteer meerdere taken in de takenlijst.
1. (Facultatief) klik het **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-icon.png) bij de bovenkant van de taaklijst, toen **Uitdrukkingen** opnieuw berekenen om alle informatie op berekende douanegebieden bij te werken.
1. Klik **uitgeven** pictogram ![&#x200B; uitgeven pictogram &#x200B;](assets/qs-edit-icon.png). Het **geeft de doos van Taken** uit opent.

   Het bewerken van de informatie over alle taken is hetzelfde als het bewerken van de informatie over één taak.

   Voor meer informatie over het uitgeven van een taak, zie [&#x200B; taken &#x200B;](../../../manage-work/tasks/manage-tasks/edit-tasks.md) uitgeven.

1. Geef de informatie op die u wilt wijzigen voor alle taken die u hebt geselecteerd op een van de volgende gebieden:

   * Overzicht
   * Toewijzingen
   * Aangepaste Forms
   * Financiën
   * Instellingen
   * Instellingen
   * Opmerking

   >[!NOTE]
   >
   >* De informatie u op alle geselecteerde taken verandert zal de bestaande informatie over individuele taken met voeten treden, behalve het **gebied van Taken**. Als u een nieuwe toewijzing toevoegt in bulkbewerking, wordt die toewijzing toegevoegd aan alle geselecteerde taken. Als er andere toewijzingen zijn toegewezen aan de geselecteerde taken, blijven deze toegewezen naast de toewijzing die via bulkbewerking wordt toegevoegd.
   >* Als u taakduur wilt bewerken, moeten de geselecteerde taken dezelfde taakbeperking hebben. Anders, bevolkt het **gebied van de Duur** niet.
   >
   >* Alleen actieve aangepaste formulieren worden in de lijst weergegeven. Als de geselecteerde taken geen aangepaste formulieren hebben, worden in deze sectie geen formulieren weergegeven.
   >* U kunt alleen de velden in de formulieren bewerken die zijn gekoppeld aan alle geselecteerde taken en die u kunt bewerken.  Voor informatie over bulk die douaneformulieren uitgeven, zie [&#x200B; douaneformulieren beheren in bijlage aan voorwerpen &#x200B;](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).

1. Klik **sparen**.

</div>

