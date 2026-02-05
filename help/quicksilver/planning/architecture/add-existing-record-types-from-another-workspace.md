---
title: Bestaande recordtypen toevoegen uit een andere Workspace
description: Recordtypen zijn de objecttypen voor Adobe Workfront Planning. In de Planning van Workfront, kunt u een bestaand verslagtype toevoegen dat in een andere werkruimte wordt gecreeerd.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: c9fa6d97607990710e6c2a74f3b373d06201d721
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 0%

---


# Bestaande recordtypen uit een andere werkruimte toevoegen

{{planning-important-intro}}

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [&#x200B; snelle versies voor uw organisatie &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

Als werkruimtenmanager, kunt u een verslagtype toevoegen dat in een andere werkruimte aan een werkruimte bestaat die u in de Planning van Adobe Workfront beheert.

Een werkruimtemanager moet eerst een recordtype aanwijzen als een globaal recordtype voordat u dit kunt toevoegen aan werkruimten die u als een bestaand recordtype beheert. Workspace-managers kunnen een recordtype als globaal aanwijzen wanneer ze deze maken of bewerken, door de instellingen voor de werkruimte van het recordtype te definiëren.

Voor informatie, zie [&#x200B; mogelijkheden van de dwars-werkruimte voor verslagtypes &#x200B;](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.

In dit artikel wordt beschreven hoe u een recordtype uit een bestaand recordtype kunt toevoegen.

Alvorens verslagen aan een werkruimte van een globaal verslagtype toe te voegen, zie ook het artikel [&#x200B; overzicht van de types van het interwerkruimterecord &#x200B;](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).


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
<ul><li><p>Willekeurig Workfront-pakket en een plannings Plus-pakket</p></li>
of
<li><p>Willekeurige workflow en planningpakket voor Prime of Ultimate</p></p></li></ul>
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

Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul><li><p>Any Workfront package</p></li>
<p>And</p>
<li><p>Any Planning package to create connectable record types</p></li>
<li><p>A Planning Plus package to create global record types</p></li>
</ul>
Or:
<ul><li><p>A Prime or Ultimate Workflow package</p> </li>
And
<li><p>A Planning Prime or Ultimate package</p></li></ul>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
   </td> 

  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and to the record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table>-->

## Een recordtype maken door een bestaand type uit een andere werkruimte toe te voegen

>[!NOTE]
>
>Zorg ervoor dat er ten minste één recordtype is opgegeven dat globaal is in ten minste één andere primaire werkruimte.
>
>Voor informatie, zie [&#x200B; mogelijkheden van de dwars-werkruimte voor verslagtypes &#x200B;](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.

1. Ga naar een werkruimte waar u een recordtype (secundaire werkruimte) wilt creëren.
1. Begin creërend een verslagtype, zoals die in het artikel [&#x200B; wordt beschreven creeer verslagtypes &#x200B;](/help/quicksilver/planning/architecture/create-record-types.md), dan klik **voegt bestaand** toe. <!--check this - the option might have been renamed in the UI-->

   ![&#x200B; Modal om verslagtype met optie toe te voegen van een andere werkruimte &#x200B;](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

   >[!TIP]
   >
   >Wanneer er geen verslagtypes zijn die worden gevormd om aan andere werkruimten in uw systeem worden toegevoegd, **voegt bestaande** optie toe toont niet.

1. Klik **verdergaan**.
1. In **kies het verslagtype** doos, klik de kaart voor het verslagtype dat u van een bestaande werkruimte wilt toevoegen, dan klik **toevoegen**.

   <span class="preview"> het verslagtype wordt toegevoegd aan de secundaire werkruimte die u selecteerde en het **globale verslagtype** pictogram ![&#x200B; Globale verslagpictogram op de secundaire werkruimte &#x200B;](assets/global-icon-secondary-workspace.png) vertoningen op de kaart van het verslagtype. </span>
   <span class="preview"> het globale verslagtype pictogram omvat een pijl wanneer getoond op een verslagtype in de secundaire werkruimte, om erop te wijzen dat het verslagtype van een bestaand verslagtype werd toegevoegd.</span>

   De volgende dingen doen zich voor:

   * De volgende informatie wordt ook toegevoegd van het bestaande algemene recordtype:

      * Alle oorspronkelijke velden
      * Alle recordverbindingen
   * U kunt geen verslagen bekijken die van de originele werkruimte van het verslagtype van de secundaire werkruimte worden toegevoegd.
   * U kunt records die zijn toegevoegd vanuit de oorspronkelijke werkruimte van het recordtype alleen in de oorspronkelijke werkruimte weergeven als u ten minste weergavemachtigingen hebt voor die werkruimte.
   * Het read-only **Workspace** gebied wordt toegevoegd aan de nieuwe lijst van het verslagtype mening. In het veld wordt de werkruimte weergegeven waarin elke record is gemaakt.

     >[!NOTE]
     >
     >U kunt de weergave, aanvullende instellingen of originele velden van het nieuwe recordtype niet bewerken. U kunt het recordtype en alle oorspronkelijke velden en instellingen alleen vanuit de oorspronkelijke werkruimte bewerken.
     >

1. <span class="preview"> (Facultatieve) Bedekking over het globale verslagtype pictogram ![&#x200B; Globaal verslagpictogram op de secundaire werkruimte &#x200B;](assets/global-icon-secondary-workspace.png) om de naam van de originele werkruimte te bekijken waar het verslagtype van werd toegevoegd. </span>
1. (Optioneel) Klik en sleep het nieuwe recordtype naar een willekeurige sectie in de werkruimte.
1. (Facultatief) klik het **Meer** menu op de kaart van het nieuwe verslagtype of rechts van de naam van het verslagtype op zijn pagina, dan klik één van het volgende:

   * **Aandeel** om het verslagtype van de secundaire werkruimte te delen.
   * **Schrapping** om het verslagtype van de secundaire werkruimte te schrappen. Als u recordtypen verwijdert uit de secundaire werkruimte, worden ook records verwijderd die zijn toegevoegd uit de secundaire werkruimte.

     Weergaven die worden toegevoegd vanuit de secundaire werkruimte, worden niet verwijderd. <!--checking with Lilit - not sure if this is by design??-->

   Voor meer informatie, zie de sectie &quot;schrap globale verslagtypes&quot;in het artikel [&#x200B; schrapt verslagtypes &#x200B;](/help/quicksilver/planning/architecture/delete-record-types.md).

<!--This will be released later with another epic: 
1. In the table view, click the **+** icon in the upper-right corner to add new fields. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.
-->

&lt;!—controleren met Lilit of wij automatiseringen of aanvraagformulieren aan secundaire globale RTs kunnen toevoegen???-voeg stap met verbindingen aan die artikelen toe als/ wanneer ja—>







