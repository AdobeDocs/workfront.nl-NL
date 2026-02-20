---
title: De lijstweergave beheren in de Adobe Workfront-planning
description: U kunt objecten en hun velden in een lijstweergave weergeven, wanneer u ze opent in de Verbonden recordpagina van een record, in Adobe Workfront Planning. In dit artikel wordt beschreven hoe u een lijstweergave kunt maken of bewerken op de pagina Verbonden records van een record.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
source-git-commit: a5f33f914dabaa9368dea919510375bcb6ee03e2
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 0%

---


# De lijstweergave beheren in Adobe Workfront Planning

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

U kunt objecten en hun velden in een lijstweergave weergeven, wanneer u ze opent in de Verbonden recordpagina van een record, in Adobe Workfront Planning.

In dit artikel wordt beschreven hoe u een lijstweergave kunt maken of bewerken op de pagina Verbonden records van een record en hoe u de objecten in de weergave kunt bewerken.

## Toegangsvereisten

+++ Breid uit om de toegangsvereisten voor de functionaliteit in dit artikel te bekijken. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Alle Workfront en alle planningspakketten</p>
<p>Willekeurige workflow en planningspakket</p>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p> Standaard voor het maken en verwijderen van weergaven</p>
   <p>Medewerker of hoger om weergave-elementen bij te werken</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Rechten beheren voor een weergave</p>  
   <p>Machtigingen weergeven voor een weergave om de weergave-instellingen tijdelijk te wijzigen of te dupliceren</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> De gebruikers met een Licht of de vergunning van de Medewerker moeten een lay-outmalplaatje worden toegewezen dat Planning omvat.
   <p>De standaardgebruikers en de Beheerders van het Systeem hebben de Gebieden van de Planning die door gebrek worden toegelaten.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

## Overwegingen over lijstweergaven

* U kunt geen records weergeven in de recordtypepagina&#39;s in een lijstweergave. U kunt de volgende objecten alleen weergeven in een lijstweergave wanneer u ze bekijkt op de pagina Verbonden records van een record:

   * Workfront-projecten

  Voor informatie over het creëren van een verbonden verslagenpagina, zie [&#x200B; een Verbonden verslagenpagina aan een verslag &#x200B;](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md) toevoegen.
* Voordat u een lijstweergave kunt weergeven in een verbonden recordpagina van een record, moet u Workfront-projecten verbinden met de recordtypen Planning. Voor informatie, zie [&#x200B; verbind verslagtypes &#x200B;](/help/quicksilver/planning/architecture/connect-record-types.md).
* Lijstweergaven zijn vergelijkbaar met Uitgebreide lijsten. Voor meer informatie, zie [&#x200B; Gebruik verbeterde lijsten &#x200B;](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


## Een lijstweergave beheren {#manage-a-list-view}

Voor meer informatie over het beheren van lijstmeningen in Workfront, zie [&#x200B; Uitgebreide lijsten van het Gebruik &#x200B;](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

{{step1-to-planning}}

1. Klik op een werkruimtekaart en klik vervolgens op een opnametype.
1. Klik vanuit een willekeurige weergave op de naam van een record om de voorvertoning of detailpagina van de record te openen.
1. Voeg a **Verbonden verslagenpagina** voor verbonden projecten toe zoals die in het artikel [&#x200B; worden beschreven een Verbonden verslagenpagina aan een verslag &#x200B;](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md) toevoegen.

   Op de pagina Verbonden records worden projecten weergegeven die zijn verbonden met de record in de lijstweergave.

   <!--add new screen shot when they release Row colors/ special formatting for rows-->

   ![&#x200B; Projecten op verbonden verslagenpagina in lijstmening &#x200B;](assets/projects-on-connected-records-page-list-view.png)

1. (Optioneel) Voer een van de volgende handelingen uit om de lijstweergave te wijzigen:

   1. Vouw het menu van dropdown meningen in de hoger-juiste hoek van de lijst uit om een andere mening te selecteren, of klik **Nieuwe mening** en creeer een andere.

      Weergaven worden door het hele systeem gedeeld. Als u een mening van Projecten voor één verslagtype creeert, kunt u het op andere verslagtypes bekijken die verbonden projecten tonen.

   1. Beweeg over de naam van een bestaande mening en klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png), dan klik één van het volgende:
      * **noem** anders, om de mening een nieuwe naam te geven
      * **Aandeel**, om de mening met anderen te delen
      * **Schrapping**, om de mening te schrappen.

      >[!NOTE]
      >
      >* U moet over beheerdersmachtigingen voor een weergave beschikken om de weergave te kunnen bewerken, delen of verwijderen.
      >
      >* U kunt de systeemweergaven niet wijzigen.
      >
      <!--* <span class="preview">You can reset a view that was shared with you after you modified it to restore its original preferences, or you can copy it with your changes and share the copy. For more information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>
        -->
   1. Klik het **pictogram van de Filter** pictogram ![&#x200B; van de Filter &#x200B;](assets/filter-icon.png) om een filter aan de mening toe te voegen. De resultaten worden direct in de lijst gefilterd. U kunt filters niet opslaan en een naam geven. Filters worden onthouden wanneer u de pagina in de toekomst opent en maken deel uit van gedeelde weergaven.
   1. Klik het **pictogram van Kolommen** pictogram van Kolommen ![&#x200B; &#x200B;](assets/columns-icon.png) om te selecteren welke kolommen aan vertoning of in de mening te verbergen.
   1. Houd de cursor boven de naam van een kolom en klik op de pijl omlaag links van de kolomnaam en klik op een van de volgende opties:
      * **noem** anders, om a **Eigen etiket** voor de kolom toe te voegen. De naam van het oorspronkelijke veld in Workfront verandert niet.
      * **Soort**, om de lijst door het geselecteerde gebied te sorteren. Aan de kolomkop wordt een sorteerpictogram toegevoegd dat de richting van het sorteren aangeeft.
   1. Klik het **+** pictogram in de hoger-juiste hoek van de lijst om kolommen aan de lijst toe te voegen of te verwijderen, dan klik **sparen**.

      De **manager van de Kolom** opent.

      U kunt alleen bestaande velden toevoegen aan de lijstweergave.
U kunt het primaire veld niet verwijderen in de lijstweergave die in de eerste kolom wordt weergegeven.


   <!--
    1. <span class="preview">Click **Row colors** <!-insert icon and edit the name of the icon if they changed it->. The **Format** box opens. <!-change the name of the box when they update it-></span>
        <span class="preview">Do the following: </span>
        <div class="preview">
        1. Define the formatting conditions in the **If** area by clicking **Add condition**, then select a field you want to format by and choose a field value. 
            >[!TIP]
            >
            >Only field visible in the list view are available for conditional formatting.
        1. (Optional) Click **Add condition** in the If area to add more conditions. 
        1. Click the **Or** connector between conditions to change to **And**. **Or** is the default connector.  
        1. In the **Format** area, select a field to indicate which column will be formatted. <!-edit this area, if it changes names???->
        1. Click on the color circle to expand and choose another color.
        1. Turn on the **Apply to row** setting to apply the formatting to the entire row that meets the conditions. 
        1. (Optional) Click **Clear all** to remove all formatting.
            The formatting is applies immediately.
        1. Click outside the **Format** box to close it. 
            This returns you to the list view. There is a blue dot next to the **Row colors** icon to indicate that the view has special formatting applied. <!-might need to edit the icon name and get a screen shot of the icon with the dot and insert it here->
        </div>
    -->

1. (Optioneel) Voeg een trefwoord toe in het zoekvak rechtsboven in de lijst om naar een item te zoeken.


   Objecten die overeenkomen met de zoekterm worden gemarkeerd in de lijst.
1. (Optioneel) Als u meer items aan de lijst wilt toevoegen en deze automatisch wilt verbinden met de geselecteerde record, voert u een van de volgende handelingen uit:

   * Klik **verbinden verslagen** in de hoger-juiste hoek van de lijst om bestaande punten toe te voegen.
   * Klik **Nieuwe rij** bij de bodem van de lijst om nieuwe punten toe te voegen.
1. Klik op de naam van een verbonden item in de lijst om het te openen op een ander browsertabblad.
1. Dubbelklik in een cel in de lijst om de gegevens van een veld te bewerken en druk vervolgens op Enter om de wijzigingen op te slaan.

   Sommige velden zijn alleen-lezen. Het percentage voltooide van een project is bijvoorbeeld een veld dat door het systeem wordt berekend en u kunt het niet handmatig bewerken.

1. Beweeg over de naam van een punt in de lijst en klik **Meer** menu [&#x200B; Meer menu &#x200B;](assets/more-menu.png) en klik **Mening** om het project in een ander lusje te openen

   of

   Selecteer een of meer items en bekijk de actiebalk onder aan de lijst en klik op een van de volgende opties:

   * **Schrapping** om het project te schrappen. Als u een project verwijdert, wordt de verbinding met het project verbroken en verplaatst naar de prullenbak van Workfront. Workfront-beheerders kunnen verwijderde projecten herstellen tot 30 dagen nadat ze zijn verwijderd.
   * **maak** los om het project van het verslag los te maken. Als u een project loskoppelt, verwijdert u het project en alle waarden van de opzoekvelden uit de huidige record.

   ![&#x200B; bar van Acties in de Verbonden mening van de Lijst van de verslagenpagina &#x200B;](assets/actions-bar-connected-records-page-list-view.png)

