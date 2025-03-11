---
title: Records verwijderen
description: U kunt records verwijderen die u of een andere gebruiker heeft gemaakt.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---


# Records verwijderen

<!--take Preview and Production references out at release-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

U kunt records verwijderen die niet meer relevant zijn in Adobe Workfront Planning. U kunt verwijderde records herstellen gedurende 30 dagen nadat ze zijn verwijderd. Voor informatie over het terugkrijgen van geschrapte verslagen, zie [ Recover geschrapte verslagen ](/help/quicksilver/planning/records/restore-deleted-records.md).

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
   <td>   <p>Contribute of hoger machtigingen voor een werkruimte <!--<span class="preview">and record type</span>--> </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het verwijderen van records

* U kunt records verwijderen die u of een andere gebruiker heeft gemaakt.
* U kunt verwijderde records niet herstellen in de productieomgeving. U kunt verwijderde records herstellen in de voorvertoningsomgeving.
* Als de verwijderde records zijn gekoppeld aan andere records, worden de gekoppelde records niet verwijderd, maar worden de gegevens uit de verwijderde record ook verwijderd.
* U kunt records niet verwijderen uit de tijdlijn of de kalenderweergaven.

## Records verwijderen

U kunt een record uit de volgende gebieden verwijderen:

* [Van de recordpagina](#delete-a-record-from-the-records-page)
* [ Van de lijstmening van een verslagtype ](#delete-a-record-from-the-record-type-table-view)

### Een record verwijderen van de recordpagina

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de records wilt verwijderen.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.
1. Voer een van de volgende handelingen uit:

   * Klik in een tabelweergave op de naam van een record.
   * Van de mening van de Lijst, houd over de naam van een verslag, dan klik **Meer** menu ![](assets/more-menu.png), dan klik **Mening**

     ![](assets/contextual-menu-for-record-row.png)
   * Klik in een tijdlijnweergave op een recordbalk.

   De recordpagina wordt geopend.

1. Klik **Meer** menu ![](assets/more-menu.png) aan het recht van de verslagnaam, dan klik **Schrapping**, dan **Schrapping** opnieuw om te bevestigen.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
De record wordt verwijderd.
1. (Facultatief en voorwaardelijk) als u het verslag in het milieu van de Voorproef schrapt, ga naar de lijstmening van de verslagpagina, en klik **ongedaan maken** pictogram ![](assets/undo-icon.png) in de hoger-juiste hoek van de mening, dan klik **onlangs geschrapt** om de geschrapte verslagen terug te krijgen.

Voor informatie over het terugkrijgen van geschrapte verslagen, zie [ Recover geschrapte verslagen ](/help/quicksilver/planning/records/restore-deleted-records.md).

### Een record verwijderen uit de tabelweergave van het recordtype

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de records wilt verwijderen.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.
1. (Voorwaardelijk) van **Mening** drop-down menu in de upper-left hoek van de lijst, selecteer een mening van de Lijst. Dit moet de standaardweergave zijn, tenzij u het recordtype in de tijdlijnweergave hebt bekeken toen u het als laatste opende.

   De records die aan het geselecteerde recordtype zijn gekoppeld, worden in de tabelweergave weergegeven.
1. Voer een van de volgende handelingen uit:

   * Klik een verslagrij met de rechtermuisknop aan, dan klik **Schrapping**.
   * Klik **Meer** menu ![](assets/more-menu.png) aan het recht van de verslagnaam, dan klik **Schrapping**.

     ![](assets/contextual-menu-for-record-row.png)

   * Klik het **Open detailleert** pictogram ![](assets/open-details-icon-in-table-name-field.png) om de doos met de gedetailleerde informatie van het verslag te openen, en klik **Meer** ![](assets/more-menu.png) rechts van de verslagnaam, dan **Schrapping**.

   De record wordt verwijderd.

1. (Optioneel) Voer een van de volgende handelingen uit om een record ongedaan te maken of opnieuw te verwijderen:

   * Klik **ongedaan maken** pictogram ![](assets/undo-icon.png), dan **onlangs geschrapt** om de geschrapte verslagen terug te krijgen. Voor informatie over het terugkrijgen van geschrapte verslagen, zie [ Recover geschrapte verslagen ](/help/quicksilver/planning/records/restore-deleted-records.md).
   * Gebruik de volgende sneltoetsen om een record ongedaan te maken of opnieuw te verwijderen:

      * CTRL + Z ( ⌘ + Z voor Mac) om het verwijderen van een record ongedaan te maken
      * CTRL + Shift + Z ( ⌘ + Shift + Z voor Mac) om record opnieuw te verwijderen




