---
title: Velden bewerken
description: In Adobe Maestro, kunt u de gebiedsmontages voor gebieden uitgeven die reeds worden gecreeerd.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Velden bewerken

>[!IMPORTANT]
>
>Adobe Maestro maakt momenteel deel uit van een bètaprogramma dat voor een beperkt aantal klanten toegankelijk is.
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro-overview.md).

U kunt de veldinstellingen bewerken voor velden die al zijn gemaakt.

Voor informatie over het maken van Adobe Maestro gebieden, zie [Velden maken](../architecture-and-fields/create-fields.md).

In dit artikel wordt beschreven hoe u de instellingen voor Maestro-velden kunt bewerken. Voor informatie over het bewerken van veldwaarden voor Maestro-records raadpleegt u [Records bewerken](../records/edit-records.md).

## Overwegingen bij het bewerken van veldgegevens

* U kunt velden bewerken die u hebt gemaakt of velden die door andere gebruikers zijn gemaakt. <!--this will change with access levels/ permissions-->
* U kunt een veld in de tabel met recordtypen bewerken.
* U kunt het veldtype niet bewerken nadat het veld is opgeslagen.
* U kunt de eerder geselecteerde instelling voor negatieve getallen toestaan niet uitschakelen voor een veld Getal, Percentage of Valuta als er al negatieve waarden zijn opgeslagen in de records waaraan deze is gekoppeld.
<!--this is not true yet; one piece of it is true and I added it as the bullet above: 
* You cannot edit the options, or the special format of the following fields, after they are saved:

    * Allow negative numbers option from a Number, Percentage, or Currency field. 
    * The Options of a Single-select or a Multi-select field.
-->

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

## Velden bewerken

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-workfront.png) in de rechterbovenhoek van Workfront <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> klik vervolgens op **Maestro** ![](assets/maestro-icon.png).

   De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Breid de pijl omlaag naar rechts uit naar de naam van een bestaande werkruimte en selecteer de werkruimte waarvoor u recordtypen wilt verwijderen.

   De werkruimte wordt geopend en de recordtypen en bijbehorende taxonomieën worden weergegeven.
1. Klik op de kaart voor het recordtype of de taxonomie waarvan u de velden wilt bewerken.

   Hierdoor wordt de pagina van het recordtype geopend.
1. (Voorwaardelijk) Selecteer een **Tabelweergave** van de **Weergave** in de rechterbovenhoek van de pagina met recordtypen.
1. Houd de cursor boven de kolomkop van een veld dat u wilt bewerken en klik op de pijl omlaag na de veldnaam.
1. Klikken **Veld bewerken** en werkt u vervolgens de gegevens in het veld bij en klikt u op **Opslaan**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >U kunt het veldtype niet bijwerken nadat het veld is opgeslagen.


1. (Voorwaardelijk) Klik voor gekoppelde recordvelden op **Opzoekvelden bewerken** en voeg of verwijder om het even welke gebieden van het verbonden verslagtype toe.

   Zie voor meer informatie [Verbind recordtypen](../architecture-and-fields/connect-record-types.md).
