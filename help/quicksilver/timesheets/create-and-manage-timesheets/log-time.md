---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Logtijd
description: U kunt tijd voor het werkpunten in&nbsp registreren;Adobe Workfront om op het aantal uren te wijzen u het werken aan hen doorwerkt. U kunt tijd ook registreren die niet met het werk, zoals vakantie, zieke tijd, of tijd u in vergaderingen doorbrengt. De tijd u registreert toont in uw timesheet.
author: Alina
feature: Timesheets
exl-id: 120173a8-95f1-4233-ab40-d3bcfe38c977
source-git-commit: f87f71be1b5f60b95859f3632bae4cf392cc5e84
workflow-type: tm+mt
source-wordcount: '2971'
ht-degree: 0%

---

# Logtijd

U kunt de tijd voor het werk in Adobe Workfront registreren om op het aantal uren te wijzen u het werken aan hen doorwerkt. U kunt tijd ook registreren die niet met het werk, zoals vakantie, zieke tijd, of tijd u in vergaderingen doorbrengt. De tijd u registreert toont in uw timesheet.

Voor meer informatie over het type uren dat u kunt aanmelden in Workfront, raadpleegt u [Uurtypen beheren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Toegangsvereisten

<!--drafted for P&P - replace the table:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Light or higher</p>
   <p>Legacy license: Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to the type of work item you log time for </p> <p>For example, you need Edit access to Issues, to log time for issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions on the work item you log time for that includes permissions to Log Hours</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren en de Specifieke uren van het Project te registreren:

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
   <td> <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Geef toegang tot het type van het werkpunt uit u tijd voor registreert </p> <p>U hebt bijvoorbeeld toegang tot problemen bewerken nodig om u aan te melden bij problemen</p> <p>Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Draag of hogere toestemmingen op het het werkpunt bij u tijd voor dat omvat toestemmingen aan Loguren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Overwegingen bij het aanmelden in Workfront

* U kunt tijd voor projecten, taken, of kwesties registreren, of u kunt tijd in uw timesheet direct registreren.

   Voor informatie over het creëren van timesheets, zie [Een timesheet voor eenmalig gebruik maken](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

* Alle tijd die door hulpmiddelen buiten timesheet wordt geregistreerd verschijnt in timesheet voor de overeenkomstige tijdspanne.
* Taken en problemen met een project dat niet actueel is, worden niet vooraf in een tijdspagina geplaatst.
* De tijd die in timesheet wordt geregistreerd wordt onmiddellijk toegepast op de taak, de kwestie, of het project.
* De tijdbladen bevatten de totale tijd voor alle geregistreerde datums. Weekends worden altijd opgenomen, zelfs als tijdlijnberekeningen zijn geconfigureerd om ze uit te sluiten (zoals beschreven in [Projectvoorkeuren voor het hele systeem configureren](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)).
* Het maximumaantal punten dat in een timesheet wordt getoond is 45. Als er meer dan 45 punten zijn de waarvan data het timesheet tijdkader aanpassen, slechts de onlangs bijgewerkte punten tonen.
* Uur-items die in factureringsrecords zijn opgenomen, worden grijs weergegeven en kunnen niet worden bewerkt in de tijdpagina. Zie voor meer informatie [Factureringsrecords maken](../../manage-work/projects/project-finances/create-billing-records.md).

## Logtijd

U kunt zich in Workfront aanmelden in de volgende gebieden:

* [Tijdschema](#timesheet)
* [Home](#home)
* [Project, taak of uitgave](#project-task-or-issue)
* [Het deelvenster Samenvatting](#summary-panel)
* [Borden](#boards)
* [Mobiele app](#mobile-app)

### Tijdschema {#timesheet}

U kunt algemene uren of project-specifieke uren op een timesheet registreren.

>[!NOTE]
>
>Gebruikers die een tijdlijnprofiel hebben toegewezen, kunnen het tabblad Timesheets en de algemene logtijden bekijken. Nochtans, kunnen zij geen uren op om het even welke taken of kwesties registreren die aan hen worden toegewezen die op timesheet verschijnen.

1. Klik op de knop [!UICONTROL **Hoofdmenu**] pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront.

1. Klikken [!UICONTROL **Timesheets**]. Uw huidige timesheet wordt standaard weergegeven.
   ![Tijdschema](assets/timesheet-redesigned-nwe.png)

   Het timesheet is vooraf bevolkt met punten die aan u tijdens het tijdkader van timesheet worden toegewezen. Voor informatie over hoe timesheets vooraf bevolkt zijn, zie [Voorkeuren voor tijdpagina&#39;s en uren configureren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md). Als u geen punt op timesheet ziet, kunt u het toevoegen.

   >[!NOTE]
   >
   >In het tijdlijnvenster worden alleen items ingevuld die aan u zijn toegewezen. Het vult niet met punten vooraf die aan uw teams of baanrollen worden toegewezen.
   >
   >Als u op het item klikt op het item dat aan uw teams is toegewezen, wordt het item aan u toegewezen en wordt het item in uw tijdspagina weergegeven.


1. (Optioneel) Klik op de knop **volledig scherm** pictogram ![](assets/full-screen.png) om timesheet op volledig-schermwijze te tonen, dan klik **afsluiten op volledig scherm** ![](assets/exit-full-screen.png) om terug te keren naar de tijdpagina.

   <!-- drafted for the resize columns in timesheet story: 1. (optional) Click on the separator lines between weeks or between the time frame area and the work item area to resize the columns of the timesheet.-->

1. (Optioneel) Als u een project, taak of uitgave wilt toevoegen aan de tijdpagina, klikt u op de knop **Item toevoegen** vervolgkeuzemenu in de linkerbovenhoek van de tijdpagina en klik vervolgens op **Projecten toevoegen**, **Taken toevoegen**, of **Problemen toevoegen**.

   Een lijst met projecten, taken of uitgaven wordt weergegeven.

   <!--drafted for full screen mode for add projects story - align it with the rest of the steps when you enable this:: 1. (Optional) Click the **full-screen** icon ![](assets/full-screen.png) to display the list of objects in full-screen mode.-->

1. (Optioneel) Klik op het zoekpictogram ![Zoeken naar een object](assets/search-icon.png) om naar een specifiek punt te zoeken gebruikend een sleutelwoord om aan timesheet toe te voegen.

1. (Optioneel) Vouw de vervolgkeuzemenu&#39;s voor het filter, de weergave of de groepering uit om er een toe te passen of aan te passen en om de gewenste iteminformatie weer te geven.

1. Selecteer een of meerdere items in de lijst en klik op **Toevoegen**.

   >[!NOTE]
   >
   >Wanneer u taken of kwesties aan timesheet toevoegt, wordt het project ook toegevoegd.


1. (Voorwaardelijk) als u 50 of meer punten in één keer toevoegt, een bevestigingsbericht die het aantal punten toont die aan uw timesheet worden toegevoegd.

   Klikken **Alles toevoegen** om alle items toe te voegen of klik op **Annuleren** om het toevoegen van de geselecteerde items te stoppen, **Annuleren** om de lijst met items te sluiten.

   De taken en de kwesties zijn vermeld onder de naam van het project.

   >[!NOTE]
   >
   >De punten die u manueel aan timesheet toevoegt worden vastgezet en zullen op huidige en toekomstige chronologie blijven tot u hen manueel losmaakt om hen te verwijderen. Voor informatie over het ongedaan maken van punten om hen uit timesheet te verwijderen, ga met Stap 10 verder.

   <!--(ensure this stays accurate)-->

1. (Optioneel) Klik op de knop **Samenvouwen** ![](assets/collapse-icon.png) of **Uitbreiden** ![](assets/expand-icon.png) pictogrammen naast de projectnaam om de lijst met taken en problemen voor het project weer te geven of te verbergen.


   >[!TIP]
   >
   >   Wanneer het gebruiken van een standaardQWERTY toetsenbord, en na het klikken van de naam van een project in timesheet, druk de volgende reeks sleutels om het project samen te vouwen of uit te breiden:
   >   * Het project uitbreiden en zijn het werkpunten tonen:
      >     * Shift + Alt + pijl-omhoog voor Windows-computers
      >     * Shift + Option + pijl-omhoog voor Mac-computers
   >   * Het project samenvouwen en de bijbehorende werkitems verbergen:
      >     * Shift + Alt + pijl-omlaag voor Windows-computers
      >     * Shift + Option + pijl-omlaag voor Mac-computers.



1. (Optioneel) Als u een item dat automatisch wordt weergegeven op het tijdblad handmatig wilt vastzetten, houdt u de muisaanwijzer boven de naam van het item en klikt u op de knop **speld** pictogram ![](assets/empty-pin-icon.png).

   >[!TIP]
   >
   >   Wanneer u een standaard QWERTY-toetsenbord gebruikt nadat u op een item in de tijdpagina hebt geklikt, drukt u op de volgende toetsen om een item vast te zetten:
   >   * Option + P voor zowel Windows- als Mac-computers.



1. (Optioneel) Klik op het zoekpictogram ![](assets/search-icon.png) en beginnen een sleutelwoord te typen om een project, een taak, of een kwestie op timesheet te vinden.

1. (Optioneel) U kunt een item (project, taak of uitgave) verwijderen uit de tijdlijn als u het item handmatig hebt toegevoegd (zoals beschreven in Stap 3-6) en als u nog geen tijd hebt aangemeld tegen het item door het uit te lijnen. <!--ensure this stays accurate-->

   U kunt geen punten verwijderen die in timesheet volgens timesheet voorkeur in uw systeem of groep van Workfront worden omvat die worden gevormd om de timesheets (zoals beschreven in [Voorkeuren voor tijdpagina&#39;s en uren configureren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   Om een punt uit timesheet te verwijderen dat manueel werd toegevoegd:

   1. Zorg ervoor dat geen tijd tegen het punt wordt geregistreerd.
   1. Klik op de knop **vrijmaken** pictogram ![Een item vastzetten](assets/pin-icon.png) naast het punt om het punt van timesheet los te maken.

   >[!TIP]
   >
   >   Wanneer u een standaard QWERTY-toetsenbord gebruikt nadat u op een item in de tijdpagina hebt geklikt, drukt u op de volgende toetsen om het vastzetten van een item ongedaan te maken:
   >   * Option + P voor zowel Windows- als Mac-computers.



   Het item wordt verwijderd uit de tijdpagina nadat u de pagina hebt vernieuwd.

1. (Voorwaardelijk) Als uw Workfront of groepsbeheerder de optie **Taken handmatig toewijzen aan uren** Selecteer een taakrol in het keuzemenu. De rol die wordt gespecificeerd wanneer u aan de het werkpuntvertoningen door gebrek wordt toegewezen. Als u geen rol op het voorwerp wordt toegewezen, toont uw Primaire Rol als gebrek. Raadpleeg het artikel voor meer informatie over deze instelling [Voorkeuren voor tijdpagina&#39;s en uren configureren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   ![De tijd van het logboek voor veelvoudige rollen in timesheet](assets/job-role-plus-sign-and-boxes-in-redesigned-timesheet.png)


1. (Optioneel) Klik op de knop **+** om nog een rij toe te voegen, selecteert u vervolgens een nieuw uurtype in het keuzemenu in het dialoogvenster [!UICONTROL Hour Type] kolom aan logboektijd voor een verschillend uurtype.

   ![Vervolgkeuzemenu voor type uur](assets/hour-type-drop-down-expanded-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Afhankelijk van uw besturingssysteem of browser en wanneer u een standaard QWERTY-toetsenbord gebruikt, drukt u op de volgende toetsen om nog een rij toe te voegen:
   >   * Ctrl + Option + voor Windows-computers
   >   * Cmd + Option + + voor Mac-computers


   De types van uren zijn beschikbaar afhankelijk van wat op het systeem, het project, en gebruikersniveaus, zoals die in wordt beschreven [Bepaal uurtypes en beschikbaarheid voor timesheets](define-hour-types-and-availability.md).

   Het uurtype kan niet worden veranderd nadat een timesheet wordt gesloten.

   >[!TIP]
   >
   >Als u eerder registreerde tijd en het geselecteerde uurtype nu wordt gedeactiveerd, wordt de volledige rij voor de geregistreerde tijd gedimd. Als u een ander uurtype selecteert en de pagina vernieuwt, wordt de optie voor het gedeactiveerde uurtype verwijderd uit de vervolgkeuzelijst, zodat u geen extra uren aan dat uurtype kunt toevoegen.
   >
   >Denk na toevoegend een nieuwe lijn voor het het werkpunt u extra tijd voor en het selecteren van een nieuw uurtype wilt registreren, als u het gedeactiveerde uurtype verbonden aan de afgelopen geregistreerde tijd wilt houden.

1. Klik op de knop **delete** pictogram  ![](assets/delete.png) naast de taakrol om deze te verwijderen. De tijd die voor de rol wordt geregistreerd, wordt ook verwijderd.

   >[!TIP]
   >
   >   Afhankelijk van uw besturingssysteem of browser en wanneer u een standaard QWERTY-toetsenbord gebruikt, drukt u op de volgende toetsen om een rij te verwijderen:
   >   * Ctrl + Option + - voor Windows-computers
   >   * Cmd + Option + - voor Mac-computers



1. Geef op hoeveel tijd u zich op een bepaalde dag in het tijdlijngedeelte van het tijdlijnvak wilt aanmelden en klik vervolgens buiten het uurvak om het uuritem op te slaan. De uren worden automatisch opgeslagen. De rij waarvoor u logboektijd wordt benadrukt in lichtblauw en de doos van de ureningang wordt geschetst in donkerblauw.

   ![Logtijdvak in tijdblad](assets/log-time-with-blue-hightlight-redesigned-timesheet.png)

   U meldt de tijd in uren of dagen. Dit plaatsen wordt gevormd door gebruikers met een vergunning van het Plan of de systeembeheerder, zoals die in wordt beschreven [Configureer of de tijd uren of dagen is aangemeld](../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

   >[!IMPORTANT]
   >
   >Als een baanrol waarvoor u tijd registreerde is veranderd en **Taken handmatig toewijzen aan uren** instelling is uitgeschakeld, moet u de tijdinvoer handmatig opslaan. De tijdpagina bespaart uw tijd automatisch opnieuw slechts wanneer er geen tijd meer voor de baanrol wordt geregistreerd die is veranderd.
   >
   >Als de rol is gewijzigd en de **Taken handmatig toewijzen aan uren** Als deze instelling is ingeschakeld, kunt u de tijd vastleggen of de rol bijwerken en worden uw wijzigingen automatisch opgeslagen.

1. (Optioneel) Geef de hoeveelheid overwerk op in het veld Overwerk in de koptekst van het tijdblad.

   >[!TIP]
   >
   >U kunt geen groter aantal overuren dan de huidige totale uren op timesheet registreren. Bijvoorbeeld, als u 7 uren op timesheet tot dusver het programma opende, kunt u 8 uren van overwerk niet registreren.

1. (Optioneel) Klik op **Opmerking** om een opmerking toe te voegen voor het invoeren van het uur.

   ![](assets/commment-button-on-hour-log-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Als u een standaard QWERTY-toetsenbord gebruikt nadat u op het invoervak voor uren hebt geklikt, drukt u op de volgende toetsen om het opmerkingsvak te openen:
   >   * Shift + F2 voor zowel Windows- als Mac-computers.


1. Klikken **Gereed** om de opmerking op te slaan.

   >[!TIP]
   >
   >   Als u een standaard QWERTY-toetsenbord gebruikt, drukt u vanuit het vak Opmerking op de volgende toetsen om de opmerking op te slaan:
   >   * Ctrl + Enter voor Windows-computers.
   >   * Cmd + Return voor Mac-computers.



1. (Optioneel) Klik op **Opmerkingen tonen** in de werkbalk om opmerkingen over het ingangspunt in uren weer te geven onder het werkitem.

   ![Opmerkingen vermeld onder item in timesheet](assets/comments-expanded-under-tasks-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Alle wijzigingen die u aanbrengt in de tijdpagina, worden automatisch opgeslagen.

1. (Optioneel) Klik op de rij van een taak of uitgave en klik vervolgens op **Samenvatting openen** in de rechterbovenhoek van het tijdspad om een update toe te voegen of om informatie over de taak of kwestie bij te werken. Het deelvenster Samenvatting wordt aan de rechterkant geopend.

   ![summary-panel-for-task-opened-in-timesheet](assets/summary-panel-for-task-opened-in-timesheet-redesigned-timesheet.png)

   Uw update wordt weergegeven in het gedeelte Updates van het werkitem dat is gekoppeld aan de geregistreerde tijd.

   >[!TIP]
   >
   >U kunt geen opmerkingen maken over projecten of de items voor algemene tijd.

1. Klikken [!UICONTROL **Samenvatting sluiten**] om het deelvenster Samenvatting te sluiten en terug te keren naar de tijdpagina.

1. (Optioneel) Klik op [!UICONTROL **Updates**] in het linkerpaneel, dan voeg een update aan timesheet toe. Ga voor meer informatie over Workfront-updates naar [Werk bijwerken](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   ![enter-an-update-in-redesign-time-left-panel](assets/enter-an-update-in-redesigned-timesheet-left-panel.png)

   * **Sluiten**: Sluit de tijdpagina wanneer u klaar bent met het bijwerken. Deze optie is alleen beschikbaar wanneer uw tijdspagina niet aan een fiatteur is gekoppeld.

   * **Ter goedkeuring indienen:** Deze optie is beschikbaar slechts als er een fiatteur op timesheet is. Sla uw wijzigingen op en verzend deze ter goedkeuring. U kunt de tijdpagina openen nadat u deze hebt gesloten door op **Herstellen**, indien nog geen goedkeuring is verleend. Zie voor meer informatie [Een tijdschema ter goedkeuring indienen](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

   * **Afwijzen**: Deze optie wordt weergegeven wanneer u een fiatteur van het tijdspad bent en het tijdblad ter goedkeuring aan u is voorgelegd. Als u erop klikt, wordt de status van de tijdlijn gewijzigd in Geweigerd en blijft de tijdlijn geopend.

   * **Goedkeuren**: Deze optie wordt weergegeven wanneer u een fiatteur van het tijdspad bent en het tijdblad ter goedkeuring aan u is voorgelegd. Als u erop klikt, wordt de status van de tijdlijn gewijzigd in Goedgekeurd en wordt de tijdlijn gesloten.
   >[!TIP]
   >
   >De opties Afwijzen en Goedkeuren worden ook op uw tijdspagina weergegeven wanneer u een systeembeheerder bent en het tijdsplaat is gekoppeld aan een fiatteur.

1. (Voorwaardelijk) Als u of gesloten of uw timesheet voor goedkeuring hebt voorgelegd, klik één van de volgende opties:

   * **Opnieuw openen**: Deze optie is beschikbaar voor timesheets die u reeds hebt gesloten en die geen fiatteurs, of timesheets hebben die reeds zijn goedgekeurd. Open de tijdpagina opnieuw om de uren te wijzigen.
   * **Herstellen**: Deze optie is beschikbaar voor timesheets die ter goedkeuring zijn ingediend maar nog niet zijn goedgekeurd of afgewezen. Klikken **Herstellen** om timesheet opnieuw te openen en uuringangen te wijzigen.

### Home {#home}

U kunt project-specifieke tijd in Huis registreren.

Voor algemene informatie over het gebruik van het gebied Home raadpleegt u [Het gebied Home gebruiken](../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

U kunt als volgt de tijd vastleggen op een tijdelijk onderdeel in het gebied Home:

1. In de **Werklijst** selecteert u het item waar u de tijd wilt vastleggen.
1. Klik in het rechterdeelvenster op **Logtijd**.

   ![](assets/log-time-home-350x181.png)

1. In de **Uren invoeren** selecteert u het gewenste uurtype.\
   De types van uren zijn beschikbaar afhankelijk van wat op het systeem, het project, en gebruikersniveaus, zoals die in wordt beschreven [Bepaal uurtypes en beschikbaarheid voor timesheets](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
1. (Voorwaardelijk) Als uw Workfront of groepsbeheerder de optie **Taken handmatig toewijzen aan uren** Selecteer een taakrol in het keuzemenu. De rol die wordt gespecificeerd wanneer u aan de het werkpuntvertoningen door gebrek wordt toegewezen. Als u geen rol op het voorwerp wordt toegewezen, toont uw Primaire Rol als gebrek. Raadpleeg het artikel voor meer informatie over deze instelling [Voorkeuren voor tijdpagina&#39;s en uren configureren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
1. Geef de tijd op die u wilt vastleggen en klik vervolgens op **Logtijd**.

### Project, taak of uitgave {#project-task-or-issue}

U kunt projectspecifieke tijd op een project, een taak, of een kwestie registreren.

#### Machtigingen vereist voor logtijd

Om uren op een project, een taak, of een kwestie te registreren, moet u specifieke toestemmingen hebben. U kunt tijd in twee plaatsen op een project, een taak, of een kwestie registreren:

* [Tabblad Updates](#updates-tab)
* [Tabblad Uren](#hours-tab)

##### Tabblad Updates{#updates-tab}

Het volgende wordt vereist alvorens u uren op het lusje van Updates van een project, een taak, of een kwestie kunt registreren:

* U moet een licentie voor werken of abonnementen hebben.
* U moet ten minste beschikken over Contribute-machtigingen voor het project, de taak of het probleem met toegang tot Log-uren.\
   Voor meer informatie over het verlenen van toestemmingen op projecten, zie [Een project delen in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* Als u tijd aan een project direct wilt registreren, moet uw beheerder van Workfront de tijd van het Logboek op projecten toelaten die onder plaatsen [!UICONTROL **Tijdschema en uren** ]> [!UICONTROL **Voorkeuren**].\
   Voor meer informatie over het toestaan van gebruikers om uren aan projecten direct te registreren, zie [Voorkeuren voor tijdpagina&#39;s en uren configureren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

##### Tabblad Uren{#hours-tab}

Het volgende wordt vereist alvorens u uren op het lusje van Uren van een project, een taak, of een kwestie kunt registreren:

* U moet de systeembeheerder zijn.

Of u moet het volgende hebben:

* U moet beschikken over een licentie voor abonnementen met beheerdersrechten voor timesheets en uren. Voor meer informatie over het verlenen van administratieve toegang tot Tijdopnamen &amp; uren, zie [Gebruikers administratieve toegang verlenen tot bepaalde gebieden](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).
* U moet ten minste beschikken over Contribute-machtigingen voor het project met toegang tot logarituren. Voor meer informatie over het verlenen van toestemmingen op projecten, zie [Een project delen in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
* Als u de tijd rechtstreeks aan een project wilt registreren, moet uw beheerder van Workfront de tijd van het Logboek bij projecten toelaten die onder de Tijdopname &amp; Uren > Voorkeur plaatsen. Voor meer informatie over het toestaan van gebruikers om uren aan projecten direct te registreren, zie [Voorkeuren voor tijdpagina&#39;s en uren configureren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Aan logboektijd op een project, een taak, of een kwestie:

1. Navigeer naar een project, taak of probleem.
1. Selecteer in het linkerdeelvenster de optie **Uren**.
1. Klikken **Logtijd**.

   Het dialoogvenster Logboekuren wordt weergegeven.

1. Geef de volgende informatie op:

   * **Eigenaar:** Standaard wordt uw naam in dit veld weergegeven.\
      Als u de uren voor een andere gebruiker registreert, specificeer hun naam.

   * **Uren**: Voer het aantal uren in voor het project, de taak of de uitgave.
   * **Uurtype**: Selecteer een Type van Uur van het drop-down menu, als het van getoond door gebrek verschillend is.

      Afhankelijk van welke uurtypes in uw systeem worden gevormd, zouden de opties hier kunnen variëren. Voor meer informatie over het vormen van uurtypes, zie [Bepaal uurtypes en beschikbaarheid voor timesheets](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **Functie**: (Voorwaardelijk) Als uw Workfront of groepsbeheerder de optie **Taken handmatig toewijzen aan uren** instellen, selecteert u een **Functie** in het keuzemenu. De rol die wordt opgegeven wanneer u aan het object bent toegewezen, wordt standaard weergegeven. Als u geen Rol op het voorwerp wordt toegewezen, toont uw Primaire Rol als gebrek. Raadpleeg het artikel voor meer informatie over deze instelling [Voorkeuren voor tijdpagina&#39;s en uren configureren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

      ![Screen_Shot_2017-05-03_at_10.16.52_AM.png](assets/screen-shot-2017-05-03-at-10.16.52-am-350x346.png)

1. Klikken **Logboekuren**.

### Het deelvenster Samenvatting

U kunt tijd voor taken en kwesties in het Summiere paneel registreren.
Zie voor meer informatie [Overzicht van samenvattingen](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

![](assets/summary-hour-log.png)

### Borden {#boards}

>[!NOTE]
>
>Deze functie is alleen beschikbaar via de vroege functie opt-in voor Workfront Boards.

U kunt zich aanmelden op verbonden kaarten op een Workfront-board. Dit is hetzelfde proces als het aanmelden bij een taak of uitgave en de uren die op de kaart zijn aangemeld, worden opgeslagen op de aangesloten taak of uitgave.
Zie voor meer informatie [Gekoppelde kaarten op borden gebruiken](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

### Mobiele app {#mobile-app}

U kunt de tijd vastleggen via de mobiele app van Workfront.
Zie voor meer informatie [Adobe Workfront voor Android](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md) of [Adobe Workfront voor iOS](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md).
