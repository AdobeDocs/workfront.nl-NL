---
title: Bestaande recordtypen toevoegen uit een andere Workspace
description: Recordtypen zijn de objecttypen voor Adobe Workfront Planning. In de Planning van Workfront, kunt u een bestaand verslagtype toevoegen dat in een andere werkruimte wordt gecreeerd.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 7d37481fc5b468f6f8ea1fce6ccd7ae064f00251
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Bestaande recordtypen uit een andere werkruimte toevoegen

{{planning-important-intro}}

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

Als werkruimtenmanager, kunt u een verslagtype toevoegen dat in een andere werkruimte aan een werkruimte bestaat die u in de Planning van Adobe Workfront beheert.

Een werkruimtemanager moet eerst een recordtype aanwijzen als een globaal recordtype voordat u dit kunt toevoegen aan werkruimten die u als een bestaand recordtype beheert. Workspace-managers kunnen een recordtype als globaal aanwijzen wanneer ze deze maken of bewerken, door de instellingen voor de werkruimte van het recordtype te definiëren.

Voor informatie, zie [ mogelijkheden van de dwars-werkruimte voor verslagtypes ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.

In dit artikel wordt beschreven hoe u een recordtype uit een bestaand recordtype kunt toevoegen en hoe u het kunt verwijderen als het niet meer nodig is.

Alvorens verslagen aan een werkruimte van een globaal verslagtype toe te voegen, zie ook het artikel [ overzicht van de types van het interwerkruimterecord ](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).


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
<ul><li><p>Willekeurig Workfront-pakket</p></li>
<p>en</p>
<li><p>Willekeurig planningspakket om verbindingbare recordtypen te maken</p></li>
<li><p>Een Plannings plus pakket om globale verslagtypes tot stand te brengen</p></li>
</ul>
Of:
<ul><li><p>Een Prime- of Ultimate-workflowpakket</p> </li>
en
<li><p>Een planningpakket voor Prime of Ultimate</p></li></ul>
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningspakket wordt opgenomen. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Rechten beheren in een werkruimte en op het recordtype </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr>  
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Een recordtype maken door een bestaand type uit een andere werkruimte toe te voegen

>[!NOTE]
>
>Zorg ervoor dat er ten minste één recordtype is opgegeven dat globaal is in ten minste één andere werkruimte.

1. Begin creërend een verslagtype, zoals die in het artikel [ wordt beschreven creeer verslagtypes ](/help/quicksilver/planning/architecture/create-record-types.md), dan klik **voegt bestaand** toe. <!--check this - the option might have been renamed in the UI-->

   ![ Modal om verslagtype met optie toe te voegen van een andere werkruimte ](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

   >[!TIP]
   >
   >Wanneer er geen verslagtypes zijn die worden gevormd om aan andere werkruimten in uw systeem worden toegevoegd, **voegt bestaande** optie toe toont niet.

1. Klik **verdergaan**.
1. In **kies het verslagtype** doos, klik de kaart voor het verslagtype dat u van een bestaande werkruimte wilt toevoegen, dan klik **toevoegen**.

   Het verslagtype wordt toegevoegd aan de werkruimte u selecteerde en **globale verslagtype** pictogram ![](assets/global-icon.png) vertoningen op de kaart van het verslagtype.

   De volgende dingen doen zich voor:

   * De volgende informatie wordt ook toegevoegd van het bestaande algemene recordtype:

      * Alle oorspronkelijke velden
      * Alle recordverbindingen
   * U kunt records weergeven die zijn toegevoegd vanuit andere werkruimten die hetzelfde algemene recordtype gebruiken, alleen als u ten minste weergavemachtigingen hebt voor die werkruimten.
   * Het read-only **Workspace** gebied wordt toegevoegd aan de nieuwe lijst van het verslagtype mening. In het veld wordt de werkruimte weergegeven waarin elke record is gemaakt.

     >[!NOTE]
     >
     >U kunt de weergave, aanvullende instellingen of originele velden van het nieuwe recordtype niet bewerken. U kunt het recordtype en alle oorspronkelijke velden en instellingen alleen vanuit de oorspronkelijke werkruimte bewerken.

1. (Optioneel) Klik en sleep het nieuwe recordtype naar een willekeurige sectie in de werkruimte.

<!--This will be released later with another epic: 
1. In the table view, click the **+** icon in the upper-right corner to add new fields. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.
-->

&lt;!—controleren met Lilit of wij automatiseringen of aanvraagformulieren aan secundaire globale RTs kunnen toevoegen???-voeg stap met verbindingen aan die artikelen toe als/ wanneer ja—>

## Een algemeen recordtype uit een secundaire werkruimte verwijderen

U kunt een recordtype dat u hebt toegevoegd uit een andere werkruimte verwijderen als u dit niet meer nodig hebt. Als u deze verwijdert, wordt deze alleen verwijderd uit de secundaire werkruimte.

Wanneer u een globaal recordtype uit een secundaire werkruimte schrapt, worden het volgende ook geschrapt:

* De records die vanuit de secundaire werkruimte worden toegevoegd.
* De velden die worden toegevoegd vanuit de secundaire werkruimte.

Algemene recordtypen die uit de secundaire werkruimten zijn verwijderd, kunnen niet worden hersteld.

Het oorspronkelijke recordtype blijft in de oorspronkelijke werkruimte en in andere werkruimten waar het is toegevoegd.

Een algemeen recordtype uit een secundaire werkruimte verwijderen:

1. Ga naar het algemene recordtype in de secundaire werkruimte.

1. (Facultatief) klik op **Meer** menu ![ Meer menu ](assets/more-menu.png) op de kaart van het verslagtype, of rechts van de naam van het verslagtype op zijn pagina, dan klik **Schrapping**.
1. (Voorwaardelijk) Type **schrapt** op het verstrekte gebied, dan klik **permanent schrapt**.

   ![ Schrap secundaire globale doos van de verslagtype bevestiging ](assets/delete-secondary-global-record-type.png)

   De volgende dingen doen zich voor:

   * Het recordtype dat is gemaakt van een algemeen recordtype, wordt verwijderd uit de geselecteerde werkruimte.
   * Het oorspronkelijke recordtype en de bijbehorende velden blijven in de oorspronkelijke werkruimte staan.
   * Het recordtype blijft in alle andere werkruimten waar het is toegevoegd.
   * De records en velden die vanuit de huidige werkruimte aan het recordtype zijn toegevoegd, worden verwijderd. Alle andere records die zijn toegevoegd vanuit aanvullende werkruimten waar het algemene recordtype is toegevoegd, blijven behouden. Velden blijven behouden in de werkruimten waar ze zijn toegevoegd.





