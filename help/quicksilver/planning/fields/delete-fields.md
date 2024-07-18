---
title: Velden verwijderen
description: In de Planning van Adobe Workfront, kunt u douanegebieden schrappen die niet meer relevant zijn.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Delete fields
description: In Adobe Planning, you can delete custom fields that are no longer relevant.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Velden verwijderen

{{planning-important-intro}}

In de Planning van Adobe Workfront, kunt u douanevelden tot stand brengen om informatie over verslagen op te slaan.

Voor informatie over het creëren van douanegebieden in de Planning van Workfront, zie [ gebieden ](/help/quicksilver/planning/fields/create-fields.md) creëren.

U kunt Workfront-planningsvelden verwijderen die niet meer relevant zijn.

## Overwegingen bij het verwijderen van Workfront-planningsvelden:

* U kunt een veld alleen verwijderen in de tabelweergave van het recordtype.
* U kunt het primaire veld van een record niet verwijderen.
* Alle informatie die in het veld is opgeslagen, wordt verwijderd en kan niet worden hersteld.
* Wanneer u een gekoppeld recordveld verwijdert, worden alle gekoppelde opzoekvelden ook verwijderd uit het recordtype waaruit u een koppeling maakt. De gekoppelde recordvelden van de recordtypen waarnaar u een koppeling maakt, worden niet verwijderd.

  Voor meer informatie, zie [ Connect verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

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
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td>
   <td>
   <p>Alle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Workfront</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Voor informatie, zie <a href="/help/quicksilver/planning/access/access-overview.md"> overzicht van de Toegang </a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Rechten beheren in een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
</td>
  </tr>
 </tbody>
</table>



<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Velden verwijderen

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de recordvelden wilt verwijderen.

   De werkruimte wordt geopend en de recordtypen worden weergegeven.

1. Klik op de kaart van een recordtype.

1. (Voorwaardelijk) als niet reeds geselecteerd, klik het lusje van de mening van de a **Lijst** op de verslagtype pagina.

   Alle bestaande records die aan het recordtype zijn gekoppeld, worden in de rijen van de tabelweergave weergegeven.

1. Zoek het veld dat u wilt verwijderen in de kolomkoppen en houd de cursor boven de kolomkop en klik vervolgens op de pijl omlaag na de veldnaam.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Klik **Schrapping**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Klik **Schrapping** om te bevestigen.

   Het veld wordt verwijderd, kan niet worden hersteld en kan niet meer aan records worden gekoppeld.
