---
title: Records beheren in het gedeelte Planning van Adobe Workfront-objecten
description: U kunt de verslagen van de Planning van Workfront tonen die met de voorwerpen van Adobe Workfront in de sectie van de Planning van een voorwerp van Workfront, in het linkerpaneel worden verbonden.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '1433'
ht-degree: 0%

---


<!--add also Group and Company when they are available-->

# Recordverbindingen beheren vanuit Workfront-objecten

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

U kunt Workfront Planning-records en de bijbehorende records die zijn verbonden met Adobe Workfront-objecten weergeven in de volgende gebieden in Workfront:

* Het gedeelte Planning van een Workfront-object: geeft alle recordtypen weer die zijn verbonden met een object en de bijbehorende gekoppelde records.
* A Planning connection custom field: Toont één recordtype en zijn respectieve verbonden verslagen.

## Toegangsvereisten

+++ Breid uit om toegangsvereisten voor de Planning van Workfront te bekijken.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Producten</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront-abonnement*</p></td>
   <td>
<p>Een van de volgende Workfront-plannen:</p>
<ul><li>Selecteren</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning is niet beschikbaar voor oudere Workfront-plannen</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-planningspakket*</p></td>
   <td>
<p>Alle</p>
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningsplan is opgenomen. </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-platform</p></td>
   <td>
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden genegeerd om tot alle mogelijkheden van de Planning van Workfront te kunnen toegang hebben.</p>
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td>
   <td>
   <p>Standaard</p>
   <p>Workfront Planning is niet beschikbaar voor oudere Workfront-licenties</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td>
   <td> <p>De mening of hogere toegang tot Projecten, Programma's, en Portfolio's</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objectmachtigingen</p></td>
   <td>
   <p>In Workfront, Mening of hogere toestemmingen aan een project, portefeuille, of programma </a> </p> 
   <p>In de Planning van Workfront, de toestemmingen van de Mening aan een werkruimte om het even welke verbonden verslagen of Contribute of hogere toestemmingen aan een werkruimte te bekijken om verslagen te verbinden of los te maken </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten voor Workfront Planning, inclusief de werkruimten die ze niet hebben gemaakt</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Om het planningsgebied of de sectie van de Planning voor een voorwerp van Workfront te bekijken, moeten alle gebruikers, met inbegrip van de beheerders van Workfront, een lay-outmalplaatje worden toegewezen dat het gebied van de Planning in het Belangrijkste Menu en het gebied van de Planning voor projecten, portefeuilles, en programma's omvat. </p> Voor meer informatie, zie <a href="/help/quicksilver/planning/access/access-overview.md"> Adobe plannend toegangsoverzicht </a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

   ![](assets/planning-section-on-project.png)

1. (Facultatief) klik **tonen alle verbindingen** om alle verbonden verslagtypes, met inbegrip van degenen zonder verbonden verslagen te tonen. Standaard worden recordtypen zonder verbonden records niet weergegeven.
1. Klik op een opnamekaart voor meer informatie over de record. Het voorvertoningsvak voor records wordt weergegeven.
1. (Optioneel) Wijzig de velden in het voorvertoningsvak van de record. Uw wijzigingen worden automatisch opgeslagen.
1. (Facultatief) klik **Open in een nieuw lusje** pictogram ![](assets/open-details-in-a-new-tab-icon.png) in de hoger-juiste hoek van de voorproefdoos om de de detailspagina van het verslag te openen. De detailpagina van het verslag opent in de Planning van Workfront.
1. (Optioneel) Houd de muisaanwijzer boven een opnamekaart en klik op het pictogram voor het verbreken van de verbinding **-** en klik vervolgens op **Verbinding verbreken** .
De volgende dingen doen zich voor:
   * De record is niet meer verbonden met het Workfront-object.
   * Het Workfront-object wordt ook verwijderd uit het verbonden veld van de record uit Workfront Planning.
   * De waarden voor de opzoekvelden van Workfront die zijn verbonden met de planningsrecord, worden ook verwijderd.
1. Klik **verbinden** om meer verslagen voor de verbonden verslagtypes te verbinden. Voor meer informatie, zie [ verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).

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

* U kunt slechts één verslagtype met één de verbindingsgebied van de Planning associëren.
* U moet een douaneformulier met een de verbindingsdouane van de Planning aan een voorwerp van Workfront vastmaken dat van de Planning van Workfront kan worden verbonden, als u de correcte toegang hebt.
* Workfront Planning-recordtypen moeten eerst worden verbonden met Workfront-objecttypen. Voor informatie, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).
* U kunt records van het verbindingsveld Planning van een Workfront-object alleen verbinden of verbreken voor objecten die Workfront-planningsverbindingen kunnen hebben.
* U moet Contribute toestemmingen voor een werkruimte in de Planning van Workfront hebben om verslagen van het de verbindingsgebied van de Planning van een voorwerp van Workfront te kunnen verbinden of los te maken.
* U kunt een veld voor de planningsverbinding niet bewerken als u Workfront-objecten bulksgewijs bewerkt.

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

   ![](assets/planning-connection-field-on-project-with-record-list-open.png)

   >[!TIP]
   >
   >U kunt geen verslagen aan de Verbindingsgebieden van de Planning toevoegen die met de voorwerpen van Workfront buiten het voorwerp worden geassocieerd u selecteerde toen het gebied werd gevormd.
   >
   >U kunt bijvoorbeeld geen records toevoegen aan een veld voor een planningsverbinding dat is gemaakt voor een Portfolio-verbinding vanuit het aangepaste formulier van een project.
   >
   >Er is een aanwijzing dat het object van het veld en het object dat u hebt geselecteerd niet overeenkomen.
   >
   >![](assets/warning-unsupported-object-planning-connection-field-on-form.png)

1. Klik buiten de lijst om deze te sluiten.

   De volgende dingen doen zich voor:

   * De records worden direct verbonden met het Workfront-object en worden weergegeven in het verbindingsveld Planning en in het gedeelte Planning van het Workfront-object.
   * Het Workfront-object wordt toegevoegd aan het veld voor het maken van een verbinding in het Workfront-planningsrecord.
   * De waarden voor de opzoekvelden van Workfront die zijn verbonden met de planningsrecord, worden ingevuld in Workfront Planning.
1. (Optioneel) Klik op de naam van een record in het veld Verbinding plannen om de record te openen in Workfront Planning.
Het tabblad met recorddetails wordt geopend in Workfront Planning.
U kunt informatie over de record controleren of naar de pagina met recordtypen navigeren.

1. (Facultatief) van de douanevorm in Workfront, klik **verwijderen** pictogram ![](assets/remove-icon.png) op een verslag om het uit het de verbindingsgebied van de Planning te verwijderen en het van het voorwerp van Workfront los te maken.
Het Workfront-object wordt losgekoppeld van de planningsrecord en alle opzoekgegevens uit Workfront worden uit de record verwijderd.