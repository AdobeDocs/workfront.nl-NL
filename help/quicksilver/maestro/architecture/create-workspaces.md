---
title: Werkruimten maken
description: Een werkruimte is een inzameling van verslagtypes die door een team worden gebruikt en vertegenwoordigt de het werklevenscyclus van het team. U kunt werkruimten volledig aanpassen in Adobe Workfront Planning. Recordtypen worden ingedeeld in secties in een werkruimte.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: eaf1cd4142b83a42d068e2d02fe673fa4dd25769
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Werkruimten maken

{{maestro-important-intro}}

In de Planning van Adobe Workfront, zijn de werkruimten gecentraliseerde plaatsen voor teams om het werk te plannen.

Een werkruimte is een inzameling van verslagtypes die door een team worden gebruikt en vertegenwoordigt de het werklevenscyclus van het team. U kunt werkruimten volledig aanpassen in Adobe Workfront Planning.

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-overeenkomst</p></td>
   <td>
<p>Uw organisatie moet zijn ingeschreven voor het gesloten bètaprogramma voor Adobe-werknemers. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-plan</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td>
   <td>
   <p>Nieuw: Standaard</p>
   of
   <p>Huidig: Plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>U ontvangt beheermachtigingen voor de werkruimten die u maakt. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>U moet het gebied van de Planning aan uw lay-outmalplaatje toevoegen. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Voor meer informatie over toegangsvereisten, zie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Overwegingen over werkruimten

* U kunt werkruimten voor specifieke organisatorische eenheden binnen uw organisatie tot stand brengen, om de unieke manier aan te passen elke eenheid werkt.
* De recordtypen die een werkruimte bevat, moeten de levenscyclus van een organisatie weerspiegelen.
* Wanneer u een werkruimte maakt, hebt u alleen de toestemming om de werkruimte te openen en te beheren. U moet het met andere gebruikers delen opdat zij met u in de zelfde ruimte kunnen samenwerken. Zie voor meer informatie [Een werkruimte delen](/help/quicksilver/maestro/access/share-workspaces.md). Systeembeheerders kunnen alle werkruimten beheren, zelfs de werkruimten die ze niet hebben gemaakt.
* U kunt het volgende hebben:

   * Tot 50 secties in één werkruimte.
   * Maximaal 1.000 recordtypen uit alle secties in één werkruimte. Alle recordtypen zijn uniek voor elke werkruimte. <!--this might change-->
   * Tot 1.000 werkruimten in de Workfront-instantie van uw organisatie.


## Een werkruimte maken

{{step1-to-maestro}}

1. (Voorwaardelijk) Als u geen werkruimten in uw omgeving hebt, klikt u op **Werkruimte maken**

   Of klik in een bestaande werkruimte op de knop voor het naar beneden wijzen rechts van de naam van de werkruimte en klik vervolgens op **Werkruimte maken**.

   ![](assets/workspace-drop-down-right-menu.png)

   Hiermee opent u het gedeelte Workspaces van Workfront Planning.
1. (Optioneel en voorwaardelijk) Klik op **Voorvertoning** binnen een van de volgende vooraf gedefinieerde werkruimtjablonen:

   * Marketing management
   * Verkoopbeheer
   * Productbeheer

   Er is een indicatie van welke operationele recordtypen, taxonomieën en hoeveel velden aan elke sjabloon zijn gekoppeld.

   ![](assets/previewing-a-workspace-template.png)

   Voor informatie over de sjablonen van de Workfront Planning-werkruimte raadpleegt u [Lijst met werkruimtemalplaatjes](../architecture/workspace-templates.md).

1. Klikken **Sjabloon gebruiken** om de werkruimte te maken op basis van de geselecteerde sjabloon

   of

   Klikken **Werkruimte maken** om een werkruimte helemaal opnieuw te maken.

   Er wordt een werkruimte gemaakt voor de volgende typen werkruimten:

   * Een lege werkruimte waarin u recordtypen handmatig kunt toevoegen wanneer u een werkruimte maakt.
   * Een werkruimte die is gevuld met voorbeeldrecordtypen die u verder kunt aanpassen wanneer u een van de sjablonen gebruikt.

1. Klik binnen de naam van de werkruimte in de koptekst van de nieuwe werkruimte om de naam ervan te wijzigen en druk vervolgens op Enter

   of

   Klik op de knop **Meer** menu ![](assets/more-menu.png)rechts van de naam van de werkruimte in de koptekst klikt u op **Naam wijzigen**.

1. (Optioneel en voorwaardelijk) Als u de werkruimte hebt gemaakt op basis van een sjabloon, klikt u binnen de naam van het **Operationele recordtypen** of **Taxonomieën** secties

   of

   Houd de naam van een sectie boven en klik vervolgens op de knop **Meer** menu ![](assets/more-menu.png)en klik vervolgens op **Naam wijzigen** om de naam van de sectie te wijzigen.

   >[!TIP]
   >
   >U kunt de naam van elke sectie vanuit elke werkruimte wijzigen, zelfs als u de sectie hebt gemaakt.

1. (Optioneel) Voer een van de volgende handelingen uit om de locatie van een sectie te wijzigen:

   * Houd de muisaanwijzer boven de naam van een sectie en klik op de knop **grijpen** pictogram ![](assets/grab-icon.png)en sleep deze vervolgens naar de rechterkant.
   * Houd de muisaanwijzer boven de naam van een sectie en klik op de knop **Meer** menu ![](assets/more-menu.png)en klik vervolgens op **Omhoog verplaatsen** of **Omlaag verplaatsen**. De sectie wordt omhoog of omlaag verplaatst binnen de werkruimte.

1. (Optioneel) Voer een van de volgende handelingen uit om een nieuwe sectie toe te voegen:

   * Klikken **Sectie toevoegen** onder aan de werkruimte.
   * Houd de muisaanwijzer boven de naam van een sectie en klik op de knop **Meer** menu ![](assets/more-menu.png)en klik vervolgens op **Sectie toevoegen hierboven** of **Sectie toevoegen hieronder**.

1. (Optioneel) Klik op **Recordtype toevoegen** om recordtypen toe te voegen aan de werkruimte in een willekeurige sectie.

   Zie voor meer informatie [Recordtypen maken](../architecture/create-record-types.md).

1. (Optioneel) Ga als volgt te werk om een sectie te verwijderen:

   1. Houd de cursor boven de naam van een sectie en klik vervolgens op de knop **Meer** menu ![](assets/more-menu.png)en klik vervolgens op **Verwijderen**. <!--add screen shot when UI is final?-->
   1. Selecteer een nieuwe sectie om alle recordtypen naar de sectie te verplaatsen en klik vervolgens op **Verwijderen**. <!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      Alle recordtypen worden naar de selectiesectie verplaatst en de sectie wordt verwijderd.
