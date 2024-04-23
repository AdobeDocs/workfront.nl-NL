---
title: Een omslagafbeelding aan een record toevoegen
description: U kunt recordgegevens bewerken in Adobe Workfront Planning en elke record koppelen aan een omslagafbeelding om de pagina van de record aan te passen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 6bea34403e45c2b50986f79272f7a46959d67c6d
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

<!--update the metadata with real information-->

# Een omslagafbeelding aan een record toevoegen

{{maestro-important-intro}}

U kunt recordgegevens bewerken in Adobe Workfront Planning en elke record koppelen aan een omslagafbeelding om de pagina van de record aan te passen.

U moet recordtypen maken voordat u records kunt maken en bewerken.
Zie voor meer informatie [Recordtypen maken](../architecture/create-record-types.md).

## Toegangsvereisten

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
<p>Uw organisatie moet zijn ingeschreven voor het bètaprogramma Adobe Workfront Planning. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
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
   <td> <p>Er zijn geen toegangscontroles voor de Planning van Workfront </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Contribute of hoger machtigingen voor een werkruimte </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td>  <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p> <p>Zie voor meer informatie <a href="/help/quicksilver/maestro/access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## Overwegingen bij omslagafbeeldingen van recordpagina&#39;s

U kunt de pagina van een record personaliseren door er een omslagafbeelding aan toe te voegen. De afbeelding is uniek voor elke record en is niet van toepassing op alle records van hetzelfde type.

Overweeg het volgende:

* U kunt alleen afbeeldingsbestanden als omslagafbeeldingen toevoegen.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* U kunt een omslagafbeelding aan afzonderlijke records toevoegen vanuit het recordvak in elke weergave of vanaf de recordpagina.
* U kunt omslagafbeeldingen niet inline toevoegen vanuit de tabelweergave.

## Een omslagafbeelding aan een record toevoegen

U kunt een record personaliseren door boven aan het recordvak of de pagina een omslagafbeelding toe te voegen.

{{step1-to-maestro}}

De werkruimte die u als laatste opent.

1. (Optioneel) Klik op de pijl omlaag rechts van de naam van de werkruimte om de werkruimte te selecteren waarvan u de records wilt bijwerken.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.

1. Klik vanuit een weergave van een willekeurig type op de naam van een record

   of

   Klik in de tabelweergave op de knop **Details openen** pictogram ![](assets/open-details-icon-in-table-name-field.png) links van een recordnaam.

   Het vak van de record wordt in de weergave geopend.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >U kunt de **Details openen** pictogram links van het veld Naam van een record alleen in een tabelweergave als het veld Naam een primair veld is.

1. (Optioneel) Klik op de knop **Openen op nieuw tabblad** pictogram ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in de rechterbovenhoek van het recordvak om de pagina van de record op een nieuw tabblad te openen.

   De recordpagina wordt geopend.

   ![](assets/details-page.png)

1. Klik in het recordvak of op de pagina op **omslag toevoegen**. <!--check the casing here; I logged a bug for this-->
De **Omslag van record** wordt geopend.

1. Klikken **Selecteren om te uploaden** en blader naar een afbeelding op uw computer om deze te selecteren, voeg deze toe en klik vervolgens op **Afbeelding gebruiken**.

   De afbeelding wordt boven in het recordvak of op de pagina geüpload en de wijzigingen worden automatisch opgeslagen.

   ![](assets/record-page-with-cover-image.png)

1. (Optioneel) Houd de muisaanwijzer boven de afbeelding en klik op de knop **Meer** menu ![](assets/more-menu.png) in de rechterbenedenhoek van de omslagafbeelding voert u een van de volgende handelingen uit:

   * Klikken **Uploaden** als u de omslagafbeelding wilt vervangen en stap 6 wilt herhalen om een nieuwe afbeelding te uploaden en op te slaan.
   * Klikken **Opnieuw plaatsen** en de **Opnieuw plaatsen** gereedschap ![](assets/reposition-tool-icon.png) om de omslagafbeelding te centreren, klikt u op **Opslaan** wanneer gereed.
   * Klikken **Verwijderen** om de omslagafbeelding te verwijderen.

   Workfront slaat uw wijzigingen automatisch op.