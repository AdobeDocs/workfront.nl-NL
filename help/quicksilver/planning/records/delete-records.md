---
title: Records verwijderen
description: U kunt records verwijderen die u of een andere gebruiker heeft gemaakt. U kunt verwijderde records niet herstellen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Records verwijderen

{{planning-important-intro}}

U kunt records verwijderen die niet meer relevant zijn in Adobe Workfront Planning.

## Toegangsvereisten

+++ Breid uit om toegangsvereisten voor de Planning van Workfront te bekijken.

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
   <td role="rowheader"><p>Adobe Workfront-licentie*</p>
   </td>
   <td>
   <p>Nieuw: Standaard</p>
   <p>Huidig: Plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Contribute of hogere toestemmingen aan een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Voor informatie, zie <a href="/help/quicksilver/planning/access/access-overview.md"> overzicht van de Toegang </a>. </p>  
</td>
  </tr>

</tbody>
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++
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
De record wordt verwijderd en kan niet worden hersteld.

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
   * Klik **Meer** menu ![](assets/more-menu.png) aan het recht van de verslagnaam, dan klik **Schrapping**

     ![](assets/contextual-menu-for-record-row.png)

   * Klik het **Open detailleert** pictogram ![](assets/open-details-icon-in-table-name-field.png) om de doos met de gedetailleerde informatie van het verslag te openen, en klik **Meer** ![](assets/more-menu.png) rechts van de verslagnaam, dan **Schrapping**.

   De record wordt verwijderd en kan niet worden hersteld.

1. (Optioneel) Gebruik de volgende sneltoetsen om een record ongedaan te maken of opnieuw te verwijderen:

   * CTRL + Z ( ⌘ + Z voor Mac) om een wijziging ongedaan te maken
   * CTRL + Shift + Z ( ⌘ + Shift + Z voor Mac) om een wijziging opnieuw uit te voeren
