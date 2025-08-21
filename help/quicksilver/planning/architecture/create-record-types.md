---
title: Recordtypen maken
description: Recordtypen zijn de objecttypen voor Adobe Workfront Planning. In de Planning van Workfront, kunt u de types van douaneverslag tot stand brengen die de het werkpunten nodig in de levenscyclus van uw organisatie illustreren.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 4569b5bd004a93396257f3f1f8964831f69399dc
workflow-type: tm+mt
source-wordcount: '1102'
ht-degree: 0%

---


<!--this is linked to the UI in an empty workspace screen-->

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
   <td>   <p>Rechten beheren in een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

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
        * <span class="preview">By importing them from another workspace or adding cross-workspace record types</span>
            <span class="preview">For information, see [Add existing record types](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md). </span>-->


* U kunt recordtypen binnen een sectie en van de ene sectie van een werkruimte naar de andere verplaatsen. U kunt recordtypen niet van de ene werkruimte naar de andere verplaatsen.

## Recordtypen maken met een werkruimtemalplaatje

U kunt automatisch recordtypen maken wanneer u een werkruimte maakt met een Workfront-planningssjabloon. Elke sjabloon bevat voorbeeldrecordtypen.

Wanneer u een werkruimte maakt op basis van een sjabloon, worden de recordtypen gegroepeerd in de volgende secties:

* Typen operationele record
* Taxonomieën

U kunt recordtypen handmatig toevoegen in zowel de secties Typen operationele records als Taxonomies.

Voor informatie over het creëren van werkruimten, zie [ werkruimten ](/help/quicksilver/planning/architecture/create-workspaces.md) creëren.

Voor informatie over welke verslagtypes met elk malplaatje inbegrepen zijn, zie [ Lijst van werkruimtesjablonen ](/help/quicksilver/planning/architecture/workspace-templates.md).

## Een geheel nieuw recordtype maken

{{step1-to-planning}}

1. Klik op de werkruimte waar u een recordtype wilt maken.

   of

   Vouw in een werkruimte de pijl omlaag naar rechts uit, zoek naar een werkruimte en selecteer deze wanneer de werkruimte in de lijst wordt weergegeven.
1. (Facultatief) klik **sectie** toevoegen om een nieuwe sectie aan de werkruimte toe te voegen.
1. Klik **voeg verslagtype** toe, dan **voeg manueel** toe.

   Het vak Recordtype toevoegen wordt geopend.
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

   ![ voeg verslagtype doos met verschijningsopties ](assets/add-record-type-box-with-appearance-options.png) toe

1. Werk de volgende informatie op het **Verschijning** lusje bij:

   * Vervang &quot;Naamloos recordtype&quot; door de naam van het toekomstige recordtype. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Beschrijving**: Voeg meer informatie over het verslagtype toe.
   * Selecteer een kleur en vorm voor het pictogram dat aan het recordtype is gekoppeld. Ga als volgt te werk:
      * Selecteer een kleur voor het nieuwe recordtype. Dit is de kleur van het pictogram voor recordtype. Grijs is standaard geselecteerd.
      * Selecteer een pictogram in de lijst of typ de naam van een pictogram om te beschrijven wat het vertegenwoordigt en selecteer het pictogram wanneer het wordt weergegeven. Dit is het pictogram van het recordtype. Een bestandspictogram is standaard geselecteerd.


   <!--old setting:
    1. (Optional and conditional) If you are a system administrator, click **Advanced settings** and update the following information in the **Connectivity scope** section: 
        * Enable the **Connect from other workspace** setting. When enabled, the record type is accessible and can be connected from other workspaces. 
        * Choose from which workspaces the record type can be accessed. Choose from the following options:
            * **System wide**: Users can connect to this record type from all workspaces where they have manage permissions. 
            * **Specific workspaces**: Add the names of the workspaces where workspace managers can connect to this record type. 
    -->

1. (Facultatief en voorwaardelijk) als u een systeembeheerder bent, klik **Geavanceerde montages** en werk de volgende informatie in de **dwars-werkruimtesectie** bij: <!--the info here is duplicated in the Edit record types article-->
   * Laat **toe toestaan verbindend met dit verslagtype in andere werkruimten** het plaatsen: Dit staat werkruimtemanagers toe om met dit verslagtype van andere werkruimten te verbinden.\
     U kunt aangeven van welke werkruimten dit recordtype verbinding kan worden gemaakt. U kunt het voor alle werkruimten ter beschikking stellen of specifieke degenen aanwijzen waar u het kunt invoeren.
Voor meer informatie, zie [ mogelijkheden van de dwars-werkruimte voor verslagtypes ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.


   ![ creeer verslagtype doos op geavanceerde montages tabel ](assets/create-record-type-box-advanced-settings-tab.png)

   <!--replace last point with this when we release dynamic record types; the preview tags might need to be edited, too:
        <div class="preview">
        1. (Optional and conditional) If you are a system administrator, click **Advanced settings** and update the following information in the **Cross-workspace capability** section: **** the info here is duplicated in the Edit record types article ***
            * Enable the **Allow adding this record type to other workspaces** setting: This allows workspace managers to add this record type to other workspaces. 
                You can designate specific users who can add this record type to other workspaces. 
            * Enable the **Allow connecting to this record type in other workspaces** setting: This allows workspace managers to connect to this record type from other workspaces.  
                You can designate which workspaces this record type can be connected from. You can make it available for all workspaces or designate specific ones where you can import it.
            For more information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).  </div>
            ******** replace screen shot below **********
            ![Create record type box on advanced settings tab](assets/create-record-type-box-advanced-settings-tab.png) 
        -->

1. Klik **sparen**.

   De recordtypekaart wordt toegevoegd aan de sectie en de werkruimte die u hebt geselecteerd.
De beschrijving van het recordtype wordt weergegeven op de kaart.

   ![ het typekaart van het Verslag met beschrijving ](assets/record-type-card-with-description.png)

   Als u selecteerde om dit verslag van andere werkruimten aan te sluiten, **verbind van andere ruimten** pictogram ![ verbind van ander spaties pictogram ](assets/connect-from-other-workspaces-icon.png) vertoningen op de verslagkaart.

   <!--<span class="preview">If you configured the cross-workspace capabilities for the record, the **connect from other spaces** icon ![Connect record type from other spaces icon](assets/connect-from-other-workspaces-icon.png) and the **add to other workspaces** icon ![Add record type to other workspaces](assets/global-icon.png) also display on the card. </span>-->

1. (Facultatief) Beweeg over de kaart van het verslagtype, klik **Meer** pictogram ![ Meer menu ](assets/more-menu.png) in de hoger-juiste hoek, dan klik **uitgeven** om informatie over het verslagtype te wijzigen.
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

## Create record types by importing them from another workspace 

You can add record types to a workspace by importing them from another workspace. You can only add record types that have been configured as centralized record types. 

For information, see [Add existing record types](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).

</div>

-->