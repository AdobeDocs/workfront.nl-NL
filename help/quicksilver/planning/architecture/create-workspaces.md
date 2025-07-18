---
title: Werkruimten maken
description: Een werkruimte is een inzameling van verslagtypes die door een team worden gebruikt en vertegenwoordigt de het werklevenscyclus van het team. U kunt werkruimten volledig aanpassen in Adobe Workfront Planning. Recordtypen worden ingedeeld in secties in een werkruimte.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Werkruimten maken

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

In de Planning van Adobe Workfront, zijn de werkruimten gecentraliseerde plaatsen voor teams om het werk te plannen.

Een werkruimte is een inzameling van verslagtypes die door een team worden gebruikt en vertegenwoordigt de het werklevenscyclus van het team. U kunt werkruimten volledig aanpassen in Adobe Workfront Planning.

Voor algemene informatie over werkruimten, zie [ Overzicht van Werkruimten ](/help/quicksilver/planning/architecture/workspaces-overview.md).

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
<p>Het geval van Workfront van uw organisatie moet aan de Verenigde Ervaring van Adobe worden genegeerd om tot de Planning van Workfront te kunnen toegang hebben.</p> 
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td><p> Standaard </p>
   <p>Workfront Planning is niet beschikbaar voor oudere Workfront-licenties</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td> 
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>U ontvangt beheermachtigingen voor de werkruimten die u maakt. </p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een werkruimte maken

U kunt een werkruimte maken en er recordtypen aan toevoegen om uw objecten te ordenen in Workfront Planning. Voor meer informatie over het uitgeven van een werkruimte, zie [ werkruimten ](/help/quicksilver/planning/architecture/edit-workspaces.md) uitgeven.

{{step1-to-planning}}

1. Klik **creëren werkruimte**

   Het dialoogvenster Maken wordt weergegeven. U kunt een werkruimte helemaal opnieuw maken of maken met een van de beschikbare sjablonen.

1. (Facultatief en voorwaardelijk) klik **Voorproef** binnen om het even welke volgende vooraf bepaalde werkruimtesjablonen:

   * Basis: Marketing Management
   * Geavanceerd: marketingbeheer
   * Enterprise: Marketing Management
   * Verkoopbeheer
   * Productbeheer

   Het voorbeeldvak voor de sjabloon wordt geopend.

   Er is een indicatie van welke operationele recordtypen, taxonomieën en hoeveel velden aan elke sjabloon zijn gekoppeld.

   ![ Previewing een werkruimtemalplaatje ](assets/previewing-a-workspace-template.png)

   Voor informatie over de malplaatjes van de werkruimte van de Planning van Workfront, zie [ Lijst van werkruimtesjablonen ](/help/quicksilver/planning/architecture/workspace-templates.md).

1. Van het vakje van de malplaatjevoorproef, klik **malplaatje van het Gebruik** beginnen de werkruimte van het geselecteerde malplaatje te creëren

   of

   Klik **terug**, dan klik **Nieuwe werkruimte** om een werkruimte van kras tot stand te brengen.

   Er wordt een werkruimte gemaakt voor de volgende typen werkruimten:

   * Een lege werkruimte genoemd **Naamloze Workspace** waar u recordtypes kunt beginnen manueel toe te voegen, wanneer u een werkruimte van kras creeert.
   * Een werkruimte die wordt genoemd naar de geselecteerde sjabloon en die is gevuld met typen voorbeeldrecords. U kunt de recordtypen en de werkruimte verder aanpassen.

   Voor de beheerders van Workfront, de nieuwe werkruimtevertoningen op de **Werkruimten ik op** tabel ben.

   Voor alle andere gebruikers die werkruimten kunnen tot stand brengen, toont de nieuwe werkruimte in het **1&rbrace; gebied van de Werkruimten &lbrace;.**

1. Klik binnen de naam van de werkruimte in de koptekst van de nieuwe werkruimte om de naam ervan te wijzigen en druk vervolgens op Enter.

1. (Facultatief en voorwaardelijk) als u de werkruimte van een malplaatje creeerde, klik binnen de naam van de **Operationele Types van Verslag** of **taxonomieën** secties

   of

   Beweeg de naam van een sectie, dan klik **Meer** menu ![ Meer menu ](assets/more-menu.png), dan klik **anders noemen** om de sectie anders te noemen.

   >[!TIP]
   >
   >U kunt de naam van elke sectie vanuit elke werkruimte wijzigen, zelfs als u de sectie niet hebt gemaakt.

   Voor meer informatie over het uitgeven van werkruimten, met inbegrip van het uitgeven van werkruimtesecties, zie [ werkruimten ](/help/quicksilver/planning/architecture/edit-workspaces.md) uitgeven.

1. (Facultatief) klik **recordtype** toevoegen om verslagtypes aan de werkruimte in om het even welke sectie toe te voegen.

   Voor informatie, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

   Voor meer informatie over het uitgeven van en het schrappen van verslagtypes in een werkruimte, zie [ werkruimten ](/help/quicksilver/planning/architecture/edit-workspaces.md) uitgeven.


