---
title: GenStudio Workspace beheren in Adobe Workfront Planning
description: De werkruimte van GenStudio for Performance Marketing is beschikbaar in Adobe Workfront Planning wanneer uw bedrijf beide producten heeft aangeschaft en uw exemplaar van Workfront is geïntegreerd met het exemplaar van uw bedrijf GenStudio. U kunt de GenStudio-werkruimte vanuit plannings- en updategegevens weergeven in beide systemen.
hide: true
hidefromtoc: true
exl-id: d6140b05-26c3-4298-a2f9-53695aa021cb
source-git-commit: 4569b5bd004a93396257f3f1f8964831f69399dc
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---


<!--Better metadata, at publishing:
---
title: Manage the GenStudio Workspace in Adobe Workfront Planning
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products and your instance of Workfront is integrated with your company's instance of GenStudio. You can view the GenStudio workspace from Planning and update information in both systems.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->

<!--MUST update the access requirements below - not complete!!!!!!!!!-->

# De GenStudio-werkruimte beheren in Adobe Workfront Planning

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

De werkruimte van Adobe GenStudio for Performance Marketing is beschikbaar in Adobe Workfront Planning wanneer uw bedrijf beide producten heeft aangeschaft en uw exemplaar van Workfront is geïntegreerd met het exemplaar van uw bedrijf GenStudio.

U kunt de GenStudio-werkruimte vanuit plannings- en updategegevens weergeven in beide systemen.

Voor informatie over het gebruiken van en het beheren van de werkruimte van GenStudio van de Marketing van de Prestaties van GenStudio, zie {de Gids van de Gebruiker van 0} Adobe GenStudio for Performance Marketing [.](https://experienceleague.adobe.com/nl/docs/genstudio-for-performance-marketing/user-guide/home)

Voor algemene informatie over GenStudio aan de Planningsintegratie van Workfront, zie [ begonnen met de Planning van Adobe Workfront en de integratie van Adobe GenStudio for Performance Marketing ](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

## Toegangsvereisten

+++ Breid uit om de toegangsvereisten voor de functionaliteit in dit artikel te bekijken. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Elk Adobe Workfront Workflow-pakket</p>
<p>Willekeurig Adobe Workfront-planningspakket</p>

</td> </tr>
<tr> 
   <td role="rowheader"><p>Adobe GenStudio-pakket</p></td> 
   <td> 
<p>??? HEEFT GEN STUDIO EEN PAKKET DAT DIT ONDERSTEUNT?</p>

</td> </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-platform</p></td> 
   <td> 
<p>Het geval van Workfront van uw organisatie moet aan de Verenigde Ervaring van Adobe worden genegeerd om tot de Planning van Workfront te kunnen toegang hebben.</p> 
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio-licentie</p></td> 
   <td><p> ??? VEREIST GEEN STUDIO EEN SPECIFIEKE LICENTIE DIE DIT ONDERSTEUNT?</p>
  </td> 
  </tr> 
  <tr> 
<td> 
   <p> Aanvullende producten</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>   
  <tr> 
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td> 
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p>  
   <p>Configuratie voor GenStudio: ???WAT BEHOEFT HET TOEGANGSNIVEAU VOOR GENS??</p> 
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen*</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Contribute of hoger machtigingen voor een werkruimte en recordtype  </p> </li> 
   <li><p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p></li>
   </ul>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Eventuele machtigingen in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Machtigingen maken in Adobe GenStudio for Performance Marketing om items te maken</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
*Voor meer informatie over Adobe GenStudio for Performance Marketing, zie {de Gids van de Gebruiker van 0} Adobe GenStudio for Performance Marketing [.](https://experienceleague.adobe.com/nl/docs/genstudio-for-performance-marketing/user-guide/home)

+++   

## Overwegingen bij het beheren van een GenStudio-werkruimte in Workfront Planning

* Uw organisatie moet Adobe GenStudio for Performance Marketing aanschaffen voordat u een GenStudio-werkruimte kunt weergeven in Workfront Planning.

* Workfront-gebruikers moeten toegang hebben tot GenStudio om de GenStudio-werkruimte te kunnen zien in Workfront Planning.

* U kunt de volgende gegevens van een GenStudio-werkruimte bijwerken via Workfront Planning:

   * De werkruimte-instellingen bewerken <!--check to see if this is correct? is this editable or read only from Planning??-->
   * De recordtypen en de bijbehorende velden bewerken <!--check on this-->
   * Weergaven delen, bewerken en toevoegen
   * Nieuwe recordtypen toevoegen
   * Records bewerken, toevoegen of verwijderen

* Het bijwerken van de werkruimteconfiguratie, recordtypen, weergaven en velden voor een GenStudio-werkruimte is identiek aan het bijwerken van een Workfront-planningswerkruimte met de bijbehorende elementen.

<!--
## Manage GenStudio workspace from Workfront Planning

CAN YOU DO THIS?? 
- OPTIONS FROM THE WORKSPACE CARD ??
- OPTIONS FROM THE MORE MENU ON A WORKSPACE ??
-->

## GenStudio-recordtypen beheren vanuit Workfront Planning

>[!NOTE]
>
>Alvorens de werkruimte van GenStudio te beheren, zie het artikel [ begonnen worden met de Planning van Workfront en de integratie van GenStudio for Performance Marketing ](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

1. Meld u aan bij Workfront als een gebruiker die ook toegang heeft tot GenStudio.
1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Planning]**.

   De hoofdpagina Workfront Planning wordt geopend.

1. Klik **Andere werkruimten** en vind een werkruimte die een aanwijzing heeft die door het **Systeem** werd gecreeerd en de **GenStudio** markering op zijn kaart heeft.

   ![ de werkruimtekaart van GenStudio met markering ](assets/genstudio-card-with-tag-highlighted.png)

1. Klik de **werkruimtekaart van GenStudio** om de werkruimte van GenStudio in de Planning van Workfront te openen.
1. Standaard worden de volgende GenStudio-recordtypen gemaakt en zichtbaar in Workfront Planning:

   * Campagnes
   * Producten
   * Activering
   * Kanalen
   * Regio&#39;s

   Op de GenStudio-kaart met recordtype staat dat deze oorspronkelijk in GenStudio zijn gemaakt.

   <!--check screen shot-->

   ![ GenStudio verslagtype kaart met markering ](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)

1. Klik op een van de kaarten met recordtypen om records voor dat type weer te geven.

1. Voer een van de volgende handelingen uit:

   * Klik **Aandeel** in de hoger-juiste hoek van de verslagtype pagina, dan klik één van het volgende:
      * **Exemplaar de meningsverbinding** om een verbinding aan het verslagtype te delen
      * **voer de huidige mening** uit om het naar een CSV of een dossier van Excel uit te voeren.
U kunt de tabelweergave alleen exporteren. <!--check on this later; is this true or are there more options in the Share button-->

   * Klik op **+ View** om een weergave voor het GenStudio-recordtype te maken.

     Voor informatie, zie [ verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md) leiden.

   * Klik het **Volledige het schermpictogram** pictogram ![ Open volledige mening in volledig het schermpictogram ](assets/open-full-screen-icon.png) om het even welke mening op volledig-schermwijze te openen.

   * De elementen van een weergave vanuit elke weergave beheren.

     U kunt bijvoorbeeld het filter, de groepen, de sortering en de instellingen van een weergave wijzigen, indien beschikbaar.

     Voor informatie, zie [ verslagmeningen ](/help/quicksilver/planning/views/manage-record-views.md) leiden.

   * Voeg records toe aan de tabel- of tijdlijnweergave.

     U kunt alleen helemaal nieuwe records maken of een CSV- of Excel-bestand importeren.

     Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/create-records.md) creëren.

     Records zijn zowel in Workfront als in GenStudio zichtbaar.

   * Bewerk records inline vanuit de tabelweergave of klik op een record om de detailpagina te openen.

     Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/edit-records.md) uitgeven.

   * Records verwijderen in de tabelweergave.

     Voor informatie, zie [ verslagen van de Schrapping ](/help/quicksilver/planning/records/delete-records.md).

     Verwijderde records kunnen uit de prullenbak van de tabelweergave worden hersteld in Workfront Planning, als ze uit Workfront worden verwijderd.

     Voor informatie, zie [ schrapte verslagen ](/help/quicksilver/planning/records/restore-deleted-records.md) herstellen

   * Houd de cursor boven een veld in de tabelweergave om het veld te sorteren of te verbergen.

     >[!NOTE]
     >
     >U kunt de configuratie van een veld alleen bewerken en meer velden toevoegen als u beheerdersmachtigingen hebt in GenStudio. <!--check to see if this is true??-->
