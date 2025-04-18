---
title: Workfront-objecten maken met Adobe Workfront Planning Record Automations
description: U kunt automatiseringen in de Planning van Adobe Workfront vormen die, wanneer geactiveerd, tot voorwerpen in Workfront of verslagen in de Planning van Workfront leiden. De gemaakte objecten en records worden automatisch verbonden met bestaande planningsrecords. In dit artikel wordt beschreven hoe u automatiseringen kunt beheren, zoals het bewerken, uitschakelen, verwijderen en activeren van objecten en records.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 4bdd4510a5ff7faf8f497299eac0a10f4fe7fbc2
workflow-type: tm+mt
source-wordcount: '2203'
ht-degree: 0%

---

# Objecten maken met Adobe Workfront Planning-recordautomatisering

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->

<!--you might need to add something about notifications and emails?!-->
<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

U kunt automatiseringen in de Planning van Adobe Workfront vormen die, wanneer geactiveerd, tot voorwerpen in Workfront of verslagen in de Planning van Workfront leiden wanneer teweeggebracht van een verslag van de Planning. De gemaakte objecten of records worden automatisch verbonden met de records waaruit u de automatisering activeert.

U kunt de automatisering in de verslagtype pagina in de Planning van Workfront vormen en activeren. Het verbonden object dat wordt gemaakt, wordt in het verbonden veld van het recordtype geplaatst waaruit u de automatisering uitvoert.

U kunt bijvoorbeeld een automatisering maken die een Workfront-planningscampagne voert en een project maakt in Workfront om de voortgang van die campagne te volgen. Het project zou worden verbonden met de campagne van de Planning van Workfront op het Verbonden gebied van het Project op de campagne.

Voor meer informatie over verbonden verslagen, zie [ Verbonden verslagenoverzicht ](/help/quicksilver/planning/records/connected-records-overview.md).

U kunt het volgende tot stand brengen gebruikend automatisering in de Planning van Workfront:

* Eén of meerdere projecten
* Een groep
* Een programma
* Een portfolio
* Een project
* Een record

## Toegangsvereisten

+++ Breid uit om toegangsvereisten te bekijken..

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
<p>Alle </p> 
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningsplan is opgenomen. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-platform</p></td> 
   <td> 
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden bezeten om tot alle mogelijkheden van de Planning van Workfront toegang te hebben.</p> 
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td> Standaard
   <p>Workfront Planning is niet beschikbaar voor oudere Workfront-licenties</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td> 
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p> 
   <p>Bewerk de toegang tot Create-objecten in Workfront voor de objecttypen die u wilt maken (projecten, portfolio's, programma's). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td> <p>Machtigingen voor de werkruimte beheren om automatiseringen te maken. </p>
   <p>Draag of hogere toestemmingen aan de werkruimte <span class="preview"> en aan het verslagtype </span> bij waar u voorwerp gebruikend bestaande automatiseringen wilt tot stand brengen. </p>  
   <p>Rechten voor Workfront-objecten (portfolio's) beheren om onderliggende objecten (programma's of projecten) toe te voegen.</p>
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat </p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Overwegingen bij het maken van objecten en records via een automatisering

* De naam van het object of de record die door een automatisering is gemaakt, is gelijk aan de naam van de record waaruit u het object of de record maakt, wanneer u één object maakt.

* Wanneer u veelvoudige projecten creeert, worden zij automatisch genoemd volgens het volgende patroon:

  `[ Name of the record ] Name of the field choice`

  Voor meer informatie, zie het [ Gebruik een automatisering van de Planning van Workfront om een voorwerp of een verslag ](#use-a-workfront-planning-automation-to-create-an-object-or-a-record) sectie in dit artikel tot stand te brengen.

* Nieuwe objecten of records overschrijven bestaande in hetzelfde veld niet. Als u dezelfde automatisering meerdere keren voor dezelfde record trigt, worden de nieuwe objecten of records in hetzelfde verbonden veld van de oorspronkelijke record toegevoegd, naast de objecten of records die u eerder hebt gemaakt.

<!--hide this for now; they are trying to remove this limitation: * The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered.-->

## Automatisering configureren in Workfront-planning

U moet een automatisering voor een verslagtype in de Planning van Workfront vormen alvorens u het kunt gebruiken om voorwerpen te creëren.

{{step1-to-planning}}

1. Klik op een recordtypekaart en klik vervolgens op de naam van een record.

   De pagina met recordtypen wordt geopend.
1. Klik **Meer** menu ![ Meer menu ](assets/more-menu.png) aan het recht van de naam van het verslagtype, dan klik **leiden automatiseringen**.

   De lijst met beschikbare automatiseringen voor het geselecteerde recordtype wordt geopend.

1. Klik **Nieuwe automatisering** in de hoger-juiste hoek van het scherm. Het **Nieuwe automatiserings** vakje opent.
1. Werk de volgende velden bij:

   * Vervang **Naamloze automatisering** met de tekst die u op de automatiseringsknoop wilt verschijnen. Gebruikers klikken op deze knop wanneer ze de automatisering gebruiken om een Workfront-object of een planningsrecord te maken.
   * **Beschrijving**: Voeg een beschrijving toe om het doel van de automatisering te identificeren.
1. Klik **sparen**.
De pagina met gegevens over automatisering wordt geopend.

1. Voor de detailspagina van de automatisering, werk de volgende gebieden in de **1} sectie van Trekkers bij {:**

   * **Trekker**: Selecteer de actie die de automatisering zal teweegbrengen. Bijvoorbeeld, uitgezochte **Knoop klikt**. <!--update this step with a list of all possible triggers; right now only Button click is available-->

1. Werk de volgende gebieden in de **sectie van Acties** bij: <!--submitted bugs for these fields - see if they need changing here-->
   * **Acties**: Selecteer de actie die u Workfront wilt uitvoeren wanneer het teweegbrengen van de automatisering. Dit is een verplicht veld.
Selecteer een van de volgende handelingen:

      * Meerdere projecten maken
      * Eén project maken
      * Project maken
      * Record maken
      * Programma maken
      * Portefeuille maken
      * Groep maken

     >[!TIP]
     >
     >Nadat u de automatisering hebt opgeslagen, kunt u de geselecteerde actie in dit veld niet meer wijzigen.

1. (Voorwaardelijk) Afhankelijk van de actie die u hebt geselecteerd, werkt u de volgende velden bij:

   * **creeer één enkel project**: <!--replace to the left: Create a single project-->
      * **Verbonden gebied waar het project** wordt gecreeerd: Dit is het verbonden gebied waar het nieuwe project zal tonen. Dit is een verplicht veld.
      * **malplaatje van het Project**: Selecteer een projectmalplaatje dat Workfront zal gebruiken om het project tot stand te brengen.

   * Meerdere projecten maken:
      * **Verbonden gebied waar het project** wordt gecreeerd: Dit is het verbonden gebied waar het nieuwe project zal tonen. Dit is een verplicht veld.
      * **Gebied de waarvan keuzen tot de verslagen** zullen leiden: Kies een multi- of enig-uitgezocht gebied van het geselecteerde verslagtype. Workfront maakt een project voor elke veldkeuze die momenteel is geselecteerd in de record waaruit de automatisering wordt geactiveerd.

     >[!TIP]
     >
     >Een project wordt gecreeerd slechts voor de opties die momenteel op het multi- of enig-uitgezochte gebied van het verslag worden geselecteerd u de automatisering van in werking stelt, en niet voor alle mogelijke keuzen voor dat gebied.
     >

      * **Gebruik het zelfde malplaatje**: Selecteer deze optie om het zelfde malplaatje voor elk nieuw project te gebruiken. Als de optie wordt geschrapt, selecteer a **malplaatje van het Project** voor elke gebiedskeuze.
      * **malplaatje van het Project**: Als u **het zelfde malplaatje** optie selecteerde, selecteer een projectmalplaatje dat Workfront zal gebruiken om de projecten tot stand te brengen.

   * **creeer portefeuille**:
      * **Verbonden gebied waar de portefeuille** wordt gecreeerd: Dit is het verbonden gebied waar de nieuwe portefeuille zal tonen. Dit is een verplicht veld.
      * **Vorm van de Douane aan bijlage aan de nieuwe portefeuille**: Selecteer een douaneformulier om aan de nieuwe portefeuille vast te maken. U moet een aangepast portfolioformulier maken voordat u het kunt selecteren.
   * **creeer programma**:
      * **Verbonden gebied waar het programma** wordt gecreeerd: Dit is het verbonden gebied waar het nieuwe programma zal tonen. Dit is een verplicht veld.
      * **portefeuille van het Programma**: Selecteer een portefeuille waar het nieuwe programma zal worden toegevoegd. Dit is een verplicht veld.
      * **Vorm van de Douane aan het nieuwe programma** vast te maken: Selecteer een douanevorm om aan het nieuwe programma vast te maken. U moet een aangepast programma maken voordat u het kunt selecteren.
   * **creeer groep**:
      * **Verbonden gebied waar de groep** wordt gecreeerd: Dit is het verbonden gebied waar de nieuwe groep zal tonen. Dit is een verplicht veld.
      * **Vorm van de Douane aan de nieuwe groep** vast te maken: Selecteer een douaneformulier om aan het nieuwe programma vast te maken. U moet een aangepast programma maken voordat u het kunt selecteren.
   * **creeer verslag**:
      * **Type van Verslag**: Selecteer het verslagtype u wilt tot stand brengen.

        De **sub-sectievertoningen van Montages**. Werk de volgende gebieden in de **sub-sectie van Montages** bij:

         * **Gebied op het verbonden verslagtype waar het huidige verslag** zal tonen: Dit is het verbonden gebied op het verslagtype dat voor de actie wordt geselecteerd waar het huidige verslag zal tonen.

        Als u bijvoorbeeld een automatisering maakt voor campagnes om productrecords met elkaar te verbinden, is dit het verbonden veld op het productrecordtype waarin de campagnes worden weergegeven, nadat de producten met de automatisering zijn gemaakt.

        Dit is een verplicht veld.

        <!--submitted a change in functionality and UI text for this - revise??-->
Op het **gebied van de Kaart**, werk de volgende informatie bij:

         * **Overdracht van**: Selecteer gebieden van het verslagtype de automatisering voor wordt gecreeerd om hen aan de gebieden van het verbonden verslagtype in kaart te brengen.
         * **Overdracht aan**: Selecteer gebieden van het pas gecreëerde verslag dat met informatie van het verslag zal bevolken u de automatisering van in werking stelt.

        >[!TIP]
        >
        >* De veldtypen van het oorspronkelijke recordtype moeten overeenkomen met de veldtypen van het nieuwe recordtype.
        >* Als u geen gebieden kiest, zullen de namen van de nieuwe verslagen **Naamloos verslag** zijn.

1. (Facultatief en voorwaardelijk) als u selecteerde om een verslag tot stand te brengen, **voegt gebieden** toe om extra raadplegingsgebieden van één verslag aan een andere in kaart te brengen.
1. (Voorwaardelijk) als er geen verbindingsgebieden tussen het originele verslagtype en het verslagtype zijn dat op het **wordt geselecteerd het type van Verslag** gebied, **klikken voegt verbonden gebied** toe.

   ![ opstelling van de Automatisering om een verslag ](assets/automation-setup-create-record.png) te creëren

   De volgende twee velden worden gemaakt:

   * Een nieuw verbindingsgebied genoemd **Verbonden verslag** wordt gecreeerd voor het verslagtype u op het **type van Verslag** gebied wees.
   * Een nieuw verbindingsgebied met de zelfde naam zoals die op het **wordt vermeld het type van het Verslag** gebied wordt gecreeerd voor het verslagtype u de automatisering voor vormt.

     Bijvoorbeeld, als u een automatisering voor Campagnes vormt om een ander verslagtype automatisch tot stand te brengen genoemd Banden en u **klikt voeg verbonden gebied** toe, worden de volgende gebieden gecreeerd:

      * Het **Verbonden verslag** verbindingsgebied wordt gecreeerd voor het **Merken** verslagtype.
      * Het **Merken** verbindingsgebied wordt gecreeerd voor het **3} verslagtype van Campagnes {.**

1. (Facultatief) als er geen verbindingsgebieden tussen het originele verslagtype en het voorwerp van Workfront dat op het gebied van Acties wordt geselecteerd zijn, klik **voeg verbonden gebied** toe.

   ![ opstelling van de Automatisering om veelvoudige projecten ](assets/automation-setup-create-multiple-projects.png) tot stand te brengen

   Het volgende wordt gemaakt:

   * Een nieuw verbindingsgebied genoemd **Verbonden &lt; naam van het voorwerp van Workfront >** wordt gecreeerd voor het verslagtype u de automatisering voor bouwt. Bijvoorbeeld, wordt het a **Verbonden project** gebied gecreeerd voor het verslagtype u de automatisering voor bouwt, wanneer u verkiest om projecten automatisch tot stand te brengen.
   * Er wordt een nieuwe recordtypekaart toegevoegd aan de sectie Planning van een Workfront-project, in Workfront met de naam van het recordtype waarvoor u de automatisering configureert.

1. Klik **sparen** in de hoger-juiste hoek van de pagina van de automatiseringsdetails.

   De automatisering wordt weergegeven in de lijst met automatiseringen en is beschikbaar voor gebruik in records.

## Bestaande automatisering beheren

{{step1-to-planning}}

1. Klik op een recordtypekaart en klik vervolgens op de naam van een record.

   De pagina met recordtypen wordt geopend.
1. Klik **Meer** menu ![ Meer menu ](assets/more-menu.png) aan het recht van de naam van het verslagtype, dan klik **leiden automatiseringen**.

   De lijst met beschikbare automatiseringen voor het geselecteerde recordtype wordt geopend.

1. (Optioneel) Voer een van de volgende handelingen uit om een automatisering te bewerken, uit te schakelen of te verwijderen:

   1. Van de lijst van automatiseringen, houd over de naam van een bewaarde automatisering, dan klik **Meer** menu ![ Meer menu ](assets/more-menu.png).

   1. Klik **uitgeven** om de volgende informatie bij te werken:

      * Klik **Meer** menu ![ Meer menu ](assets/more-menu.png) rechts van de automatiseringsnaam, dan klik **uitgeven** om de naam van de automatisering te veranderen.
      * Om het even welke gebieden in de automatisering, behalve het **gebied van Acties**.

        >[!TIP]
        >
        >U kunt de oorspronkelijk geselecteerde actie voor een automatisering niet wijzigen.


   1. Klik **onbruikbaar maken** om de automatisering uit de de lijstmening van het verslag te verwijderen en gebruikers te verhinderen het te gebruiken om verslagen of voorwerpen tot stand te brengen.

      Records die zijn gemaakt met een uitgeschakelde automatisering, blijven verbonden met de oorspronkelijk geselecteerde record.

      Om het opnieuw beschikbaar te maken, klik **Meer** menu ![ ](assets/more-menu.png) opnieuw, dan klik **activeren**.
   1. Klik **Schrapping** om de automatisering te schrappen. Een verwijderde automatisering kan niet worden hersteld.

      Records die zijn gemaakt met een verwijderde automatisering, blijven verbonden met de oorspronkelijk geselecteerde record.

## Een Workfront-planningsautomatisering gebruiken om een object of record te maken

1. Open in Workfront Planning de pagina met recordtypen die de automatisering bevat die u wilt gebruiken om automatisch records of objecten te maken en te verbinden.
1. Open de tabelweergave.
1. Selecteer een of meer records.

   Onder aan de tabel wordt een blauwe balk weergegeven met extra knoppen, zoals automatiseringsknoppen.
1. Klik op de automatiseringsknop in de rechterbenedenhoek van het scherm.

   ![ knoop van de Automatisering ](assets/automation-custom-button.png)

   De volgende dingen doen zich voor:

   * Onder aan het scherm wordt een bevestigingsbericht weergegeven als met succes een object of record is gemaakt.

   * Het nieuwe object wordt weergegeven in het verbonden veld dat wordt aangegeven in de instelling van de automatiseringsknop. Mogelijk moet u de pagina vernieuwen voordat u het nieuwe object kunt bekijken. Het nieuwe object heeft dezelfde naam als de oorspronkelijke record.

   * Als er meerdere projecten zijn gemaakt op basis van de keuzes van meerdere of één-selectievelden, krijgen de projecten automatisch een naam op basis van het volgende patroon:

     `[ Name of the record ] Name of the field choice`

     Als een campagne met de naam `Summer breeze` bijvoorbeeld een project heeft gegenereerd op basis van een keuze uit een veld in `EMEA` , krijgt het project de naam `[ Summer breeze ] EMEA` .

   * De record waaruit u de automatisering activeert, wordt toegevoegd aan het verbonden veld van de nieuwe records.

   >[!NOTE]
   >
   >We raden u aan te controleren of de objecten of records zijn gemaakt en verbonden zoals u had verwacht.

1. (Optioneel) Klik op het nieuwe object in het verbonden veld. De objectpagina wordt geopend en u kunt aanvullende wijzigingen in het nieuwe object aanbrengen.

<!--ORIGINAL AUTOMATION FUNCTIONALITY - BEFORE FEB. 20, 2025

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. The created objects or records are automatically connected to the records you are triggering the automation from. 

You can configure and activate the automation in the record type's page in Workfront Planning. The connected object that is created is placed in the connected field of the record type you run the automation from. 

For example, you could create an automation that takes a Workfront Planning campaign and creates a project in Workfront to track that campaign's progress. The project would be connected to the Workfront Planning campaign in the Connected Project field on the campaign.

For more information on connected records, see [Connected records overview](/help/quicksilver/planning/records/connected-records-overview.md).

## Access requirements

+++ Expand to view access requirements.. 

You must have the following access to perform the steps in this article:  

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
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace you want to add records to. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).   

+++


## Considerations about creating objects and records using an automation

* The new object or record name is the same as the record name from which you create it. 
* New objects or records don't override existing ones in the same field. Triggering the same automation multiple times for the same records adds the new objects or records in the same connected field of the original record, in addition to the ones created before. 
* The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered. 

## Configure an automation in Workfront Planning

You must configure an automation for a record type in Workfront Planning, before you can use it to create objects.

{{step1-to-planning}}

1. Click a record type card, then click the name of a record. 

   The record type page opens. 
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Manage automations**. 

   The list of available automations for the selected record type opens.

1. Click **New automation** in the upper-right corner of the screen. The **New automation** box opens.
1. Update the following fields:

   * Replace **Untitled automation** with the text that you want to appear on the automation button. Users will click this button when using the automation to create a Workfront object or a Planning record.
   * **Description**: Add a description to identify the purpose of the automation.
1. Click **Save**.
   The automation details page opens. 

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. For example, select **Button click**. (********update this step with a list of all possible triggers; right not only Button click is available***********)

1. Update the following fields in the **Actions** section: <********submitted bugs for these fields - see if they need changing here*********)
   * **Object type**: Select the object that you want the automation to create. This is a required field.
      
      You can create the following objects from Workfront Planning records: 

      * Project
      * Portfolio
      * Program
      * Group
      * Record

      >[!TIP]
      >
      >After you saved the automation, you can no longer change the object type in this field.

1. (Conditional) Depending on what type of object you want to create, update the following fields:


   * **Project**: 
      * **Connected field where the object is created**: This is the connected field where the new project will display. This is a required field. 
      * **Template from which to create the project**: Select a project template that Workfront will use to create the project.  
   * **Portfolio**:
      * **Connected field where the object is created**: This is the connected field where the new portfolio will display. This is a required field.
      * **Custom form to attach to the new portfolio**: Select a custom form to attach to the new portfolio. You must create a portfolio custom form before you can select it. 
   * **Program**: 
      * **Connected field where the object is created**: This is the connected field where the new program will display. This is a required field.
      * **Program portfolio**: Select a portfolio where the new program will be added. This is a required field.
      * **Custom form to attach to the new program**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Group**:
      * **Connected field where the object is created**: This is the connected field where the new group will display. This is a required field.
      * **Custom form to attach to the new group**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Record**: 
      * **Connected record type**: Select the record type you want to create. 
      * **Connected field where the record is created**: This is the connected field where the new record will display. This is a required field. (******this might need revision as right now it shows the field on the connected record table where the current record will display; submitted a bug to correct this label*********)
      * **Map fields**
         * **Transfer from**: Select fields from the record type the automation is created for to map them to the fields of the connected record type. 
      * **Transfer to**: Select fields from the newly created record that will populate with information from the record you are running the automation from. 
1. (Optional and conditional) If you selected to create a record, click **Add fields** to map additional lookup fields from one record to another.
1. (Optional and conditional) If you don't have a connection field for a Workfront object type, click the **Create a connection field** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a field.

   The new field is automatically created and named **Connected < Workfront object name >**. For example, when a portfolio connected field is created for the record, it is named "Connected portfolio." 

1. Click **Save** in the upper-right corner of the automation details page. 

   The automation displays on the list of automations, and is available to use in records.
1. (Optional) To edit, disable, or delete an automation, do the following:

   1. From the list of automations, hover over the name of a saved automation, then click the **More** menu ![More menu](assets/more-menu.png).

   1. Click **Edit** to update information about and configure fields on the automation.
   1. Click **Disable** to remove the automation from the table view and prevent users from using it to create records or objects. To make it available again, click the **More** menu ![More menu](assets/more-menu.png) again, then click **Activate**.
   1. Click **Delete** to delete the automation. A deleted automation cannot be recovered. Records that have been created using the automation remain connected to the record originally selected.  

## Use a Workfront Planning automation to create an object or a record

1. In Workfront Planning, open the record type page that contains the records you want to use to create Workfront objects or Planning records. 
1. Open the table view. 
1. Select one or more records.
   
   A blue bar displays at the bottom of the table with additional buttons, including automation buttons. 
1. Click the automation button near the lower-right corner of the screen. 

   ![Automation button](assets/automation-custom-button.png)

   A confirmation message displays at the bottom of the screen, if the automation successfully created an object or a record. 

   The new object displays in the connected field you indicated in the setup of the automation button. You might need to refresh your page before viewing the new object. 

   >[!NOTE]
   >
   >We recommend checking that the object was created and connected as expected.

1. (Optional) Click the new object in the connected field. The object page opens and you can make additional changes to the new object. 

-->

