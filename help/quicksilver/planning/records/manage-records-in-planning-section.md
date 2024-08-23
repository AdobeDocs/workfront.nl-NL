---
title: Records beheren in het gedeelte Planning van Adobe Workfront-objecten
description: U kunt de verslagen van de Planning van Workfront tonen die met de voorwerpen van Adobe Workfront in de sectie van de Planning van een voorwerp van Workfront, in het linkerpaneel worden verbonden.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: 61cad7dc76ba04ea84ff0bd5052182f040f7b4d9
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--add also Group and Company when they are available-->

<!-- opening the Details preview and page is not possible yet - hid those steps, but add them when released-->


# Records beheren in het gedeelte Planning van Adobe Workfront-objecten

{{planning-important-intro}}

U kunt de verslagen van de Planning van Workfront tonen die met de voorwerpen van Adobe Workfront in de sectie van de Planning van een voorwerp van Workfront, in het linkerpaneel worden verbonden.

Het gedeelte Planning is beschikbaar voor de volgende Workfront-objecten:

* Project
* Portfolio
* Programma
<!--* Group
* Company-->

## Toegangsvereisten

<!--Updated for GA-->

+++ Breid uit om toegangsvereisten voor de Planning van Workfront te bekijken.

U moet het volgende hebben om tot de Planning van Workfront toegang te hebben:

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
<li>Eerste</li>
<li>Ultieme</li></ul>
<p>Workfront Planning is niet beschikbaar voor oudere Workfront-plannen</p>
   </td>

<tr>
   <td role="rowheader"><p>Planning van Adobe Workfront*</p></td>
   <td>
<p>Alle</p>
<p>Voor meer informatie over wat in elk Plan van de Planning van Workfront inbegrepen is, zie <a href="https://business.adobe.com/products/workfront/pricing.html"> Adobe Workfront tarifering en verpakking </a>. </p>
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
   <p>In de Planning van Workfront, Contribute of hogere toestemmingen aan een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten voor Workfront Planning, inclusief de werkruimten die ze niet hebben gemaakt</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Alle gebruikers, met inbegrip van de beheerders van Workfront, moeten een lay-outmalplaatje worden toegewezen dat het Gebied van de Planning in het Belangrijkste Menu en het Gebied van de Planning voor projecten, portefeuilles, en programma's omvat. </p> Voor meer informatie, zie <a href="/help/quicksilver/planning/access/access-overview.md"> overzicht van de Toegang </a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen over de sectie Planning van Workfront-objecten

* Workfront Planning-recordtypen moeten zijn verbonden met Workfront-objecttypen.

  Raadpleeg de volgende artikelen voor meer informatie:

   * [Verbind recordtypen](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Connect-records](/help/quicksilver/planning/records/connect-records.md)
* U kunt de sectie Planning weergeven in een Workfront-object, zelfs als er geen records zijn gekoppeld aan het Workfront-object.
* U kunt Planningsrecords verbinden met Workfront-objecten vanuit Workfront, in de sectie Planning wanneer ten minste één record is verbonden met het Workfront-object.

## Records beheren in de sectie Planning

{{step1-to-planning}}

1. Klik op de kaart van een werkruimte.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op de kaart van een recordtype die is verbonden met een Workfront-project, -portfolio of -programma.
1. Ga naar een verbonden verslaggebied dat een verbinding met een voorwerp van Workfront heeft, of in de lijstmening of van de detailspagina van een verslag. Voor informatie, zie [ verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).
1. Klik op de naam van een Workfront-object in het verbonden recordveld.
De objectpagina wordt geopend in Workfront.

1. Klik **Planning** in het linkerpaneel.

   >[!NOTE]
   >
   >   Uw Workfront of groepsbeheerder moet de sectie Planning toevoegen aan uw lay-outmalplaatje alvorens het voor een project, een portefeuille, of een programma van de Wereld toont.

   Het gedeelte Planning wordt weergegeven met de volgende informatie:

   * De verbonden verslagen tonen op individuele kaarten die de volgende informatie bevatten:
      * Naam van de record
      * De recordminiatuur
      * De naam van het verbonden verslaggebied zoals het in de Planning van Workfront toont.
   * Records worden weergegeven in hun respectievelijke werkruimte.

   ![](assets/planning-section-on-project.png)

1. (Facultatief) klik **tonen alle verbindingen** om alle verbonden verslagtypes, met inbegrip van degenen zonder verbonden verslagen te tonen. Standaard worden recordtypen zonder verbonden records niet weergegeven.
1. Klik op een opnamekaart voor meer informatie over de record. Het voorvertoningsvak voor records wordt weergegeven.
1. (Optioneel) Wijzig de velden in het voorvertoningsvak van de record. Uw wijzigingen worden automatisch opgeslagen.
1. (Facultatief) klik **Open in een nieuw lusje** pictogram ![](assets/open-details-in-a-new-tab-icon.png) in de hoger-juiste hoek van de voorproefdoos om de de detailspagina van het verslag te openen. De detailpagina van het verslag opent in de Planning van Workfront.
1. Beweeg over een verslagkaart, dan klik los verslagpictogram **-**, dan klik **losmaakt**.
De volgende dingen doen zich voor:
   * De record is niet meer verbonden met het Workfront-object.
   * Het Workfront-object wordt ook verwijderd uit het verbonden veld van de record uit Workfront Planning.
   * De waarden voor de opzoekvelden van Workfront die zijn verbonden met de planningsrecord, worden ook verwijderd.
1. Klik **verbinden** om meer verslagen voor de verbonden verslagtypes te verbinden. Voor meer informatie, zie [ verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).

   De volgende dingen doen zich voor:

   * De records zijn direct verbonden met het Workfront-object en worden weergegeven in het gedeelte Planning.
   * Het Workfront-object wordt toegevoegd aan het veld voor het maken van een verbinding in het Workfront-planningsrecord.
   * De waarden voor de opzoekvelden van Workfront die zijn verbonden met de planningsrecord, worden ingevuld in Workfront Planning.


