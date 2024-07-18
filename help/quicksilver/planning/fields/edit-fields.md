---
title: Veldinstellingen bewerken
description: In de Planning van Adobe Workfront, kunt u de gebiedsmontages voor gebieden uitgeven die reeds worden gecreeerd. In dit artikel wordt beschreven hoe u de instellingen voor Workfront-planningsvelden kunt bewerken.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: dc8e6f730ec88fc66c3486987e064b5f0760fb80
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Edit fields
description: In Adobe Workfront Planning, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Veldinstellingen bewerken

{{planning-important-intro}}

U kunt de gebiedsmontages voor gebieden uitgeven die reeds in de Planning van Adobe Workfront worden gecreeerd.

Voor informatie over het creëren van de gebieden van de Planning van Adobe Workfront, zie [ gebieden ](/help/quicksilver/planning/fields/create-fields.md) creëren.

In dit artikel wordt beschreven hoe u de instellingen voor Workfront-planningsvelden kunt bewerken. Voor informatie over het uitgeven van gebiedswaarden voor verslagen, zie [ verslagen ](/help/quicksilver/planning/records/edit-records.md) uitgeven.

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
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td>
   <td>
   <p>Nieuw: Standaard</p>
   <p>Huidig: Plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangscontroles voor de Planning van Workfront</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Rechten beheren in een werkruimte </a> </p>  
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

*Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

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

## Veldinstellingen bewerken

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de recordvelden wilt bewerken.

   De werkruimte wordt geopend en alle recordtypen in de werkruimte worden op kaarten weergegeven.

1. Klik op de kaart van een recordtype.

   Hierdoor wordt de pagina van het recordtype geopend.

1. (Voorwaardelijk) klik het lusje van de mening van de a **Lijst**.

   Alle bestaande records die aan het recordtype zijn gekoppeld, worden in de rijen van de tabelweergave weergegeven.
1. Plaats over de kolomkopbal van een gebied u wilt uitgeven, dan de naar beneden wijzende pijl na de gebiedsnaam klikken, dan **uitgeeft gebied**

   of

   Dubbelklik op de kolomkop voor het veld.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Update informatie over het gebied en klik **sparen**. <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* U kunt het veldtype niet bijwerken nadat het veld is opgeslagen.
   >
   >* Als u veldconfiguraties wijzigt (veldopties of formule-expressies), worden de waarden van records die al informatie in de gewijzigde velden bevatten, in real-time bijgewerkt. Er is geen waarschuwing en geen controlelogboek voor de waardeveranderingen die door de veranderingen van de gebiedsconfiguratie worden teweeggebracht. Alle gebruikers die de velden weergeven, zien de nieuwe waarden direct met de wijzigingen.

   De veldinformatie wordt bijgewerkt voor iedereen die toegang heeft tot de werkruimte.

1. (Voorwaardelijk) voor verbonden verslaggebieden, klik **uitgeeft raadplegingsgebieden** en voeg of verwijder om het even welke gebieden van het verbonden verslagtype toe.

   Voor meer informatie, zie [ Connect verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).

