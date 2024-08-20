---
title: Recordtypen bewerken
description: U kunt recordtypen bewerken nadat u deze hebt opgeslagen. Recordtypen zijn de objecttypen voor Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: ded6db27fa3fba9195e2133134f60bcadb0f897a
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the object types of Adobe Workfront Planning.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# Recordtypen bewerken

{{planning-important-intro}}

Recordtypen zijn de objecttypen voor Adobe Workfront Planning. U kunt de weergave van recordtypen bewerken die u of iemand anders heeft gemaakt. Voor informatie over het creëren van het verslagtypes van de Planning van Workfront, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

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
   <p> Adobe Workfront</p> <p>Als u Adobe Workfront Planning-recordtypen wilt verbinden met Experience Manager Assets, hebt u een Adobe Experience Manager Assets-licentie nodig en moet het Workfront-exemplaar van uw organisatie zijn aangemeld bij het Adobe Business Platform of de Adobe Admin Console.</p> </td>
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
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Workfront</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Rechten beheren in een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
   <p>Alleen systeembeheerders kunnen recordtypen inschakelen om verbinding te maken met andere werkruimten</p>
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

## Recordtypen bewerken

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de recordtypen wilt bewerken.

   De werkruimtepagina wordt geopend en de recordtypen worden weergegeven.
1. Voer een van de volgende handelingen uit:

   * Beweeg over de kaart van een verslagtype en klik **Meer** menu ![](assets/more-menu.png) in de hoger-juiste hoek van de kaart van het verslagtype, dan klik **uitgeven**
of
   * Klik een kaart van het verslagtype om de verslagtype pagina te openen, klik **Meer** menu ![](assets/more-menu.png) rechts van de naam van het verslagtype, dan klik **uitgeven**.

   ![](assets/more-menu-options-from-record-type-card.png)

1. In **geef verslagtype** doos uit, opent het **3} lusje van de Verschijning {door gebrek.**

   ![](assets/edit-record-type-box-appearance-tab.png)

   Werk de volgende informatie in het **Verschijning** lusje bij:

   * Bewerk indien nodig de naam van het recordtype. <!--did they add a field label for this?-->
   * **Beschrijving**: geef of voeg een beschrijving voor het verslagtype met meer informatie over het uit.
   * Bewerk de kleur en vorm van het pictogram dat aan het recordtype is gekoppeld. Ga als volgt te werk:
      * Selecteer een kleur om het recordtype te identificeren. Dit is de kleur van het pictogram voor recordtype.
      * Selecteer een pictogram in de lijst of typ de naam van een pictogram om te beschrijven wat het vertegenwoordigt en selecteer het pictogram wanneer het wordt weergegeven. Dit is het pictogram van het recordtype. Een bestandspictogram is standaard geselecteerd.

1. (Voorwaardelijk) als u een systeembeheerder bent, klik het **Geavanceerde montages** lusje in **geef verslagtype** doos uit.

   ![](assets/edit-record-type-box-advanced-settings-tab.png)

1. (Voorwaardelijk) als systeembeheerder, werk de volgende informatie in de **Geavanceerde montages** tabel bij:

   * **verbind van andere werkruimten**: Selecteer deze knevel om gebruikers toe te staan om met dit verslagtype van andere werkruimten te verbinden. Deze optie is standaard uitgeschakeld.
   * **Systeem wijd**: Selecteer deze optie om gebruikers toe te staan om met dit verslag van alle werkruimten in het systeem te verbinden.
   * **Specifieke werkruimten**: Selecteer deze optie om de werkruimten te beperken waarvan de gebruikers met dit verslagtype kunnen verbinden, dan het drop-down menu uitbreiden en de werkruimten selecteren u gebruikers met dit verslagtype van wilt verbinden. U kunt de naam van een werkruimte typen en deze selecteren wanneer deze in de lijst wordt weergegeven.

1. Klik **sparen**.

   Op de kaart met recordtype in de werkruimte wordt een connectiviteitspictogram ![](assets/connect-from-other-workspaces-icon.png) weergegeven in de rechterbovenhoek om aan te geven dat de record nu toegankelijk is vanuit andere werkruimten.

1. (Optioneel) Klik op de kaart met recordtype in de werkruimte om de pagina van het recordtype te openen en geef vervolgens het recordtype in de koptekst een andere naam.

1. (Optioneel) Als u een ander recordtype wilt bewerken, vouwt u de pijl omlaag naar rechts van de naam van een recordtype uit, zoekt u naar een recordtype en selecteert u deze pijl wanneer deze in de lijst wordt weergegeven.

   ![](assets/record-type-drop-down-on-record-type-page-with-search-box.png)