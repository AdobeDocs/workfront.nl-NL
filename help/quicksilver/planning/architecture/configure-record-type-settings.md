---
title: Het instellingengebied van een recordtype configureren
description: Naast het bewerken van een recordtype in het vak Recordtype bewerken kunt u ook recordtypen bewerken op de pagina Instellingen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 40891b0e960e38c4fca55eec428a4e3a6397b316
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---


# Het gebied Instellingen van een recordtype configureren

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

U kunt extra montages voor een verslagtype vormen nadat zij in de Planning van Adobe Workfront zijn bewaard.

Afhankelijk van welke mogelijkheden u voor een verslagtype wilt bepalen, kunt u extra montages vormen door één van het volgende te doen:

<!--the above will need to be reworded when we add automations and manage request forms to this area-->

* Ze bewerken

  Voor informatie, zie [ recordtypes ](/help/quicksilver/planning/architecture/edit-record-types.md) uitgeven.

* De pagina Instellingen van een recordtype configureren.

  In dit artikel wordt beschreven hoe u een recordtype kunt bewerken door de bijbehorende pagina Instellingen te configureren.

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
<p>Willekeurig workflowpakket en planningspakket</p>

<p><b>OPMERKING</b></p>

<p>Verbindbare recordtypen configureren:</p>

<ul> 
<li><p>Alle Workfront- en planningspakketten</p></li>
of
<li><p>Elk workflowpakket en een planningpakket voor Prime of Ultimate</p></li></ul>

<div class="preview">

<p>Globale recordtypen configureren:</p>

<ul> 
<li><p>Willekeurig Workfront-pakket en een plannings Plus-pakket</p></li>
of
<li><p>Elk workflowpakket en een planningpakket voor Prime of Ultimate</p></li></ul>
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
</table> 

-->

## Recordtype-informatie configureren op de pagina Instellingen

U kunt de mogelijkheden voor werkruimten voor een recordtype definiëren door de gegevens op de pagina Instellingen te configureren.

<!--the intro above will change when we can configure more in this area -->

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de recordtypen wilt bewerken.

   De werkruimtepagina wordt geopend en de recordtypen worden weergegeven.
1. Voer een van de volgende handelingen uit:

   * Beweeg over de kaart van een verslagtype en klik **Meer** menu ![ Meer menu ](assets/more-menu.png) in de hoger-juiste hoek van de kaart van het verslagtype, dan klik **Montages**

     ![ Meer menuopties van verslagtype kaart ](assets/more-menu-options-from-record-type-card-with-settings-link.png)

     of

   * Klik een kaart van het verslagtype om de verslagtype pagina te openen, klik **Meer** menu ![ ](assets/more-menu.png) rechts van de naam van het verslagtype, dan klik **Montages**.

   <!--update screen shot at prod??-->

   ![ dwars-werkruimte montages op de pagina van Montages ](assets/settings-page-cross-workspace-settings.png)

1. De **sectie van de montages van de dwars-werkruimte** wordt geselecteerd door gebrek.
1. Schakel een van de volgende instellingen in of uit:

   * **staat het toevoegen van dit verslagtype aan andere werkruimten** toe om erop te wijzen dat dit een globaal verslagtype is
   * **staat het verbinden met dit verslagtype in andere werkruimten** toe om erop te wijzen dat dit een connectable verslagtype is.

   De instellingen zijn standaard uitgeschakeld.

   Voor meer informatie, zie [ dwars-werkruimtemogelijkheden voor verslagtypes ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen