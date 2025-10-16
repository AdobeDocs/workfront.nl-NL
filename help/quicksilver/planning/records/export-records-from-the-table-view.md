---
title: Records exporteren uit de tabelweergave
description: U kunt records en de bijbehorende informatie uit de tabelweergave exporteren naar een CSV- of Excel-bestand.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d8ac4d94-28b5-41d6-acb8-259696897c8a
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---

# Records exporteren uit de tabelweergave

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

U kunt verslagen en hun informatie van de lijstmening naar een Excel of een Csv- dossier in de Planning van Adobe Workfront uitvoeren.

## Toegangsvereisten

+++ Breid uit om de toegangsvereisten voor de functionaliteit in dit artikel te bekijken. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Alle Workfront en alle planningspakketten</p> <p>Willekeurige workflow en planningspakket</p>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Licht of hoger</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td> <p>Machtigingen weergeven of hoger voor een werkruimte en een recordtype</p>   
   <p>Machtigingen voor een weergave of hoger weergeven</p>

</td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> De gebruikers met een Licht of de vergunning van de Medewerker moeten een lay-outmalplaatje worden toegewezen dat Planning omvat.
   <p>De standaardgebruikers en de Beheerders van het Systeem hebben de Gebieden van de Planning die door gebrek worden toegelaten.</p></div></li></ul>
</td>
  </tr>  
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


<!--Old:
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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Light or higher </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>View or higher permissions to a view</p>  
   </td> 
  </tr> 
</tbody> 
</table> -->


## Records exporteren uit de tabelweergave

Houd rekening met het volgende wanneer u de tabelweergave exporteert:

* Bij de informatie die naar een Excel-bestand wordt geëxporteerd, blijven de filters, groepen en sorteren behouden die op de tabelweergave in Workfront Planning zijn toegepast. Groepen zijn niet zichtbaar in het CSV-bestand.

* Miniaturen en aangepaste rijkleuren worden niet ondersteund in geëxporteerde bestanden.

* Alleen velden die zichtbaar zijn gemaakt in de Workfront-interface worden geëxporteerd. Verborgen velden worden niet geëxporteerd.

Informatie exporteren uit de tabelweergave of een recordtype:

1. Ga naar een pagina met recordtypen en klik op een tabblad met tabelweergave.
1. Voer een van de volgende handelingen uit:

   * Beweeg over de naam van het lusje van de lijstmening, dan klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png) rechts van de meningsnaam, dan klik **Uitvoer**.

   ![&#x200B; Meer menu op een mening &#x200B;](assets/view-more-menu-with-duplicate-option.png)

   * Klik **Aandeel** > **Uitvoer de huidige mening**. Deze optie is alleen beschikbaar wanneer u de tabelweergave weergeeft.

   ![&#x200B; knoop van het Aandeel met verslagtype en mening die opties delen &#x200B;](assets/share-button-with-record-type-and-view-sharing-options.png)

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
