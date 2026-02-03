---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Verbonden kaarten op borden gebruiken
description: U kunt een kaart aan uw bord toevoegen die met bestaande taken en kwesties in Workfront wordt verbonden.
author: Jenny
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: 6e136bed16c2b20f05267ac181dcc462b1a2aed4
workflow-type: tm+mt
source-wordcount: '1412'
ht-degree: 0%

---

# Gekoppelde kaarten op borden gebruiken

<!-- Audited: 2/2024 -->

U kunt een kaart aan uw board toevoegen die met bestaande taken en kwesties in [!DNL Workfront] wordt verbonden.

Wanneer een van de volgende gegevens voor de kaart op de ene locatie wordt bijgewerkt, wordt deze automatisch op de andere locatie bijgewerkt:

* [!UICONTROL Name]
* [!UICONTROL Description]
* [!UICONTROL Assignees]
* [!UICONTROL Status]
* [!UICONTROL Planned completion date]
* [!UICONTROL Estimation] / [!UICONTROL Story Points]
* [!UICONTROL Subtasks]
* [!UICONTROL Documents]

Als u verbonden kaarten wilt synchroniseren met Workfront, klikt u op het menu **[!UICONTROL More]** ![[!UICONTROL More menu]](assets/more-icon-spectrum.png) naast de naam van het tekengebied en selecteert u **[!UICONTROL Sync connected items]** . Gearchiveerde kaarten synchroniseren niet met Workfront-taken en -problemen. Als u een kaart herstelt, wordt deze opnieuw gesynchroniseerd.

>[!NOTE]
>
>Eén verbonden taak of uitgave kan slechts eenmaal per board worden toegevoegd. Dezelfde taak of uitgave kan met meerdere borden worden verbonden.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Medewerker of hoger</p> 
   <p>Aanvraag of hoger</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader">Configuraties op toegangsniveau</td>
   <td><p>Toegang tot taken en problemen weergeven of vergroten</p></td>
  </tr>
  <tr>
   <td role="rowheader">Objectmachtigingen</td>
   <td><p>Machtigingen weergeven of hoger voor de Workfront-taak of -uitgave</p>
</td>
  </tr>
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een aangesloten kaart toevoegen

{{step1-to-boards}}

1. Toegang tot een bord. Voor informatie, zie [&#x200B; creeer of geef een raad &#x200B;](../../agile/get-started-with-boards/create-edit-board.md) uit.
1. Klik op **[!UICONTROL Add card]>[!UICONTROL Connected card]** .
1. Kies een project en kies vervolgens een taak of uitgave die u als kaart aan de kaart wilt toevoegen.

   U kunt meerdere objecten selecteren en deze worden allemaal als aparte kaarten toegevoegd.

   >[!NOTE]
   >
   >* Alleen objecten waarvoor u machtigingen hebt, zijn beschikbaar in de zoekresultaten. Als een item grijs wordt weergegeven, is het al aan het bord toegevoegd.
   >* Wanneer u filtert op **[!UICONTROL Projects I Own]** of **[!UICONTROL Projects I'm On]** , worden projecten die overeenkomen met de status Voltooid, Dode of Geweigerd niet opgenomen. U kunt nog steeds naar die projecten zoeken met het filter **[!UICONTROL All]** .

1. Klik op **[!UICONTROL Add]**.

   ![&#x200B; Onderzoek naar taak of kwestie om &#x200B;](assets/boards-tasksissues-350x94.png) te verbinden

   De kaart wordt onder aan de linkerkolom toegevoegd. Het aangesloten [!DNL Workfront] -object en de bijbehorende toewijzingen worden weergegeven op de kaart.

   ![&#x200B; Verbonden kaart &#x200B;](assets/boards-connected-card-first-added.png)

1. Klik ![&#x200B; Open taak of kwestie &#x200B;](assets/boards-launch-icon.png) om de [!DNL Workfront] taak of kwestie in een nieuwe browser tabel te openen.
1. Als u de kaartgegevens wilt bewerken, klikt u op de kaart (niet op de kaartnaam).

   of

   Klik het **[!UICONTROL More]** menu ![&#x200B; Meer menu &#x200B;](assets/more-icon-spectrum.png) op de kaart en selecteer **[!UICONTROL Edit]**.

1. Voeg in het vak **[!UICONTROL Card Details]** de volgende informatie toe of werk deze bij:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Name]</strong></td> 
      <td>Als u de naam wijzigt, verandert ook de naam in het verbonden [!DNL Workfront] -object.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td> 
      <td>Als u de beschrijving wijzigt, verandert ook de beschrijving van het gekoppelde [!DNL Workfront] -object. U kunt URL's toevoegen in de beschrijving en deze worden klikbare koppelingen wanneer de kaart wordt opgeslagen.</td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Column]</strong></td>
      <td>Selecteer de kolom voor de kaart.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Status]</strong></td>
      <td><p>Selecteer een status voor de kaart. De standaardinstellingen zijn [!UICONTROL New] , [!UICONTROL In Progress] en [!UICONTROL Complete] , maar aangepaste statussen die voor het item in [!DNL Workfront] zijn gedefinieerd, zijn ook beschikbaar.</p>
      <p>Als u kolombeleid hebt ingeschakeld voor het bijwerken van veldwaarden, wordt bij het wijzigen van de status op de kaart de kaart automatisch naar de corresponderende kolom verplaatst. Voor meer informatie, zie "kolommontages en beleid"in het artikel <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref"> leiden boardkolommen </a>.</p>
      <p>Als u op <strong>[!UICONTROL Mark Complete]</strong> boven aan de kaart klikt, verandert de status automatisch in Voltooien.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Planned Completion]</strong></td>
      <td>Als u deze datum wijzigt, wordt ook de geplande voltooiingsdatum voor het gekoppelde [!DNL Workfront] -object gewijzigd.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimation]</strong></td>
      <td><p>Het aantal uren dat de kaart moet worden ingevuld.</p><p>Als u de schatting wijzigt, verandert ook de waarde van de artikelpunten in het verbonden [!DNL Workfront] -object.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Assignments]</strong></td>
      <td><p>Als u meer personen of een team aan de kaart wilt toewijzen, klikt u op <strong>[!UICONTROL Add Assignment]</strong> en typt u een naam in het zoekveld. Selecteer vervolgens de optie wanneer deze wordt weergegeven in de lijst met resultaten. U kunt zowel personen als teams toevoegen. Er is slechts één teamtoewijzing toegestaan op een aangesloten kaart.</p>
      <p>Toewijzingen die u selecteert, worden ook toegewezen aan de taak of uitgave in [!DNL Workfront] .</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tags]</strong></td>
      <td><p>Zoek naar en selecteer markeringen voor de kaart.</p>
      <p>Voor informatie bij het creëren van nieuwe markeringen, zie <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref"> markeringen </a> toevoegen.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom fields]</strong></td>
      <td><p>Aangepaste velden die u toevoegt, worden in dit gebied weergegeven.</p>
      <p>Voor meer informatie, zie <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md"> aanpassen welke gebieden op een kaart </a> worden getoond.</p></td>
     </tr>
     <tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Subtask]</strong></td>
      <td><p>Eventuele bestaande subtaken voor de taak worden in deze sectie weergegeven. Klik op <strong>[!UICONTROL Add Subtask]</strong> om een nieuwe subtaak toe te voegen.</p>
      <p>De teller bij de bovenkant van de sectie toont het aantal voltooide subtaken en het totale aantal subtaken.</p>
      <p>Voor meer informatie over subtaken, zie <a href="/help/quicksilver/agile/get-started-with-boards/manage-subtasks-on-boards.md"> subtaken op raad </a> leiden.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Checklist]</strong></td>
      <td><p>Klik op <strong>[!UICONTROL Add checklist item]</strong>. Typ vervolgens de titel van het item en druk op Enter. Er wordt automatisch een ander item toegevoegd. Ga door met titels om meer objecten toe te voegen.</p>
      <p>De teller boven aan de checklist toont het aantal voltooide items en het totale aantal items.</p> <p>Voor meer informatie over controlelijstitems, zie <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md"> controlelijstitems op kaarten </a> beheren.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Documents]</strong></td>
      <td>Voor een bestaand document, houd over de documentduimnagel, en klik <strong> Voorproef </strong> om het dossier in browser te bekijken of <strong> Download </strong> om het dossier aan uw computer te downloaden. Voor een nieuw document, zie <a href="/help/quicksilver/agile/get-started-with-boards/add-documents-on-cards.md"> documenten op kaarten </a> toevoegen.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Hours]</strong></td>
      <td>Zie "Loguren op een aangesloten kaart" hieronder.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Comments]</strong></td>
      <td><p>Klik in het veld <strong>[!UICONTROL New comment]</strong> en voer de opmerking in. Gebruik de opmaakgereedschappen om de tekst op te maken. Als u een persoon of team wilt labelen, gebruikt u het zoekvak onder aan het gebied met opmerkingen. De gebruiker hoeft geen lid van de raad te zijn. Gecodeerde gebruikers op verbonden kaarten ontvangen e-mailmeldingen.</p><p>Klik op <strong>[!UICONTROL Submit]</strong> om de opmerking aan de kaart toe te voegen.</p>
      <p>Voor meer informatie bij het becommentariëren, zie <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md"> het werk van de Update </a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL System activity]</strong></td> 
      <td><p>Als u <strong> toegelaten de activiteit van het 0&rbrace; Systeem als kaartsectie hebt, wordt de activiteit getoond op dit gebied.</strong></p> <p>Voor meer informatie, zie <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md"> aanpassen welke gebieden op een kaart </a> worden getoond en <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md"> systeem-geleide updates </a>.</p></td>
     </tr>     
    </tbody> 
   </table>

   Gebruik het linkernavigatievenster om tussen secties van gebieden op de kaartdetails te bewegen.

1. Klik op **[!UICONTROL Close]** om terug te keren naar het toetsenbord.
Het verbonden object, de toewijzingen, de tags, de vervaldatum, de controlelijstteller, de geschatte uren en de status worden weergegeven op de kaart.

   ![&#x200B; Kaart die aan raad &#x200B;](assets/boards-connected-card-details-110922.png) wordt toegevoegd

## Verbinding met een aangesloten kaart verbreken

U kunt een aangesloten kaart loskoppelen van het Workfront-object en de kaart blijft op het bord staan als een ad-hockaart die u kunt bewerken.

>[!NOTE]
>
>Als u een verbonden kaart op een dynamische raad losmaakt, zal het opnieuw verschijnen wanneer u de raad verfrist omdat dit bordtype alle taken en kwesties van een specifiek project vult.
>
>Als u een aangesloten kaart loskoppelt van een ander bordtype dat een innamekolom heeft, zal de kaart opnieuw in de innamekolom verschijnen wanneer u het board vernieuwt als de verbonden taak of de kwestie nog niet duidelijk volledig is.
>
>In beide scenario&#39;s, na verfrissen zult u twee kaarten voor de zelfde taak of kwestie hebben: een ad hoc kaart en een aangesloten kaart.

Om een kaart op het niveau van de raad los te maken:

1. Toegang tot het bord.
1. Klik het **[!UICONTROL More]** menu ![&#x200B; Meer menu &#x200B;](assets/more-icon-spectrum.png) op de verbonden kaart en selecteer **[!UICONTROL Disconnect]**.
1. Klik op **[!UICONTROL Disconnect]** in het bevestigingsbericht.

Een kaart op kaartniveau loskoppelen:

1. Open de kaart en open de kaart.
1. Klik het **[!UICONTROL More]** menu ![&#x200B; Meer menu &#x200B;](assets/more-icon-spectrum.png) op het gebied van de Verbinding van de kaartdetails, en selecteer **[!UICONTROL Disconnect]**.
1. Klik op **[!UICONTROL Disconnect]** in het bevestigingsbericht.

## Een ad-hockaart converteren naar een aangesloten kaart

Nadat u een ad-hockaart hebt gemaakt, kunt u deze converteren naar een aangesloten kaart. Voor details over ad hoc kaarten, zie [&#x200B; een ad hoc kaart aan een raad &#x200B;](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) toevoegen.

1. Open de kaart en open de ad-hockaart.
1. Controleer de naam en beschrijving op de kaart. Deze worden toegevoegd aan de taak of uitgave die u maakt in [!DNL Workfront] .
1. Klik in het gedeelte [!UICONTROL Connection] van de kaartgegevens op **[!UICONTROL Connect with Workfront]** .
1. Selecteer in het venster [!UICONTROL Connect Card] of u een taak of een uitgave maakt.
1. Zoek naar en selecteer een project om de taak of kwestie aan toe te voegen.

   >[!NOTE]
   >
   >* Alleen objecten waarvoor u machtigingen hebt, zijn beschikbaar in de zoekresultaten.
   >* Wanneer u filtert op **[!UICONTROL Projects I Own]** of **[!UICONTROL Projects I'm On]** , worden projecten die overeenkomen met de status [!UICONTROL Complete] , [!UICONTROL Dead] of [!UICONTROL Rejected] niet opgenomen. U kunt nog steeds naar die projecten zoeken met het filter **[!UICONTROL All]** .

1. Klik op **[!UICONTROL Connect]**.

   ![&#x200B; verbind ad hoc kaart met Workfront &#x200B;](assets/boards-connect-ad-hoc-card.png)

   De projectnaam wordt weergegeven in het gebied Verbinding op de kaartdetails.

1. Klik op **[!UICONTROL Close]** om terug te keren naar het toetsenbord.

## Uren vastleggen op een aangesloten kaart

U moet over de juiste machtigingen beschikken om de uren te kunnen vastleggen voor de verbonden taak of uitgave.

De velden voor tijdregistratie worden standaard niet weergegeven op verbonden kaarten. U moet [!UICONTROL **Uren**] in het [!UICONTROL Configure] gebied onder [!UICONTROL Cards] toelaten. Voor meer informatie, zie [&#x200B; aanpassen welke gebieden op een kaart &#x200B;](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md) worden getoond.

1. Voer het aantal uren in voor de taak of uitgave.
1. Selecteer een [!UICONTROL Hour Type] in het keuzemenu als deze niet de standaardwaarde heeft.
1. Klik [!UICONTROL **Tijd van het Logboek**].

   ![&#x200B; de uren van het Logboek op kaart &#x200B;](assets/log-hours-on-card.png)

   De tijd die op de kaart wordt geregistreerd wordt ook bewaard op de verbonden taak of de kwestie.

De registratietijd op de kaart is hetzelfde als de tijd die u nodig hebt om u aan te melden bij een taak of uitgave. Voor meer informatie, zie &quot;tijd van het Logboek op een project, een taak, of een kwestie&quot;in de tijd van het artikel [&#x200B; Logboek &#x200B;](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

