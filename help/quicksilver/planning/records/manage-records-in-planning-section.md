---
title: Records beheren in het gedeelte Planning van Adobe Workfront-objecten
description: U kunt de verslagen van de Planning van Workfront tonen die met de voorwerpen van Adobe Workfront in de sectie van de Planning van een voorwerp van Workfront, in het linkerpaneel worden verbonden.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '1828'
ht-degree: 0%

---


<!--add also Group and Company when they are available-->

# Recordverbindingen beheren vanuit Workfront-objecten

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken.</span>

{{planning-important-intro}}

U kunt Workfront Planning-records in Workfront weergeven in de volgende gebieden van de objecten die ermee zijn verbonden:

* Het gedeelte Planning van een Workfront-object: geeft alle recordtypen weer die zijn verbonden met een object en de bijbehorende gekoppelde records.
* A Planning connection custom field: Toont één verslagtype, zijn respectieve verbonden verslagen, en tot 7 raadplegingsgebieden van de verbonden verslagen.

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
<ul> 
<li><p>Alle Workfront en alle planningspakketten</p></li>
of
<li><p>Willekeurige workflow en planningspakket</p></li></ul>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td>
   <td> <p>Toegang tot projecten, programma's en portfolio's weergeven of vergroten</p>  
   <p>Er is geen configuratie van het toegangsniveau voor de Planning van Workfront. </p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objectmachtigingen</p></td>
   <td>
   <p>In Workfront, Mening of hogere toestemmingen aan een project, portefeuille, of programma </a> </p> 
   <p>In Workfront Planning:</p>
   <ul><li>Machtigingen weergeven voor een werkruimte en het type record weergeven voor het weergeven van alle verbonden records </li>
   of
   <li> Contribute of hoger machtigingen voor een werkruimte en recordtype voor het maken of verbreken van de verbinding met records</a></li></ul> 
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten voor Workfront Planning, inclusief de werkruimten die ze niet hebben gemaakt</p> 
  </td>
  </tr>   
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


<!--Old:
<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Products</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any of the following Workfront plans:</p>
<ul><li>Select</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning is not available for legacy Workfront plans</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td>
   <td>
<p>Any</p>
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>View or higher access to Projects, Programs, and Portfolios</p>  
   <p>There is no access level configuration for Workfront Planning. </p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td>
   <p>In Workfront, View or higher permissions to a project, portfolio, or program</a> </p> 
   <p>In Workfront Planning:
   <ul><li>
   View permissions to a workspace and record type to view any connected records </li>
   or
   <li> Contribute or higher permissions to a workspace and record type  to connect or disconnect records</a></li></ul> </p>  
   <p>System Administrators have permissions to all Workfront Planning workspaces, including the ones they did not create</p> 
  </td>
  </tr>
 </tbody>
</table>-->


## Records beheren in de sectie Planning

U kunt het gedeelte Planning van een Workfront-object gebruiken om alle recordtypen en de bijbehorende records weer te geven die zijn verbonden met het Workfront-object.
Het gedeelte Planning is beschikbaar voor de volgende Workfront-objecten:

* Project
* Portfolio
* Programma
<!--* Group
* Company-->

### Overwegingen over de sectie Planning van Workfront-objecten

Overweeg het volgende wanneer u de verslagen van de Planning van Workfront van de sectie van de Planning van een voorwerp van Workfront bekijkt:

* Workfront Planning-recordtypen moeten eerst worden verbonden met Workfront-objecttypen.

  Raadpleeg de volgende artikelen voor meer informatie:

   * [Verbind recordtypen](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Connect-records](/help/quicksilver/planning/records/connect-records.md)
* U kunt de sectie Planning weergeven vanuit een Workfront-object, zelfs als er geen records zijn gekoppeld aan het Workfront-object.
* <span class="preview"> het verslagtype van A toont slechts op het Gebied van de Planning van een voorwerp van Workfront wanneer u creeert het corresponderende gebied op het verbonden verslagtype dat wanneer het creëren van de verbinding tussen twee verslagtypes plaatst.</span>

  Voor informatie, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).

### Recordverbindingen beheren vanuit de sectie Planning

{{step1-to-planning}}

1. Klik op de kaart van een werkruimte.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op de kaart van een recordtype die is verbonden met een Workfront-project, -portfolio of -programma.
1. Ga naar een verbonden verslaggebied dat een verbinding met een voorwerp van Workfront heeft, of in de lijstmening of van de detailspagina van een verslag. Voor informatie, zie [ verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).
1. Klik op de naam van een Workfront-object in het verbonden recordveld.
De objectpagina wordt geopend in Workfront.

   >[!NOTE]
   >
   >  Als u een Workfront-object kent dat al is verbonden met een planningsrecord, kunt u vanuit het Workfront-object naar de sectie Planning navigeren.

1. Klik **Planning** in het linkerpaneel.

   >[!NOTE]
   >
   >   Uw Workfront of groepsbeheerder moet de sectie Planning toevoegen aan uw lay-outsjabloon voordat deze wordt weergegeven voor een Workfront-project, -portfolio of -programma.

   Het gedeelte Planning wordt weergegeven met de volgende informatie:

   * De verbonden verslagen tonen op individuele kaarten die de volgende informatie bevatten:
      * Naam van de record
      * De recordminiatuur
      * De naam van het verbonden verslaggebied zoals het in de Planning van Workfront toont.
   * Records worden weergegeven in hun respectieve werkruimte en recordtype.

   ![ de sectie van de Planning op project ](assets/planning-section-on-project.png)

1. (Facultatief) klik **tonen alle verbindingen** om alle verbonden verslagtypes, met inbegrip van degenen zonder verbonden verslagen te tonen. Standaard worden recordtypen zonder verbonden records niet weergegeven.
1. Klik op een opnamekaart voor meer informatie over de record. Het voorvertoningsvak voor records wordt weergegeven.
1. (Optioneel) Wijzig de velden in het voorvertoningsvak van de record. Uw wijzigingen worden automatisch opgeslagen.
1. (Facultatief) klik **Open in een nieuw lusje** pictogram ![ Open details in een nieuw lusjepictogram ](assets/open-details-in-a-new-tab-icon.png) in de hoger-juiste hoek van de voorproefdoos om de de detailspagina van het verslag te openen. De detailpagina van het verslag opent in de Planning van Workfront.
1. (Optioneel) Houd de muisaanwijzer boven een opnamekaart en klik op het pictogram voor het verbreken van de verbinding **-** en klik vervolgens op **Verbinding verbreken** .
De volgende dingen doen zich voor:
   * De record is niet meer verbonden met het Workfront-object.
   * Het Workfront-object wordt ook verwijderd uit het verbonden veld van de record uit Workfront Planning.
   * De waarden voor de opzoekvelden van Workfront die zijn verbonden met de planningsrecord, worden ook verwijderd.
1. Klik **verbinden** om meer verslagen voor de verbonden verslagtypes te verbinden.

   Voor meer informatie, zie [ verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).
1. (Optioneel) Als u een record niet kunt vinden om verbinding te maken en u wilt deze toevoegen, klikt u op **+ Toevoegen** om een nieuwe record toe te voegen. Voor meer informatie, zie de sectie &quot;verslagen tot stand brengen aangezien u hen van andere verslagen&quot;in het artikel [ verbindt tot verslagen ](/help/quicksilver/planning/records/create-records.md).

   De volgende dingen doen zich voor:

   * De records zijn direct verbonden met het Workfront-object en worden weergegeven in het gedeelte Planning.
   * Het Workfront-object wordt toegevoegd aan het veld voor het maken van een verbinding in het Workfront-planningsrecord.
   * De waarden voor de opzoekvelden van Workfront die zijn verbonden met de planningsrecord, worden ingevuld in Workfront Planning.

## Records beheren in het verbindingstype Planning

U kunt een aangepast veld voor de planningsverbinding op een Workfront-object gebruiken om één recordtype en de bijbehorende records die met het Workfront-object zijn verbonden, weer te geven.

U kunt controleren welke de verslagtypes van Planning voor het voorwerp van Workfront tonen wanneer u de gebieden van de Verbinding van de Planning creeert douane.

* In het veld Verbinding plannen worden planningsrecords weergegeven nadat een verbinding tot stand is gebracht en wanneer het veld is gekoppeld aan formulieren voor de volgende Workfront-objecten:

   * Project
   * Portfolio
   * Programma
   * Groep
   * Bedrijf

Voor meer informatie, zie [ een vorm ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

### Overwegingen over het type van het de verbindingsgebied van de Planning

Overweeg het volgende wanneer u de verslagen van de Planning van Workfront van een de verbindingsgebied van de Planning van een voorwerp van Workfront bekijkt:

* Een de verbindingsgebied van de Planning toont op de volgende manieren op de douanevorm van een voorwerp van Workfront, nadat de verslagen van de Planning met het voorwerp van Workfront worden verbonden:

   * Als alleen het primaire veld van de verbonden record is geselecteerd, wordt het veld voor de planningsverbinding weergegeven als een veld met meerdere waarden, als de verbinding toestaat dat meerdere records worden gekoppeld. Voor informatie, zie [ verbind verslagtypes overzicht ](/help/quicksilver/planning/architecture/connect-record-types-overview.md).
   * Als uw Workfront of groepsbeheerder extra opzoekvelden heeft toegevoegd van de verbonden record op het aangepaste formulier, wordt het veld voor de planningsverbinding weergegeven als een tabel. U kunt maximaal 7 velden selecteren voor het verbindingsveld Planning. De tabelweergave is alleen-lezen.

* U kunt slechts één verslagtype met één de verbindingsgebied van de Planning associëren. Er geldt geen limiet voor het aantal planningsverbindingsvelden dat u op een formulier hebt.
* U moet de correcte toegang en de toestemmingen aan het voorwerp, het verslag, en de Planning van Workfront hebben om een douaneformulier met een de verbindingsdouanegebied van de Planning aan een voorwerp van Workfront vast te maken.
* U moet Contribute-machtigingen hebben voor een werkruimte in Workfront Planning om verbinding te kunnen maken met records in het veld voor planningsverbinding van een Workfront-object of om de verbinding met records te verbreken.
* Workfront Planning-recordtypen moeten eerst worden verbonden met Workfront-objecttypen. Voor informatie, zie [ Connect verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).Dit maakt de verslagen van de Planning van Workfront toegankelijk van Workfront.
* U kunt records van het verbindingsveld Planning van een Workfront-object alleen verbinden of verbreken voor objecten die Workfront-planningsverbindingen kunnen hebben.

  U kunt bijvoorbeeld een aangepast formulier met een veld voor een planningsverbinding aan taken koppelen, maar u kunt geen objecten voor Workfront-planning aan taken koppelen.
* U kunt een veld voor de planningsverbinding niet bewerken als u Workfront-objecten bulksgewijs bewerkt.
* <span class="preview"> het verslagtype van A toont slechts in een gebied van de de verbindingsdouane van de Planning van een voorwerp van Workfront wanneer u creeert het Create overeenkomstige gebied op het verbonden verslagtype dat wanneer het creëren van de verbinding tussen twee verslagtypes plaatst.</span>

  Voor informatie, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).

### Recordverbindingen beheren vanuit het type Verbindingsveld Planning

1. Ga naar een van de volgende objecttypen die zijn verbonden met een recordtype voor Workfront Planning:

   * Project
   * Portfolio
   * Programma
   * Bedrijf
   * Groep

1. Klik op **&lt; Object > Details** in het linkerdeelvenster.
1. (Voorwaardelijk) Voeg een douaneformulier met minstens één de verbindingsgebied van de Planning voor het voorwerp toe u selecteerde, als één niet aanwezig is.

   >[!NOTE]
   >
   >Uw Workfront of groepsbeheerder moet eerst het formulier maken en er een veld voor een planningsverbinding aan toevoegen voordat u het aan een object kunt toevoegen.


1. Klik in het veld om verbonden records toe te voegen en klik vervolgens op de pijl omlaag in het veld om records in de lijst te selecteren.

   ![ het verbindingsgebied van de Planning op project met open verslaglijst ](assets/planning-connection-field-on-project-with-record-list-open.png)

   >[!TIP]
   >
   >U kunt geen verslagen aan de Verbindingsgebieden van de Planning toevoegen die met de voorwerpen van Workfront buiten het voorwerp worden geassocieerd u selecteerde toen het gebied werd gevormd.
   >
   >U kunt bijvoorbeeld geen records vanuit het aangepaste formulier van een project toevoegen aan een verbindingsveld voor planning dat is gemaakt voor een Portfolio-verbinding.
   >
   >Er is een aanwijzing dat het object van het veld en het object dat u hebt geselecteerd niet overeenkomen.
   >
   >![ Waarschuwing niet gestaafde voorwerp die het gebied van de Verbinding van de Planning op vorm ](assets/warning-unsupported-object-planning-connection-field-on-form.png) plannen

1. Klik buiten de lijst om deze te sluiten.

   De volgende dingen doen zich voor:

   * De records worden direct verbonden met het Workfront-object en worden weergegeven in het verbindingsveld Planning en in het gedeelte Planning van het Workfront-object.
   * Het Workfront-object wordt toegevoegd aan het veld voor het maken van een verbinding in het Workfront-planningsrecord.
   * De waarden voor de opzoekvelden van Workfront die zijn verbonden met de planningsrecord, worden ingevuld in Workfront Planning.
   * Als uw Workfront of groepsbeheerder recordopzoekvelden heeft toegevoegd bij het maken van het aangepaste formulier, worden de opzoekvelden van de record automatisch ingevuld in een tabelweergave. De lijstmening in het de verbindingsgebied van de Planning is read-only.

     ![ de verbindingsgebied van de Planning met lijst op de douaneformulier van de Details van het project ](assets/planning-connection-field-with-table-on-project-details-custom-form.png)

     >[!NOTE]
     >
     >De lijstmening toont slechts wanneer de raadplegingsgebieden aan het gebied van de Verbindingen van de Planning op de douaneformulier zijn toegevoegd.


1. (Facultatief) klik de naam van een verslag of houd de naam van het verslag in de lijst, dan klik het **Open verslag** pictogram ![ Open verslagpictogram op de Vorm van de Verbindingsdouane van de Planning ](assets/open-record-icon-on-planning-connection-custom-form.png) op het de verbindingsgebied van de Planning om het in de Planning van Workfront te openen.
Het voorvertoningsvenster voor details van de Workfront-planningsrecord wordt geopend.
1. Herzie of geef informatie over het verslag uit, of klik **Open in een nieuw lusje** pictogram ![ Open verslag in nieuw lusje ](assets/open-details-in-a-new-tab-icon.png) om de pagina van de verslagdetails te openen.

1. (Facultatief) van de douanevorm in Workfront, klik **verwijderen** pictogram ![ pictogram ](assets/remove-icon.png) op een verslag verwijderen om het uit het de verbindingsgebied van de Planning te verwijderen en het van het voorwerp van Workfront los te maken.
Het Workfront-object wordt losgekoppeld van de planningsrecord en alle opzoekgegevens uit Workfront worden uit de record verwijderd.

1. Klik **sparen Veranderingen** om de douanevorm en om het even welke andere veranderingen te bewaren u aan het voorwerp van Workfront aanbracht.
