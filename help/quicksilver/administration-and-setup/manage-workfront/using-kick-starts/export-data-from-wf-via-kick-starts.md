---
user-type: administrator
product-area: system-administration
keywords: kickstart,trap-start,kickstart,trap-start
navigation-topic: use-kick-starts
title: Gegevens exporteren uit Workfront via Kick-start
description: Als Adobe Workfront-beheerder kunt u de Kick-Starts-gegevensexportfunctie gebruiken om gegevens uit Workfront te exporteren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7f56b63e-a674-43e4-bef6-d276898e2074
source-git-commit: 156341072c291b5c03432da399a509d9772b73ea
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 0%

---

# Gegevens exporteren uit Workfront via Kick-start

<!-- Audited: 2/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Als Adobe Workfront-beheerder kunt u de Kick-Starts-gegevensexportfunctie gebruiken om gegevens uit Workfront te exporteren. U kunt het in andere toepassingen gebruiken nadat u het uitvoert.

Het exporteren van gegevens via Kick-Starts is ook handig om te begrijpen welke velden aan elk object zijn gekoppeld, hoe deze velden worden gecodeerd en hoe de waarden van deze velden in de database worden opgemaakt.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>Systeembeheerder</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voordelen en nadelen van het gebruik van de startfunctie voor het exporteren van gegevens

Er zijn twee manieren om gegevens te exporteren in Workfront:

* Gegevens uit een rapport of lijst exporteren

  Voor meer informatie over het uitvoeren van gegevens van een rapport of een lijst, zie [ gegevens van de Uitvoer ](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* Gegevens exporteren via een startprocedure

In de volgende tabel worden de voor- en nadelen van elke methode weergegeven:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>  </th> 
   <th> <p>De geëxporteerde gegevens bevatten object- en veldwaarden</p> </th> 
   <th> <p>Mogelijkheid om gegevens over meerdere objecttypen tegelijk te exporteren</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong> het Uitvoeren Gegevens van een Mening van de Lijst </strong> </p> <p>Voor meer informatie over het uitvoeren van gegevens van een lijst, zie <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref"> Gegevens van de Uitvoer </a></p> </td> 
   <td> <p>Ja</p> <p>Zowel eigen Workfront-velden als aangepaste velden die aan de objecten zijn gekoppeld, worden geëxporteerd.</p> </td> 
   <td> <p>Nee</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> het Uitvoeren Gegevens via Kick-Begint </strong> </p> </td> 
   <td> <p>Ja (beperkt)</p> <p>De meeste eigen Workfront-velden die aan objecten zijn gekoppeld, worden geëxporteerd, maar sommige niet. U kunt bijvoorbeeld de velden Planning, Projecteigenaar of Projectsponsor niet exporteren via het exporteren van de start van een project.</p> <p>In een project waaraan een aangepast formulier is gekoppeld, worden de gegevens die zijn ingevoerd in de velden op het formulier, niet geëxporteerd.</p> <p>Maar u kunt een aangepast formulier exporteren. In het resulterende bestand worden de velden weergegeven die in het formulier zijn geconfigureerd, zoals tekstvakken en keuzerondjes.</p> </td> 
   <td> <p>Ja</p> <p>Met Kick-Starts kunt u Workfront-gegevens exporteren, zodat u gegevens die betrekking hebben op meerdere objecttypen in één exportbewerking kunt exporteren. U kunt bijvoorbeeld taken, problemen en projecten in één exportbewerking opnemen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Exportlimieten

De volgende beperkingen gelden voor het exporteren van gegevens via de functie voor het starten van een computer (gegevens worden geëxporteerd in Excel-bestandsindeling):

* **50.000 rijen:** het aantal rijen toegestaan in het dossier.
* **65.530 hyperlinks:** dit is een grens die door Excel op documenten wordt opgelegd die meer dan 65.530 hyperlinks bevatten. Deze documenten kunnen niet worden geopend nadat ze zijn geëxporteerd. Een Excel-document kan slechts 200 rijen gegevens bevatten, maar als het document meer dan 65.530 koppelingen bevat, wordt het document niet geopend.

## Gegevens exporteren via de startprocedure

{{step-1-to-setup}}

1. Klik **Systeem** > **Kick-Begint,** dan klik **Gegevens van de Uitvoer.**

1. Selecteer het object dat u wilt exporteren. Door gebrek, worden de volgende voorwerpen getoond onder **wat te omvatten**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong> Voorwerp </strong> </p> </th> 
      <th> <p><strong> Uitgevoerde Bladen van het Dossier van Excel </strong> </p> </th> 
      <th> <p> <strong> het Formaat van de Uitvoer </strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>Dashboard</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>De Optie van de Parameter <br> van de Optie van de Parameter <br> Categorie van de Parameter <br> Categorie <br> van het Rapport <br> Poorttabs van het Poort <br> Dashboard <br> Voorkeur<br></p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Rapport</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">De Optie van de Parameter van de Optie van de Parameter <br> <br> Categorie van de Parameter <br> Categorie <br> Voorkeur van het Rapport <br><br></td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Goedkeuring</p> </td> 
      <td scope="col" valign="top"> <p>De Stap van de Stap van de Goedkeuring <br> Stap van de Goedkeuring <br> <br> Voorkeur van het Proces van de Goedkeuring<br></p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Aangepaste gegevens</p> </td> 
      <td scope="col" valign="top"> <p>De Optie van de Parameter <br> van de Optie van de Parameter van de 1} <br> Categorie van de Parameter <br> Voorkeur <br><br></p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Type uitgave</p> </td> 
      <td valign="top"> <p>Het Type van onkosten <br> Voorkeur</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Uurtype</p> </td> 
      <td valign="top"> <p>Het Type van uur <br> Voorkeur</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Team</p> </td> 
      <td valign="top"> De Voorkeur van het Team van het Lid van het team <br> <br> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Gebruiker</p> </td> 
      <td valign="top"> <p>Gebruiker <br> Voorkeur</p> </td> 
      <td valign="top"> <p> Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Als de **optie van het Dashboard** niet beschikbaar is, betekent het dat u geen dashboards in uw systeem hebt die worden gedeeld systeem-breed. U kunt privédashboards niet exporteren.

1. Klik **Meer Opties** om de volledige lijst van voorwerpen te zien.

   Alle objecten die hier worden vermeld, kunnen ook worden gebruikt om gegevens te importeren in Workfront.

   De enige uitzondering is het **voorwerp van de Niveaus van de Toegang**. Het gegevensblad van de Niveaus van de Toegang dat in de uitvoer inbegrepen is wordt verstrekt slechts voor verwijzingsdoeleinden. Hiermee kunt u een toegangsniveau aan een nieuwe gebruikersaccount toewijzen met een id.

   Voor meer informatie over het invoeren van gegevens in Workfront via schop-begin, zie [ Gegevens van de Invoer in Adobe Workfront gebruikend een Kick-Begin malplaatje ](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md). Hieronder volgt een lijst met alle objecten die kunnen worden geëxporteerd via het starten van een trap:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p>Object</p> </th> 
      <th> <p>Geëxporteerde bladen van het Excel-bestand</p> </th> 
      <th> <p>Exportindeling</p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top">Toegangsniveau</td> 
      <td scope="col" valign="top">De Voorkeur van het Niveau van de toegang <br></td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Toewijzing</td> 
      <td scope="col" valign="top">De Voorkeur van de toewijzing <br></td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Bedrijf</td> 
      <td scope="col" valign="top"> Bedrijfs <br> Voorkeur </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">E-mailsjabloon</td> 
      <td scope="col" valign="top"> E-mailMalplaatje <br> Voorkeur </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Kosten</td> 
      <td valign="top"> De onkosten <br> Voorkeur </td> 
      <td scope="col" valign="top"> Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Externe pagina</td> 
      <td valign="top"> Externe pagina <br> Voorkeur </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Filter</td> 
      <td valign="top"> Filter <br> Voorkeur </td> 
      <td valign="top">ZIP </td> 
     </tr> 
     <tr> 
      <td valign="top">Groep</td> 
      <td valign="top"> Groep <br> Voorkeur  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Groepering</td> 
      <td valign="top"> <br> Voorkeuren groeperen </td> 
      <td valign="top">ZIP</td> 
     </tr> 
     <tr> 
      <td valign="top">Uur</td> 
      <td valign="top"> Uur <br> Voorkeur </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Probleem</td> 
      <td valign="top"> Uitgave <br> Voorkeur </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Functie</td> 
      <td valign="top"> De rol van de baan <br> Voorkeur </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Mijlpad</td> 
      <td valign="top"> De Weg van de Mijlsteen <br> Voorkeur van de Weg van 0} Mijl<br> </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Opmerking</td> 
      <td valign="top"> Nota <br> Voorkeur </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Portfolio</td> 
      <td valign="top"> Portfolio <br> Voorkeur  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Project</td> 
      <td valign="top"> Het Project van de rij <br> <br> Verpletterend het Onderwerp van de Rij <br> <br> Voorkeur </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Bronschatting</td> 
      <td valign="top"> De Raming van het middel <br> Voorkeur </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Bronpool</td> 
      <td valign="top"> De Pool van het middel <br> Voorkeur </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Risico</td> 
      <td valign="top"> Voorkeuren voor risico <br>  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Type risico</td> 
      <td valign="top"> Het Type van risico <br> Voorkeur  </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Scorecard</td> 
      <td valign="top">De Optie van het Scorecard van de Vragen van het scorebord <br> Scorecard <br> Voorkeur<br> </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Taak</td> 
      <td valign="top"> Taak <br> Voorkeur </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Sjabloon</td> 
      <td valign="top"> Het Malplaatje van de rij <br> <br> Verpletterend het Onderwerp van de Rij <br> <br> Voorkeur </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top">Sjabloontoewijzing</td> 
      <td valign="top"> Sjabloontoewijzing <br> Voorkeuren </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Sjabloontaak</td> 
      <td valign="top"> De Taak van het malplaatje <br> Voorkeur </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Tijdschema</td> 
      <td valign="top"> De Voorkeur van het Profiel van de Tijdopnemer <br><br> </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top"> Weergave </td> 
      <td valign="top"> <br> Voorkeur van de mening  </td> 
      <td valign="top">ZIP</td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **Download.**

   Het geëxporteerde bestand met de startfunctie wordt als Excel-bestand of als een bestand met de startfunctie naar de computer gedownload. ZIP-bestand met meerdere Excel- en eigenschappenbestanden. Elk Excel-bestand is een verzameling bladen, waarin elk blad een veld vertegenwoordigt dat is gekoppeld aan het object dat u hebt geselecteerd. Er is a **Eigenschappen** blad verbonden aan elke uitvoer.

   De **opties van het Dashboard** en **Rapport** staan u toe om specifieke dashboards en rapporten te selecteren om in de download te omvatten. Voor dashboards, kunt u dashboards slechts uitvoeren die systeem-wijd worden gedeeld.

   U kunt matrixrapporten niet exporteren. Voor meer informatie over matrixrapporten, zie [ een matrixrapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md) creëren.

   Kick-Starts ondersteunt geen filters of groepen in de tekstmodus. Voor een geslaagde export moeten de rapportfilters en -groepen worden overgeschakeld op de standaardmodus.

   U kunt maximaal 100 dashboards en 100 rapporten selecteren in één export.

   ![ Kickstart de uitvoer ](assets/kickstart-export-spreadsheet-options.png)

   U kunt meerdere objecten tegelijk exporteren.

1. (Aanbevolen) Analyseer de geëxporteerde gegevens om ervoor te zorgen dat alle informatie die u verwacht te zien, is geëxporteerd.

   Voor grote exportbewerkingen werkt Workfront op de achtergrond om het Excel-bestand te maken. Er verschijnt dan een waarschuwingsbericht over de vertraging. Het startbestand wordt naar u gemaild wanneer het downloaden is voltooid.

