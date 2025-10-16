---
title: Recordtypen bewerken
description: U kunt recordtypen bewerken nadat u deze hebt opgeslagen. Recordtypen zijn de objecttypen voor Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 2fb95d37c32984e248767993c4858038d27e0590
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 0%

---


# Recordtypen bewerken

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

Recordtypen zijn de objecttypen voor Adobe Workfront Planning. U kunt de weergave van recordtypen bewerken die u of iemand anders heeft gemaakt. Voor informatie over het creëren van het verslagtypes van de Planning van Workfront, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

## Toegangsvereisten

+++ Breid uit om de toegangsvereisten voor de functionaliteit in dit artikel te bekijken. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Alle Workfront- en planningspakketten</p>
<p>Alle Workfront- en planningspakketten</p>
<p><b>OPMERKING</b></p>
<p>Verbindbare recordtypen configureren: </p>
<ul> 
<li><p>Alle Workfront-pakketten en alle planningspakketten</p></li>
<p>of</p>
<li><p>Willekeurige workflow en planningpakket voor Prime of Ultimate</p></li></ul>

<div class="preview">
<p>Globale recordtypen configureren:</p>

<ul> 
<li><p>Willekeurig Workfront-pakket en een plannings Plus-pakket</p></li>
<p>of</p>
<li><p>Willekeurige workflow en planningpakket voor Prime of Ultimate</p></li></ul>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p>

</div>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Machtigingen beheren in een werkruimte</p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr>  
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p> </td> 
  </tr> 

</tbody> 
</table> -->

## Recordtypen bewerken

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de recordtypen wilt bewerken.

   De werkruimtepagina wordt geopend en de recordtypen worden weergegeven.
1. Voer een van de volgende handelingen uit:

   * Beweeg over de kaart van een verslagtype en klik **Meer** menu ![ Meer menu ](assets/more-menu.png) in de hoger-juiste hoek van de kaart van het verslagtype, dan klik **uitgeven**
     <span class="preview"> of **Montages**</span>
of
   * Klik een kaart van het verslagtype om de verslagtype pagina te openen, klik **Meer** menu ![ ](assets/more-menu.png) rechts van de naam van het verslagtype, dan klik **uitgeven** <span class="preview"> of **Montages**</span>.

   <span class="preview">![ Meer menuopties van verslagtype kaart met Montages ](assets/more-menu-options-from-record-type-card-with-settings-link.png)</span>

1. In **geef verslagtype** doos uit, opent het **3} lusje van de Verschijning {door gebrek.**<!--update screen shot below at production-->

   ![ Weergavetabblad van recordtekstvak bewerken ](assets/edit-record-type-box-appearance-tab.png)

   Werk de volgende informatie in het **Verschijning** lusje bij:

   * Bewerk indien nodig de naam van het recordtype. <!--did they add a field label for this?-->
   * **Beschrijving**: geef of voeg een beschrijving voor het verslagtype met meer informatie over het uit.
   * Bewerk de kleur en vorm van het pictogram dat aan het recordtype is gekoppeld. Ga als volgt te werk:
      * Selecteer een kleur om het recordtype te identificeren. Dit is de kleur van het pictogram voor recordtype.
      * Selecteer een pictogram in de lijst of typ de naam van een pictogram om te beschrijven wat het vertegenwoordigt en selecteer het pictogram wanneer het wordt weergegeven. Dit is het pictogram van het recordtype. Een bestandspictogram is standaard geselecteerd.

1. (Facultatief en voorwaardelijk) als u een systeembeheerder bent, klik de **Geavanceerde montages** <span class="preview"> of **dwars-werkruimtemontages**</span> tabel en werk informatie over de dwars-werkruimtemogelijkheden van het verslagtype bij.

   Voor meer informatie, zie [ mogelijkheden van de dwars-werkruimte voor verslagtypes ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen. <!--update screen shot at production - Jan 2026-->

   ![ geef verslagtype doos met geavanceerde montages tabel ](assets/edit-record-type-box-advanced-settings-tab.png) uit

1. Klik **sparen**.

   Als u selecteerde om dit verslag van andere werkruimten te verbinden, **pictogram** verbindbare verslag ![ verbind van ander spaties pictogram ](assets/connect-from-other-workspaces-icon.png) vertoningen op de verslagkaart.

   <span class="preview"> Als u selecteerde om toe te staan toevoegend dit verslag aan andere werkruimten, **Globale 2} pictogram van het verslag** Globale verslagtype ![ vertoningen op de verslagkaart. ](assets/global-icon.png)</span>

1. (Optioneel) Klik op de kaart met recordtype in de werkruimte om de pagina van het recordtype te openen en geef vervolgens het recordtype in de koptekst een andere naam.

1. (Optioneel) Als u een ander recordtype wilt bewerken, vouwt u de pijl omlaag naar rechts van de naam van een recordtype uit, zoekt u naar een recordtype en selecteert u deze pijl wanneer deze in de lijst wordt weergegeven.

   ![ het type van Verslag drop-down op verslagtype pagina met onderzoeksdoos ](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
