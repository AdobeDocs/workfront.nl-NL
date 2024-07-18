---
title: Werkruimten bewerken
description: U kunt de gegevens van een bestaande werkruimte op dezelfde manier bewerken als de naam ervan wijzigen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: 8a4da96562b18977f56567f0fc5f72b369078432
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Werkruimten bewerken

{{planning-important-intro}}

In de Planning van Adobe Workfront, zijn de werkruimten gecentraliseerde plaatsen voor teams om het werk te plannen.

Een werkruimte is een inzameling van verslagtypes die door een team worden gebruikt en vertegenwoordigt de het werklevenscyclus van het team. U kunt werkruimten volledig aanpassen in Adobe Workfront Planning.

Voor informatie over het creëren van werkruimten, zie [ werkruimten ](/help/quicksilver/planning/architecture/create-workspaces.md) creëren.

Alle wijzigingen die u aanbrengt in een werkruimte, zijn zichtbaar voor iedereen die beschikt over minstens weergavemachtigingen voor de werkruimte.

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
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td>
   <td>
   <p>Nieuw: Standaard</p>
   <p>Huidig: Plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Workfront</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Rechten voor de werkruimte beheren </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>U moet het gebied van de Planning aan uw lay-outmalplaatje toevoegen. Voor informatie, zie <a href="/help/quicksilver/planning/access/access-overview.md"> overzicht van de Toegang </a>. </p>  
</td>
  </tr>

</tbody>
</table>

Voor meer informatie over toegangsvereisten, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Een werkruimte bewerken

{{step1-to-planning}}

1. Klik op een werkruimtekaart om de werkruimte te openen.
1. Klik binnen de naam van de werkruimte in de kopbal van de nieuwe werkruimte om het anders te noemen, dan druk **binnengaan**.
1. Klik **Meer** menu ![](assets/more-menu.png) aan het recht van de werkruimtenaam in de kopbal, dan klik **uitgeven**.

   ![](assets/edit-workspace-box.png)

   Werk de volgende informatie in **uit geeft werkruimte** doos:

   * Voeg een naam voor de werkruimte toe. <!--did they add a label for this field?-->
   * **Beschrijving**: Voeg informatie over de werkruimte toe.
   * Selecteer een pictogram dat u aan de werkruimte wilt koppelen.

1. Klik **sparen** om het Edit werkruimtevakje te sluiten en uw veranderingen toe te passen.

1. (Optioneel) Voer een van de volgende handelingen uit om een nieuwe werkruimtesectie toe te voegen:

   * Klik **toevoegen sectie** bij de bodem van de werkruimte.
   * Beweeg over de naam van een sectie en klik **Meer** menu ![](assets/more-menu.png), dan klik **toevoegen sectie hierboven** of **voeg hieronder sectie toe**.

1. (Optioneel) Voer een van de volgende handelingen uit om de locatie van een sectie te wijzigen:

   * Beweeg over de naam van een sectie en klik **greep** pictogram ![](assets/grab-icon.png), dan belemmering en laat vallen het in de juiste vlek.
   * Beweeg over de naam van een sectie en klik **Meer** menu ![](assets/more-menu.png), dan klik **Beweging omhoog** of **Beweging neer**. De sectie wordt omhoog of omlaag verplaatst binnen de werkruimte.

1. (Optioneel) Ga als volgt te werk om een sectie van een werkruimte te verwijderen:

   1. Beweeg over de naam van een sectie, dan klik **Meer** menu ![](assets/more-menu.png), dan klik **Schrapping**. <!--add screen shot when UI is final?-->
   1. Selecteer een nieuwe sectie om alle verslagtypes aan het te bewegen, dan **Schrapping** te klikken. <!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      Alle recordtypen worden naar de selectiesectie verplaatst en de sectie wordt verwijderd.

1. (Facultatief) klik **recordtype** toevoegen om verslagtypes aan de werkruimte toe te voegen.

   Voor informatie, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

1. (Facultatief) Beweeg over een kaart van het verslagtype, klik **Meer** menu ![](assets/more-menu.png) in de hoger-juiste hoek, dan klik **geef** uit om de verschijning van een verslagtype te wijzigen.

   Voor informatie, zie [ recordtypes ](/help/quicksilver/planning/architecture/edit-record-types.md) uitgeven.

1. (Facultatief) Beweeg over een kaart van het verslagtype, klik **Meer** menu ![](assets/more-menu.png) in de hoger-juiste hoek, dan klik **Schrapping** om een verslagtype te schrappen.

   Voor informatie, zie [ verslagtypes van Schrapping ](/help/quicksilver/planning/architecture/delete-record-types.md).

1. (Optioneel) Klik op een opnametype om het te slepen en neer te zetten op een nieuwe locatie. U kunt recordtypen van de ene werkruimtesectie naar de andere slepen.

   ![](assets/drag-and-drop-record-types-in-a-workspace.png)

1. (Facultatief) klik **Aandeel** in de hoger-juiste hoek van de werkruimte om de werkruimte met anderen te delen.

   Voor informatie, zie [ de werkruimten van het Aandeel ](/help/quicksilver/planning/access/share-workspaces.md).
