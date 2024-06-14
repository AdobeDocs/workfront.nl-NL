---
user-type: administrator
product-area: system-administration
keywords: kickstart,trap-start,kickstart,trap-start
navigation-topic: use-kick-starts
title: Gegevens exporteren uit Adobe Workfront via Kick-start
description: Als Adobe Workfront-beheerder kunt u de Kick-Starts-gegevensexportfunctie gebruiken om gegevens uit Workfront te exporteren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7f56b63e-a674-43e4-bef6-d276898e2074
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 0%

---

# Gegevens exporteren uit Adobe Workfront via Kick-start

<!-- Audited: 2/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Als Adobe Workfront-beheerder kunt u de Kick-Starts-gegevensexportfunctie gebruiken om gegevens uit Workfront te exporteren. U kunt het in andere toepassingen gebruiken nadat u het uitvoert.

Het exporteren van gegevens via Kick-Starts is ook handig om te begrijpen welke velden aan elk object zijn gekoppeld, hoe deze velden worden gecodeerd en hoe de waarden van deze velden in de database worden opgemaakt.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
   <p>Nieuw: Standaard</p>
   of
   <p>Huidig: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p></td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voordelen en nadelen van het gebruik van de startfunctie voor het exporteren van gegevens

Er zijn twee manieren om gegevens te exporteren in Workfront:

* Gegevens uit een rapport of lijst exporteren

  Voor meer informatie over het uitvoeren van gegevens uit een rapport of een lijst, zie [Gegevens exporteren](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

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
   <td> <p><strong>Gegevens exporteren uit een lijstweergave</strong> </p> <p>Zie voor meer informatie over het exporteren van gegevens uit een lijst <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Gegevens exporteren</a></p> </td> 
   <td> <p>Ja</p> <p>Zowel eigen Workfront-velden als aangepaste velden die aan de objecten zijn gekoppeld, worden geëxporteerd.</p> </td> 
   <td> <p>Nee</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Gegevens exporteren via Kick-start</strong> </p> </td> 
   <td> <p>Ja (beperkt)</p> <p>De meeste eigen Workfront-velden die aan objecten zijn gekoppeld, worden geëxporteerd, maar sommige niet. U kunt bijvoorbeeld de velden Planning, Projecteigenaar of Projectsponsor niet exporteren via het exporteren van de start van een project.</p> <p>In een project waaraan een aangepast formulier is gekoppeld, worden de gegevens die zijn ingevoerd in de velden op het formulier, niet geëxporteerd.</p> <p>Maar u kunt een aangepast formulier exporteren. In het resulterende bestand worden de velden weergegeven die in het formulier zijn geconfigureerd, zoals tekstvakken en keuzerondjes.</p> </td> 
   <td> <p>Ja</p> <p>Met Kick-Starts kunt u Workfront-gegevens exporteren, zodat u gegevens die betrekking hebben op meerdere objecttypen in één exportbewerking kunt exporteren. U kunt bijvoorbeeld taken, problemen en projecten in één exportbewerking opnemen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Exportlimieten

De volgende beperkingen gelden voor het exporteren van gegevens via de functie voor het starten van een computer (gegevens worden geëxporteerd in Excel-bestandsindeling):

* **50.000 rijen:** Het aantal rijen dat is toegestaan in het bestand.
* **65.530 hyperlinks:** Dit is een door Excel opgelegde limiet voor documenten die meer dan 65.530 hyperlinks bevatten. Deze documenten kunnen niet worden geopend nadat ze zijn geëxporteerd. Een Excel-document kan slechts 200 rijen gegevens bevatten, maar als het document meer dan 65.530 koppelingen bevat, wordt het document niet geopend.

## Gegevens exporteren via de startprocedure

{{step-1-to-setup}}

1. Klikken **Systeem** > **Kick-start,** klik vervolgens op **Gegevens exporteren.**

1. Selecteer het object dat u wilt exporteren. Standaard worden de volgende objecten onder **Wat moet u opnemen?**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Object</strong> </p> </th> 
      <th> <p><strong>Geëxporteerde bladen van het Excel-bestand</strong> </p> </th> 
      <th> <p> <strong>Exportindeling</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>Dashboard</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>Parameter<br>Parameteroptie<br>Parametergroep<br>Categorieparameter<br>Categorie<br>Rapport<br>Sectie tabblad Portal<br>Dashboard<br>Voorkeuren</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Rapport</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">Parameter<br>Parameteroptie<br>Parametergroep<br>Categorieparameter<br>Categorie<br>Rapport<br>Voorkeuren</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Goedkeuring</p> </td> 
      <td scope="col" valign="top"> <p>Stap fiatteur<br>Goedkeuringsstap<br>Goedkeuring<br>Goedkeuringsproces<br>Voorkeuren</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Aangepaste gegevens</p> </td> 
      <td scope="col" valign="top"> <p>Parameter<br>Parameteroptie<br>Parametergroep<br>Categorieparameter<br>Categorie<br>Voorkeuren</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Type uitgave</p> </td> 
      <td valign="top"> <p>Type uitgave<br>Voorkeuren</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Uurtype</p> </td> 
      <td valign="top"> <p>Uurtype<br>Voorkeuren</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Team</p> </td> 
      <td valign="top"> Teamlid<br>Team<br>Voorkeuren </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Gebruiker</p> </td> 
      <td valign="top"> <p>Gebruiker<br>Voorkeuren</p> </td> 
      <td valign="top"> <p> Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Meer opties** om de volledige lijst met objecten weer te geven.

   Alle objecten die hier worden vermeld, kunnen ook worden gebruikt om gegevens te importeren in Workfront.

   De enige uitzondering is de **Toegangsniveaus** object. Het gegevensblad van de Niveaus van de Toegang dat in de uitvoer inbegrepen is wordt verstrekt slechts voor verwijzingsdoeleinden. Hiermee kunt u een toegangsniveau aan een nieuwe gebruikersaccount toewijzen met een id.

   Ga voor meer informatie over het importeren van gegevens naar Workfront via het starten naar [Gegevens naar Adobe Workfront importeren met een Kick-startsjabloon](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md). Hieronder volgt een lijst met alle objecten die kunnen worden geëxporteerd via het starten van een trap:

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
      <td scope="col" valign="top">Toegangsniveau<br>Voorkeuren</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Toewijzing</td> 
      <td scope="col" valign="top">Toewijzing<br>Voorkeuren</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Bedrijf</td> 
      <td scope="col" valign="top"> Bedrijf<br>Voorkeuren </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">E-mailsjabloon</td> 
      <td scope="col" valign="top"> E-mailsjabloon<br>Voorkeuren </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Kosten</td> 
      <td valign="top"> Kosten<br>Voorkeuren </td> 
      <td scope="col" valign="top"> Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Externe pagina</td> 
      <td valign="top"> Externe pagina<br>Voorkeuren </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Filter</td> 
      <td valign="top"> Filter<br>Voorkeuren </td> 
      <td valign="top">ZIP </td> 
     </tr> 
     <tr> 
      <td valign="top">Groep</td> 
      <td valign="top"> Groep<br>Voorkeuren  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Groepering</td> 
      <td valign="top"> Groepering<br>Voorkeuren </td> 
      <td valign="top">ZIP</td> 
     </tr> 
     <tr> 
      <td valign="top">Uur</td> 
      <td valign="top"> Uur<br>Voorkeuren </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Probleem</td> 
      <td valign="top"> Probleem<br>Voorkeuren </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Functie</td> 
      <td valign="top"> Functie<br>Voorkeuren </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Mijlpad</td> 
      <td valign="top"> Mijlsteen<br>Mijlpad<br>Voorkeuren </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Opmerking</td> 
      <td valign="top"> Opmerking<br>Voorkeuren </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Portfolio</td> 
      <td valign="top"> Portfolio<br>Voorkeuren  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Project</td> 
      <td valign="top"> Wachtrij<br>Project<br>Routeringsregel<br>Onderwerp van wachtrij<br>Voorkeuren </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Bronschatting</td> 
      <td valign="top"> Bronschatting<br>Voorkeuren </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Bronpool</td> 
      <td valign="top"> Bronpool<br>Voorkeuren </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Risico</td> 
      <td valign="top"> Risico<br>Voorkeuren  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Type risico</td> 
      <td valign="top"> Type risico<br>Voorkeuren  </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Scorecard</td> 
      <td valign="top">Scorecard-vragen<br>Scorecard-optie<br>Scorecard<br>Voorkeuren </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Taak</td> 
      <td valign="top"> Taak<br>Voorkeuren </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Sjabloon</td> 
      <td valign="top"> Wachtrij<br>Sjabloon<br>Routeringsregel<br>Onderwerp van wachtrij<br>Voorkeuren </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top">Sjabloontoewijzing</td> 
      <td valign="top"> Sjabloontoewijzing<br>Voorkeuren </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Sjabloontaak</td> 
      <td valign="top"> Sjabloontaak<br>Voorkeuren </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Tijdschema</td> 
      <td valign="top"> Tijdbladprofiel<br>Tijdschema<br>Voorkeuren </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top"> Weergave </td> 
      <td valign="top"> Weergave<br>Voorkeuren  </td> 
      <td valign="top">ZIP</td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Downloaden.**

   Het geëxporteerde bestand met de startfunctie wordt als Excel-bestand of als een bestand met de startfunctie naar de computer gedownload. ZIP-bestand met meerdere Excel- en eigenschappenbestanden. Elk Excel-bestand is een verzameling bladen, waarin elk blad een veld vertegenwoordigt dat is gekoppeld aan het object dat u hebt geselecteerd. Er is een **Eigenschappen** blad dat aan elke export is gekoppeld.

   De **Dashboard** en **Rapport** Met opties kunt u specifieke dashboards en rapporten selecteren die u in de download wilt opnemen. U kunt alleen dashboards exporteren die op het hele systeem worden gedeeld.

   U kunt matrixrapporten niet exporteren. Voor meer informatie over matrixrapporten, zie [Een matrixrapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

   U kunt maximaal 100 dashboards en 100 rapporten selecteren in één exportbewerking.

   ![](assets/kickstart-export-350x381.png)

   U kunt meerdere objecten tegelijk exporteren.



1. (Aanbevolen) Analyseer de geëxporteerde gegevens om ervoor te zorgen dat alle informatie die u verwacht te zien, is geëxporteerd.

   Voor grote exportbewerkingen werkt Workfront op de achtergrond om het Excel-bestand te maken. Er verschijnt dan een waarschuwingsbericht over de vertraging. Het startbestand wordt naar u gemaild wanneer het downloaden is voltooid.

   ![](assets/large-kick-start-file-warning-350x65.png)
