---
title: Velden bewerken
description: In de Planning van Adobe Workfront, kunt u de gebiedsmontages voor gebieden uitgeven die reeds worden gecreeerd. In dit artikel wordt beschreven hoe u de instellingen voor Workfront-planningsvelden kunt bewerken.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 3a819fc18e0b5f438a55265ea0c5c9679ef0fdd6
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Edit foelds
description: In Adobe Workfront Planning, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Velden bewerken

{{planning-important-intro}}

U kunt de gebiedsmontages voor gebieden uitgeven die reeds in de Planning van Adobe Workfront worden gecreeerd.

Voor informatie over het maken van Adobe Workfront-planningsvelden raadpleegt u [Velden maken](/help/quicksilver/planning/fields/create-fields.md).

In dit artikel wordt beschreven hoe u de instellingen voor Workfront-planningsvelden kunt bewerken. Voor informatie over het bewerken van veldwaarden voor records raadpleegt u [Records bewerken](/help/quicksilver/planning/records/edit-records.md).

## Overwegingen bij het bewerken van veldinstellingen

U moet het volgende in overweging nemen voordat u wijzigingen aanbrengt in de configuratie van een veld:

* U kunt velden bewerken die u hebt gemaakt of velden die door andere gebruikers zijn gemaakt, als u beheerdersmachtigingen hebt voor de werkruimte waartoe de velden behoren.
* U kunt een veld in de tabel met recordtypen bewerken.
* U kunt een veld op de recordpagina of in een andere weergave, buiten de tabelweergave, niet bewerken.
* U kunt het veldtype niet bewerken nadat het veld is opgeslagen.
* U kunt de eerder geselecteerde instelling voor negatieve getallen toestaan niet uitschakelen voor een veld Getal, Percentage of Valuta als er al negatieve waarden zijn opgeslagen in de records waaraan deze is gekoppeld.
* U kunt de configuratie van de volgende veldelementen bewerken nadat u het veld hebt opgeslagen:

   * De naam of beschrijving van een veld
   * De Opties van een Enig-uitgezochte of multi-uitgezochte gebied.
   * De expressie van een veld Formule.

  >[!WARNING]
  >
  >Wanneer formulerendingen veranderen, of de opties van een uitgezocht-type gebied worden toegevoegd of verwijderd, zal er gegevensverlies voor de verslagen zijn die reeds informatie hebben die in de gebieden wordt opgeslagen de waarvan configuratie wordt gewijzigd.
  >
  >Er is geen waarschuwing of indicatie dat dit gegevensverlies kan optreden wanneer u de configuratie van velden wijzigt.
  >
  >Er is geen bericht aan andere gebruikers dat de gebiedsconfiguratie is veranderd.

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
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
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangscontroles voor de Planning van Workfront</p>  
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
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Zie voor meer informatie <a href="/help/quicksilver/planning/access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Veldinstellingen bewerken

{{step1-to-planning}}

1. (Optioneel) Breid de pijl omlaag naar rechts uit naar de naam van een bestaande werkruimte en selecteer de werkruimte waarvoor u recordtypen wilt verwijderen.

   De werkruimte wordt geopend en de recordtypen die eraan zijn gekoppeld, worden weergegeven.
1. Klik op de kaart voor het recordtype waarvan u de velden wilt bewerken.

   Hierdoor wordt de pagina van het recordtype geopend.
1. (Voorwaardelijk) Klik op de tab van een **Tabelweergave**.
1. Houd de cursor boven de kolomkop van een veld dat u wilt bewerken, klik op de pijl omlaag na de veldnaam en klik vervolgens op **Veld bewerken**

   of

   Dubbelklik op de kolomkop voor het veld.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Werk informatie over het veld bij en klik op **Opslaan**. <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >U kunt het veldtype niet bijwerken nadat het veld is opgeslagen.

   De veldinformatie wordt bijgewerkt voor iedereen die toegang heeft tot de werkruimte.

1. (Voorwaardelijk) Klik voor gekoppelde recordvelden op **Opzoekvelden bewerken** en voeg of verwijder om het even welke gebieden van het verbonden verslagtype toe.

   Zie voor meer informatie [Verbind recordtypen](/help/quicksilver/planning/architecture/connect-record-types.md).

<!--After the release of the RTBE for field configurations, replace the tip with this:
>[!TIP]
>
>* You cannot update the field type after the field is saved.
>
>* When you modify field configurations (field options or formula expressions), records that already contain information in the modified fields will update their values in real-time. There is no warning and no audit log for the value changes triggered by field configuration changes. All users who view the fields will immediately see the new values with the modifications. -->
