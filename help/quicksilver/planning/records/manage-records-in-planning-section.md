---
title: Records beheren in het gedeelte Planning van Adobe Workfront-objecten
description: U kunt de verslagen van de Planning van Workfront tonen die met de voorwerpen van Adobe Workfront in de sectie van de Planning van een voorwerp van Workfront, in het linkerpaneel worden verbonden.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 0%

---


<!--add also Group and Company when they are available-->

# Recordverbindingen beheren vanuit Workfront-objecten

{{planning-important-intro}}

U kunt de verslagen van de Planning van Workfront tonen die met de voorwerpen van Adobe Workfront in de sectie van de Planning van een voorwerp van Workfront, in het linkerpaneel worden verbonden.

<!--replace above with this: 

You can display Workfront Planning records and their respective records connected to Adobe Workfront objects in the following areas in Workfront:

* The Planning section of a Workfront object: Displays all record types connected to an object and their respective connected records. 
* A Planning connection custom field: Displays one record type and its respective connected records .-->

Het gedeelte Planning is beschikbaar voor de volgende Workfront-objecten:

* Project
* Portfolio
* Programma
<!--* Group
* Company-->

<!--move the above to a lower place below when releasing Planning connection custom field-->


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
<li>Eerste</li>
<li>Ultieme</li></ul>
<p>Workfront Planning is niet beschikbaar voor oudere Workfront-plannen</p>
   </td>

<tr>
   <td role="rowheader"><p>Planning van Adobe Workfront*</p></td>
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
   <p>In de Planning van Workfront, Contribute of hogere toestemmingen aan een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten voor Workfront Planning, inclusief de werkruimten die ze niet hebben gemaakt</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Alle gebruikers, met inbegrip van de beheerders van Workfront, moeten een lay-outmalplaatje worden toegewezen dat het Gebied van de Planning in het Belangrijkste Menu en het Gebied van de Planning voor projecten, portefeuilles, en programma's omvat. </p> Voor meer informatie, zie <a href="/help/quicksilver/planning/access/access-overview.md"> Adobe plannend toegangsoverzicht </a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Records beheren in de sectie Planning

U kunt het gedeelte Planning van een Workfront-object gebruiken om alle recordtypen en de bijbehorende records weer te geven die zijn verbonden met het Workfront-object.

<!--move the section above starting with "The Planning section is available ..." here-->

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
   * Records worden weergegeven in hun respectievelijke werkruimte.

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

<!--

## Manage records in the Planning connection field type

You can use a Planning connection custom field on a Workfront object to view one record type and its respective records connected to the Workfront object. 

You can control which Planning records display for the Workfront object when you create Planning connection custom fields. 

* The Planning connection field can be populated with Planning records when it is attached to forms for the following Workfront objects:

   * Project
   * Portfolio
   * Program
   * Group
   * Company

For more information, see [Create a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). 

### Considerations about the Planning connection field type

Consider the following when you view Workfront Planning records from a Planning connection field of a Workfront object: 

* You can associate only one record type with one Planning connection field.
* Your Workfront or group administrator must add a Planning connection field on a Workfront custom form.
* You must attach the custom form to a Workfront object that can be connected from Workfront Planning, if you have the correct access.
* Workfront Planning record types must first be connected to Workfront object types. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 
* You can connect or disconnect records from the Planning connection field of a Workfront object only for objects that can have Workfront Planning connections.
* You must have Contribute permissions for a workspace in Workfront Planning to be able to connect or disconnect records from the Planning connection field of a Workfront object.
* You can view a Planning connection field for a Workfront object, even when there are no records connected to the object yet. 
* You cannot edit a Planning connection field when editing Workfront objects in bulk. 

### Manage record connections from the Planning connection field type

1. Go to one of the following object types that has been connected with a Workfront Planning record type: 

   * Project
   * Portfolio
   * Program
   * Company
   * Group

1. Click **< Object > Details** in the left panel.
1. (Conditional) Add a custom form with at least one Planning connection field for the object you selected, if one is not present. 

   >[!NOTE]
   >
   >Your Workfront or group administrator must first create the form and add a Planning connection field on it before you can add it to an object. 


1. Click inside the field to add connected records.
1. Click the downward-pointing arrow inside the field, to select records from the list. 

   ![](assets/planning-connection-field-on-project-with-record-list-open.png)

   >[!TIP]
   >
   >   You cannot add records to Planning connection fields that are associated with Workfront objects other than the object you selected. 
   >
   >For example, you cannot add records to a Planning connection field created for a Portfolio connection from a Project's custom form. 
   >
   >There is an indication that the object of the field and the object you selected don't match.  
   >
   >![](assets/warning-unsupported-object-planning-connection-field-on-form.png)

1. Click outside the list to close it. 

   The following things occur:

   * The records are immediately connected to the Workfront object and they display in the Planning connection field as well as the Planning section of the Workfront object. 
   * The Workfront object is added to the Workfront Planning record's connected field. 
   * The values for the Workfront lookup fields connected to the Planning record are populated in Workfront Planning. 
1. (Optional) Click the name of a record in the Planning connection field to open it in Workfront Planning. 
   The record details tab opens in Workfront Planning. 
   You can review information about the record, or navigate to the record type page. 

1. (Optional) From the custom form in Workfront, click the **Remove** icon ![](assets/remove-icon.png) on a record to remove it from the Planning connection field and disconnect it from the Workfront object. 
   The Workfront object is disconnected from the Planning record, and any lookup information from Workfront is removed from the record. 

-->