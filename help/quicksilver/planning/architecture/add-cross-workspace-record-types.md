---
title: Recordtypen tussen werkruimten toevoegen
description: Recordtypen zijn de objecttypen voor Adobe Workfront Planning. In de Planning van Workfront, kunt u een bestaand verslagtype van een andere werkruimte invoeren.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: b6ced451cdd6b38b5661a076b2311a34c2c70432
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Recordtypen voor meerdere werkruimten toevoegen

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

Als werkruimtebeheerder kunt u een bestaand recordtype importeren of toevoegen aan een andere werkruimte.

U moet een recordtype eerst als gecentraliseerd aanwijzen voordat werkruimtenmanagers het in andere werkruimten kunnen importeren.

U kunt een recordtype instellen als gecentraliseerd wanneer u het maakt of bewerkt terwijl u de instellingen voor de werkruimte van het recordtype definieert.

Voor informatie, zie [ mogelijkheden van de dwars-werkruimte voor verslagtypes ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.  

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
   <td><p> Standaard</p>
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
   <td>   <p>Rechten beheren in een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr>  
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Overzicht van gecentraliseerde recordtypen

Overwegingen bij het toevoegen van bestaande recordtypen vanuit een andere werkruimte

* Als er geen recordtypen zijn geconfigureerd om aan een andere werkruimte te worden toegevoegd, wordt de optie om deze uit een andere werkruimte te importeren niet weergegeven wanneer u een recordtype maakt. <!--add this a tip in the steps below, and/ or add a Conditional step that this is possible only when these record types are first enabled-->
* Nadat u het recordtype vanuit een andere werkruimte hebt toegevoegd, wordt de volgende informatie ook toegevoegd van het bestaande recordtype:

   * Velden
   * Records
   * Verbindingen opnemen

* U kunt het recordtype, inclusief de bijbehorende velden, alleen in de oorspronkelijke werkruimte bewerken. U kunt het bestand niet bewerken vanuit de werkruimten waar het is toegevoegd.

## Een recordtype maken op basis van een bestaand recordtype

1. Begin creërend een verslagtype, zoals die in het artikel [ wordt beschreven creeer verslagtypes ](/help/quicksilver/planning/architecture/create-record-types.md), dan klik **voegt bestaand** toe. <!--check this - the option might have been renamed in the UI-->

   ![ Modal om verslagtype met optie toe te voegen om van een andere werkruimte in te voeren ](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. Klik **verdergaan**.
1. In **kies verslagtype** doos, klik de kaart voor het verslagtype dat u van een bestaande werkruimte wilt toevoegen, dan **toevoegen** klikken.

   Het recordtype wordt toegevoegd aan de werkruimte die u hebt geselecteerd en de volgende dingen gebeuren:

   * Het **dwars-werkruimte verslagtype** pictogram ![ pictogram van de dwars-werkruimteverbinding ](assets/global-icon.png) wordt toegevoegd aan de kaart van het ingevoerde verslagtype.
   * Het read-only **Workspace** gebied wordt toegevoegd aan het ingevoerde verslagtype. In het veld wordt weergegeven in welke werkruimte elke record is gemaakt.

     >[!NOTE]
     >
     >* U kunt het geïmporteerde recordtype of de bijbehorende velden niet bewerken. U kunt het recordtype en de bijbehorende velden vanuit de oorspronkelijke werkruimte bewerken.

1. (Facultatief) klik op **Meer** menu ![ Meer menu ](assets/more-menu.png) in de ingevoerde kaart van het verslagtype, of rechts van de naam van het verslagtype op zijn pagina, dan klik **Schrapping**.
1. (Voorwaardelijk) Type **schrapt** op het verstrekte gebied, dan klik **permanent schrapt**.

   Hierdoor wordt het geïmporteerde recordtype verwijderd uit de geselecteerde werkruimte. Het oorspronkelijke recordtype en de bijbehorende velden blijven in de oorspronkelijke werkruimte staan.

   <!--**************************ASK LILIT ON THIS ONE, NOT SURE IF THIS IS TRUE: Any records added in the current workspace are saved in the original workspace.**********-->



