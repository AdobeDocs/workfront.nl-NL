---
title: Recordtypen maken
description: Recordtypen zijn de objecttypen voor Adobe Workfront Planning. In de Planning van Workfront, kunt u de types van douaneverslag tot stand brengen die de het werkpunten nodig in de levenscyclus van uw organisatie illustreren.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '1073'
ht-degree: 0%

---


<!--this is linked to the UI in an empty workspace screen-->

<!--keep the yellow for cross-workspace functionality till Jan 2026-->

# Recordtypen maken

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Recordtypen zijn de objecttypen voor Adobe Workfront Planning. In de Planning van Workfront, kunt u de types van douaneverslag tot stand brengen die de werk-verwante punten nodig in de levenscyclus van uw organisatie illustreren.

Voor meer informatie over verslagtypes, zie [ overzicht van de types van Verslag ](/help/quicksilver/planning/architecture/overview-of-record-types.md).

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
<p>Verbindbare recordtypen inschakelen: </p>
<ul> 
<li><p>Alle Workfront-pakketten en alle planningspakketten</p></li>
<p>of</p>
<li><p>Workflow en planning voor Prime- en Ultimate-pakketten</p></li></ul>

<p>Globale recordtypen inschakelen:</p>

<ul> 
<li><p>Willekeurig Workfront-pakket en een plannings Plus-pakket</p></li>
<p>of</p>
<li><p>Workflow en planning voor Prime- en Ultimate-pakketten</p></li></ul>
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
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
</tbody> 
</table> -->

## Overwegingen bij het maken van recordtypen

* U kunt recordtypen in een werkruimte op de volgende manieren maken:

   * Automatisch:
      * Wanneer u een werkruimte maakt met een sjabloon.

        Voor informatie, zie [ werkruimten ](/help/quicksilver/planning/architecture/create-workspaces.md) creëren.

      * Wanneer u deze importeert met een CSV- of Excel-bestand.

        Voor meer informatie, zie [ de Types van Verslag tot stand brengen door informatie van een CSV of dossier van Excel ](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md) in te voeren.

     >[!TIP]
     >
     >Wanneer u een recordtype uit een CSV- of Excel-bestand importeert, kunt u ook records en velden importeren.

   * Handmatig:

      * Van nul.

        In dit artikel wordt beschreven hoe u geheel nieuwe recordtypen maakt.

     <!--
        * <span class="preview">By adding them from another workspace</span>
            <span class="preview">For information, see [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md). </span>-->


* U kunt recordtypen binnen een sectie en van de ene sectie van een werkruimte naar de andere verplaatsen. U kunt recordtypen niet van de ene werkruimte naar de andere verplaatsen.

## Recordtypen maken met een werkruimtemalplaatje

U kunt automatisch recordtypen maken wanneer u een werkruimte maakt met een Workfront-planningssjabloon. Elke sjabloon bevat voorbeeldrecordtypen.

Voor informatie over het creëren van werkruimten, zie [ werkruimten ](/help/quicksilver/planning/architecture/create-workspaces.md) creëren.

Voor informatie over welke verslagtypes met elk malplaatje inbegrepen zijn, zie [ Lijst van werkruimtesjablonen ](/help/quicksilver/planning/architecture/workspace-templates.md).

Wanneer u een werkruimte maakt op basis van een sjabloon, worden de recordtypen gegroepeerd in de volgende secties:

* Typen operationele record
* Taxonomieën

U kunt recordtypen handmatig toevoegen in zowel de secties Typen operationele records als Taxonomies. Voor informatie, zie de sectie [ een verslag van kras ](#create-a-record-type-from-scratch) in dit artikel creëren.

## Een geheel nieuw recordtype maken

{{step1-to-planning}}

1. Klik op de werkruimte waar u een recordtype wilt maken.

   of

   Vouw in een werkruimte de pijl omlaag naar rechts uit, zoek naar een werkruimte en selecteer deze wanneer de werkruimte in de lijst wordt weergegeven.
1. (Facultatief) klik **sectie** toevoegen om een nieuwe sectie aan de werkruimte toe te voegen.
1. Klik **voeg verslagtype** toe, dan **voeg manueel** toe.

   Het vak Recordtype toevoegen wordt geopend. <!--update screen shot for preview-->

   ![ voeg verslagtype doos met verschijningsopties ](assets/add-record-type-box-with-appearance-options.png) toe

1. Werk de volgende informatie op het **Verschijning** lusje bij:

   * Vervang &quot;Naamloos recordtype&quot; door de naam van het toekomstige recordtype. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Beschrijving**: Voeg meer informatie over het verslagtype toe.
   * Selecteer een kleur en vorm voor het pictogram dat aan het recordtype is gekoppeld. Ga als volgt te werk:
      * Selecteer een kleur voor het nieuwe recordtype. Dit is de kleur van het pictogram voor recordtype. Grijs is standaard geselecteerd.
      * Selecteer een pictogram in de lijst of typ de naam van een pictogram om te beschrijven wat het vertegenwoordigt en selecteer het pictogram wanneer het wordt weergegeven. Dit is het pictogram van het recordtype. Een bestandspictogram is standaard geselecteerd.

1. (Facultatief en voorwaardelijk) als u een systeembeheerder bent, klik **Geavanceerde montages** en werk de volgende informatie in de **dwars-werkruimtesectie** bij: <!--the info here is duplicated in the Edit record types article-->
   * Laat **toe toestaan verbindend met dit verslagtype in andere werkruimten** het plaatsen: Dit staat werkruimtemanagers toe om met dit verslagtype van andere werkruimten te verbinden.\
     U kunt aangeven van welke werkruimten dit recordtype verbinding kan worden gemaakt. U kunt het voor alle werkruimten ter beschikking stellen of specifieke degenen aanwijzen waar u het kunt invoeren.
Voor meer informatie, zie [ mogelijkheden van de dwars-werkruimte voor verslagtypes ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.


   ![ creeer verslagtype doos op geavanceerde montages tabel ](assets/create-record-type-box-advanced-settings-tab.png)

   <!--replace last point with this when we release global record types; the preview tags might need to be edited, too:
    1. <span class="preview">(Optional and conditional) If you are a system administrator, update the information in the **Cross-workspace settings** tab.</span>
    <span class="preview">For more information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).</span>
    ***********Add screenshot***********
    -->

1. Klik **sparen**.

   De recordtypekaart wordt toegevoegd aan de sectie en de werkruimte die u hebt geselecteerd.
De beschrijving van het recordtype wordt weergegeven op de kaart.

   ![ het typekaart van het Verslag met beschrijving ](assets/record-type-card-with-description.png)

   Als u selecteerde om dit verslag van andere werkruimten aan te sluiten, **verbind van andere ruimten** pictogram ![ verbind van ander spaties pictogram ](assets/connect-from-other-workspaces-icon.png) vertoningen op de verslagkaart.

   <!--<span class="preview">If you configured the cross-workspace capabilities for the record, the **connectable record type** icon ![Connectable record type icon](assets/connect-from-other-workspaces-icon.png) and the **global record type** icon ![Global record type icon](assets/global-icon.png) also display on the card. </span>-->

1. (Facultatief) Beweeg over de kaart van het verslagtype, klik **Meer** pictogram ![ Meer menu ](assets/more-menu.png) in de hoger-juiste hoek, dan klik **uitgeven** om informatie over het verslagtype te wijzigen.

   <!--replace the last point with this at the preview release of global record types:
    <span class="preview">(Optional) Hover over the record type card, click the **More** icon ![More menu](assets/more-menu.png) in the upper-right corner, then click **Edit** or **Settings** to modify information about the record type. </span>
    >[!TIP]
    >
    ><span class="preview">You can access the **Edit** and **Settings** options from the **More** menu of a record type in the record type page.</span>
    -->

1. (Optioneel) Klik op de kaart met het recordtype om de pagina met het recordtype te openen.

   ![ Operationeel verslagtype leeg ](assets/operational-record-type-blank.png)

   De pagina met recordtypen wordt standaard in de tabelweergave weergegeven. De kolommen van de lijst zijn gebieden verbonden aan het nieuwe verslagtype. Elke rij is een unieke record die u moet toevoegen.

   Standaard worden de volgende velden weergegeven in de tabelkolommen van een operationeel recordtype:

   * Naam
   * Beschrijving
   * Begindatum
   * Einddatum
   * Status

1. (Optioneel) Werk de naam van het recordtype bij in de koptekst van de pagina

   of

   Klik het **Meer** pictogram ![ Meer menu ](assets/more-menu.png) rechts van de naam van het verslagtype en klik **uitgeven** om het anders te noemen of de informatie over het te veranderen. Voor meer informatie, zie [ recordtypes ](/help/quicksilver/planning/architecture/edit-record-types.md) uitgeven.

1. (Optioneel) Klik op **+ Nieuwe record** om records van het geselecteerde recordtype toe te voegen. Voor meer informatie, zie [ verslagen ](/help/quicksilver/planning/records/create-records.md) creëren.
1. (Optioneel) Klik op het pictogram **+** rechtsboven in de tabel om meer velden aan het recordtype toe te voegen.

   Voor meer informatie over het creëren van gebieden, zie [ gebieden ](/help/quicksilver/planning/fields/create-fields.md) creëren.

1. (Optioneel) Klik op de pijl die naar links wijst links van de naam van het recordtype in de koptekst om terug te gaan naar de geselecteerde werkruimte.

1. (Optioneel) Klik in de werkruimte op een recordtypekaart en houd deze ingedrukt om het recordtype op een gewenste plaats te slepen of naar een andere sectie te verplaatsen.

   De wijzigingen worden automatisch opgeslagen.

   Raadpleeg de volgende artikelen voor meer informatie over het toevoegen van records, het verwijderen of bewerken van recordtypen of het bijwerken van de weergave op de pagina met recordtypen:

   * [Records maken](/help/quicksilver/planning/records/create-records.md)
   * [Recordtypen verwijderen](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [Recordtypen bewerken](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [ beheer verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md)

## Recordtypen maken door gegevens uit een CSV- of Excel-bestand te importeren

U kunt het volgende importeren wanneer u gegevens importeert uit een CSV- of Excel-bestand:

* Recordtypen
* Records
* Opnamevelden

Voor meer informatie, zie [ de Types van Verslag tot stand brengen door informatie van een CSV of dossier van Excel ](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md) in te voeren.

<!--

<div class="preview">

## Create record types by adding existing ones from another workspace 

You can add record types to a workspace by adding existing ones from another workspace. You can only add record types that have been configured as global record types. 

For information, see [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

</div>

-->