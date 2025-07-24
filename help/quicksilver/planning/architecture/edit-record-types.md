---
title: Recordtypen bewerken
description: U kunt recordtypen bewerken nadat u deze hebt opgeslagen. Recordtypen zijn de objecttypen voor Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: a4bb3582eb476acbefa5d11db1f2c06eafc13cdd
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---


# Recordtypen bewerken

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

Recordtypen zijn de objecttypen voor Adobe Workfront Planning. U kunt de weergave van recordtypen bewerken die u of iemand anders heeft gemaakt. Voor informatie over het creëren van het verslagtypes van de Planning van Workfront, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Producten</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-abonnement*</p></td> 
   <td> 
<p>Een van de volgende Workfront-plannen:</p> 
<ul><li>Selecteren</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is niet beschikbaar voor oudere Workfront-plannen</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-planningspakket*</p></td> 
   <td> 
<p>Alle </p> 
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningsplan is opgenomen. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-platform</p></td> 
   <td> 
<p>Het geval van Workfront van uw organisatie moet aan de Verenigde Ervaring van Adobe worden genegeerd om tot de Planning van Workfront te kunnen toegang hebben.</p> 
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td><p> Standaard </p>
   <p>Workfront Planning is niet beschikbaar voor oudere Workfront-licenties</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td> 
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Machtigingen beheren in een werkruimte en recordtype </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
   <p>Alleen systeembeheerders kunnen recordtypen inschakelen om verbinding te maken met andere werkruimten</p> </td> 
  </tr>

</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Recordtypen bewerken

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de recordtypen wilt bewerken.

   De werkruimtepagina wordt geopend en de recordtypen worden weergegeven.
1. Voer een van de volgende handelingen uit:

   * Beweeg over de kaart van een verslagtype en klik **Meer** menu ![ Meer menu ](assets/more-menu.png) in de hoger-juiste hoek van de kaart van het verslagtype, dan klik **uitgeven**
of
   * <span class="preview"> klik een kaart van het verslagtype om de verslagtype pagina te openen, klik het **Meer** menu ![ Meer menu ](assets/more-menu.png) aan het recht van het verslagtype naam, dan klik **uitgeven**. </span>

   <span class="preview">![ Meer menuopties van verslagtype kaart ](assets/more-menu-options-from-record-type-card.png)</span>

1. In **geef verslagtype** doos uit, opent het **3} lusje van de Verschijning {door gebrek.**

   ![ Weergavetabblad van recordtekstvak bewerken ](assets/edit-record-type-box-appearance-tab.png)

   Werk de volgende informatie in het **Verschijning** lusje bij:

   * Bewerk indien nodig de naam van het recordtype. <!--did they add a field label for this?-->
   * **Beschrijving**: geef of voeg een beschrijving voor het verslagtype met meer informatie over het uit.
   * Bewerk de kleur en vorm van het pictogram dat aan het recordtype is gekoppeld. Ga als volgt te werk:
      * Selecteer een kleur om het recordtype te identificeren. Dit is de kleur van het pictogram voor recordtype.
      * Selecteer een pictogram in de lijst of typ de naam van een pictogram om te beschrijven wat het vertegenwoordigt en selecteer het pictogram wanneer het wordt weergegeven. Dit is het pictogram van het recordtype. Een bestandspictogram is standaard geselecteerd.

   <!--old info: 
   1. (Conditional) If you are a system administrator, click the **Advanced settings** tab in the **Edit record type** box. 
      ![Edit record type box advanced settings tab](assets/edit-record-type-box-advanced-settings-tab.png)
   1. (Conditional) Update the following information in the **Advanced settings** tab: 
      * Enable the **Connect from other workspace** setting. When enabled, the record type is accessible and can be connected from other workspaces. 
      * Choose from which workspaces the record type can be accessed. Choose from the following options:
         * **System wide**: Users can connect to this record type from all workspaces where they have manage permissions. 
         * **Specific workspaces**: Add the names of the workspaces where workspace managers can connect to this record type.-->


1. (Facultatief en voorwaardelijk) als u een systeembeheerder bent, klik **Geavanceerde montages** en werk de volgende informatie in de **dwars-werkruimtesectie** bij: <!--the info here is duplicated in the Create record types article-->
   * Laat **toe toestaan verbindend met dit verslagtype in andere werkruimten** het plaatsen: Dit staat werkruimtemanagers toe om met dit verslagtype van andere werkruimten te verbinden.\
     U kunt aangeven van welke werkruimten dit recordtype verbinding kan worden gemaakt. U kunt het voor alle werkruimten ter beschikking stellen of specifieke degenen aanwijzen waar u het kunt invoeren.
Voor meer informatie, zie [ mogelijkheden van de dwars-werkruimte voor verslagtypes ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.

   ![ geef recordtype doos geavanceerde montages tabel uit ](assets/edit-record-type-box-advanced-settings-tab.png)

   <!--replace last point with this when we release dynamic record types:
      1. (Optional and conditional) If you are a system administrator, click **Advanced settings** and update the following information in the **Cross-workspace capability** section: **** the info here is duplicated in the Edit record types article ***
         * Enable the **Allow adding this record type to other workspaces** setting: This allows workspace managers to add this record type to other workspaces. 
               You can designate specific users who can add this record type to other workspaces. 
         * Enable the **Allow connecting to this record type in other workspaces** setting: This allows workspace managers to connect to this record type from other workspaces.  
               You can designate which workspaces this record type can be connected from. You can make it available for all workspaces or designate specific ones where you can import it.
         For more information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).  
         ******** replace screen shot below **********
         ![Create record type box on advanced settings tab](assets/create-record-type-box-advanced-settings-tab.png) 
      -->

1. Klik **sparen**.

   De kaart van het verslagtype op de werkruimte toont een connectiviteitspictogram ![ verbind van ander werkruimtepictogram ](assets/connect-from-other-workspaces-icon.png) in de hoger-juiste hoek om erop te wijzen dat het verslag nu toegankelijk van andere werkruimten is.

1. (Optioneel) Klik op de kaart met recordtype in de werkruimte om de pagina van het recordtype te openen en geef vervolgens het recordtype in de koptekst een andere naam.

1. (Optioneel) Als u een ander recordtype wilt bewerken, vouwt u de pijl omlaag naar rechts van de naam van een recordtype uit, zoekt u naar een recordtype en selecteert u deze pijl wanneer deze in de lijst wordt weergegeven.

   ![ het type van Verslag drop-down op verslagtype pagina met onderzoeksdoos ](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
