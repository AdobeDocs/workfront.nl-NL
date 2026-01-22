---
title: Recordtypen verwijderen
description: U kunt recordtypen verwijderen wanneer deze niet meer relevant zijn. Als u recordtypen verwijdert, verwijdert u ook alle informatie die is gekoppeld aan de recordtypen, zoals records, velden en weergaven.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 5bccad02f90fd99135b50c5a929913b16cc5b809
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 0%

---


<!--keep the global record type reference in yellow till January 2026-->

# Recordtypen verwijderen

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

U kunt recordtypen verwijderen wanneer deze niet meer relevant zijn.

Als u echter recordtypen verwijdert, wordt ook alle informatie verwijderd die aan de recordtypen is gekoppeld. Voor meer informatie, zie de [ Overwegingen wanneer het schrappen van verslagtypes ](#considerations-when-deleting-record-types) sectie in dit artikel.

Voor informatie over verslagtypes, zie [ overzicht van de types van Verslag ](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
<ul> 
<li><p>Alle Workfront en alle planningspakketten</p></li>
of
<li><p>Willekeurige workflow en planningspakket</p></li></ul>

<p>Globale recordtypen verwijderen:</p>
<ul><li><p>Willekeurig Workfront-pakket en een plannings Plus-pakket</p></li>
of
<li><p>Willekeurige workflow en planningpakket voor Prime of Ultimate</p></li></ul>

<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
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
   <td><p> Standard</p>
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
   <td>   <p>Manage permissions to a workspace and record type</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> 
-->


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

* U kunt geen algemeen recordtype verwijderen dat aan andere werkruimten is toegevoegd.

  Voor meer informatie, zie de sectie [ globale verslagtypes van de Schrapping ](#delete-global-record-types) in dit artikel.

## Recordtypen verwijderen

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de recordtypen wilt verwijderen.

   of

   Vouw in een werkruimte de pijl omlaag naar rechts uit, zoek naar een werkruimte en selecteer deze wanneer de werkruimte in de lijst wordt weergegeven.

   De werkruimte wordt geopend en de recordtypen worden weergegeven.
1. Voer een van de volgende handelingen uit:

   * Beweeg over de kaart van het verslagtype, klik **Meer** menu, toen **Schrapping**.
   * Klik de kaart voor het verslagtype dat u, en van de verslagtype pagina wilt schrappen, **Meer** menu ![ Meer menu ](assets/more-menu.png) aan het recht van de verslagtype naam klikken, dan **Schrapping**.

     >[!TIP]
     >
     >U kunt geen globaal recordtype verwijderen uit de secundaire werkruimte waar het is toegevoegd van de pagina met recordtypen. U kunt deze alleen verwijderen van de kaart met recordtypen in de werkruimte.

     ![ permanent schrapt verslagtype bevestiging ](assets/permanently-delete-record-type-confirmation.png)


1. Het type **schrapt** in de bevestigingsdoos, dan klikt **permanent schrapt**. Dit is niet hoofdlettergevoelig.

   Het geselecteerde recordtype en de bijbehorende velden, bijbehorende records en weergaven worden verwijderd en kunnen niet worden hersteld.

## Algemene recordtypen verwijderen

De volgende scenario&#39;s bestaan wanneer het schrappen van globale verslagtypes:

* Als een recordtype dat als globaal is geconfigureerd, nog niet aan een andere werkruimte is toegevoegd, kunt u het verwijderen uit de oorspronkelijke werkruimte.

* Als een recordtype dat als een globaal recordtype is geconfigureerd, aan ten minste één andere werkruimte is toegevoegd, kunt u het niet verwijderen uit de oorspronkelijke werkruimte. U moet eerst het algemene recordtype verwijderen (door deze te verwijderen) uit de secundaire werkruimten waar ze zijn toegevoegd en vervolgens kunt u het algemene recordtype definitief verwijderen uit de oorspronkelijke werkruimte.

### Een algemeen recordtype uit de oorspronkelijke werkruimte verwijderen

U kunt een recordtype uit de originele werkruimte verwijderen als het niet meer relevant is.

Alle records en velden worden ook verwijderd en kunnen niet worden hersteld.

1. Ga naar het algemene recordtype in de oorspronkelijke werkruimte.

1. (Voorwaardelijk) doe één van het volgende, afhankelijk van of het globale verslagtype aan secundaire werkruimten is toegevoegd:

   * Als het verslagtype niet aan een secundaire werkruimte werd toegevoegd, klik op **Meer** menu ![ Meer menu ](assets/more-menu.png) op de kaart van het verslagtype, of rechts van de naam van het verslagtype op zijn pagina, dan klik **Schrapping**.
   * Als het recordtype aan minstens één andere secundaire werkruimte werd toegevoegd, eerst, ga naar de secundaire werkruimte en schrap het globale verslag van die ruimte.

     Voor informatie, zie de sectie [ een globaal verslagtype van een secundaire werkruimte ](#delete-a-global-record-type-from-a-secondary-workspace) in dit artikel schrappen.

1. (Voorwaardelijk) blijven het schrappen van het verslagtype, zoals die in de sectie [ wordt beschreven de verslagtypes van Schrapping ](#delete-record-types-1) in dit artikel.

   De volgende dingen doen zich voor:

   * Het algemene recordtype wordt verwijderd uit de oorspronkelijke werkruimte en het recordtype, de records en velden kunnen niet worden hersteld.
   * Alle globale verslagen van de secundaire werkruimten en hun verslagen worden ook verwijderd uit deze werkruimte.

### Een algemeen recordtype uit een secundaire werkruimte verwijderen

U kunt een recordtype dat u hebt toegevoegd uit een andere werkruimte verwijderen als u dit niet meer nodig hebt.

Overweeg het volgende:

* Wanneer u een globaal recordtype uit een secundaire werkruimte verwijdert, blijft het recordtype in de oorspronkelijke werkruimte.

* Wanneer u een globaal recordtype uit een secundaire werkruimte schrapt, worden het volgende ook geschrapt:

   * De records die worden toegevoegd vanuit de secundaire werkruimte, worden verwijderd uit de secundaire werkruimte en de oorspronkelijke werkruimte en kunnen niet worden hersteld.

  <!--Coming later: * The fields added from the secondary workspace.-->

* Algemene recordtypen die uit de secundaire werkruimten zijn verwijderd, kunnen niet worden hersteld.

* Het oorspronkelijke recordtype blijft in de oorspronkelijke werkruimte en in andere werkruimten waar het is toegevoegd.

* Weergaven die aan het recordtype in de secundaire werkruimte worden toegevoegd, blijven behouden en zijn zichtbaar in andere werkruimten, als ze met u worden gedeeld.

Een algemeen recordtype uit een secundaire werkruimte verwijderen:

1. Ga naar het algemene recordtype in de secundaire werkruimte.

1. (Facultatief) klik op **Meer** menu ![ Meer menu ](assets/more-menu.png) op de kaart van het verslagtype, dan klik **Schrapping**.
1. (Voorwaardelijk) Type **schrapt** op het verstrekte gebied, dan klik **permanent schrapt**.

   ![ Schrap secundaire globale doos van de verslagtype bevestiging ](assets/delete-secondary-global-record-type.png)

   De volgende dingen doen zich voor:

   * Het recordtype dat is gemaakt op basis van een globaal recordtype, wordt verwijderd uit de geselecteerde secundaire werkruimte.
   * Het oorspronkelijke recordtype met de bijbehorende velden blijft in de oorspronkelijke werkruimte staan.
   * Het recordtype blijft in alle andere werkruimten waar het is toegevoegd.
   * De records <!--and fields--> die vanuit de secundaire werkruimte aan het recordtype zijn toegevoegd, worden verwijderd. Alle andere records die zijn toegevoegd vanuit aanvullende werkruimten waar het algemene recordtype is toegevoegd, blijven behouden in de desbetreffende werkruimte en in de oorspronkelijke werkruimte. &lt;!—Velden blijven behouden in de werkruimten waar ze zijn toegevoegd.


