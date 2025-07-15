---
title: Records exporteren uit de tabelweergave
description: U kunt records en de bijbehorende informatie uit de tabelweergave exporteren naar een CSV- of Excel-bestand.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 8f4c1be156094d18df4bc3628d4f1fca90372119
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---


# Records exporteren uit de tabelweergave

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

U kunt verslagen en hun informatie van de lijstmening naar een Excel of een Csv- dossier in de Planning van Adobe Workfront uitvoeren.

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
   <td>   <p>Rechten beheren voor een weergave</p>  
   <p>Machtigingen weergeven voor een weergave om de weergave-instellingen tijdelijk te wijzigen, te dupliceren of te exporteren.</p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Records exporteren uit de tabelweergave

Houd rekening met het volgende wanneer u de tabelweergave exporteert:

* Bij de informatie die naar een Excel-bestand wordt geëxporteerd, blijven de filters, groepen en sorteren behouden die op de tabelweergave in Workfront Planning zijn toegepast. Groepen zijn niet zichtbaar in het CSV-bestand.

* Miniaturen en aangepaste rijkleuren worden niet ondersteund in geëxporteerde bestanden.

* Alleen velden die zichtbaar zijn gemaakt in de Workfront-interface worden geëxporteerd. Verborgen velden worden niet geëxporteerd.

Informatie exporteren uit de tabelweergave of een recordtype:

1. Ga naar een pagina met recordtypen en klik op een tabblad met tabelweergave.
1. Voer een van de volgende handelingen uit:

   * Beweeg over de naam van het lusje van de lijstmening, dan klik **Meer** menu ![ Meer menu ](assets/more-menu.png) rechts van de meningsnaam, dan klik **Uitvoer**.

   ![ Meer menu op een mening ](assets/view-more-menu-with-duplicate-option.png)

   * Klik **Aandeel** > **Uitvoer de huidige mening**. Deze optie is alleen beschikbaar wanneer u de tabelweergave weergeeft.

   ![ knoop van het Aandeel met verslagtype en mening die opties delen ](assets/share-button-with-record-type-and-view-sharing-options.png)

1. Selecteer een van de volgende indelingen:

   * **Excel**
   * **CSV**

   >[!IMPORTANT]
   >
   >U kunt geen informatie uit de lijstmening uitvoeren wanneer u een verschillende mening op het scherm toont. U moet de lijstmening tonen die u wilt uitvoeren om tot de optie van de Uitvoer in het Meer menu toegang te hebben.

   Het bestand wordt naar de computer gedownload.

1. (Optioneel) Ga naar de map Downloads op uw computer en zoek het gedownloade bestand.

   De naam van het geëxporteerde bestand heeft de volgende indeling:

   `Name of the view - name of the record type`

   Een tabelweergave voor het recordtype Campagnes genereert bijvoorbeeld een bestand met de naam `Table view - Campaigns` .

   Het bestand bevat de volgende informatie:

   * De kolomkoppen worden in het Excel-bestand zwart gemarkeerd.
   * Alle velden die zichtbaar zijn in de Workfront-interface, worden op dezelfde criteria gesorteerd en gefilterd
   * Groepen blijven behouden in het Excel-bestand

   U kunt de geëxporteerde bestanden nu delen met anderen of koppelen aan communicatie.

</div>
