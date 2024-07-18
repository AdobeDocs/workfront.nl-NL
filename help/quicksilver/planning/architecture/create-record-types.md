---
title: Recordtypen maken
description: Recordtypen zijn de objecttypen voor Adobe Workfront Planning. In de Planning van Workfront, kunt u de types van douaneverslag tot stand brengen die de het werkpunten nodig in de levenscyclus van uw organisatie illustreren.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 8a4da96562b18977f56567f0fc5f72b369078432
workflow-type: tm+mt
source-wordcount: '1273'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->
<!--this is linked to the UI in an empty workspace screen-->

# Recordtypen maken

{{planning-important-intro}}

Recordtypen zijn de objecttypen voor Adobe Workfront Planning. In de Planning van Workfront, kunt u de types van douaneverslag tot stand brengen die de werk-verwante punten nodig in de levenscyclus van uw organisatie illustreren.

Voor meer informatie over verslagtypes, zie [ overzicht van de types van Verslag ](/help/quicksilver/planning/architecture/overview-of-record-types.md).

## Toegangsvereisten

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
   <p> Product</p> </td>
   <td> Adobe Workfront
   </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-overeenkomst</p></td>
   <td>
<p>Uw organisatie moet zijn ingeschreven in de vroege toegangsfase voor Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-plan</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td>
   <td>
   <p>Huidig: Plan</p>
   of
   <p>Nieuw: Standaard </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Workfront</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Voor informatie, zie <a href="/help/quicksilver/planning/access/access-overview.md"> overzicht van de Toegang </a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Rechten beheren in een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Overwegingen bij het maken van recordtypen

* U kunt recordtypen in een werkruimte op de volgende manieren maken:

   * Automatisch:
      * Wanneer u een werkruimte maakt met een sjabloon.

        Voor informatie, zie [ werkruimten ](/help/quicksilver/planning/architecture/create-workspaces.md) creëren.

      * Wanneer u ze importeert met een Excel- of CSV-bestand.

        >[!IMPORTANT]
        >
        >Deze functie is sinds 21 maart 2024 tijdelijk uitgeschakeld. De functie wordt later ingeschakeld.

     <!--this should not ne known anymore: * When you add objects from another application to a linked record field of a record. This creates a read-only record type in Workfront Planning which is connected to object types from the original application. 
        For information about connecting record types with object types from another application, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).
        For information about connecting objects with records, see [Connect records](/help/quicksilver/planning/records/connect-records.md). -->
   * Handmatig:

      * Van nul.

        In dit artikel wordt beschreven hoe u geheel nieuwe recordtypen maakt.

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
1. Klik **toevoegen verslagtype**.
1. (Voorwaardelijk) wanneer het creëren van verslagtypes door een dossier van Excel of CSV in te voeren wordt toegelaten, klik **van kras**. Anders, voegt **recordtype** doos toe opent.

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Werk de volgende gegevens bij:

   * Vervang &quot;Naamloos recordtype&quot; door de naam van het toekomstige recordtype. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Beschrijving**: Voeg meer informatie over het verslagtype toe.
   * Selecteer een kleur en vorm voor het pictogram dat aan het recordtype is gekoppeld. Ga als volgt te werk:
      * Selecteer een kleur voor het nieuwe recordtype. Dit is de kleur van het pictogram voor recordtype. Grijs is standaard geselecteerd.
      * Selecteer een pictogram in de lijst of typ de naam van een pictogram om te beschrijven wat het vertegenwoordigt en selecteer het pictogram wanneer het wordt weergegeven. Dit is het pictogram van het recordtype. Een bestandspictogram is standaard geselecteerd.

1. Klik **creëren**.

   De recordtypekaart wordt toegevoegd aan de sectie en de werkruimte die u hebt geselecteerd.
De beschrijving van het recordtype wordt weergegeven op de kaart.

   ![](assets/record-type-card-with-description.png)

1. (Facultatief) Beweeg over de kaart van het verslagtype, klik **Meer** pictogram ![](assets/more-menu.png) in de hoger-juiste hoek, dan klik **geeft** uit om informatie over het verslagtype te wijzigen.
1. (Optioneel) Klik op de kaart met het recordtype om de pagina met het recordtype te openen.

   ![](assets/operational-record-type-blank.png)

   De pagina met recordtypen wordt standaard in de tabelweergave weergegeven. De kolommen van de lijst zijn gebieden verbonden aan het nieuwe verslagtype. Elke rij is een unieke record die u moet toevoegen.

   >[!TIP]
   >
   >    Als u een recordtype uit een Excel- of CSV-bestand importeert, worden records ook geïmporteerd.

   Standaard worden de volgende velden weergegeven in de tabelkolommen van een operationeel recordtype:

   * Naam
   * Beschrijving
   * Begindatum
   * Einddatum
   * Status

1. (Optioneel) Werk de naam van het recordtype bij in de koptekst van de pagina

   of

   Klik **Meer** pictogram ![](assets/more-menu.png) aan het recht van de naam van het verslagtype en klik **uitgeven** om het anders te noemen of de informatie over het te veranderen. Voor meer informatie, zie [ recordtypes ](/help/quicksilver/planning/architecture/edit-record-types.md) uitgeven.

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

## Recordtypen maken door een Excel- of CSV-bestand te importeren

>[!IMPORTANT]
>
>Deze functie is sinds 21 maart 2024 tijdelijk uitgeschakeld. De functie wordt later ingeschakeld.

Houd rekening met het volgende wanneer u recordtypen importeert met een Excel- of CSV-bestand:

* Elk blad van het Excel-bestand wordt een recordtype.
* De kolommen van elk blad worden de gebieden verbonden aan elk verslagtype.
* Velden zijn uniek voor hun respectievelijke recordtypen.
* Elke rij in elk blad wordt een unieke record die is gekoppeld aan het respectievelijke recordtype.
* Elk blad van het Excel-bestand mag het volgende niet overschrijden:
   * 50.000 rijen
   * 500 kolommen
* Het Excel-bestand mag niet groter zijn dan 5 MB.
* Lege bladen worden niet ondersteund.

Recordtypen importeren met een Excel-bestand:

{{step1-to-planning}}

1. Klik op de werkruimte waar u recordtypen wilt maken.

   of

   Vouw in een werkruimte de pijl omlaag naar rechts uit, zoek naar een werkruimte en selecteer deze wanneer de werkruimte in de lijst wordt weergegeven.
1. Klik **toevoegen verslagtype**.
1. Klik **Excel/CSV**.
1. Sleep en laat vallen een Excel of Csv- dossier eerder op uw computer, of klik **Uitgezocht een Csv of dossier van Excel** om voor te doorbladeren.
1. Klik **Overzicht uw gegevens**.

   Het vak Voorbeeld en bewerking wordt weergegeven met de volgende informatie:

   * De namen van de bladen of van de toekomstige recordtypen worden weergegeven in het linkerdeelvenster. Workfront Planning selecteert standaard een pictogram en een kleur voor elk nieuw recordtype.
   * Het eerste blad of recordtype wordt geselecteerd en de namen van de bijbehorende velden worden als kolomkoppen weergegeven. Het type van elk gebied wordt geselecteerd door gebrek.
   * Elke rij vertegenwoordigt een nieuwe record. Alleen de eerste 10 records worden weergegeven in het vak Voorbeeld en bewerken.

   ![](assets/preview-and-edit-box.png)

1. (Optioneel) Klik op de naam van elk blad in het linkerdeelvenster om de informatie in het blad te bekijken.

   >[!NOTE]
   >
   >    Lege bladen worden niet ondersteund en worden grijs weergegeven.


1. (Facultatief) klik de **Uitgezochte bladen om** drop-down menu in te voeren en de bladen te schrappen die u niet wilt invoeren.

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   Bladen die u hebt uitgeschakeld, worden weergegeven met een grijze achtergrond.

1. Klik **Invoer** wanneer u bereid bent om uw dossier in te voeren.

   De volgende informatie wordt geïmporteerd in Workfront Planning:

   * Nieuwe recordtypen
   * Nieuwe velden die zijn gekoppeld aan elk recordtype
   * Nieuwe records gekoppeld aan elk recordtype

   U kunt velden en records op de recordtypepagina&#39;s gaan beheren.

   Iedereen met toegang tot de Planning van Workfront kan nu de ingevoerde verslagtypes en hun informatie bekijken en uitgeven. <!--this will change with permissions-->

<!--## Connect record types with object types from another application

You can connect a record type and an object type from another application. This creates a read-only record type in Workfront Planning that corresponds to the object type in the other application. 

For example, you can create record types by connecting Workfront Planning record types with Workfront projects. As a result, the Workfront project object type is imported into Workfront Planning as a read-only record type. By default, the record type is named "Workfront Project." (********************)has this name changed? Lusine wanted to change it at some point***********)
    
You can import the following objects from the following applications: 

* From Workfront:

    * Projects
    * Portfolios
    * Programs
    * Company
    * Group

For more information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 
-->