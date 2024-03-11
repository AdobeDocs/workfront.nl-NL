---
product-area: projects
navigation-topic: manage-tasks
title: Taken in een lijst bewerken
description: U kunt de taakgegevens in een takenlijst bewerken door de velden in de lijst te bewerken. Zie Taken bewerken voor informatie over andere manieren om taken te bewerken.
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: 1da2e6448f7ac6f4bd5bd76846fbfc1a23c3da77
workflow-type: tm+mt
source-wordcount: '2848'
ht-degree: 0%

---

# Taken in een lijst bewerken {#edit-tasks-in-a-list}

U kunt de taakgegevens in een takenlijst bewerken door de velden in de lijst te bewerken. Voor informatie over andere manieren om taken uit te geven, zie [Taken bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot taken en projecten bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute of hoger machtigingen voor de taak en het project</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Overwegingen bij het bewerken van taken in een lijst {#considerations-about-editing-tasks-in-a-list}

Het uitgeven van taken in een lijst is een snelle manier om veranderingen in veelvoudige taken gelijktijdig aan te brengen, met een duidelijke mening van hoe uw veranderingen de projectchronologie zouden kunnen beïnvloeden.

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

* U kunt bepalen wanneer Workfront de wijzigingen opslaat die u in de taken in een lijst aanbrengt. De wijzigingen kunnen automatisch worden opgeslagen of u kunt ze handmatig opslaan.

  Voor informatie over het configureren wanneer Workfront wijzigingen opslaat die u in taken in een lijst aanbrengt, raadpleegt u de [Selecteer een optie voor opslaan wanneer u taken in een lijst bewerkt](#select-a-save-option-when-editing-tasks-in-a-list) in dit artikel.

* Andere gebruikers moeten hun pagina&#39;s vernieuwen voordat ze de updates die u voor een taak maakt, kunnen bekijken.

## Selecteer een optie voor opslaan wanneer u taken in een lijst bewerkt {#select-a-save-option-when-editing-tasks-in-a-list}

U kunt bepalen waar de wijzigingen die u in taken in een lijst aanbrengt, automatisch worden opgeslagen, zoals ze zich voordoen, of u wilt elke wijziging handmatig opslaan.

>[!IMPORTANT]
>
>Afhankelijk van of u de taken automatisch of manueel opslaat, zou u de informatie van iemand anders kunnen beschrijven aangezien u taken in een lijst uitgeeft. Zie voor meer informatie over hoe Workfront wijzigingen opslaat in taken die u tegelijkertijd met andere gebruikers aanbrengt [Overzicht van het opslaan van gelijktijdige wijzigingen in een takenlijst](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

Wanneer u uw veranderingen in een lijst voor een project opslaat dat of Automatisch of bij Verandering als Type van Update wordt geselecteerd, werkt Workfront de projectchronologie, samen met alle in-project en dwars-projectgebiedsdelen bij. De berekeningen van de Chronologie kunnen lange tijd vergen als het project groot is of als er veel gebiedsdelen zijn. Sommige methoden voor het bewerken van een takenlijst zijn mogelijk sneller dan andere, afhankelijk van de methode die u selecteert om uw wijzigingen op te slaan.

U kunt bepalen wanneer Workfront de wijzigingen opslaat die u in de taken in een lijst aanbrengt. De volgende scenario&#39;s bestaan: 

* Workfront kan de wijzigingen na elke update automatisch laten opslaan.

  Zie de sectie [Taken in een lijst bewerken en wijzigingen automatisch opslaan](#edit-tasks-in-a-list-and-automatically-save-changes) in dit artikel.

* Met de knop Opslaan kunt u zelf bepalen wanneer u meerdere wijzigingen tegelijk toepast.

  Zie de sectie [Taken in een lijst bewerken en wijzigingen handmatig opslaan](#edit-tasks-in-a-list-and-manually-save-changes) in dit artikel.

### Taken in een lijst bewerken en wijzigingen automatisch opslaan {#edit-tasks-in-a-list-and-automatically-save-changes}

>[!TIP]
>
>Het opslaan van uw veranderingen en alle projectgebiedsdelen zou langzamer kunnen zijn als uw project meer dan 2000 taken heeft of als het veel gebiedsdelen heeft.

Houd rekening met het volgende wanneer u uw takenlijst automatisch opslaat:

* U kunt een aangepaste weergave toepassen op de takenlijst en alle taakgerelateerde velden bewerken die u kunt bijwerken.
* U kunt automatisch opgeslagen wijzigingen niet ongedaan maken. Dit is de standaardinstelling.
* Workfront berekent automatisch de chronologie van het project en alle in-project en dwars-projecten gebiedsdelen na elke verandering opnieuw, wanneer het Type van projectupdate Automatisch of Automatisch en bij Verandering is. Voor informatie over het Type van projectupdate, zie [Selecteer het Type van projectupdate](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Taken in een lijst bewerken en wijzigingen automatisch opslaan:

1. Ga naar het project en klik vervolgens op de knop **Taken** sectie.
1. Klik op de knop **Menu van de overzichtsmodus** ![](assets/qs-list-mode-or-save-mode-icon-small.png) boven aan de lijst en zorg ervoor dat de **Automatisch opslaan** is geselecteerd.

   ![](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. Bewerk elk veld dat u gemachtigd bent om handmatig bij te werken.

   ![](assets/inline-editing-a-task-350x26.png)

1. (Optioneel) Druk op **Escape** om uw wijzigingen te annuleren.
1. Druk op Enter om uw wijzigingen in de taken en de projecttijdlijn op te slaan.
1. (Optioneel) Klik met de rechtermuisknop op een taak die u wilt wijzigen.

   of

   Klik op de knop **Meer** menu ![](assets/more-icon-task-list.png) rechts van de taaknaam.

1. (Optioneel) Kies een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Openen in een nieuw tabblad</strong></td> 
      <td>Hiermee opent u de taak in een nieuw browsertabblad. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Bewerken</strong></td> 
      <td><p>Hiermee opent u de <strong>Taak bewerken</strong> , waarin u de taak kunt bewerken.</p><p>Voor informatie over het bewerken van een taak raadpleegt u <a href="#edit-tasks-in-a-list" class="MCXref xref">Taken in een lijst bewerken</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verwijderen</td> 
      <td><p>Hiermee verwijdert u de taak.</p><p>Voor informatie over het verwijderen van taken raadpleegt u <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Taken verwijderen</a>.</p></td> 
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
      <td role="rowheader">Taak invoegen boven</td> 
      <td>Hiermee voegt u een taak in boven de geselecteerde taak.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taak invoegen onder</td> 
      <td>Hiermee voegt u een taak in onder de geselecteerde taak</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dupliceren</td> 
      <td><p>Hiermee maakt u een gedupliceerde versie van de taak in hetzelfde project. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kopiëren naar</td> 
      <td><p>Kopieert de taak naar een ander project.</p><p>Voor informatie over het kopiëren en dupliceren van taken raadpleegt u <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Taken kopiëren en dupliceren</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verplaatsen naar</td> 
      <td><p>Verplaatst de taak naar een ander project.</p><p>Voor informatie over het verplaatsen van taken raadpleegt u <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">Taken verplaatsen</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

   Wijzigingen worden automatisch opgeslagen en u kunt ze niet omkeren.

### Taken in een lijst bewerken en wijzigingen handmatig opslaan {#edit-tasks-in-a-list-and-manually-save-changes}

U kunt wijzigingen die u aanbrengt in taken in een lijst handmatig opslaan. Als u wijzigingen op deze manier opslaat, hebt u de flexibiliteit om deze om te keren voordat u ze opslaat.

>[!TIP]
>
>* U kunt wijzigingen die u aanbrengt in taken in een lijst niet omkeren wanneer u deze bewerkt in de sectie Subtaken of in een taakrapport.
>* Er gelden geen beperkingen voor het aantal wijzigingen dat u kunt terugdraaien. U kunt ze allemaal een voor een omkeren totdat u de oorspronkelijke staat van de taken bereikt.
>

Houd rekening met het volgende wanneer u wijzigingen handmatig opslaat in een takenlijst:

* Als u wijzigingen in de takenlijst handmatig wilt opslaan, hebt u machtigingen nodig om zowel de taken als het project te beheren.
* U kunt het project niet bewerken. De optie om het project te bewerken is uitgeschakeld.
* U kunt geen informatie in de kopbal van het project bijwerken. U kunt alleen het volgende doen wanneer u de wijzigingen handmatig opslaat in de takenlijst:

   * Abonneren op het project.
   * Voeg het project toe aan uw lijst met favorieten.
   * Open een taak door op de naam ervan in de lijst te klikken.

* Geef de taken in bulk uit. Het pictogram Bewerken is uitgeschakeld wanneer u meerdere taken selecteert.
* Workfront activeert alleen meldingen over de wijzigingen die u in de taken aanbrengt nadat u de wijzigingen hebt opgeslagen.

U kunt wijzigingen in taken in een lijst op twee manieren handmatig opslaan. Deze twee manieren worden hieronder beschreven.

* [Wijzigingen handmatig opslaan in een takenlijst wanneer u de optie Handmatig opslaan kiest](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [Wijzigingen handmatig opslaan in een takenlijst wanneer u de optie Tijdlijnplanning handmatig opslaan selecteert](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### Wijzigingen handmatig opslaan in een takenlijst wanneer u de optie Handmatig opslaan kiest {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>Als uw project meer dan 2000 taken heeft, of als het veel gebiedsdelen heeft, zou het een tijdje kunnen nemen om visueel de veranderingen te identificeren u aan uw taken aanbrengt en hoe deze veranderingen alle projectgebiedsdelen beïnvloeden. In dit geval, zou het bewaren van uw veranderingen langer kunnen duren als uw project meer dan 2000 taken heeft of als het veel gebiedsdelen heeft.

Houd rekening met het volgende wanneer u taken in een lijst bijwerkt nadat u de optie Standaard handmatig opslaan hebt geselecteerd:

* U kunt een aangepaste weergave toepassen op de takenlijst en alle taakgerelateerde velden bewerken die u in die weergave hebt gemachtigd om te beheren.
* Workfront berekent de chronologie van het project en alle in-project en dwars-project gebiedsdelen nadat u sparen klikt, wanneer het Type van projectupdate Automatisch of Automatisch en bij Verandering is. Voor informatie over het Type van projectupdate, zie [Selecteer het Type van projectupdate](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Taken in een lijst bewerken wanneer u de optie Handmatig opslaan kiest:

1. Ga naar een project en klik vervolgens op de knop **Taken** deel .
1. Klik op de knop **Abonnementsmodus** menu ![](assets/qs-list-mode-or-save-mode-icon-small.png) boven aan de lijst en selecteer **Handmatig opslaan** en klik vervolgens op **Standaard** > **Toepassen**.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

   Er wordt een werkbalkinstelling weergegeven met opties voor het ongedaan maken, opnieuw uitvoeren en opslaan van de wijzigingen.

   ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Klik in een veld waarvoor u gemachtigd bent om handmatig bij te werken. Het veld wordt bewerkbaar en u kunt de wijzigingen aanbrengen.

   ![](assets/inline-editing-a-task-350x26.png)

1. Druk op Enter om de aangebrachte wijzigingen tijdelijk op te slaan.
1. (Optioneel) Klik op de knop **Pictogram Ongedaan maken** ![](assets/undo-icon-on-task-list.png) om een wijziging om te keren en een veld terug te brengen naar de oorspronkelijke staat.
1. (Optioneel en voorwaardelijk) Klik op de knop **Opnieuw pictogram** ![](assets/redo-icon-on-task-list.png) om de teruggezette wijziging te herstellen.

1. (Optioneel) Klik met de rechtermuisknop op een taak die u wilt wijzigen.

   of

   Klik op de knop **Meer** menu ![](assets/more-icon-task-list.png).

1. (Optioneel) Kies een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Openen in een nieuw tabblad</strong> </td> 
      <td>Hiermee opent u de taak in een nieuw browsertabblad. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verwijderen</td> 
      <td>Voor informatie over het verwijderen van taken raadpleegt u <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Taken verwijderen</a>.</td> 
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
      <td role="rowheader">Taak invoegen boven</td> 
      <td>Hiermee voegt u een taak in boven de geselecteerde taak.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taak invoegen onder</td> 
      <td>Hiermee voegt u een taak in onder de geselecteerde taak</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dupliceren</td> 
      <td> <p>Hiermee maakt u een gedupliceerde versie van de taak in hetzelfde project. </p> <p>Voor informatie over het kopiëren en dupliceren van taken raadpleegt u <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Taken kopiëren en dupliceren</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront werkt alle in-project en dwars-project gebiedsdelen bij wanneer u veranderingen in de chronologie van taken aanbrengt.
1. Klikken **Opslaan** als u uw taakveranderingen permanent wilt houden en de chronologie van het project wilt bewaren.

#### Wijzigingen handmatig opslaan in een takenlijst wanneer u de optie Tijdlijnplanning handmatig opslaan selecteert {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

Het opslaan van uw veranderingen en alle projectgebiedsdelen is sneller. Dit is niet beschikbaar voor projecten met meer dan 2000 taken.

>[!IMPORTANT]
>
>Wij adviseren dat u deze optie gebruikt wanneer het uitgeven van een grote lijst van taken van meer dan een paar honderd die veel gebiedsdelen hebben. Met deze optie kunt u uw wijzigingen veel sneller visueel identificeren dan met de optie Handmatig opslaan.

Houd rekening met het volgende wanneer u de optie Tijdlijnplanning handmatig opslaan gebruikt in een takenlijst:

* U kunt de optie voor het handmatig opslaan van tijdlijnplanning niet toepassen op projecten met meer dan 2000 taken.
* U kunt geen aangepaste weergave, filter of groep toepassen op de takenlijst. De vervolgkeuzemenu&#39;s Weergave, Filter en Groeperen en het pictogram Gegraveerde weergave zijn uitgeschakeld. De weergave die standaard wordt toegepast, bevat een beperkt aantal velden.
* De chronologie van het project en alle in-projectgebiedsdelen worden automatisch berekend na elke verandering wanneer het Type van projectupdate Automatisch of Automatisch en bij Verandering is.
* De dwars-projectgebiedsdelen worden berekend nadat u sparen klikt, wanneer het Type van projectupdate Automatisch of Automatisch en op Verandering is. Voor informatie over het Type van projectupdate, zie [Selecteer het Type van projectupdate](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Taken in een lijst bewerken wanneer u de optie Tijdlijnplanning handmatig opslaan gebruikt:

1. Ga naar een project en klik vervolgens op de knop **Taken** sectie.
1. Klik op de knop **Abonnementsmodus** menu ![](assets/qs-list-mode-or-save-mode-icon-small.png) boven aan de lijst en selecteer **Handmatig opslaan** en klik vervolgens op **Tijdlijnplanning**> **Toepassen**.

   Deze optie is grijs voor projecten met meer dan 2000 taken.

   ![](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >Wanneer u bij deze pagina vandaan navigeert, schakelt Workfront de optie Automatisch opslaan opnieuw in.

   U ziet de volgende wijzigingen in de lijst:

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

     ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Bewerk elk veld dat u gemachtigd bent om handmatig bij te werken.

   ![](assets/inline-editing-a-task-350x26.png)

1. Druk op Enter om de aangebrachte wijzigingen tijdelijk op te slaan.
1. (Optioneel) Klik op de knop **Pictogram Ongedaan maken** ![](assets/undo-icon-on-task-list.png) om een wijziging om te keren en een veld terug te brengen naar de oorspronkelijke staat.
1. (Optioneel en voorwaardelijk) Klik op de knop **Opnieuw pictogram** ![](assets/redo-icon-on-task-list.png) om de wijziging die u hebt teruggedraaid, opnieuw in te voeren.

1. (Optioneel) Klik met de rechtermuisknop op een taak die u wilt wijzigen

   of

   Klik op de knop **Meer** menu ![](assets/more-icon-task-list.png).

1. Selecteer een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Openen in een nieuw tabblad</strong> </td> 
      <td>Hiermee opent u de taak in een nieuw browsertabblad. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verwijderen</td> 
      <td>Voor informatie over het verwijderen van taken raadpleegt u <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Taken verwijderen</a>.</td> 
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
      <td role="rowheader">Taak invoegen boven</td> 
      <td>Hiermee voegt u een taak in boven de geselecteerde taak.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taak invoegen onder</td> 
      <td>Hiermee voegt u een taak in onder de geselecteerde taak</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dupliceren</td> 
      <td> <p>Hiermee maakt u een gedupliceerde versie van de taak in hetzelfde project. </p> <p>Voor informatie over het kopiëren en dupliceren van taken raadpleegt u <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Taken kopiëren en dupliceren</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront werkt alle in-project en dwars-project gebiedsdelen bij wanneer u de chronologie van een taak verandert.
1. Klikken **Opslaan** als u uw taakveranderingen permanent wilt houden en de chronologie van het project wilt bewaren.

## Een taak in een lijst bewerken met Overzicht

1. Ga naar het project dat taken bevat u wilt uitgeven.
1. Klikken **Taken** in het linkerdeelvenster.

   De lijst van taken op de projectvertoningen.

1. Klik op het menu Meer ![](assets/more-icon-task-list.png) na de naam van de taak klikt u op **Samenvatting openen**. Selecteer de taak die u wilt bewerken en klik op de knop **Pictogram Samenvatting openen** ![](assets/qs-open-summary-icon-in-new-toolbar-small.png) rechtsboven in de lijst.

   De **Samenvatting** wordt geopend.

   ![](assets/qs-task-right-panel-in-a-task-list-350x328.png)

1. (Optioneel) Klik op de knop **X-pictogram** in de rechterbovenhoek van de samenvatting om het deelvenster te sluiten en de taken inline te bewerken.

   Voer de stappen uit over het bewerken van een taak in een lijst om de taak inline te bewerken.

   Voor informatie over het bewerken van de taak in een lijst raadpleegt u [Overwegingen bij het bewerken van taken in een lijst](#considerations-about-editing-tasks-in-a-list) in dit artikel.

1. (Optioneel) Typ een update voor de taak in het dialoogvenster **Updates** gebied.
1. Klik op een van de volgende pictogrammen of gebieden om naar de taak te gaan en gegevens op taakniveau te bewerken:

   | Documenten | Klikken **Klik hier voor toevoegen** om documenten aan de taak toe te voegen. |
   |---|---|
   | Details | Klik om informatie over de taak bij te werken. |
   | Aangepaste Forms | Klik om aangepaste Forms toe te voegen of te verwijderen of om informatie bij te werken op de formulieren. |
   | Uren | Klik om de uren te registreren. |
   | Goedkeuringen | Klik om taakgoedkeuringen toe te voegen. |

   {style="table-layout:auto"}

1. Klik op de knop Vorige in uw browser om terug te keren naar de takenlijst wanneer u klaar bent met het bijwerken van de taak.

## Taken bulksgewijs bewerken

U kunt meerdere taken tegelijk bewerken. Zorg ervoor dat u beheermachtigingen voor de taken hebt om deze te kunnen bewerken.

1. Ga naar een project dat taken bevat u in bulk wilt uitgeven.
1. Klikken **Taken** in het linkerdeelvenster.
1. Zorg ervoor dat de **Automatisch opslaan** is geselecteerd.

   >[!IMPORTANT]
   >
   >U kunt taken niet bulksgewijs bewerken wanneer u taken handmatig opslaat.

   Zie de sectie voor meer informatie over manieren om wijzigingen in taken in een lijst op te slaan [Overwegingen bij het bewerken van taken in een lijst](#considerations-about-editing-tasks-in-a-list) in dit artikel.

1. Selecteer verschillende taken in de takenlijst.
1. Klik op de knop **Pictogram Bewerken** ![](assets/qs-edit-icon.png).

   De **Taken bewerken** wordt geopend.

1. Geef de informatie op die u wilt wijzigen voor alle geselecteerde taken.

   Het bewerken van de informatie over alle taken is hetzelfde als het bewerken van de informatie over één taak. Als u taakduur wilt bewerken, moeten de geselecteerde taken dezelfde taakbeperking hebben; anders moet de **Duur** wordt niet gevuld.

   Zie voor meer informatie over het bewerken van een taak [Taken bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   >[!NOTE]
   >
   >De informatie die u wijzigt over alle geselecteerde taken overschrijft de bestaande informatie over afzonderlijke taken, behalve over de **Toewijzingen** veld. Als u een nieuwe toewijzing toevoegt in bulkbewerking, wordt die toewijzing toegevoegd aan alle geselecteerde taken. Als er andere toewijzingen zijn toegewezen aan de geselecteerde taken, blijven deze toegewezen naast de toewijzing die via bulkbewerking wordt toegevoegd.

1. Klikken **Aangepaste Forms** om de aangepaste formulieren te bewerken die zijn gekoppeld aan alle geselecteerde taken. Alleen actieve aangepaste formulieren worden in de lijst weergegeven.

   Als de geselecteerde taken geen aangepaste formulieren hebben, worden in deze sectie geen formulieren weergegeven.

   U kunt alleen de velden in de formulieren bewerken die zijn gekoppeld aan alle geselecteerde taken en die u kunt bewerken.

1. (Optioneel) Selecteer in de sectie Aangepaste Forms de optie **Aangepaste expressies opnieuw berekenen** zorgt u ervoor dat alle berekende aangepaste velden die zich bevinden op de aangepaste formulieren die zijn gekoppeld aan de geselecteerde taken, up-to-date zijn.
1. Klikken **Wijzigingen opslaan**.

   Alle wijzigingen die u hebt aangebracht, zijn nu zichtbaar voor alle geselecteerde taken.

Zie de sectie Meerdere aangepaste Forms bewerken wanneer objecten voor bulkbewerking worden bewerkt in [Aangepaste formulieren beheren die zijn gekoppeld aan objecten](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).
