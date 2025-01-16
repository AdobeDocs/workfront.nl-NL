---
title: Recordtypen maken
description: Recordtypen zijn de objecttypen voor Adobe Workfront Planning. In de Planning van Workfront, kunt u de types van douaneverslag tot stand brengen die de het werkpunten nodig in de levenscyclus van uw organisatie illustreren.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '1394'
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

+++ Breid uit om toegangsvereisten voor de Planning van Workfront te bekijken.

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
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden genegeerd om tot alle mogelijkheden van de Planning van Workfront te kunnen toegang hebben.</p> 
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td><p> Standaard</p>
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
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p> </td> 
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

      * Wanneer u ze importeert met een Excel- of CSV-bestand.

     >[!TIP]
     >
     >Wanneer u een recordtype uit een Excel- of CSV-bestand importeert, kunt u ook records en velden importeren.

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
1. Klik **recordtype** toevoegen, toen **Nieuw**.

   Het vak Recordtype toevoegen wordt geopend.
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

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

Houd rekening met het volgende wanneer u recordtypen importeert met een Excel- of CSV-bestand:

* Elk blad van het Excel-bestand wordt een recordtype. De naam van het blad wordt de naam van het recordtype.
* Als er slechts één blad is, of als u een Csv- dossier invoert, wordt de naam van het dossier de naam van het verslagtype.
* De kolomkopteksten van elk blad worden de gebieden verbonden aan elk verslagtype.
* Velden zijn uniek voor hun respectievelijke recordtypen.
* Elke rij in elk blad wordt een unieke record die is gekoppeld aan het respectievelijke recordtype.
* Elk blad van het Excel-bestand mag het volgende niet overschrijden:
   * 10.000 rijen
   * 500 kolommen
* Het Excel-bestand mag niet groter zijn dan 5 MB.
* Lege bladen worden niet ondersteund.

Recordtypen importeren met een Excel- of CSV-bestand:

{{step1-to-planning}}

1. Klik op de werkruimte waar u recordtypen wilt maken.

   of

   Vouw in een werkruimte de pijl omlaag naar rechts uit, zoek naar een werkruimte en selecteer deze wanneer de werkruimte in de lijst wordt weergegeven.
1. Klik **toevoegen verslagtype**.
1. Klik **van dossier**.
1. Sleep en laat vallen een Excel of Csv- dossier eerder op uw computer, of klik **Uitgezocht een Csv of dossier van Excel** om voor te doorbladeren.
1. Klik **Voorproef en geef uit**.

   De **Voorproef en geeft** vakvertoningen uit met de volgende informatie:

   * De namen van de bladen of van de toekomstige recordtypen worden weergegeven in het linkerdeelvenster. Workfront Planning selecteert standaard een pictogram en een kleur voor elk nieuw recordtype.
   * Het eerste blad of recordtype wordt geselecteerd en de namen van de bijbehorende velden worden als kolomkoppen weergegeven. Het type van elk gebied wordt geselecteerd door gebrek.
   * Elke rij vertegenwoordigt een nieuwe record. Alleen de eerste 10 records worden weergegeven in het vak Voorbeeld en bewerken.

   ![](assets/preview-and-edit-box.png)

1. (Optioneel) Klik op de naam van elk blad in het linkerdeelvenster om de informatie in het blad te bekijken.

   >[!NOTE]
   >
   >Lege bladen worden niet ondersteund en worden grijs weergegeven.

1. (Optioneel) Schakel de bladen uit die u niet vanuit het linkerdeelvenster wilt importeren.

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   Bladen die u hebt uitgeschakeld, worden weergegeven met een grijze achtergrond.

1. (Optioneel) Klik op de pijl omlaag rechts van de kolomkop om een van de volgende handelingen uit te voeren:

   * De naam van een veld wijzigen
   * Verander het **type van Gebied**
   * Werk het gebied **Beschrijving** bij

1. (Voorwaardelijk) na het bijwerken van informatie over het gebied, klik **sparen**.

1. Klik **Invoer** wanneer u bereid bent om uw dossier in te voeren.

   De volgende informatie wordt geïmporteerd in Workfront Planning:

   * Nieuwe recordtypen
   * Nieuwe velden die zijn gekoppeld aan elk recordtype
   * Nieuwe records gekoppeld aan elk recordtype

   U kunt velden en records op de recordtypepagina&#39;s gaan beheren.

   Iedereen met toegang tot de Planning van Workfront kan nu de ingevoerde verslagtypes en hun informatie bekijken en uitgeven.
