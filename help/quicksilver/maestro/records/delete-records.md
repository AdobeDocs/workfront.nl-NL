---
title: Records verwijderen
description: U kunt records verwijderen die u of een andere gebruiker heeft gemaakt. U kunt verwijderde records niet herstellen.
hidefromtoc: true
hide: true
source-git-commit: 14b456f32dd2c8735e0a5252387f25305efc7610
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---


<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# Records verwijderen

>[!IMPORTANT]
>
>Adobe Maestro maakt momenteel deel uit van een gesloten bètaprogramma dat voor een beperkt aantal klanten toegankelijk is.
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro-overview.md).

U kunt records verwijderen die niet meer relevant zijn voor de Adobe Maestro.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-overeenkomst</p></td>
   <td>
<p>Uw organisatie moet zijn ingeschreven voor het afgesloten bètaprogramma van de Adobe Maestro. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-plan</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td>
   <td>
   <p>Alle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Toegangsniveau</td>
   <td> <p>Alle</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Lay-outsjabloon</td>
   <td> <p>Uw systeembeheerder moet het gebied Maestro in uw lay-outmalplaatje toevoegen. Zie voor meer informatie <a href="../access/grant-access.md">Toegang verlenen tot Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Overwegingen bij het verwijderen van records

* U kunt records verwijderen die u of een andere gebruiker heeft gemaakt.
* U kunt verwijderde records niet herstellen. <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* Als de verwijderde records zijn gekoppeld aan andere records, worden de gekoppelde records niet verwijderd, maar worden de gegevens uit de verwijderde record ook verwijderd.
* U kunt records in bulk niet verwijderen. <!--this will probably change-->
* U kunt records niet verwijderen uit de tijdlijnweergave.

## Records verwijderen

U kunt een record uit de volgende gebieden verwijderen:

* [Via de pagina Details van een record](#delete-a-record-from-the-records-details-page)
* [Vanuit de tabelweergave van een recordtype](#delete-a-record-from-the-record-type-table-view)

### Een record verwijderen van de pagina Details van de record

1. Klik op de knop **Hoofdmenu** ![](assets/main-menu-workfront.png) in de rechterbovenhoek, of de **Hoofdmenu** ![](assets/main-menu-shell.png) in de linkerbovenhoek, als deze beschikbaar is, klikt u op Maestro.

   De werkruimte die u als laatste opent.
1. Klik op een recordtype.

   De pagina met recordtypen wordt geopend.
1. Voer een van de volgende handelingen uit:

   * Klik in een tabelweergave op de naam van een record.
   * Houd de muisaanwijzer in de tabelweergave boven de naam van een record en klik vervolgens op de knop **Meer** menu ![](assets/more-menu.png)en klik vervolgens op **Weergave**

     ![](assets/contextual-menu-for-record-row.png)
   * Klik in een tijdlijnweergave op een recordbalk.

   De record **Details** pagina wordt geopend.

1. Klik op de knop **Meer** menu ![](assets/more-menu.png) rechts van de naam van de record klikt u op **Verwijderen** vervolgens **Verwijderen** nogmaals ter bevestiging.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
De record wordt verwijderd en kan niet worden hersteld.

### Een record verwijderen uit de tabelweergave van het recordtype

1. Klik op de knop **Hoofdmenu** ![](assets/main-menu-workfront.png) in de rechterbovenhoek, of de **Hoofdmenu** ![](assets/main-menu-shell.png) in de linkerbovenhoek, als deze beschikbaar is, klikt u op **Maestro**.

   De werkruimte die u het laatst hebt geopend.
1. Klik op een recordtype.

   De pagina met recordtypen wordt geopend.
1. (Voorwaardelijk) Van de **Weergave** Selecteer een tabelweergave in de rechterbovenhoek van de tabel. Dit moet de standaardweergave zijn, tenzij u het recordtype in de tijdlijnweergave hebt bekeken toen u het als laatste opende.

   De records die aan het geselecteerde recordtype zijn gekoppeld, worden in de tabelweergave weergegeven.
1. Klik met de rechtermuisknop op een recordrij en klik vervolgens op **Verwijderen**.

   ![](assets/contextual-menu-for-record-row.png)

   De record wordt verwijderd en kan niet worden hersteld.