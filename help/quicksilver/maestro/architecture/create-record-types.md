---
title: Operationele recordtypen maken
description: Recordtypen zijn de objecttypen van Adobe Maestro. In Maestro, kunt u de types van douaneverslag tot stand brengen die de het werkpunten nodig in de levenscyclus van uw organisatie illustreren.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 5681b540bceddaae85116b632e968d94761eec0d
workflow-type: tm+mt
source-wordcount: '1189'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# Operationele recordtypen maken

{{maestro-important-intro}}

Recordtypen zijn de objecttypen van Adobe Maestro. In Maestro, kunt u de types van douaneverslag tot stand brengen die de werk-verwante punten nodig in de levenscyclus van uw organisatie illustreren.

De types van verslag kunnen één van het volgende zijn:

* **Typen operationele record**
* **Taxonomieën**

Zie voor meer informatie over Maestro-recordtypen [Overzicht van recordtypen en taxonomieën](../architecture/overview-of-record-types-and-taxonomies.md).

Het creëren van operationele verslagtypes is gelijkaardig aan het creëren van taxonomie verslagtypes. In dit artikel wordt beschreven hoe u operationele recordtypen maakt.

Voor informatie over het maken van taxonomieën raadpleegt u [Startrecordtypen voor taxonomie maken](../architecture/create-a-taxonomy.md).

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
   <td>
   </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-overeenkomst</p></td>
   <td>
<p>Uw organisatie moet zijn ingeschreven voor het afgesloten bètaprogramma van de Adobe Maestro. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
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
   <p>Alle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor Maestro</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het Maestro-gebied aan uw lay-outsjabloon toevoegen. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Machtigingen beheren in een werkruimte</a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Overwegingen bij het maken van recordtypen

* U kunt recordtypen in een werkruimte op de volgende manieren maken:

   * Automatisch:
      * Wanneer u een werkruimte maakt met een sjabloon.

        Zie voor meer informatie [Werkruimten maken](../architecture/create-workspaces.md).
      * Wanneer u ze importeert met een Excel- of CSV-bestand. Dit is niet beschikbaar voor gegevenstypen van taxonomie.
     <!--this should not ne known anymore: * When you add objects from another application to a linked record field of a Maestro record. This creates a read-only record type in Maestro which is connected to object types from the original application. 
        For information about connecting record types with object types from another application, see [Connect record types](/help/quicksilver/maestro/architecture/connect-record-types.md).
        For information about connecting objects with Maestro records, see [Connect records](/help/quicksilver/maestro/records/connect-records.md). -->
   * Handmatig:

      * Van nul.

## Recordtypen maken met een werkruimtemalplaatje

U kunt automatisch recordtypen maken wanneer u een werkruimte maakt met behulp van een sjabloon. Elke Maestro-sjabloon bevat voorbeelden van operationele en taxonomierecordtypen.

Zie voor informatie over het maken van werkruimten [Werkruimten maken](../architecture/create-workspaces.md).

Voor informatie over welke recordtypen in elke sjabloon worden opgenomen, raadpleegt u [Lijst met werkruimtemalplaatjes](../architecture/workspace-templates.md).

## Een geheel nieuw recordtype maken

In dit artikel wordt beschreven hoe u nieuwe operationele recordtypen kunt maken. Het maken van volledig operationele recordtypen is vergelijkbaar met het maken van taxonomieën.

Zie voor meer informatie over taxonomieën [Een taxonomie maken](../architecture/create-a-taxonomy.md).

{{step1-to-maestro}}

De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Breid de pijl omlaag naar rechts uit naar de naam van een bestaande werkruimte en selecteer de werkruimte waarvoor u recordtypen wilt maken.
1. Klikken **Recordtype toevoegen**.
1. (Voorwaardelijk) Als u een operationeel recordtype maakt, klikt u **Van kras**. Deze optie is niet beschikbaar bij het maken van taxonomieën.

   Het vak Recordtype toevoegen wordt geopend.

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Werk de volgende gegevens bij:

   * **Naam recordtype**: Vervang &quot;Naamloos type operationeel record&quot; door de naam van het toekomstige recordtype.
   * **Weergave**: Definieer de kleur en vorm van het pictogram dat aan het recordtype is gekoppeld. Ga als volgt te werk:
      * Selecteer een kleur voor het nieuwe recordtype. Dit is de kleur van het pictogram voor recordtype. Grijs is standaard geselecteerd.
      * Selecteer een pictogram in de lijst of typ de naam van een pictogram om te beschrijven wat het vertegenwoordigt en selecteer het pictogram wanneer het wordt weergegeven. Dit is het pictogram van het recordtype. Een bestandspictogram is standaard geselecteerd.

1. Klik buiten de **Recordtype toevoegen** het recordtype op.

   De kaart met recordtype wordt toegevoegd aan de werkruimte die u hebt geselecteerd.
Het aantal velden dat het recordtype bevat, wordt weergegeven op de kaart.
1. (Optioneel) Klik op de kaart met het recordtype om de pagina met het recordtype te openen.

   ![](assets/operational-record-type-blank.png)

   De pagina met recordtypen wordt standaard in de tabelweergave weergegeven. De kolommen van de lijst zijn gebieden verbonden aan het nieuwe verslagtype. Elke rij is een unieke record die u moet toevoegen.

   Standaard worden de volgende velden weergegeven in de tabelkolommen van een operationeel recordtype:

   * Naam

     Het veld Naam is het enige veld dat automatisch wordt gemaakt voor taxonomieën.
   * Beschrijving
   * Begindatum
   * Einddatum
   * Status

1. (Optioneel) Werk de naam van het recordtype bij in de koptekst van de pagina

   of

   Klik op de knop **Meer** pictogram ![](assets/more-menu.png) rechts van de naam van het recordtype en klik op **Naam wijzigen** om de naam te wijzigen.

1. (Optioneel) Klik op **+ Nieuwe record** records van het geselecteerde recordtype toevoegen. Zie voor meer informatie [Records maken](../records/create-records.md).
1. (Optioneel) Klik op de knop **+** in de rechterbovenhoek van de tabel om meer velden aan het recordtype toe te voegen.

   Zie voor meer informatie over het maken van velden [Velden maken](../fields/create-fields.md).

1. (Optioneel) Klik op de pijl die naar links wijst links van de naam van het recordtype om terug te gaan naar de geselecteerde werkruimte.

   Op de kaart met recordtype wordt het aantal velden en verbindingen weergegeven dat het recordtype bevat.

   ![](assets/campaign-card-with-fields-and-connections-highlighted.png)

   Raadpleeg de volgende artikelen voor meer informatie over het toevoegen van records, het verwijderen of bewerken van recordtypen of het bijwerken van de weergave op de pagina met recordtypen:

   * [Records maken](../records/create-records.md)
   * [Recordtypen verwijderen](../architecture/delete-record-types.md)
   * [Recordtypen bewerken](../architecture/edit-record-types.md)
   * [Recordweergaven beheren](../views/manage-record-views.md)

## Recordtypen maken door een Excel- of CSV-bestand te importeren

Houd rekening met het volgende wanneer u recordtypen importeert met een Excel- of CSV-bestand:

* Elk blad van het Excel-bestand wordt een recordtype in Maestro.
* De kolommen van elk blad worden de gebieden verbonden aan elk verslagtype.
* Velden zijn uniek voor hun respectievelijke recordtypen.
* Elke rij in elk blad wordt een unieke record die is gekoppeld aan het respectievelijke recordtype.
* Elk blad van het Excel-bestand mag het volgende niet overschrijden:
   * 10.000 rijen
   * 500 kolommen
* Het Excel-bestand mag niet groter zijn dan 5 MB.
* Lege bladen worden niet ondersteund.

Recordtypen importeren met een Excel-bestand:

{{step1-to-maestro}}

De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Breid de pijl omlaag naar rechts uit naar de naam van een bestaande werkruimte en selecteer de werkruimte waarvoor u recordtypen wilt maken.
1. Klikken **Recordtype toevoegen**.
1. (Voorwaardelijk) Als u een operationeel recordtype maakt, klikt u **Excel/CSV**.

   >[!NOTE]
   >
   >    Deze optie is niet beschikbaar wanneer u recordtypen voor taxonomieën maakt.

1. Sleep en zet een Excel- of CSV-bestand neer dat eerder op uw computer is opgeslagen, of klik op **Een CSV- of Excel-bestand selecteren** om er een te zoeken.
1. Klikken **Uw gegevens bekijken**.

   Het vak Voorbeeld en bewerking wordt weergegeven met de volgende informatie:

   * De namen van de bladen of van de toekomstige recordtypen worden weergegeven in het linkerdeelvenster. Maestro selecteert standaard een pictogram en een kleur voor elk nieuw recordtype.
   * Het eerste blad of recordtype wordt geselecteerd en de namen van de bijbehorende velden worden als kolomkoppen weergegeven. Het type van elk gebied wordt geselecteerd door gebrek.
   * Elke rij vertegenwoordigt een nieuwe record. Alleen de eerste 10 records worden weergegeven in het vak Voorbeeld en bewerken.

   ![](assets/preview-and-edit-box.png)

1. (Optioneel) Klik op de naam van elk blad in het linkerdeelvenster om de informatie in het blad te bekijken.

   >[!NOTE]
   >
   >    Lege bladen worden niet ondersteund en worden grijs weergegeven.


1. (Optioneel) Klik op de knop **Te importeren bladen selecteren** en deselecteer de bladen die u niet wilt importeren.

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   Bladen die u hebt uitgeschakeld, worden weergegeven met een grijze achtergrond.

1. Klikken **Importeren** als u klaar bent om uw bestand te importeren.

   De volgende informatie wordt ingevoerd in Maestro:

   * Nieuwe recordtypen
   * Nieuwe velden die zijn gekoppeld aan elk recordtype
   * Nieuwe records gekoppeld aan elk recordtype

   U kunt velden en records op de recordtypepagina&#39;s gaan beheren.

   Iedereen met toegang tot Maestro kan nu de geïmporteerde recordtypen en hun informatie bekijken en bewerken. <!--this will change with permissions-->

<!--## Connect record types with object types from another application

You can connect a Maestro record type and an object type from another application. This creates a read-only record type in Maestro that corresponds to the object type in the other application. 

For example, you can create record types by connecting Maestro record types with Workfront projects. As a result, the Workfront project object type is imported into Maestro as a read-only record type. By default, the record type is named "Workfront Project." (********************)has this name changed? Lusine wanted to change it at some point***********)
    
You can import the following objects from the following applications: 

* From Workfront:

    * Projects
    * Portfolios
    * Programs
    * Company
    * Group

For more information, see [Connect record types](../architecture/connect-record-types.md). 
-->