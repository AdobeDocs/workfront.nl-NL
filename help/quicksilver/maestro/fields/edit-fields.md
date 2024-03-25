---
title: Velden bewerken
description: In Adobe Workfront planning, kunt u de gebiedsmontages voor gebieden uitgeven die reeds worden gecreeerd.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!---
title: Edit foelds
description: In Adobe Maestro, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->


# Velden bewerken

{{maestro-important-intro}}

U kunt de veldinstellingen bewerken voor velden die al zijn gemaakt in Adobe Workfront-planning.

Voor informatie over het maken van Adobe Workfront-planningsvelden raadpleegt u [Velden maken](../fields/create-fields.md).

In dit artikel wordt beschreven hoe u de instellingen voor Workfront-planningsvelden kunt bewerken. Voor informatie over het bewerken van veldwaarden voor records raadpleegt u [Records bewerken](/help/quicksilver/maestro/records/edit-records.md).

## Overwegingen bij het bewerken van veldgegevens

* U kunt velden bewerken die u hebt gemaakt of velden die door andere gebruikers zijn gemaakt, als u beheerdersmachtigingen hebt voor de werkruimte waartoe de velden behoren.
* U kunt een veld in de tabel met recordtypen bewerken.
* U kunt een veld op de pagina Details van een record of in de tijdlijnweergave niet bewerken.
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
<p>Uw organisatie moet zijn ingeschreven voor het bètaprogramma voor Adobe Workfront-planning. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
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
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangscontroles voor de planning van Workfront</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Machtigingen beheren in een werkruimte</a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Velden bewerken

{{step1-to-maestro}}

    De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Breid de pijl omlaag naar rechts uit naar de naam van een bestaande werkruimte en selecteer de werkruimte waarvoor u recordtypen wilt verwijderen.

   De werkruimte wordt geopend en de recordtypen die eraan zijn gekoppeld, worden weergegeven.
1. Klik op de kaart voor het recordtype waarvan u de velden wilt bewerken.

   Hierdoor wordt de pagina van het recordtype geopend.
1. (Voorwaardelijk) Selecteer een **Tabelweergave** van de **Weergave** in de rechterbovenhoek van de pagina met recordtypen.
1. Houd de cursor boven de kolomkop van een veld dat u wilt bewerken, klik op de pijl omlaag na de veldnaam en klik vervolgens op **Veld bewerken**

   of

   Dubbelklik op de kolomkop voor het veld.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Werk informatie over het veld bij en klik op **Opslaan**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >U kunt het veldtype niet bijwerken nadat het veld is opgeslagen.


1. (Voorwaardelijk) Klik voor gekoppelde recordvelden op **Opzoekvelden bewerken** en voeg of verwijder om het even welke gebieden van het verbonden verslagtype toe.

   Zie voor meer informatie [Verbind recordtypen](../architecture/connect-record-types.md).
