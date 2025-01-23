---
title: Workfront-objecten maken van Workfront-planning
description: U kunt Workfront-objecttypen maken terwijl u deze verbindt vanuit andere records in Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 9db8ea3f26dd7e8b4c8aa52fb9902832db7a6a5c
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Workfront-objecten maken van Workfront Planning

<span class="preview"> de informatie die op deze pagina wordt benadrukt verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

U kunt de volgende typen Workfront-objecten maken via Workfront Planning:

* Projecten
* Portfolio&#39;s

U kunt Workfront-projecten en -portfolio&#39;s maken via Workfront Planning wanneer u een Workfront-planningsrecord koppelt aan een project of portfolio.

>[!IMPORTANT]
>
>* U kunt alleen projecten en portfolio&#39;s maken in Workfront wanneer u deze via een record verbindt.
>
>* U kunt geen programma&#39;s, groepen, of bedrijven tot stand brengen wanneer het verbinden hen van een verslag in de Planning van Workfront.
>
<!--* You cannot create a project from a template when when you create projects by connecting them from a record. You must manually add tasks and project information or a template to the new project after you add it to the record.-->

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
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden genegeerd om tot alle mogelijkheden van de Planning van Workfront te kunnen toegang hebben.</p> 
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

* Recordtypen die verbonden zijn met Workfront-projecten of -portfolio&#39;s. Voor informatie, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).
* Records. Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/create-records.md) creëren.
* De correcte toegang en de toestemmingen in de Planning van Workfront en Workfront, zoals die in de sectie [ vereisten van de Toegang ](#access-requirements) in dit artikel worden beschreven.

## Projecten maken wanneer deze worden verbonden met records van Workfront Planning

Om projecten tot stand te brengen aangezien u hen van andere verslagen verbindt:

1. Ga naar de detailspagina van een verslag of naar de lijst van het verslagtype en begin de verslagen van de Planning van Workfront met de projecten van Workfront aan te sluiten, zoals die in artikel [ worden beschreven verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).

   U kunt projecten van een verbindingsgebied op de volgende gebieden van de Planning van Workfront verbinden:

   * De tabelweergave van een recordtype
   * De detailpagina of het voorvertoningsvak van een record

1. (Voorwaardelijk) als u geen project kunt vinden wanneer het proberen om het van het verbonden verslaggebied van een ander verslag toe te voegen, voeg een naam toe, dan klik **+ toevoegen**. De knop **+ Toevoegen** wordt gevolgd door de naam van het objecttype waarmee u verbinding maakt. Bijvoorbeeld, &quot;voeg project&quot;toe, wanneer het toevoegen van een nieuw project aan een bestaande campagne. De Add knoop wordt ook gevolgd door de projectnaam u typte.

   ![](assets/add-project-when-connecting-it-from-connection-field.png)

   <span class="preview"> **creeer project** doos opent.</span>

1. <span class="preview"> (Facultatief) werk de **naam van het Project** bij. Standaard krijgt het project de naam van wat u als zoekopdracht hebt toegevoegd wanneer u het project verbindt vanuit de record. </span>
1. <span class="preview"> (Facultatief) selecteer a **malplaatje van het Project**. Als u geen sjabloon selecteert, maakt Workfront een leeg project zonder taken. </span>
1. <span class="preview"> klik **creeer**. </span>
1. <span class="preview"> (Voorwaardelijk) Als u selecteerde om een project van een malplaatje tot stand te brengen, volg de stappen in het artikel [ een project gebruikend een malplaatje ](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) artikel om het project te beëindigen toevoegend.</span>

   Het nieuwe project wordt gecreeerd en aan het verbonden gebied van het geselecteerde verslag toegevoegd.

1. (Optioneel) Klik op de naam van het nieuwe project in Workfront Planning om de projectpagina in Workfront te openen en aanvullende updates voor het project uit te voeren.

## Portefeuilles creëren wanneer het verbinden hen met verslagen van de Planning van Workfront

Als u portfolio&#39;s wilt maken terwijl u deze verbindt vanuit andere records:

1. Ga naar de detailspagina van een verslag of naar de lijst van het verslagtype en begin de verslagen van de Planning van Workfront met de portefeuilles van Workfront aan te sluiten, zoals die in het artikel [ worden beschreven verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).

   U kunt portefeuilles van een verbindingsgebied in de volgende gebieden van de Planning van Workfront verbinden:

   * De tabelweergave van een recordtype
   * De detailpagina of het voorvertoningsvak van een record

1. (Voorwaardelijk) als u geen portefeuille kunt vinden wanneer het proberen om het van het verbonden verslaggebied van een ander verslag toe te voegen, voeg een naam toe, dan klik **+ toevoegen**. De knop **+ Toevoegen** wordt gevolgd door de naam van het objecttype waarmee u verbinding maakt. Bijvoorbeeld, &quot;voeg portefeuille&quot;toe, wanneer het toevoegen van een nieuw portefeuille aan een bestaande campagne. De knop Toevoegen wordt ook gevolgd door de naam van het portfolio die u hebt getypt.

   ![](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   Het portfolio wordt gemaakt en toegevoegd aan het verbindingsveld van de record die u hebt geselecteerd.

1. (Optioneel) Klik op de naam van het nieuwe portfolio van Workfront Planning om de pagina van het portfolio te openen in Workfront en aanvullende updates voor het portfolio uit te voeren.
