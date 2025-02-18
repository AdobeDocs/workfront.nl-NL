---
title: Workfront-objecten maken van Workfront-planning
description: U kunt Workfront-objecttypen maken terwijl u deze verbindt vanuit andere records in Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 597d8db034269e673dbe46e8c0f4934bf9509e2f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Workfront-objecten maken van Workfront Planning <!--as you connect them to records-->

<!-- update the title (and all the links to this article) at preview, to be this: Create Workfront objects from Workfront Planning as you connect them to records-->
<!-- remove preview and production at release time-->

<span class="preview"> de informatie die op deze pagina wordt benadrukt verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

<!--
You can create Adobe Workfront objects from Workfront Planning in the following ways: 

* As you try to connect Workfront objects from Planning records

    This article describes how to create Workfront objects from Workfront Planning as you try to connect them from Planning records. 
* <span class="preview">When you use automations from a record's page.</span> 

    For information about creating Workfront objects using automations, see [Create objects using Adobe Workfront Planning record automations](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md). 
-->

U kunt de volgende typen Workfront-objecten maken vanuit Workfront Planning wanneer u een Workfront Planning-record verbindt met de volgende Workfront-objecttypen:

* Projecten
* Portfolio&#39;s
  <!--* <span class="preview">Programs</span>-->

>[!IMPORTANT]
>
>* U kunt alleen projecten en portfolio&#39;s maken in Workfront wanneer u deze via een record verbindt.
>
>* U kunt geen programma&#39;s, groepen, of bedrijven tot stand brengen wanneer het verbinden hen van een verslag in de Planning van Workfront.
>

<!--replace the IMPORTANT above with this when we release programs: 

>[!IMPORTANT]
>
>* You can create only projects, portfolios, and <span class="preview">programs</span> in Workfront when connecting them from a record. 
>
>* You cannot create groups or companies when connecting them from a record in Workfront Planning. 
>
-->

U kunt projecten en portefeuilles <!--<span class="preview"> and programs </span>--> van een verbindingsgebied op de volgende gebieden van de Planning van Workfront verbinden:

* De tabelweergave van een recordtype
* De detailpagina of het voorvertoningsvak van een record

Voor informatie over het verbinden van verslagen van de Planning met de voorwerpen van Workfront, zie [ verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).

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
   <p>Bewerk de toegang in Workfront voor de objecttypen die u wilt maken (projecten en portfolio's) terwijl u de records met deze eigenschappen verbindt. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td> <p>Rechten beheren in de werkruimte waaraan u records wilt toevoegen. </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
   <p>Rechten voor Workfront-objecten (portfolio's) beheren om onderliggende objecten (projecten) toe te voegen.</p>
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

## Vereisten voor het maken van Workfront-objecten wanneer deze worden verbonden met records uit Workfront Planning

U moet het volgende hebben alvorens u nieuwe projecten of portefeuilles kunt toevoegen door hen van bestaande verslagen te verbinden:

* Recordtypen die zijn verbonden met Workfront-projecten of -portfolio&#39;s <!--or <span class="preview">programs</span>--> . Voor informatie, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).
* Records. Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/create-records.md) creëren.
* De correcte toegang en de toestemmingen in de Planning van Workfront en Workfront, zoals die in de sectie [ vereisten van de Toegang ](#access-requirements) in dit artikel worden beschreven.

## Projecten maken terwijl u ze verbindt met records van Workfront Planning

Om projecten tot stand te brengen aangezien u hen van andere verslagen verbindt:

1. Ga naar de detailspagina van een verslag of naar de lijst van het verslagtype en begin de verslagen van de Planning van Workfront met de projecten van Workfront aan te sluiten, zoals die in artikel [ worden beschreven verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).

1. (Voorwaardelijk) <!--<span class="preview">Click **Add project**</span> Or Start typing the name of a project, then click **Add project** if you cannot find it.--> als u geen project kunt vinden wanneer het proberen om het van het verbonden verslaggebied van een ander verslag toe te voegen, voeg een naam toe, dan klik **project** toevoegen. De Add knoop wordt gevolgd door de projectnaam u typte.

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction above out and say "Click Add to add a new project"; take this out too: "The Add button is followed by the project name you typed."-->

   ![ voeg project toe wanneer het verbinden van het van een verbindingsgebied ](assets/add-project-when-connecting-it-from-connection-field.png)

   <span class="preview"> **creeer project** doos opent.</span>

1. <span class="preview"> (Facultatief) werk de **naam van het Project** bij. Standaard krijgt het project de naam van wat u als zoekopdracht hebt toegevoegd wanneer u het project verbindt vanuit de record. </span>
1. <span class="preview"> (Facultatief) selecteer a **malplaatje van het Project**. Als u geen sjabloon selecteert, maakt Workfront een leeg project zonder taken. </span>
1. <span class="preview"> klik **creeer**. </span>
1. <span class="preview"> (Voorwaardelijk) Als u selecteerde om een project van een malplaatje tot stand te brengen, volg de stappen in het artikel [ een project gebruikend een malplaatje ](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) artikel om het project te beëindigen toevoegend.</span>

   Het nieuwe project wordt gecreeerd en aan het verbonden gebied van het geselecteerde verslag toegevoegd.

1. (Optioneel) Klik op de naam van het nieuwe project in Workfront Planning om de projectpagina in Workfront te openen en aanvullende updates voor het project uit te voeren.

## Portefeuilles tot stand brengen aangezien u hen met verslagen van de Planning van Workfront verbindt

Om portefeuilles tot stand te brengen aangezien u hen van de verslagen van de Planning verbindt:

1. Ga naar de detailspagina van een verslag of naar de lijst van het verslagtype en begin de verslagen van de Planning van Workfront met de portefeuilles van Workfront aan te sluiten, zoals die in het artikel [ worden beschreven verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click Add to add a new portfolio"; take this out too: "The Add button is followed by the portfolio name you typed."-->

1. (Voorwaardelijk) <!--<span class="preview">Click **Add portfolio**</span> Or Start typing the name of a portfolio, then click **Add portfolio** if you cannot find it.--> als u geen portefeuille kunt vinden wanneer het proberen om het van het verbonden verslaggebied van een ander verslag toe te voegen, voeg een naam toe, dan klik **portefeuille** toevoegen. De knop Toevoegen wordt ook gevolgd door de naam van het portfolio die u hebt getypt.

   ![ voeg portefeuille toe wanneer het verbinden van het van een verbindingsgebied ](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   Het portfolio wordt gemaakt en toegevoegd aan het verbindingsveld van de record die u hebt geselecteerd.

1. (Optioneel) Klik op de naam van het nieuwe portfolio van Workfront Planning om de pagina van het portfolio te openen in Workfront en aanvullende updates voor het portfolio uit te voeren.

<!--

<div class="preview">

## Create programs as you connect them with records from Workfront Planning

To create programs as you are connecting them from Planning records: 

1. Go to a record's details page or to the record type's table and start connecting Workfront Planning records with Workfront portfolios, as described in the article [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    ******** at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click Add to add a new program"; take this out too: "The Add button is followed by the program name you typed." ***********
    
1. Click **Add program** 

    Or 
    
    Start typing the name of a program, then click **Add program** if you cannot find it. The Add button is followed by the program name you typed. 

    ![Add Workfront program when connecting it from connection field](assets/add-wf-program-when-connecting-it-from-connection-field.png)

    The **Create program** box opens.

1. Update the **Program name**. This is a required field.
1. Choose a **Portfolio** from the drop-down, or start typing the name of a portfolio, then select it when it displays in the list. This is a required field. 
1. Click **Create**.

    The program is created and added to the connection field of the record you selected. 

1. (Optional) Click the name of the new program from Workfront Planning to open the program's page in Workfront and make additional updates to it. 

</div>

-->