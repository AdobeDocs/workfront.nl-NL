---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Logtijd
description: U kunt tijd voor het werkpunten in&amp registreren;nbsp;Adobe Workfront om op het aantal uren te wijzen u het werken aan hen doorwerkt. U kunt tijd ook registreren die niet met het werk, zoals vakantie, zieke tijd, of tijd verwant is u in vergaderingen doorbrengt. De tijd u registreert toont in uw timesheet.
author: Lisa
feature: Timesheets
role: User
exl-id: 120173a8-95f1-4233-ab40-d3bcfe38c977
source-git-commit: a23708b2534330cf942c5f950c4bee1a90583ea7
workflow-type: tm+mt
source-wordcount: '4137'
ht-degree: 0%

---

# Logtijd

<!--Audited: 5/2025-->

<!--remove all preview and production references if any-->
<!--update screen shots for the general hour entries and the mixed selection of hours at production, if they fixed the bugs -->

U kunt de tijd voor het werk in Adobe Workfront registreren om op het aantal uren te wijzen u het werken aan hen doorwerkt. U kunt tijd ook registreren die niet met het werk, zoals vakantie, zieke tijd, of tijd verwant is u in vergaderingen doorbrengt. De tijd u registreert toont in uw timesheet.

Voor meer informatie over het type van uren kunt u login Workfront, zie [&#x200B; de types van uren beheren &#x200B;](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Licht of hoger om uren op een project, een taak, een kwestie, of Algemene Uren op een timesheet te registreren</p>

<p>Of: </p>

<ul><li><p>Controle of hoger aan logboek Algemene Uren in een timesheet</p></li>
   <li><p>Werk of hoger om uren aan een project, een taak of een kwestie te registreren</p></li></ul> </td> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>Geef toegang tot het type van het werkpunt uit u tijd voor registreert </p> <p>U hebt bijvoorbeeld toegang tot problemen bewerken nodig om u aan te melden bij problemen</p> </td>
  </tr> 
  <tr> 
   <td>Objectmachtigingen</td>
   <td> <p>Draag of hogere toestemmingen op het het werkpunt bij u tijd voor dat omvat toestemmingen aan Loguren</p> </td>
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het aanmelden in Workfront

* U kunt tijd voor projecten, taken, of kwesties registreren, of u kunt tijd in uw timesheet direct registreren.

  Voor informatie over het creëren van timesheets, zie [&#x200B; een enig-gebruik timesheet &#x200B;](../../timesheets/create-and-manage-timesheets/create-tmshts.md) creëren.

* Alle tijd die door hulpmiddelen buiten timesheet wordt geregistreerd verschijnt in timesheet voor de overeenkomstige tijdspanne.
* Taken en problemen met een project dat niet actueel is, worden niet vooraf in een tijdspagina geplaatst.
* De tijd die in timesheet wordt geregistreerd wordt onmiddellijk toegepast op de taak, de kwestie, of het project.
* De tijdbladen bevatten de totale tijd voor alle geregistreerde datums. Weekends zijn altijd inbegrepen, zelfs wanneer de chronologieberekeningen zijn gevormd om hen (zoals die in [&#x200B; worden beschreven vormen systeem-brede projectvoorkeur &#x200B;](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)) uit te sluiten.
* Het maximumaantal punten dat in een timesheet wordt getoond is 45. Als er meer dan 45 punten zijn de waarvan data het timesheet tijdkader aanpassen, slechts de onlangs bijgewerkte punten tonen.
* Uur-items die in factureringsrecords zijn opgenomen, worden grijs weergegeven en kunnen niet worden bewerkt in de tijdpagina. Voor meer informatie, zie [&#x200B; het factureren verslagen &#x200B;](../../manage-work/projects/project-finances/create-billing-records.md) creëren.
* De persoonlijke taken tonen niet in timesheet door gebrek. De persoonlijke taken tonen in timesheet slechts wanneer zij tijd het programma wordt geopend. Nadat u de tijd op een persoonlijke taak registreert, kunt u de taak aan timesheet vastzetten en het zal op timesheet blijven als het vastgezet blijft. Voor meer informatie, zie [&#x200B; het werkpunten en projecten van het gebied van het Huis &#x200B;](../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md) creëren.

## Logtijd {#log-time-section}

U kunt zich in Workfront aanmelden in de volgende gebieden:

* [&#x200B; Timesheet &#x200B;](#timesheet)
* [&#x200B; Huis &#x200B;](#home)
* [&#x200B; Project, taak, of kwestie &#x200B;](#project-task-or-issue)
* [Het deelvenster Samenvatting](#summary-panel)
* [Borden](#boards)
* [Mobiele app](#mobile-app)

### Tijdschema {#timesheet}

#### De tijd van het logboek op een timesheet {#log-time-on-a-timesheet}

U kunt tijd aan de volgende punten in timesheet registreren:

* Taken, problemen en projecten die vooraf zijn ingevuld, worden automatisch weergegeven op basis van de manier waarop uw Workfront-beheerder de voorkeuren voor de tijdpagina instelt. Voor informatie over hoe timesheets pre-bevolkt zijn, zie [&#x200B; timesheet en uurvoorkeur &#x200B;](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) vormen.

  Alleen de taken en problemen die aan u zijn toegewezen, worden vooraf ingevuld in uw overzicht. De taken en de kwesties die aan uw teams of baanrollen worden toegewezen bevolken automatisch niet uw timesheet.

  Als u op het item klikt op het item dat aan uw teams is toegewezen, wordt het item aan u toegewezen en wordt het item in uw tijdspagina weergegeven.

* Taken, problemen of projecten die u handmatig toevoegt.
* Taken, kwesties, of projecten waarvoor u reeds tijd elders in Workfront registreerde.
* Algemene tijd (vakantie, opleiding, overheadtijd).

>[!NOTE]
>
>Gebruikers die een tijdlijnprofiel hebben toegewezen, kunnen het gedeelte Timesheets zien en de algemene uren van het logbestand. Nochtans, kunnen zij geen uren op om het even welke taken of kwesties registreren die aan hen worden toegewezen die op timesheet verschijnen.

Aan logboektijd op een timesheet:

{{step1-click-main-menu}}

1. Klik [!UICONTROL **Tijdopnemers**]. Uw huidige timesheet wordt standaard weergegeven.
   ![&#x200B; Timesheet &#x200B;](assets/timesheet-redesigned-nwe.png)


1. (Optioneel) Klik op het **pictogram** volledig scherm ![](assets/full-screen.png) om de tijdspagina in de modus Volledig scherm weer te geven en klik vervolgens op het pictogram **exit-full-screen** ![](assets/exit-full-screen.png) om terug te keren naar de tijdspagina.

   <!-- drafted for the resize columns in timesheet story: 1. (optional) Click on the separator lines between weeks or between the time frame area and the work item area to resize the columns of the timesheet.-->

1. (Facultatief) om een project, een taak, of een kwestie aan timesheet toe te voegen, klik **punt** drop-down menu in de upper-left hoek van timesheet, dan klik **voegt Projecten** toe, **voegt Taken** toe, of **voegt Kwesties** toe.

   Er wordt een lijst met projecten, taken of problemen weergegeven.

   <!--drafted for full screen mode for add projects story - align it with the rest of the steps when you enable this:: 1. (Optional) Click the **full-screen** icon ![](assets/full-screen.png) to display the list of objects in full-screen mode.-->

1. (Facultatief) klik het onderzoekspictogram ![&#x200B; Onderzoek naar een punt &#x200B;](assets/search-icon.png) om naar een specifiek punt te zoeken gebruikend een sleutelwoord om aan timesheet toe te voegen.

1. (Optioneel) Vouw de vervolgkeuzemenu&#39;s voor het filter, de weergave of de groepering uit om er een toe te passen of aan te passen en om de gewenste iteminformatie weer te geven.

1. Selecteer één of verscheidene punten in de lijst, dan klik **toevoegen**.

   Als u minder dan 50 punten in één keer hebt toegevoegd, worden de punten toegevoegd aan timesheet. De taken en de kwesties zijn vermeld onder de naam van het project.

   >[!NOTE]
   >
   >Wanneer u taken of kwesties aan timesheet toevoegt, wordt het project ook toegevoegd.


1. (Voorwaardelijk) als u 50 of meer punten in één keer toevoegt, een bevestigingsbericht die het aantal punten toont die aan uw timesheet worden toegevoegd.

   Klik **toevoegen allen** om alle punten toe te voegen
of
Klik **annuleren** om het toevoegen van de geselecteerde punten tegen te houden, dan **annuleert** om de lijst van punten te sluiten.

   De taken en de kwesties zijn vermeld onder de naam van het project.

   >[!NOTE]
   >
   >De punten die u manueel aan timesheet toevoegt worden vastgezet en zullen op huidige en toekomstige chronologie blijven tot u hen manueel losmaakt om hen te verwijderen. Voor informatie over het ongedaan maken van punten om hen uit timesheet te verwijderen, ga met Stap 10 verder.

   <!--(ensure this stays accurate)-->

1. (Optioneel) Klik op de pictogrammen **Samenvouwen** of ![](assets/collapse-icon.png) Uitvouwen **&#x200B;**&#x200B;naast de projectnaam om de lijst met taken en problemen voor het project weer te geven of te verbergen.![](assets/expand-icon.png)


   >[!TIP]
   >
   >   Wanneer het gebruiken van een standaardQWERTY toetsenbord, en na het klikken van de naam van een project in timesheet, druk de volgende reeks sleutels om het project samen te vouwen of uit te breiden:
   >   * Het project uitbreiden en zijn het werkpunten tonen:
   >     * Shift + Alt + pijl-omhoog voor Windows-computers
   >     * Shift + Option + pijl-omhoog voor Mac-computers
   >   * Het project samenvouwen en de bijbehorende werkitems verbergen:
   >     * Shift + Alt + pijl-omlaag voor Windows-computers
   >     * Shift + Option + pijl-omlaag voor Mac-computers.


1. (Facultatief) om een punt manueel te spelden dat op timesheet automatisch toont, over de naam van het punt, dan klik het **speld** pictogram ![](assets/empty-pin-icon.png).

   >[!TIP]
   >
   >   Wanneer u een standaard QWERTY-toetsenbord gebruikt nadat u op een item in de tijdpagina hebt geklikt, drukt u op de volgende toetsen om een item vast te zetten:
   >   * Option + P voor zowel Windows- als Mac-computers.


1. (Optioneel) Klik op het zoekpictogram ![](assets/search-icon.png) en typ een trefwoord om een project, taak of probleem op de tijdpagina te zoeken.

1. (Voorwaardelijk) als uw Workfront of groepsbeheerder **heeft toegelaten wijs baanrollen aan uuringangen manueel toe** plaatsen, selecteer een baanrol van het drop-down menu. De rol die wordt gespecificeerd wanneer u aan de het werkpuntvertoningen door gebrek wordt toegewezen. Als u geen rol op het voorwerp wordt toegewezen, toont uw Primaire Rol als gebrek. Voor meer informatie over dit plaatsen, zie het artikel [&#x200B; timesheet en uurvoorkeur &#x200B;](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) vormen.

   ![&#x200B; tijd van het Logboek voor veelvoudige rollen in timesheet &#x200B;](assets/job-role-plus-sign-and-boxes-in-redesigned-timesheet.png)


1. (Optioneel) Klik op het pictogram **+** om nog een rij toe te voegen en selecteer vervolgens een nieuw uurtype in het vervolgkeuzemenu in de kolom [!UICONTROL Hour Type] om de tijd voor een ander uurtype vast te leggen.

   ![&#x200B; het type drop-down menu van het Uur &#x200B;](assets/hour-type-drop-down-expanded-redesigned-timesheet.png)


   >[!TIP]
   >
   >   Afhankelijk van uw besturingssysteem of browser en wanneer u een standaard QWERTY-toetsenbord gebruikt, drukt u op de volgende toetsen om nog een rij toe te voegen:
   >   * Ctrl + Option + voor Windows-computers
   >   * Cmd + Option + + voor Mac-computers

   De types van uren zijn beschikbaar afhankelijk van wat bij het systeem, het project, en gebruikersniveaus is bepaald, zoals die in [&#x200B; worden beschreven bepaalt uurtypes en beschikbaarheid &#x200B;](define-hour-types-and-availability.md).

   Het uurtype kan niet worden veranderd nadat een timesheet wordt gesloten.

   >[!TIP]
   >
   >Als u eerder registreerde tijd en het geselecteerde uurtype nu wordt gedeactiveerd, wordt de volledige rij voor de geregistreerde tijd gedimd. Als u een ander uurtype selecteert en de pagina vernieuwt, wordt de optie voor het gedeactiveerde uurtype verwijderd uit de vervolgkeuzelijst, zodat u geen extra uren aan dat uurtype kunt toevoegen.
   >
   >Denk na toevoegend een nieuwe lijn voor het het werkpunt u extra tijd voor en het selecteren van een nieuw uurtype wilt registreren, als u het gedeactiveerde uurtype verbonden aan de afgelopen geregistreerde tijd wilt houden.

1. Klik het **schrapping** pictogram ![](assets/delete.png) naast de baanrol om het te verwijderen. De tijd die voor de rol wordt geregistreerd, wordt ook verwijderd.

   >[!TIP]
   >
   >   Afhankelijk van uw besturingssysteem of browser en wanneer u een standaard QWERTY-toetsenbord gebruikt, drukt u op de volgende toetsen om een rij te verwijderen:
   >   * Ctrl + Option + - voor Windows-computers
   >   * Cmd + Option + - voor Mac-computers

1. Geef op hoeveel tijd u zich op een bepaalde dag in het tijdlijngedeelte van het tijdlijnvak wilt aanmelden en klik vervolgens buiten het uurvak om het uuritem op te slaan. De uren worden automatisch opgeslagen. De rij waarvoor u logboektijd wordt benadrukt in lichtblauw en de doos van de ureningang wordt geschetst in donkerblauw.

   ![&#x200B; de tijdvakje van het Logboek in timesheet &#x200B;](assets/log-time-with-blue-hightlight-redesigned-timesheet.png)

   U meldt de tijd in uren of dagen. Dit het plaatsen wordt gevormd door gebruikers met een vergunning van het Plan of de systeembeheerder, zoals die in [&#x200B; wordt beschreven vormt of de tijd uren of dagen &#x200B;](../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md) het programma wordt geopend.

   >[!IMPORTANT]
   >
   >U moet timesheet manueel bewaren als om het even welke volgende scenario&#39;s voorkomen:
   >
   >* De baanrol verbonden aan tijd die u eerder het programma opende is veranderd en **wijst baanrollen aan uuringangen toe manueel** het plaatsen is onbruikbaar gemaakt. De tijd van het registreren voor nieuwe data zal het met een verschillende baanrol associëren.
   >   
   >   Als de rol is veranderd en **baanrollen aan uuringangen manueel toewijzen** het plaatsen wordt toegelaten, kunt u tijd registreren of de rol bijwerken en uw veranderingen worden automatisch bewaard.
   >
   >* De taakrol die aan een taak of kwestie wordt toegewezen is verschillend dan de baanrol de timesheet eigenaar registreert tijd met <!--or assigned to them_ this last  piece came from a Support note but but sure what role it's referring to. Leaving it out for now.-->.
   >
   >De tijdpagina bespaart de tijd automatisch opnieuw wanneer er geen conflicterende ingangen meer tussen de twee rollen zijn.
   >

1. (Optioneel) Geef de hoeveelheid overwerk op in het veld Overwerk in de koptekst van het tijdblad.

   >[!TIP]
   >
   >U kunt geen groter aantal overuren dan de huidige totale uren op timesheet registreren. Bijvoorbeeld, als u 7 uren op timesheet tot dusver het programma opende, kunt u 8 uren van overwerk niet registreren.

1. (Facultatief) klik **Commentaar** om een commentaar voor uw uuringang toe te voegen.

   ![](assets/commment-button-on-hour-log-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Als u een standaard QWERTY-toetsenbord gebruikt nadat u op het invoervak voor uren hebt geklikt, drukt u op de volgende toetsen om het opmerkingsvak te openen:
   >   * Shift + F2 voor zowel Windows- als Mac-computers.

1. Klik **Gedaan** om de commentaar te bewaren.

   >[!TIP]
   >
   >   Als u een standaard QWERTY-toetsenbord gebruikt, drukt u vanuit het vak Opmerking op de volgende toetsen om de opmerking op te slaan:
   >   * Ctrl + Enter voor Windows-computers.
   >   * Cmd + Return voor Mac-computers.


1. (Facultatief) klik **tonen commentaren** in de toolbar om de ingangen van uren onder het het werkpunt te tonen.

   ![&#x200B; Commentaren die onder punt in timesheet worden vermeld &#x200B;](assets/comments-expanded-under-tasks-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Alle wijzigingen die u aanbrengt in de tijdpagina, worden automatisch opgeslagen.

1. (Facultatief) klik de rij van een taak of een kwestie, dan klik **Open Samenvatting** in de hoger-juiste hoek van timesheet om een update toe te voegen of informatie op de taak of de kwestie bij te werken. Het deelvenster Samenvatting wordt aan de rechterkant geopend.

   ![&#x200B; samenvatting-paneel-voor-taak-geopend-in-timesheet &#x200B;](assets/summary-panel-for-task-opened-in-timesheet-redesigned-timesheet.png)

   Uw update wordt weergegeven in het gedeelte Updates van het werkitem dat is gekoppeld aan de geregistreerde tijd.

   >[!TIP]
   >
   >U kunt geen opmerkingen maken over projecten of de items voor algemene tijd.

1. Klik [!UICONTROL **dicht Samenvatting**] om het Summiere paneel te sluiten en op timesheet terug te keren.

1. (Facultatief) klik [!UICONTROL **Updates**] in het linkerpaneel, dan voeg een update aan timesheet toe. Voor meer informatie over de updates van Workfront, zie [&#x200B; het werk van de Update &#x200B;](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   ![&#x200B; enter-an-update-in-opnieuw ontworpen-timesheet-verlaten-paneel &#x200B;](assets/enter-an-update-in-redesigned-timesheet-left-panel.png)

1. (Facultatief) terugkeer aan het **gebied van de Tijdopnemer** om uw timesheet te sluiten of voor te leggen.

   * **dicht**: Sluit timesheet wanneer u het bijwerken doet. Deze optie is alleen beschikbaar wanneer uw tijdspagina niet aan een fiatteur is gekoppeld.

   * **voorleggen voor goedkeuring:** Deze optie is beschikbaar slechts als er een fiatteur op timesheet is. Sla uw wijzigingen op en verzend deze ter goedkeuring. U kunt timesheet openen na het sluiten van het door **Herinneren** te klikken, als een goedkeuring nog niet is verleend. Voor meer informatie, zie [&#x200B; een timesheet voor goedkeuring &#x200B;](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md) voorleggen.

   * **Weigeren**: Deze optiesvertoningen wanneer u een timesheet fiatteur bent en timesheet is voorgelegd aan u voor goedkeuring. Als u erop klikt, wordt de status van de tijdlijn gewijzigd in Geweigerd en blijft de tijdlijn geopend.

   * **keur** goed: Deze optiesvertoningen wanneer u een timesheet fiatteur bent en timesheet is voorgelegd aan u voor goedkeuring. Als u erop klikt, wordt de status van de tijdlijn gewijzigd in Goedgekeurd en wordt de tijdlijn gesloten.

   >[!TIP]
   >
   >De opties Afwijzen en Goedkeuren worden ook op uw tijdspagina weergegeven wanneer u een systeembeheerder bent en het tijdsplaat is gekoppeld aan een fiatteur.

1. (Voorwaardelijk) Als u of gesloten of uw timesheet voor goedkeuring hebt voorgelegd, klik één van de volgende opties:

   * **heropenen**: Deze optie is beschikbaar voor timesheets die u reeds hebt gesloten en die geen fiatteurs, of timesheets hebben die reeds zijn goedgekeurd. Open de tijdpagina opnieuw om de uren te wijzigen.
   * **Herinnering**: Deze optie is beschikbaar voor timesheets die voor goedkeuring zijn voorgelegd maar nog niet goedgekeurd of verworpen. Klik **Herinneren** om timesheet opnieuw te openen en uuringangen te wijzigen.

#### Een item verwijderen uit de tijdpagina

U kunt een uuringang of een punt (project, taak, of kwestie) uit een timesheet verwijderen.

Een uuringang uit een timesheet verwijderen:

1. Ga naar het timesheet en vind de uuringang u wilt verwijderen.
1. De ingevoerde uren vervangen door 0
of
Verwijder de uren en vervang hen met 0, dan druk binnengaan.

   De uren worden verwijderd en de tijdpagina wordt automatisch opgeslagen.

U kunt een punt (project, taak, of kwestie) uit timesheet verwijderen door het los te maken, als u nog niet tijd voor het hebt geregistreerd, en als u manueel het punt (zoals die in Stappen 4-8 in de [&#x200B; tijd van het Logboek op een timesheet &#x200B;](#log-time-on-a-timesheet) sectie in dit artikel wordt beschreven) toevoegde. <!--ensure this stays accurate-->

U kunt geen punten verwijderen die in timesheet automatisch volgens de timesheet voorkeur in uw systeem of groep van Workfront inbegrepen zijn die worden gevormd om timesheets (zoals die in [&#x200B; worden beschreven vormen timesheet en uurvoorkeur &#x200B;](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)) te bevolken. De punten houden pre-bevolkend timesheet op wanneer de data van de punten buiten het tijdkader van timesheet zijn.

Om een punt uit timesheet te verwijderen dat manueel werd toegevoegd:

1. Zorg ervoor dat geen tijd tegen het punt wordt geregistreerd.
1. Klik **unpin** pictogram ![&#x200B; Vastzetten een punt &#x200B;](assets/pin-icon.png) naast het punt om het punt van timesheet los te maken.

   >[!TIP]
   >
   >   Wanneer u een standaard QWERTY-toetsenbord gebruikt nadat u op een item in de tijdpagina hebt geklikt, drukt u op de volgende toetsen om het vastzetten van een item ongedaan te maken:
   > * Option + P voor zowel Windows- als Mac-computers.

   Het item wordt verwijderd uit de tijdpagina nadat u de pagina hebt vernieuwd.

### Startpagina {#home}

U kunt project-specifieke tijd in Huis registreren.

Voor algemene informatie over het gebruiken van het gebied van het Huis, zie [&#x200B; Gebruik het gebied van het Huis &#x200B;](../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

<!--#### Log time on a work item from the new Home area-->

U kunt de tijd aan taken en kwesties in om het even welke widgets registreren gebruikend het Summiere paneel in het gebied van het Huis. Voor informatie, zie de [&#x200B; Summiere paneel &#x200B;](#summary-panel) sectie in dit artikel.

Daarnaast kunt u als volgt de tijd vastleggen voor een item in de widget Mijn werk:

1. Ga naar het **Begin** gebied.
1. Voeg **Mijn werk** widget aan uw Huis toe.
1. (Facultatief) selecteer een taak, kwestie, of verzoek in een lijst, dan klik **Werk op het**.
1. Beweeg over de taak of de kwestie u tijd voor wilt registreren, dan het **pictogram** van de Tijd van het Logboek ![](assets/log-time-icon-in-new-home.png) &lbrace;aan het recht van de taakinformatie klikken.

   De **vakvertoningen van de tijd van het 0&rbrace; Logboek.**

   ![&#x200B; de tijdvakje van het Logboek voor een taak in Huis &#x200B;](assets/log-time-ui-for-task-from-new-home.png)

1. Geef de volgende informatie op:

   * **Type van Uur**: Selecteer een Type van Uur van het drop-down menu, als het van getoond door gebrek verschillend is.

     Afhankelijk van welke uurtypes in uw systeem worden gevormd, zouden de opties hier kunnen variëren. Voor meer informatie over het vormen van uurtypes, zie [&#x200B; de types en beschikbaarheid van uren bepalen &#x200B;](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **Rol van de Baan**: (Voorwaardelijk) als uw Workfront of groepsbeheerder **heeft toegelaten wijst baanrollen aan uuringangen manueel** plaatsen toe, selecteer a **Rol van de Baan** van het drop-down menu. De rol die wordt opgegeven wanneer u aan het object bent toegewezen, wordt standaard weergegeven. Als u geen Rol op het voorwerp wordt toegewezen, toont uw Primaire Rol als gebrek. Voor meer informatie over dit plaatsen, zie het artikel [&#x200B; timesheet en uurvoorkeur &#x200B;](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) vormen.

   * Voer in de wekelijkse kalender het aantal uren in voor het project, de taak of de uitgave.

1. Klik **tijd van het Logboek**.

   De geregistreerde tijdvertoningen in de sectie van de Uren van de objecten, en in uw timesheet.

   Het **Totale Uren** gebied in de de tijddoos van het Logboek toont alle uren die voor het project, de taak, of de kwestie door alle gebruikers worden geregistreerd.

<!--#### Log time on a work item from the legacy Home area

1. In the **Work List** area, select the item where you want to log time.
1. In the right panel, click **Log Time**.  
  
   ![](assets/log-time-home-350x181.png)  

1. In the **Enter Hours** drop-down menu, select the appropriate hour type.  
   Hour types are available depending on what has been defined at the system, project, and user levels, as described in [Define hour types and availability](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
1. (Conditional) If your Workfront or group administrator has enabled the **Assign job roles to hour entries manually** setting, select a job role from the drop-down menu. The role specified when you are assigned to the work item displays by default. If you are not assigned a role on the object, your Primary Role displays as the default. For more information on this setting, see the article [Configure timesheet and hour preferences](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
1. Specify the time you want to log, then click **Log Time**.

   The logged time displays in the object's Hours section, nad in your timesheet. -->

### Project, taak of uitgave {#project-task-or-issue}

U kunt projectspecifieke tijd op een project, een taak, of een kwestie in de volgende secties registreren:

* [&#x200B; sectie van Updates &#x200B;](#updates-section)
* [Uren, sectie](#hours-section)

#### Sectie Updates{#updates-section}

Om tijd in de sectie van Updates van een project, een taak, of een kwestie te registreren, moet u het volgende hebben:

* De correcte toegang en de toestemmingen, zoals die in de [&#x200B; sectie van de Vereisten van de Toegang &#x200B;](#access-requirements) in dit artikel worden beschreven. Als uw toegangsniveau Licht is, en u registreert tijd op een project, moet u ook Contribute of hogere toestemmingen aan het project met toegang tot de Uren van het Logboek hebben. Voor meer informatie over het verlenen van toestemmingen op projecten, zie [&#x200B; een project &#x200B;](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-project.md) delen.

* Uw beheerder van Workfront moet de tijd van het Logboek op projecten direct toelaten die onder [!UICONTROL **plaatsen Tijdschema &amp; Uren**]> [!UICONTROL **Voorkeur**] in het gebied van het Systeem, als u tijd aan een project direct wilt registreren.

  Voor meer informatie over het toestaan van gebruikers om uren aan projecten direct te registreren, zie [&#x200B; timesheet en uurvoorkeur &#x200B;](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) vormen.

Om tijd in de sectie van Updates van een project, een taak, of een kwestie te registreren:

1. Ga naar een project, taak of probleem.
1. In het linkerpaneel, uitgezochte **Updates**.
1. Klik **Tijd van het Logboek**. <!-- did Anna B change the casing for this button? If yes and if she changed it for the other areas, update screen shot too-->

   Het dialoogvenster Logtijd wordt weergegeven.

   >[!TIP]
   >
   >   Als de voorkeur van uw profiel aan logboektijd in dagen wordt geplaatst, de Enter doos van Dagen toont.
   >   
   >   Rechtsboven in het vak Dagen invoeren ziet u hoeveel uren er in een dag staan.

   ![&#x200B; de tijdvakje van het Logboek voor een taak op het gebied van Updates &#x200B;](assets/log-time-box-in-updates-stream.png)

1. Geef de volgende informatie op:

   * **Type van Uur**: Selecteer een Type van Uur van het drop-down menu, als het van getoond door gebrek verschillend is.

     Afhankelijk van welke uurtypes in uw systeem worden gevormd, zouden de opties hier kunnen variëren. Voor meer informatie over het vormen van uurtypes, zie [&#x200B; de types en beschikbaarheid van uren bepalen &#x200B;](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **Rol van de Baan**: (Voorwaardelijk) als uw Workfront of groepsbeheerder **heeft toegelaten wijst baanrollen aan uuringangen manueel** plaatsen toe, selecteer a **Rol van de Baan** van het drop-down menu. De rol die wordt opgegeven wanneer u aan het object bent toegewezen, wordt standaard weergegeven. Als u geen Rol op het voorwerp wordt toegewezen, toont uw Primaire Rol als gebrek. Voor meer informatie over dit plaatsen, zie het artikel [&#x200B; timesheet en uurvoorkeur &#x200B;](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) vormen.

   * Voer in de wekelijkse kalender het aantal uren in voor het project, de taak of de uitgave.

1. Klik **tijd van het Logboek**.

   De geregistreerde tijdvertoningen in de sectie van de Uren van de objecten, en in uw timesheet.

   Het **Totale Uren** gebied in de de tijddoos van het Logboek toont alle uren die voor het project, de taak, of de kwestie door alle gebruikers worden geregistreerd.

#### Uren, sectie{#hours-section}

U moet een beheerder van Workfront zijn om tijd voor projecten, taken, en kwesties in de sectie van Uren te registreren.

of

U moet alle volgende opties hebben:

* Een standaard- of planvergunning met administratieve toegang tot Tijdopnamen &amp; uren, of een Lichte vergunning met Edit toegang tot Projecten. Voor meer informatie over het verlenen van administratieve toegang tot Chronologie &amp; uren, zie [&#x200B; gebruikers administratieve toegang van de Verlening tot bepaalde gebieden &#x200B;](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md). Administratieve toegang tot timesheets en uren is niet beschikbaar voor lichte licenties.
* Draag of hogere toestemmingen aan het project met toegang tot de Uren van het Logboek bij. Voor meer informatie over het verlenen van toestemmingen op projecten, zie [&#x200B; een project in Adobe Workfront &#x200B;](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md) delen.
* Uw beheerder van Workfront moet de tijd van het Logboek direct op projecten toelaten die in de **Chronologie &amp; Uren > sectie van de Voorkeur** van het gebied van de Opstelling plaatsen, als u tijd aan een project direct wilt registreren. Voor meer informatie over het toestaan van gebruikers om uren aan projecten direct te registreren, zie [&#x200B; timesheet en uurvoorkeur &#x200B;](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) vormen.

Om tijd in de sectie van Uren van een project, een taak, of een kwestie te registreren:

1. Ga naar een project, taak of probleem.
1. In het linkerpaneel, klik **Uren**.
1. Klik **Tijd van het Logboek**.

   De **vakvertoningen van de tijd van het 0&rbrace; Logboek.**

   ![&#x200B; tijd van het Logboek in de sectie van Uren van een taak &#x200B;](assets/log-time-box-in-hours-section-on-task.png)

1. Geef de volgende informatie op:

   * **Eigenaar:** Uw naamvertoningen op dit gebied, door gebrek.\
     Als u de uren voor een andere gebruiker registreert, specificeer hun naam.

   * **Type van Uur**: Selecteer een Type van Uur van het drop-down menu, als het van getoond door gebrek verschillend is.

     Afhankelijk van welke uurtypes in uw systeem worden gevormd, zouden de opties hier kunnen variëren.

     Voor meer informatie over het vormen van uurtypes, zie [&#x200B; de types en beschikbaarheid van uren bepalen &#x200B;](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **Rol van de Baan**: (Voorwaardelijk) als uw Workfront of groepsbeheerder **heeft toegelaten wijst baanrollen aan uuringangen manueel** plaatsen toe, selecteer a **Rol van de Baan** van het drop-down menu. De rol die wordt opgegeven wanneer u aan het object bent toegewezen, wordt standaard weergegeven. Als u geen Rol op het voorwerp wordt toegewezen, toont uw Primaire Rol als gebrek. Voor meer informatie over dit plaatsen, zie het artikel [&#x200B; timesheet en uurvoorkeur &#x200B;](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) vormen.
   * **de wekelijkse kalender**: Ga het aantal uren voor het project, de taak, of de kwestie in.
   * **Nota**: Voeg een nota toe om te verklaren waar de uren voor zijn. Dit wordt bewaard als **Nota van het Uur** of een **Beschrijving van het Uur**.

1. Klik **tijd van het Logboek**.

   De geregistreerde tijdvertoningen in de sectie van de Uren van de objecten, en in uw timesheet.

   Het **Totale Uren** gebied in de de tijddoos van het Logboek toont alle uren die voor het project, de taak, of de kwestie door alle gebruikers worden geregistreerd.

### Het deelvenster Samenvatting

U kunt tijd voor taken en kwesties in het Summiere paneel registreren.
Voor meer informatie, zie [&#x200B; Overzicht van de Samenvatting &#x200B;](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

![](assets/summary-hour-log.png)

### Borden {#boards}

U kunt zich aanmelden op verbonden kaarten op een Workfront-board. Dit is hetzelfde proces als het aanmelden bij een taak of uitgave en de uren die op de kaart zijn aangemeld, worden opgeslagen op de aangesloten taak of uitgave.
Voor meer informatie, zie [&#x200B; Gebruik verbonden kaarten op raad &#x200B;](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

### Mobiele app {#mobile-app}

U kunt de tijd vastleggen via de mobiele app van Workfront.
Voor meer informatie, zie [&#x200B; Adobe Workfront voor Android &#x200B;](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md) of [&#x200B; Adobe Workfront voor iOS &#x200B;](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md).

## Aangemeld uren bewerken in lijsten en rapporten

>[!CAUTION]
>
>* U kunt geen uuringangen wijzigen die tot een gesloten timesheet behoren. U moet eerst timesheet opnieuw openen, en dan de informatie van de uuringang veranderen.
>* Wanneer u het Type van Uur van een type verandert dat niet als opbrengst aan een ander type telt dat als opbrengst telt, komen de veranderingen in de financiën van het project ook voor. Door het wijzigen van het type Uur van een type dat als inkomsten in een type telt dat niet als inkomsten telt, worden de financiën van het project ook bijgewerkt.
>
>Voor informatie, zie [&#x200B; de types van uren &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md) leiden.
>

U kunt de aangemelde uren bewerken in de volgende gebieden:

* Alle gebieden waar u de uren hebt toegevoegd, inclusief open tijdbladen
* Uur lijsten en rapporten.

U kunt de volgende elementen van een uuringang uitgeven wanneer u een uuringang in een lijst of een rapport uitgeeft:

* Aantal uren
* Uurtype
* De rol van de baan verbonden aan de ureningang
* Beschrijving van het uur-item

Afhankelijk van het type uren dat u bewerkt, zijn de volgende velden beschikbaar voor bewerking in een uurlijst of een uurrapport:

* Wanneer u projectspecifieke uren uitgeeft:

   * Het aantal uren
   * Het uurtype. U kunt het Type van Uur slechts in project-specifieke types veranderen.
   * Taak toewijzen. U kunt de taak van de Rol van de Taak slechts veranderen als het in Opstelling werd toegelaten. Voor informatie, zie [&#x200B; timesheet en uurvoorkeur &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) vormen
   * The Description of the hour entry.


  ![](assets/edit-hour-box-project-hour-type.png)

* Wanneer u algemene uren bewerkt:

   * Het aantal uren.
   * Het uurtype. U kunt het Type van Uur slechts in algemene types veranderen.
   * The Description of the hour entry.

>[!TIP]
>
> U kunt de roltoewijzing van de Rol van het uur niet veranderen, omdat de algemene uren niet met rollen kunnen worden geassocieerd.

<!--update the screen shot at production - we should not see the job role field for general hours-->

![](assets/edit-hour-box-general-overhead-hour-type.png)


* Wanneer u een mengeling van algemene en projectspecifieke uren uitgeeft, in bulk:

   * Het aantal uren.
   * The Description of the hour entry.

>[!TIP]
>
>* U kunt het Type van Uur niet veranderen, omdat de types van algemene uren niet in project-specifieke types kunnen worden veranderd en de project-specifieke uurtypes kunnen niet in algemene types worden veranderd.
>* U kunt de taakroltoewijzing niet wijzigen, omdat algemene uren niet aan rollen kunnen worden gekoppeld.


<!--update the screen shot at production - we should not see the job role and the hour type fields for mixed hour types-->

![](assets/edit-hour-box-mixed-hour-types-in-bulk.png)

Om uurtypes in een uurrapport of een lijst uit te geven:

1. Ga naar een uurlijst of rapport.
1. Klik op het vakje links van een of meerdere uurvermeldingen om deze te selecteren.
1. Klik het **uitgeven pictogram** ![](assets/edit-icon.png) bij de bovenkant van de lijst.

   Het **geeft** uur &lbrace;of **geeft de doos van Uren** uit opent.
1. Werk een van de volgende beschikbare velden bij:

   * Uren. Dit is een verplicht veld.
   * Type uur. Dit is een verplicht veld.
   * Functie
   * Beschrijving

   >[!TIP]
   >
   >   Niet alle velden zijn beschikbaar, afhankelijk van het uurtype dat aan de geselecteerde uurwaarden is gekoppeld.

1. Klik **sparen veranderingen**.

   De informatie over het uur wordt bijgewerkt.
Als u meer dan één uur hebt geselecteerd en het veld Uren hebt gewijzigd, wordt dezelfde hoeveelheid uren toegewezen aan alle geselecteerde uren. De oorspronkelijke uren worden vervangen door de nieuwe waarde voor alle geselecteerde uren.


