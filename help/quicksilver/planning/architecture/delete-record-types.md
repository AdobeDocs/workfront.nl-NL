---
title: Recordtypen verwijderen
description: U kunt recordtypen verwijderen wanneer deze niet meer relevant zijn. Als u recordtypen verwijdert, verwijdert u ook alle informatie die is gekoppeld aan de recordtypen, zoals records, velden en weergaven.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 7d37481fc5b468f6f8ea1fce6ccd7ae064f00251
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


<!--keep the global record type reference in yellow till January 2026-->

# Recordtypen verwijderen

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

U kunt recordtypen verwijderen wanneer deze niet meer relevant zijn.

Als u echter recordtypen verwijdert, wordt ook alle informatie verwijderd die aan de recordtypen is gekoppeld. Voor meer informatie, zie de [ Overwegingen wanneer het schrappen van verslagtypes ](#considerations-when-deleting-record-types) sectie in dit artikel.

Voor informatie over verslagtypes, zie [ overzicht van de types van Verslag ](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
   <td><p> Standard</p>
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
   <td>   <p>Machtigingen beheren in een werkruimte en recordtype</p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p></td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


## Overwegingen bij het verwijderen van recordtypen

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* U kunt alleen recordtypen verwijderen uit werkruimten waarvoor u beheerdersmachtigingen hebt.
* Als u recordtypen verwijdert, wordt de volgende informatie verwijderd die aan deze recordtypen is gekoppeld:

   * Alle records van dat type.
   * Alle velden die aan het recordtype zijn gekoppeld.
   * Alle weergaven (inclusief filters, groepen en sorteercriteria) van het recordtype.
* Het recordtype wordt verwijderd uit alle gebruikers die de werkruimte openen.
* U kunt verwijderde recordtypen of de bijbehorende gegevens niet herstellen.
* U wordt aangeraden de velden en records die zijn gekoppeld aan het recordtype dat u wilt verwijderen, opnieuw te maken in een ander recordtype voordat u ze verwijdert.

<!--

<div class="preview">

* You cannot delete a global record type that has been added to other workspaces. 
   
   You must first delete it from the secondary workspaces where it's been added, before you can delete it from its original workspace. 

   Deleting a global record type from their secondary workspaces only remove them, their records, and that workspace's fields from the secondary workspace. It does not delete the global record type from its original workspace.

   For information, see the section "Delete a global record type from a secondary workspace" in the article [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md). 

</div>
-->

## Recordtypen verwijderen

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de recordtypen wilt verwijderen.

   of

   Vouw in een werkruimte de pijl omlaag naar rechts uit, zoek naar een werkruimte en selecteer deze wanneer de werkruimte in de lijst wordt weergegeven.

   De werkruimte wordt geopend en de recordtypen worden weergegeven.
1. Voer een van de volgende handelingen uit:

   * Beweeg over de kaart van het verslagtype, klik **Meer** menu, toen **Schrapping**.
   * Klik de kaart voor het verslagtype dat u, en van de verslagtype pagina wilt schrappen, **Meer** menu ![ Meer menu ](assets/more-menu.png) aan het recht van de verslagtype naam klikken, dan **Schrapping**.

   ![ permanent schrapt verslagtype bevestiging ](assets/permanently-delete-record-type-confirmation.png)

   <!--[!TIP]
   >
   ><span class="preview">You cannot delete global record types added to other workspaces. First, delete the global record types form their secondary workspaces before deleting them from the original workspace.</span>-->


1. Het type **schrapt** in de bevestigingsdoos, dan klikt **permanent schrapt**. Dit is niet hoofdlettergevoelig.

   Het geselecteerde recordtype en de bijbehorende velden, bijbehorende records en weergaven worden verwijderd en kunnen niet worden hersteld.


