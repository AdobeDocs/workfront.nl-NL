---
title: Records verwijderen
description: U kunt records verwijderen die u of een andere gebruiker heeft gemaakt. U kunt verwijderde records niet herstellen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Records verwijderen

{{planning-important-intro}}

U kunt records verwijderen die niet meer relevant zijn in Adobe Workfront Planning.

## Toegangsvereisten

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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-overeenkomst</p></td>
   <td>
<p>Uw organisatie moet zijn ingeschreven in de vroege toegangsfase voor Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-plan</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licentie</p>
   </td>
   <td>
   <p>Alle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Contribute of hoger machtigingen voor een werkruimte</a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Zie voor meer informatie <a href="/help/quicksilver/planning/access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>

</tbody>
</table>


<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Overwegingen bij het verwijderen van records

* U kunt records verwijderen die u of een andere gebruiker heeft gemaakt.
* U kunt verwijderde records niet herstellen. <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* Als de verwijderde records zijn gekoppeld aan andere records, worden de gekoppelde records niet verwijderd, maar worden de gegevens uit de verwijderde record ook verwijderd.
* U kunt records in bulk niet verwijderen. <!--this will probably change-->
* U kunt records niet verwijderen uit de tijdlijnweergave.

## Records verwijderen

U kunt een record uit de volgende gebieden verwijderen:

* [Van de recordpagina](#delete-a-record-from-the-records-page)
* [Vanuit de tabelweergave van een recordtype](#delete-a-record-from-the-record-type-table-view)

### Een record verwijderen van de recordpagina

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de records wilt verwijderen.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.
1. Voer een van de volgende handelingen uit:

   * Klik in een tabelweergave op de naam van een record.
   * Houd de muisaanwijzer in de tabelweergave boven de naam van een record en klik vervolgens op de knop **Meer** menu ![](assets/more-menu.png)en klik vervolgens op **Weergave**

     ![](assets/contextual-menu-for-record-row.png)
   * Klik in een tijdlijnweergave op een recordbalk.

   De recordpagina wordt geopend.

1. Klik op de knop **Meer** menu ![](assets/more-menu.png) rechts van de naam van de record klikt u op **Verwijderen** vervolgens **Verwijderen** nogmaals ter bevestiging.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
De record wordt verwijderd en kan niet worden hersteld.

### Een record verwijderen uit de tabelweergave van het recordtype

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de records wilt verwijderen.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.
1. (Voorwaardelijk) Van de **Weergave** Selecteer een tabelweergave in de linkerbovenhoek van de tabel. Dit moet de standaardweergave zijn, tenzij u het recordtype in de tijdlijnweergave hebt bekeken toen u het als laatste opende.

   De records die aan het geselecteerde recordtype zijn gekoppeld, worden in de tabelweergave weergegeven.
1. Voer een van de volgende handelingen uit:

   * Klik met de rechtermuisknop op een recordrij en klik vervolgens op **Verwijderen**.
   * Klik op de knop **Meer** menu ![](assets/more-menu.png) rechts van de naam van de record klikt u op **Verwijderen**

     ![](assets/contextual-menu-for-record-row.png)

   * Klik op de knop **Details openen** pictogram ![](assets/open-details-icon-in-table-name-field.png) om het vak met de gedetailleerde informatie van de record te openen en klik op **Meer** ![](assets/more-menu.png) rechts van de naam van de record, vervolgens **Verwijderen**.

   De record wordt verwijderd en kan niet worden hersteld.

1. (Optioneel) Gebruik de volgende sneltoetsen om een record ongedaan te maken of opnieuw te verwijderen:

   * CTRL + Z ( ⌘ + Z voor Mac) om een wijziging ongedaan te maken
   * CTRL + Shift + Z ( ⌘ + Shift + Z voor Mac) om een wijziging opnieuw uit te voeren
