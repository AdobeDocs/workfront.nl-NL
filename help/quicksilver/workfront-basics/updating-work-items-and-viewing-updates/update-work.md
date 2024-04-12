---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Werk bijwerken
description: U kunt een update toevoegen aan een Adobe Workfront-object (project, taak of uitgave) om te communiceren over de voortgang van het object. Gebruikers die zijn toegewezen aan of geabonneerd op het object, kunnen uw update weergeven. U kunt gebruikers ook labelen om de update onder de aandacht te brengen.
author: Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: 886b5d9084cb1bfb63157152f05fa20128d34903
workflow-type: tm+mt
source-wordcount: '2971'
ht-degree: 0%

---

# Werk bijwerken

<!-- Audited: 1/2024 -->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>
-->

<!--info for April 11: hide the "Important" box below-->

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process. </span>
-->

U kunt een update toevoegen aan een Adobe Workfront-object om anderen te informeren over de voortgang van het object. Ga voor meer informatie over welke objecten u updates kunt toevoegen in Workfront naar [Overzicht van de sectie Bijwerken](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

De informatie in dit artikel beschrijft hoe u informatie voor projecten, taken, en kwesties kunt commentaren en bijwerken. Gebruikers die zijn toegewezen aan of geabonneerd op het object, kunnen uw update weergeven. U kunt gebruikers ook labelen om de update onder de aandacht te brengen.

Het toevoegen van opmerkingen aan andere objecten is vergelijkbaar met het bijwerken van projecten, taken en problemen. Zie ook de volgende artikelen voor meer informatie over opmerkingen over kaarten, doelen of herhalingen:

* [Doelopmerkingen beheren in Adobe Workfront-doelen](../../workfront-goals/goal-management/manage-goal-comments.md).

  U moet een extra licentie hebben om toegang te krijgen tot Workfront Goals.

* [Een ad-hockaart aan een kaart toevoegen](../../agile/get-started-with-boards/add-card-to-board.md)

* [Herhalingsopmerkingen beheren](/help/quicksilver/agile/use-scrum-in-an-agile-team/iterations/manage-iteration-updates.md)



## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie</strong></td> 
   <td> 
   <p>Huidig: Verzoek of hoger voor uitgaven en documenten; Controleren of hoger voor alle andere objecten</p>
   <p>Nieuw: Medewerker of hoger voor uitgaven en documenten: licht of hoger voor alle andere objecten</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau</strong></td> 
   <td> <p>Toegang weergeven of bewerken voor het object waarop de update betrekking heeft</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Toegang tot het object weergeven</p></td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Overwegingen bij het bijwerken van werkzaamheden

* In de sectie Updates kunt u opmerkingen toevoegen aan de meeste objecten in Adobe Workfront. Zie voor meer informatie over welke objecten de sectie Updates weergeven [Overzicht van de sectie Updates](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

* U kunt opmerkingen toevoegen aan Workfront-objecten vanuit andere toepassingen die zijn geïntegreerd met Workfront of vanuit de mobiele app Workfront.

  Niet alle toepassingen die zijn geïntegreerd met Workfront kunnen opmerkingen toevoegen aan Workfront-objecten.

  Niet alle functies die beschikbaar zijn in de sectie Updates van een object in Workfront zijn beschikbaar in andere toepassingen wanneer u Workfront-objecten opent vanuit de toepassing. Bijvoorbeeld, kunnen de Rich Text mogelijkheden of het maken van een commentaar privé aan het Bedrijf van iemand niet beschikbaar zijn wanneer het toevoegen van commentaren aan een voorwerp van Workfront van een derdetoepassing.

* U kunt tijdens het toevoegen van opmerkingen over het object communiceren over de voortgang van een Workfront-object (project, taak of uitgave). Gebruikers die zijn toegewezen aan of geabonneerd op het object, kunnen een melding over uw update ontvangen. Iedereen met View-toegang tot het object kan de update bekijken.

* U kunt gebruikers een tag toewijzen om hun aandacht te vestigen op de update. Gelabelde gebruikers ontvangen een melding in de app en een e-mail over uw update.

  >[!TIP]
  >
  >Eigenaars van opmerkingen worden automatisch gecodeerd. Zie voor meer informatie [Andere tags toepassen op updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).


* U kunt een opmerking toevoegen aan een object dat u kunt weergeven of u kunt zich aanmelden als Workfront of groepsbeheerder en namens een andere gebruiker een opmerking toevoegen. Zie voor meer informatie [Aanmelden als een andere gebruiker](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

* U kunt een update toevoegen aan projecten, taken en problemen in de volgende Workfront-regio&#39;s:

   * Vanuit een Workfront-object, in de sectie Updates (voor projecten, taken en problemen)
   * Vanuit het thuisgebied (voor taken en problemen)
   * Vanuit het deelvenster Samenvatting op de volgende gebieden (voor taken, problemen en documenten):

      * Een lijst met objecten
      * Een tijdschema
      * Home
      * De werklastbalans

<!--info for April 11: hide the section below: add an update to a work item-->

<!--
## Add an update to a work item

Adding an update to a work item differs depending on what version of the Updates section you use.

You can add updates to the following objects: 

* Projects
* Tasks
* Issues
* Programs
* Portfolios
* Templates
* Template tasks
* Users
* Timesheets
* Teams
* Goals
* Cards in the Boards area
* Iterations
-->

<!--info for April 11: hide the section below completely:-->

<!--
### Add an update to a work item in the legacy Updates section

>[!IMPORTANT]
>
>The information on this page describes how you update projects, tasks, and issues.

1. Go to the work item for which you want to provide an update (such as a project, task, or issue).
1. Click the **Updates** section.
1. (Conditional) If it is enabled, click the **New commenting** option in the upper-right corner of the Updates section to disable it and enable the legacy commenting experience.
1. Click **Start a new update,** then type your update.  
1. (Optional) Use the options in the Rich Text toolbar to format your text, add emojis, links, or images to your update, to enhance your content. For more information, see the [Use Rich Text in a Workfront update](#use-rich-text-in-a-workfront-update) section in this article.
1. (Optional) Update any of the following information about the work item:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Notify</strong></td> 
      <td>Identify users who must be notified of the update. Users assigned or subscribed to the object automatically receive notification when an update is made.<br><p>For information about how to include others on an update, see <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tag others on updates</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Commit Date</strong></td> 
      <td>In the date picker, select the date that you commit to complete the work item. For information about Commit Date, see <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Commit Date overview</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condition</strong></td> 
      <td>Select a new condition for the task or issue. For information about selecting a condition, see <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Update Condition for tasks and issues</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong></td> 
      <td>Click the arrow beside the current status, then select the desired status from the drop-down menu. For information about setting a Status, see <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Update task status</a>.<p>Updating the status of a work item does not automatically change the status of a project. Depending on how your project is set up, you might make updates to the project status separately. For more information on the various project update types, see <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.</p><p><b>NOTE</b>
      
      You cannot change the status of a work item while it is in a Pending Approval status.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Completion Bar</strong></td> 
      <td>(Only available on tasks) Indicate the percentage of work completed by sliding the progress bar to the desired percentage. You can also double-click the completion bar and enter the percent complete.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Private to my company</strong></td> 
      <td> <p>Disable this option to prevent users outside your company from having access to view this update.</p> 
      <p><b>NOTE</b></p>
      <p>This option displays only when the user is associated with a Company.</p>
      <p>This option is not available in all areas where you can add updates from. For example, this is not available in third-party applications where you can add updates from. </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Update** to add the update to the Workfront object.

   >[!NOTE]
   >
   >A small pop-up window will appear for seven seconds after clicking **Update**, allowing you to undo the update and return to the editing pane before the update is posted. The update is posted if you dismiss the undo pop-up, wait for it to disappear, or navigate away from the page. 
   >
   >If your Workfront administrator selects the "Never allow users to delete comments" setting in your access level, you cannot undo a comment. For more information, see [Create and modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. To reply to an update, see [Reply to updates](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).
-->

<!--info for April 11: reword the title of this section to: "Add an update to a work item"; take out the step that says you need to enable the "New commenting" toggle (I think it is step 3??)-->

## Een update toevoegen aan een werkitem

In dit artikel wordt beschreven hoe u project, taken of problemen kunt bijwerken. Het bijwerken van de meeste andere objecten is vergelijkbaar.

1. Zoek het object dat u wilt bijwerken en klik op de naam van het object om de objectpagina te openen.
1. Klikken  **Updates** in het linkerdeelvenster.
De **Opmerkingen** is standaard geselecteerd.

   <!--
   1. (Conditional) If the **New commenting** option is disabled, click to enable it. 

      This enables the new commenting experience. 

         >[!TIP]
         >
         ><span class="preview">The New commenting option has been removed in the Preview environment.</span>
   -->

1. Beginnen met een opmerking in het dialoogvenster **Nieuwe opmerking** doos.

   ![Nieuw opmerkingenvenster](assets/comment-box-all-tabs.png)

   >[!TIP]
   >
   >Als u weg navigeert uit de sectie Updates voordat u klaar bent met het typen en verzenden van een opmerking, wordt de opmerking op de pagina in de conceptmodus bewaard, zelfs nadat u zich hebt afgemeld en u weer hebt aangemeld. Afbeeldingen die aan de opmerking worden toegevoegd, worden ook in het concept opgeslagen. Concepten worden 7 dagen bewaard waarna ze worden verwijderd en kunnen niet worden hersteld. Getekende opmerkingen zijn alleen zichtbaar voor de gebruiker die ze invoert.

1. (Optioneel) Als u een wijziging ongedaan wilt maken of opnieuw wilt uitvoeren, gebruikt u de volgende sneltoetsen:
   * CTRL + Z ( ⌘+z voor Mac) om een wijziging ongedaan te maken
   * CTRL + Y ( ⌘+y voor Mac) om een wijziging opnieuw uit te voeren

1. (Optioneel) In het dialoogvenster **Tags toewijzen aan personen of teams** -gebied, typt u de naam of het e-mailadres van een gebruiker of een team dat u in deze opmerking wilt opnemen, en selecteert u deze vervolgens wanneer de opmerking in de lijst wordt weergegeven.
1. (Optioneel) Gebruik de opties op de werkbalk RTF om de tekst op te maken, emoties, koppelingen of afbeeldingen aan de update toe te voegen om de inhoud te verbeteren. Zie de klasse [RTF-bestanden gebruiken in een Workfront-update](#use-rich-text-in-a-workfront-update) in dit artikel.

   >[!TIP]
   >
   >Als een andere gebruiker een opmerking verzendt naar hetzelfde item dat u bijwerkt, wordt er een rode lijn weergegeven met de indicator &quot;Nieuw&quot; om u op de hoogte te brengen van de nieuwere opmerkingen.
   >
   >De indicator wordt alleen weergegeven nadat de opmerking op het item is verzonden, en niet wanneer de opmerking nog steeds wordt samengesteld.
   >
   >De indicator &quot;Nieuw&quot;toont slechts wanneer zowel de gebruiker die een nieuwe update inging als de gebruiker die momenteel een update ingaat de nieuwe opmerkingervaring gebruikt.
   >![](assets/real-time-new-red-indicator-unified-commenting.png)

1. Klikken **Verzenden** om de update aan het Workfront-object toe te voegen.
1. (Optioneel) Als u een opmerking wilt bewerken, klikt u op **Meer** menu ![](assets/more-menu.png) in de rechterbovenhoek van de opmerking klikt u op **Bewerken**.

   >[!IMPORTANT]
   >
   >Je kunt je opmerking alleen binnen 15 minuten bewerken nadat je deze hebt verzonden.

1. Bewerk de informatie in de opmerking, voeg afbeeldingen toe of verwijder afbeeldingen of verwijder een van de getagde gebruikers. Een indicator &quot;Bewerkt&quot; wordt toegevoegd links van de datumstempel die wordt weergegeven wanneer de opmerking is ingevoerd.

   >[!TIP]
   >
   >Opmerkingen van het lopende jaar worden niet in het datumstempel weergegeven. Als u de muis boven een tijdstempel houdt, wordt de volledige datum weergegeven, inclusief het jaar.

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >* Er wordt een e-mail gegenereerd om gebruikers alleen van uw update op de hoogte te stellen wanneer u de oorspronkelijke update verzendt. Er wordt geen e-mail gegenereerd nadat u de update hebt bewerkt.
   >* De datumstempel naast de opmerking is de datum van de oorspronkelijke opmerking en niet de datum van de laatste bewerking.
   >* Wanneer u een opmerking toevoegt namens een andere gebruiker (wanneer u zich aanmeldt als een andere gebruiker als Workfront of groepsbeheerder), kunt u de opmerking niet bewerken als u bent aangemeld als de andere gebruiker. U kunt de opmerking alleen bewerken nadat u zich hebt afgemeld als de gebruiker en u weer hebt aangemeld.

1. (Optioneel) Klik op **Antwoord** of u begint een opmerking te typen in het dialoogvenster **Antwoord toevoegen...** om te reageren op een bestaande opmerking, volgt u de bovenstaande stappen 3-7. <!--(**************insure this stays accurate***********)--> Voor informatie over het beantwoorden van een update raadpleegt u [Reageren op updates](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

1. (Voorwaardelijk en optioneel) Als andere gebruikers opmerkingen hebben toegevoegd die buiten het zichtbare gebied in de sectie Updates worden weergegeven terwijl u uw opmerkingen toevoegde, klikt u op **Weergave** in het blauw **banner voor nieuwe opmerkingen** onder aan het scherm om deze opmerkingen weer te geven.

   ![](assets/blue-new-comments-banner-with-view-button.png)

   Aanvullende opmerkingen worden onder in het scherm weergegeven.

1. (Optioneel) Klik op de knop **leuk** pictogram![](assets/like-icon.png). Het pictogram wordt bijgewerkt met het aantal ‘like’.
1. (Voorwaardelijk en optioneel) Als u extra personen hebt toegevoegd aan uw opmerking, klikt u op het aantal leden dat is opgenomen in de update om een lijst weer te geven met entiteiten waarmee de opmerking die u hebt ingevoerd, wordt gedeeld.

   ![](assets/members-icons-expanded-unshimmed.png)

   >[!TIP]
   >
   >De namen van de eerste twee getagde entiteiten worden naast hun avatars weergegeven. Als meer dan twee entiteiten zijn gelabeld, worden alleen de naam van de eerste entiteit en het aantal andere entiteiten weergegeven.

1. (Optioneel) Klik op de naam van een opmerking om de naam, de rol en het e-mailadres van de persoon of persoon weer te geven in een informatievak. Klik nogmaals op de naam van de opmerking in het informatievak om het gebruikersprofiel te openen.
1. (Optioneel) Klik op de knop **Systeemactiviteit** om updates weer te geven die zijn geregistreerd door het systeem. Wanneer het object of een van de onderliggende items wordt bijgewerkt, genereert Workfront een notitie over die update en geeft deze weer op het tabblad Systeemactiviteit.

   Zie voor meer informatie [Overzicht van de sectie Updates](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

   >[!TIP]
   >
   >U kunt geen opmerking toevoegen aan een systeemupdate. Nochtans, werden om het even welke antwoorden die aan de verslagen van de systeemactiviteit in de erfenis het becommentariëren ervaring werden gemaakt toegevoegd aan het lusje van de Activiteit van het Systeem als read-only. De ervaringen met opmerkingen uit het verleden zijn op 11 april 2024 uit Workfront verwijderd.

1. (Optioneel) Klik op de knop **Alles** -tabblad om zowel opmerkingen over de gebruikersactiviteit als opmerkingen over de systeemactiviteit op één plaats weer te geven. Dit is een alleen-weergeven tabblad.

   >[!TIP]
   >
   >U kunt niet reageren op opmerkingen of andere gebruikers tags toewijzen aan bestaande opmerkingen op het tabblad Alles. Als u wilt reageren op een opmerking op het tabblad Alles, klikt u **Reageren in opmerkingen** om de opmerking te openen op het tabblad Opmerkingen.

## RTF-bestanden gebruiken in een Workfront-update{#use-rich-text-in-a-workfront-update}

U kunt uw updates verbeteren met RTF-bestanden of door er verschillende items aan toe te voegen, zoals emojis, koppelingen of afbeeldingen.

1. Ga naar de **Updates** van een Workfront-object en een opmerking typen.
1. (Optioneel) Als u RTF-opmaak wilt toevoegen aan de update, gebruikt u de kenmerken op het tabblad **RTF** terwijl u typt.

   ![](assets/rich-text-toolbar.png)

   | **Kenmerk** | **Werkbalkknop** | **Mac-sneltoetsen** | **Windows-sneltoetsen** |
   |---|---|---|---|
   | Vet | ![](assets/mceclip10.png) | Alt+B | Ctrl+B |
   | Cursief | ![mceclip9.png](assets/mceclip9.png) | Alt+i | Ctrl+I |
   | Onderstrepen | ![mceclip8.png](assets/mceclip8.png) | Alt+u | Ctrl+U |
   | Hyperlink | ![mceclip7.png](assets/mceclip7.png) | <br>Het vak Koppelingen toevoegen openen: + K</br> <br>Als u een koppeling over de geselecteerde tekst wilt plakken, drukt u op OK+V</br> | <br>Het vak Koppelingen toevoegen openen: Ctrl+K</br> <br>Een koppeling over de geselecteerde tekst plakken: Ctrl+V</br> |
   | Lijst met opsommingstekens | ![mceclip6.png](assets/mceclip6.png) | Shift+8 | Ctrl+Shift+8 |
   | Genummerde lijst | ![mceclip5.png](assets/mceclip5.png) | Shift+7 | Ctrl+Shift+7 |
   <!--| Block Quote | ![](assets/block-quote-icon-large.png)|⌘+Shift+9 |<br>Ctrl+Shift+9</br> <br>This is not available in the new commenting experience. </br> |-->

   <!--remove the last row when we remove legacy from the system-->

   Als u de opmaak van tekst wilt stoppen, deselecteert u het kenmerk in het dialoogvenster **RTF** werkbalk.


   <!-- in the table above: take "Create Links" verbiage from the hyperlink when the old commenting is removed and the commenting beta is the only way to comment - with October 2023-->

   >[!NOTE]
   >
   >* Opmaak wordt ook weergegeven in e-mailberichten die gebruikers ontvangen met uw update.
   >* Opmaak van RTF-gegevens die wordt toegepast op een update in een e-mailbericht, wordt niet weergegeven in de update wanneer deze wordt weergegeven op het tabblad Updates.
   >* Als uw organisatie Workfront met Internet Explorer gebruikt, verliest alle opgemaakte tekst die in een update wordt geplakt zijn RTF-opmaak en wordt deze als onbewerkte tekst weergegeven. U kunt de tekst opnieuw opmaken met de kenmerken op de werkbalk RTF.
   >* Opmaak van RTF-tekst is niet beschikbaar voor updates die worden uitgevoerd in het gedeelte Timesheets of voor notitie- en laatste-voorwaardenobjecten die worden weergegeven in een rapport.

   <!--1. (Optional and conditional) If you want to include text from previous updates or from other sources and distinguish it from your own update, you can mark it as a Block Quote. Click the **Block Quote** icon ![](assets/block-quote-small.png) and type the text you want to quote. The quoted text displays marked with a vertical gray line. Click the **Block Quote** icon again to return to normal formatting. This is not available in the new commenting experience.-->

   <!--remove this picture below and the bullet above when we remove legacy-->

   <!--![](assets/block-quote-marked-350x144.png)-->

1. (Optioneel) Klik op de knop **emoji** pictogram ![](assets/emoji-icon.png) om emojis aan uw update toe te voegen.

   >[!NOTE]
   >
   >* Workfront vervangt leestekens zoals :) niet door emojis.
   >* Emojis is niet beschikbaar voor de voorwerpen van de Nota en van de Laatste Voorwaarde die in een rapport worden bekeken.
   >* De functie emoji in Workfront gebruikt Unicode-tekens en wordt als zodanig alleen weergegeven in browsers en besturingssystemen die Unicode-codepunten ondersteunen. Gebruikers van een ander platform, browser of besturingssysteem hebben mogelijk geen toegang tot hetzelfde domein.
   >* Een niet-ondersteunde emoji wordt weergegeven door een zwarte of witte doos.
   >* Windows 7 biedt alleen ondersteuning voor zwart-witafbeeldingen.
   >* Mojs die worden toegepast op een update die via e-mail wordt uitgevoerd, worden niet weergegeven in de update wanneer deze wordt weergegeven in het gedeelte Updates.

1. (Optioneel) Een URL-koppeling toevoegen aan extra informatiebronnen:

   1. Klik in de update op de plaats waar u een koppeling wilt invoegen.
   1. Op de **RTF** klikt u op de **Hyperlink** pictogram ![](assets/link-icon.png).

   1. In de **Koppeling maken** vak dat wordt weergegeven onder **URL**, typt of plakt u de URL van de bron waaraan u wilt koppelen.

   1. Onder **Weer te geven tekst**, typt of plakt u de koppelingstekst.
   1. Klikken **Opslaan**.

1. (Optioneel) Voer een van de volgende handelingen uit om een afbeelding aan de update te koppelen:

   * Sla de afbeelding op onze computer op en sleep deze naar het gebied Nieuwe opmerking.
   * Kopieer een schermafbeelding van uw computer en plak deze vervolgens in de opmerking.<!-- This is not available in the legacy commenting experience.-->
   * Klik op de knop **Afbeelding toevoegen** pictogram ![](assets/add-image-mountain-with-plus-icon.png) en bladert u naar de afbeelding op uw computer.


   >[!NOTE]
   >
   >* Uw Workfront-beheerder moet het toevoegen van afbeeldingen inschakelen in het gedeelte Voorkeuren voor feeds bijwerken van het gebied Workfront Interface voordat u de pictogrammen Afbeelding of Bijlage toevoegen kunt zien. Zie voor meer informatie [Voorkeuren voor gebruikersupdates configureren](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
   >* De maximale bestandsgrootte voor afbeeldingen is 7 MB. Ondersteunde bestandstypen zijn .jpg, .gif en .png.
   >* Afbeeldingen zijn toegankelijk vanuit de sectie Updates van een object en zijn ook beschikbaar in het gebied Documenten onder het hoofdmenu.
   >* U kunt de afbeelding plakken door met de rechtermuisknop op de nieuwe opmerking te klikken of door op CTRL + V voor Windows (of  V voor Mac) te drukken op het toetsenbord.
   >* U kunt een update verzenden met een afbeelding en geen tekst.
   >* Wanneer u een opmerking verwijdert die een afbeelding bevat, wordt de afbeelding verwijderd uit de sectie Updates en uit het gebied Documenten. De afbeelding wordt ook verwijderd uit het gebied Documenten wanneer u een opmerking bewerkt en de afbeelding verwijdert.
   >* Wanneer iemand een afbeelding verwijdert die is gekoppeld aan een opmerking in het gebied Documenten, wordt deze ook uit de opmerking verwijderd.

   <!--remove the statement above about legacy, when we remove the legacy environment.-->

1. (Optioneel) Voer een van de volgende handelingen uit om een afbeelding weer te geven in de bestaande update:

   * Klik op de knop **Voorvertoning** pictogram ![](assets/previewimageicon-31x31.png) op de miniatuur van de afbeelding om de afbeelding op volledige grootte te openen in een nieuw browsertabblad.
   * Klik op de knop **Downloaden** pictogram ![](assets/downloadimageicon.png) op de miniatuur van de afbeelding om de afbeelding te downloaden.

1. Klikken **Verzenden** om uw opmerking toe te voegen.

## Zoeken naar een update

U kunt een opmerking of antwoord zoeken in de sectie Updates van een object.

1. Ga naar de **Updates** van een object.
1. Een trefwoord beginnen te typen <!--or a user's name --> in de **Zoeken** in de rechterbovenhoek van het dialoogvenster **Opmerkingen** tab.

   <!--Add this tip or note instead of the note below - when it'll be possible: You can search for users who have been tagged or for comment owners.-->

   >[!NOTE]
   >
   >U kunt alleen zoeken naar woorden die bij de tekst van een opmerking of antwoord horen. U kunt niet zoeken naar namen van gebruikers of teams die in een update zijn getagd.

   ![Zoeken in updates](assets/updates-all-tabs-with-search-field.png)

   Het trefwoord <!--or user--> u hebt gezocht naar wordt benadrukt en de commentaren die het bevatten tonen bij de bovenkant van de sectie van Updates.

   Workfront zoekt naar de volledige updatestream van het object, buiten de opmerkingen die op het scherm zichtbaar zijn.

1. Klik op de knop **x** in het zoekveld om de zoekresultaten te wissen en terug te keren naar alle opmerkingen.

<!-- when we release search to production, check above and make sure you don't have to add that the users tagged/ owners are also searchable-->

## Updates kopiëren

U kunt een update op verschillende manieren kopiëren.

U kunt een koppeling naar de update kopiëren of de inhoud van een update kopiëren en deze gebruiken in een nieuwe update.

<!--Copying an update differs depending on which commenting experience you use.-->

<!--info for April 11: take the sentence above out and reword the section title below to: Copy an update-->

### Een update kopiëren <!--in the new commenting experience-->

<!--For information about what features are available for the new commenting experience and for what objects, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).-->

U kunt informatie uit een bestaande opmerking kopiëren door een van de volgende handelingen uit te voeren:

* [Koppeling kopiëren](#copy-link)
* [Platte tekst kopiëren](#copy-body-text)
* [Offerteantwoord](#quote-reply)

![](assets/copy-comment-ways-from-more-menu-on-comment.png)

#### Koppeling kopiëren

Met de koppelingsoptie Kopiëren kopieert u de opmerking of de koppeling naar het klembord, zodat u de opmerking of de volledige verbinding met andere gebruikers kunt delen.

1. Ga naar de update waarvan u de koppeling wilt kopiëren.

1. Klik op de knop **Meer** en klik vervolgens op **Koppeling kopiëren**.

1. Plak de koppeling die u in de vorige stap hebt gekopieerd in een e-mail of een andere toepassing om deze met anderen te delen. Met de gedeelde koppeling wordt de opmerking geopend waaruit u de koppeling hebt gedeeld.

   >[!TIP]
   >
   >Wanneer u de verbinding van een gesprek over een kindvoorwerp van een hoger-rangschikkend voorwerp deelt, opent de verbinding de draad in het hoger-rangschikkende gebied van de Updates van objecten.
   >
   >Bijvoorbeeld, als u de verbinding van een taakcommentaar van het gebied van Updates van het project kopieert, opent de commentaar de projectpagina.

#### Platte tekst kopiëren

Met de optie Tekst kopiëren wordt de tekst van een specifieke update naar het klembord gekopieerd.

1. Ga naar de update of het antwoord dat u wilt kopiëren.
1. Klik op de knop **Meer** en klik vervolgens op **Platte tekst kopiëren**.

#### Offerteantwoord

Met de antwoordoptie Citaat kopieert u de oorspronkelijke opmerking naar een nieuw antwoord als een blokcitaat.

1. Ga naar de update of het antwoord dat u wilt kopiëren.
1. Klik op de knop **Meer** en klik vervolgens op **Offerteantwoord**.

   Er wordt een nieuw opmerkingsvak geopend en het geciteerde antwoord wordt opgenomen in de nieuwe opmerking en gemarkeerd als een blokcitaat.

   ![](assets/block-quote-highlighted-mid-comment-before-submit.png)


1. Voeg je update toe en klik op **Verzenden** om de opmerking toe te voegen.

<!--info for April 11: hide the entire section below - notice that there are several sub-sub sections below this main section - hide them all, all the way up to "Delete an update"-->

<!--
### Copy an update in the legacy commenting experience

* [Copy the update](#copy-the-update) 
* [Copy the thread link](#copy-the-thread-link) 
* [Copy the update link](#copy-the-update-link)
* [Quote Reply](#quote-reply)

   >[!TIP]
   >
   >When you copy and share the link of a conversation on a child object from a higher-ranking object, the link opens the thread in the child object's Updates area. 
   >
   >For example, if you copy the link of a task comment from the project's Updates area, the comment opens the task page.

#### Copy the update {#copy-the-update}

This option copies the text from a specific update to the clipboard.

1. Go to the update or reply you want to copy.
1. Click the **More** menu, then click **Copy body text**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

#### Copy the thread link {#copy-the-thread-link}

This option copies the full thread link to the clipboard so you can share the thread with other users.

1. Go to the update thread you want to copy.

1. Click the **More** menu, then click **Copy thread link**.

   ![](assets/update-stream-comment-menu-marked-350x152.png) 

1. Paste the link you copied in the previous step in an email or another application to share it with others. The shared link opens the comment you shared the link from. 

#### Copy the update link {#copy-the-update-link}

This option copies a specific update link to the clipboard. When you share the update link, the user who follows it sees a border around the update.

1. Go to the update or reply you want to copy.
1. Click the **More** menu next to the individual update, then click **Copy update link**.

   ![](assets/copy-update-link-old-ui.png)

1. Paste the link you copied in the previous step in an email or another application to share it with others. The shared link opens the comment you shared the link from. 

#### Quote Reply  

The Quote Reply option copies the original comment to a new reply as a block quote. 

1. Go to the update or reply you want to copy.
1. Click the **More** menu, then click **Quote Reply**.

   A new comment box opens and the quoted reply is included in the new comment and marked as a block quote.

1. Continue adding your update and click **Reply** to add the comment.
-->

## Een update of antwoord verwijderen

Afhankelijk van de toegang die uw Workfront-beheerder u biedt, kunt u mogelijk updates verwijderen die u hebt toegevoegd op het tabblad Updates van een object. Zie voor meer informatie [Aangepaste toegangsniveaus maken of wijzigen](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) in het artikel [Aangepaste toegangsniveaus maken of wijzigen](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Geen enkele Workfront-gebruiker (inclusief de Workfront-beheerder) kan updates van een andere gebruiker verwijderen. Nochtans, als het de toegangsniveau van een gebruiker hen toestaat om hun eigen updates te schrappen, kan de beheerder van Workfront login als die gebruiker en schrapt updates zij aanbrachten. Zie voor meer informatie [Aangepaste toegangsniveaus maken of wijzigen](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) en [Aanmelden als een andere gebruiker](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. Ga naar de update of het antwoord dat u wilt verwijderen.
1. Klik op de knop **Meer** naast de update of het antwoord dat u wilt verwijderen, klikt u op **Verwijderen**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. Klik in het bericht dat wordt weergegeven op **Verwijderen**.

   >[!NOTE]
   >
   >Als u een update met een bijgevoegde afbeelding verwijdert, worden zowel de opmerking als de afbeelding verwijderd. Zie de klasse [RTF-bestanden gebruiken in een Workfront-update](#use-rich-text-in-a-workfront-update) in dit artikel.

   Wanneer aan de opmerking die u verwijdert, reacties zijn gekoppeld, wordt aangegeven dat de opmerking is verwijderd met de naam van de gebruiker die de opmerking heeft verwijderd.

   ![](assets/removed-comment-indicator-new-experience.png)

   Verwijderde opmerkingen worden direct uit Workfront verwijderd. Een gebruiker die de sectie van Updates gebruikt ziet een commentaar dat door een andere gebruiker in echt - tijd wordt geschrapt.


## Systeemupdates controleren

In de sectie Updates van een Workfront-object worden twee soorten gegevens weergegeven:

* **Gebruikers: updates:** De updates van de gebruiker zijn commentaren die u en andere gebruikers in uw systeem ingaan. De gebruikersupdates worden weergegeven in de tabbladen Opmerkingen en Alle van de sectie Updates.

  ![](assets/user-update-cl-350x277.png)

* **Systeemupdates:** Bij systeemupdates worden taken of problemen verwijderd, documentversies toegevoegd of verwijderd, een goedkeuringsaanvraag bijgevoegd of verwijderd, en eventuele bewerkingen of wijzigingen die in het object zijn aangebracht. De updates van het systeem tonen in de Activiteit van het Systeem en de Alle lusjes van de sectie van Updates.

  ![](assets/system-updates-cl-350x277.png)

  Workfront-beheerders kunnen bepalen wat wordt bijgehouden in systeemupdates, zoals wordt uitgelegd in [Door het systeem bijgehouden updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). U kunt ook systeemupdates of -activiteiten uitfilteren, zodat alleen gebruikersupdates voor alle objecten worden weergegeven.

  De volgende objecten hebben geen door het systeem gegenereerde updates:

   * Team
   * Sjabloon
   * Sjabloontaak
   * Ad-hockaart

Zie voor meer informatie over systeemupdates in de sectie Updates [Overzicht van de sectie Updates](../updating-work-items-and-viewing-updates/updates-tab-overview.md).


<!--
After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  
-->

<!-- with October 26 release: add somewhere this, and decide where we need to keep information about the legacy commenting. Should we create an article about iterations comments like we have for goals and cards?!:

>[!NOTE]
>
>Iterations display the legacy commenting experience.-->

<!--old message, before Auhust 17: 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>For more information about the new commenting experience, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>You can access the new experience for the following objects:
> * Issues, projects, tasks, and documents.
>
>     This is available when you enable the commenting Beta experience.
>
>     This functionality is available only for the Updates section, and it is not available for the following areas:
>
>     * Home
>     * Summary panel in lists
>     * Summary panel in timesheets
>
> * Goals, cards in the Boards area
>
>   The new commenting experience is the only experience for goals and cards. You must have an additional license to access Workfront Goals. For more information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 
>
>     You can add and view updates to cards in the Boards area when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md).
-->