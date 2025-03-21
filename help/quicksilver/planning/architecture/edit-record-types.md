---
title: Recordtypen bewerken
description: U kunt recordtypen bewerken nadat u deze hebt opgeslagen. Recordtypen zijn de objecttypen voor Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 609396b2eb6413c8f6e84361757f00c2cc5e3ad6
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---


# Recordtypen bewerken

{{planning-important-intro}}

Recordtypen zijn de objecttypen voor Adobe Workfront Planning. U kunt de weergave van recordtypen bewerken die u of iemand anders heeft gemaakt. Voor informatie over het creëren van het verslagtypes van de Planning van Workfront, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

## Toegangsvereisten

+++ Breid uit om toegangsvereisten te bekijken..

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
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden bezeten om tot alle mogelijkheden van de Planning van Workfront toegang te hebben.</p> 
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
   <td>   <p>Rechten beheren in een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
   <p>Alleen systeembeheerders kunnen recordtypen inschakelen om verbinding te maken met andere werkruimten</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
OLD:

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
   <p> Adobe Workfront</p> <p>To connect Adobe Workfront Planning record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Business Platform or the Adobe Admin Console.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->

## Recordtypen bewerken

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de recordtypen wilt bewerken.

   De werkruimtepagina wordt geopend en de recordtypen worden weergegeven.
1. Voer een van de volgende handelingen uit:

   * Beweeg over de kaart van een verslagtype en klik **Meer** menu ![ Meer menu ](assets/more-menu.png) in de hoger-juiste hoek van de kaart van het verslagtype, dan klik **uitgeven**
of
   * Klik een kaart van het verslagtype om de verslagtype pagina te openen, klik **Meer** menu ![ Meer menu ](assets/more-menu.png) rechts van de naam van het verslagtype, dan klik **uitgeven**.

   ![ Meer menuopties van verslagtype kaart ](assets/more-menu-options-from-record-type-card.png)

1. In **geef verslagtype** doos uit, opent het **3} lusje van de Verschijning {door gebrek.**

   ![ Weergavetabblad van recordtekstvak bewerken ](assets/edit-record-type-box-appearance-tab.png)

   Werk de volgende informatie in het **Verschijning** lusje bij:

   * Bewerk indien nodig de naam van het recordtype. <!--did they add a field label for this?-->
   * **Beschrijving**: geef of voeg een beschrijving voor het verslagtype met meer informatie over het uit.
   * Bewerk de kleur en vorm van het pictogram dat aan het recordtype is gekoppeld. Ga als volgt te werk:
      * Selecteer een kleur om het recordtype te identificeren. Dit is de kleur van het pictogram voor recordtype.
      * Selecteer een pictogram in de lijst of typ de naam van een pictogram om te beschrijven wat het vertegenwoordigt en selecteer het pictogram wanneer het wordt weergegeven. Dit is het pictogram van het recordtype. Een bestandspictogram is standaard geselecteerd.

1. (Voorwaardelijk) als u een systeembeheerder bent, klik het **Geavanceerde montages** lusje in **geef verslagtype** doos uit.

   ![ geef recordtype doos geavanceerde montages tabel uit ](assets/edit-record-type-box-advanced-settings-tab.png)

1. (Voorwaardelijk) als systeembeheerder, werk de volgende informatie in de **Geavanceerde montages** tabel bij:

   * **verbind van andere werkruimten**: Selecteer deze knevel om gebruikers toe te staan om met dit verslagtype van andere werkruimten te verbinden. Deze optie is standaard uitgeschakeld.
   * **Systeem wijd**: Selecteer deze optie om gebruikers toe te staan om met dit verslag van alle werkruimten in het systeem te verbinden.
   * **Specifieke werkruimten**: Selecteer deze optie om de werkruimten te beperken waarvan de gebruikers met dit verslagtype kunnen verbinden, dan het drop-down menu uitbreiden en de werkruimten selecteren u gebruikers met dit verslagtype van wilt verbinden. U kunt de naam van een werkruimte typen en deze selecteren wanneer deze in de lijst wordt weergegeven.

1. Klik **sparen**.

   De kaart van het verslagtype op de werkruimte toont een connectiviteitspictogram ![ verbind van ander werkruimtepictogram ](assets/connect-from-other-workspaces-icon.png) in de hoger-juiste hoek om erop te wijzen dat het verslag nu toegankelijk van andere werkruimten is.

1. (Optioneel) Klik op de kaart met recordtype in de werkruimte om de pagina van het recordtype te openen en geef vervolgens het recordtype in de koptekst een andere naam.

1. (Optioneel) Als u een ander recordtype wilt bewerken, vouwt u de pijl omlaag naar rechts van de naam van een recordtype uit, zoekt u naar een recordtype en selecteert u deze pijl wanneer deze in de lijst wordt weergegeven.

   ![ het type van Verslag drop-down op verslagtype pagina met onderzoeksdoos ](assets/record-type-drop-down-on-record-type-page-with-search-box.png)