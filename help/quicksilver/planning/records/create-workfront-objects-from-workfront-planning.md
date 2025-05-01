---
title: Workfront-objecten maken van Workfront-planning
description: U kunt Workfront-objecttypen maken terwijl u deze verbindt vanuit andere records in Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '1102'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Workfront-objecten maken vanuit Workfront Planning wanneer u deze verbindt met records

<!-- update the title (and all the links to this article) at preview, to be this: Create Workfront objects from Workfront Planning as you connect them to records-->
<!-- remove preview and production at release time-->

<span class="preview"> de informatie die op deze pagina wordt benadrukt verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

U kunt op de volgende manieren Adobe Workfront-objecten maken via Workfront Planning:

* Als u Workfront-objecten verbindt met planningsrecords

  In dit artikel wordt beschreven hoe u Workfront-objecten kunt maken via Workfront Planning terwijl u deze verbindt vanuit planningsrecords.
* Wanneer u automatisering vanaf de pagina van een record gebruikt.

  Voor informatie over het creëren van de voorwerpen van Workfront die automatiseringen gebruiken, zie [ voorwerpen creëren gebruikend Adobe Workfront de verslagautomatiseringen van de Planning van ](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

U kunt de volgende typen Workfront-objecten maken vanuit Workfront Planning wanneer u een Workfront Planning-record verbindt met de volgende Workfront-objecttypen:

* Projecten
* Portfolio&#39;s
* Programma&#39;s

>[!IMPORTANT]
>
>* U kunt alleen projecten, portfolio&#39;s en programma&#39;s maken in Workfront wanneer u deze via een record verbindt.
>
>* U kunt geen groepen of bedrijven maken wanneer u deze verbindt vanuit een record in Workfront Planning.
>

U kunt projecten, portefeuilles, en programma&#39;s van een verbindingsgebied op de volgende gebieden van de Planning van Workfront verbinden:

* De tabelweergave van een recordtype
* De pagina Details of het voorvertoningsvak van een record
* Het tabblad Verbindingen van een record

Voor informatie over het verbinden van verslagen van de Planning met de voorwerpen van Workfront, zie [ verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.

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
   <p>Bewerk de toegang in Workfront voor de objecttypen die u wilt maken (projecten, programma's en portfolio's) terwijl u de records met deze eigenschappen verbindt. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td> <p>Beheer toestemmingen aan de werkruimte <span class="preview"> en verslagtype </span> waar u verslagen wilt toevoegen. </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
   <p>Rechten voor Workfront-objecten (portfolio's) beheren om onderliggende objecten (projecten) toe te voegen.</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>In het milieu van de Productie, moeten alle gebruikers met inbegrip van de Beheerders van het Systeem aan een lay-outmalplaatje worden toegewezen dat Planning omvat.</p>
<p><span class="preview">In het milieu van de Voorproef, hebben de Standaardgebruikers en de Beheerders van het Systeem Planning die door gebrek wordt toegelaten.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten voor het maken van Workfront-objecten wanneer deze worden verbonden met records uit Workfront Planning

U moet het volgende hebben alvorens u nieuwe projecten of portefeuilles kunt toevoegen door hen van bestaande verslagen te verbinden:

* Recordtypen die zijn verbonden met Workfront-projecten, -portfolio&#39;s of -programma&#39;s. Voor informatie, zie [ verbind verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).
* Records. Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/create-records.md) creëren.
* De correcte toegang en de toestemmingen in de Planning van Workfront en Workfront, zoals die in de sectie [ vereisten van de Toegang ](#access-requirements) in dit artikel worden beschreven.

## Projecten maken terwijl u ze verbindt met records van Workfront Planning

Om projecten tot stand te brengen aangezien u hen van andere verslagen verbindt:

1. Ga naar de detailspagina van een verslag of naar de lijst van het verslagtype en begin de verslagen van de Planning van Workfront met de projecten van Workfront aan te sluiten, zoals die in artikel [ worden beschreven verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).

1. (Voorwaardelijk) klik **toevoegen project**
of
Begin de naam van een project te typen, dan klik **voegt project** toe als u het niet kunt vinden. De Add knoop wordt gevolgd door de projectnaam u typte.

   ![ voeg project toe wanneer het verbinden van het van een verbindingsgebied ](assets/add-project-when-connecting-it-from-connection-field.png)

   **creeer project** doos opent.

1. (Facultatief) werk de **naam van het Project** bij. Standaard krijgt het project de naam van wat u als zoekopdracht hebt toegevoegd wanneer u het project verbindt vanuit de record.
1. (Facultatief) selecteer a **malplaatje van het Project**. Als u geen sjabloon selecteert, maakt Workfront een leeg project zonder taken.
1. Klik **creëren**.
1. (Voorwaardelijk) als u selecteerde om een project van een malplaatje tot stand te brengen, volg de stappen in het artikel [ een project tot stand brengen gebruikend een malplaatje ](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) artikel om het project te beëindigen toevoegend.

   Het nieuwe project wordt gecreeerd en aan het verbonden gebied van het geselecteerde verslag toegevoegd.

1. (Optioneel) Klik op de naam van het nieuwe project in Workfront Planning om de projectpagina in Workfront te openen en aanvullende updates voor het project uit te voeren.

## Portefeuilles tot stand brengen aangezien u hen met verslagen van de Planning van Workfront verbindt

Om portefeuilles tot stand te brengen aangezien u hen van de verslagen van de Planning verbindt:

1. Ga naar de detailspagina van een verslag of naar de lijst van het verslagtype en begin de verslagen van de Planning van Workfront met de portefeuilles van Workfront aan te sluiten, zoals die in het artikel [ worden beschreven verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).

1. (Voorwaardelijk) klik **toevoegen portefeuille**

   of

   Begin de naam van een portefeuille te typen, dan klik **toevoegen portefeuille** als u het niet kunt vinden. De knop Toevoegen wordt gevolgd door de naam van het portfolio die u hebt opgegeven.

   ![ voeg portefeuille toe wanneer het verbinden van het van een verbindingsgebied ](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   Het portfolio wordt gemaakt en toegevoegd aan het verbindingsveld van de record die u hebt geselecteerd.

1. (Optioneel) Klik op de naam van het nieuwe portfolio van Workfront Planning om de pagina van het portfolio te openen in Workfront en aanvullende updates voor het portfolio uit te voeren.

## Programma&#39;s maken terwijl u deze verbindt met records van Workfront Planning

Om programma&#39;s tot stand te brengen aangezien u hen van de verslagen van de Planning verbindt:

1. Ga naar de detailspagina van een verslag of naar de lijst van het verslagtype en begin de verslagen van de Planning van Workfront met de portefeuilles van Workfront aan te sluiten, zoals die in het artikel [ worden beschreven verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).

1. Klik **toevoegen programma**

   of

   Begin de naam van een programma te typen, dan klik **programma** toevoegen als u het niet kunt vinden. De Add knoop wordt gevolgd door de programmanaam u typt.

   ![ voeg het programma van Workfront toe wanneer het verbinden van het verbindingsgebied ](assets/add-wf-program-when-connecting-it-from-connection-field.png)

   Het **Create programma** vakje opent.

1. Werk de **naam van het Programma** bij. Dit is een verplicht veld.
1. Kies a **Portfolio** van drop-down, of begin de naam van een portefeuille te typen, dan het te selecteren wanneer het in de lijst toont. Dit is een verplicht veld.
1. Klik **creëren**.

   Het programma wordt gemaakt en toegevoegd aan het verbindingsveld van de geselecteerde record.

1. (Optioneel) Klik op de naam van het nieuwe programma in Workfront Planning om de pagina van het programma in Workfront te openen en aanvullende updates voor het programma uit te voeren.

