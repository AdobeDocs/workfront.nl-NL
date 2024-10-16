---
title: Opmerkingen opnemen beheren
description: U kunt aan de verslagen van de Planning van Adobe Workfront samenwerken, door commentaren of antwoorden in het juiste paneel van een verslag toe te voegen. U kunt ook andere wijzigingen bekijken die in de record zijn aangebracht en door het systeem in dit gebied zijn opgenomen.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '981'
ht-degree: 0%

---

# Opnameopmerkingen beheren

{{planning-important-intro}}

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

U kunt aan de verslagen van de Planning van Adobe Workfront samenwerken, door commentaren of antwoorden in het juiste paneel van een verslag toe te voegen. U kunt ook andere wijzigingen bekijken die in de record zijn aangebracht en door het systeem in dit gebied zijn opgenomen.

In het rechterdeelvenster van een record worden de volgende secties weergegeven:

* **Commentaren**: De commentaren van vertoningen en antwoorden gebruikers voegen aan verslagen toe.
* **Geschiedenis**: De systeem-geregistreerde veranderingen van vertoningen die de gebruikers aan de verslaggebieden aanbrengen. Voor meer informatie, zie [ het sectieoverzicht van de Geschiedenis ](/help/quicksilver/planning/records/history-section-overview.md).

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
<li>Eerste</li> 
<li>Ultieme</li></ul> 
<p>Workfront Planning is niet beschikbaar voor oudere Workfront-plannen</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Planning van Adobe Workfront*</p></td> 
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
   <td><p> Medewerker, licht of standaard</p>
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
   <td>   <p>De mening of hogere toestemmingen aan een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij opmerkingen in een record

* U kunt opmerkingen en antwoorden toevoegen aan records in Workfront Planning, in de sectie Opmerkingen van een record.

* Opmerkingen die zijn toegevoegd aan gekoppelde records, worden niet weergegeven op de records waarvan u een koppeling maakt. Bijvoorbeeld, als u op een verslag van het Product van de Planning van Workfront opmerkt dat met een verslag van de Campagne verbonden is, toont de commentaarvertoningen slechts op het verslag van het Product in de Planning van Workfront en niet op het verslag van de Campagne waarvan u koppelt.

* U kunt opmerkingen toevoegen aan Workfront Planning-records die zijn gemaakt als gevolg van een verbinding tussen een record en een object uit een andere toepassing.

  Bijvoorbeeld, kunt u op het verslag van de Planning van Workfront van het Project commentaar geven nadat u de projecten van Workfront met de verslagen van de Planning van Workfront verbindt. Voor meer informatie, zie [ verbindt verslagen ](/help/quicksilver/planning/records/connect-records.md).

* Opmerkingen die zijn toegevoegd aan gekoppelde objecten in andere toepassingen, worden niet weergegeven in Workfront Planning en opmerkingen die zijn toegevoegd aan gekoppelde objecten in Workfront Planning worden niet weergegeven in andere toepassingen.

  Bijvoorbeeld, tonen de commentaren die aan projecten in Workfront worden toegevoegd niet op het zelfde project verbonden aan een campagne in de Planning van Workfront, en de commentaren die aan het verslag van de Planning van Workfront van het project worden toegevoegd tonen niet in Workfront.

* U kunt gebruikers tags toewijzen om hun aandacht te vestigen op een update. Gelabelde gebruikers ontvangen geen melding in de app of een e-mail over uw update. <!--this might change??-->

* U kunt gebruikers tags toewijzen om hun aandacht te vestigen op een update. Gelabelde gebruikers ontvangen een melding in de app of een e-mailmelding over uw update.

  >[!NOTE]
  >
  >   Slechts ontvangen de gebruikers van klanten die met de Adobe Verenigde Ervaring zijn ingegaan zowel een in-app bericht als een e-mailbericht. Om te bepalen of uw bedrijf de Adobe Verenigde Ervaring gebruikt, zie [ Adobe Verenigde Ervaring voor Workfront ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* U kunt een update aan verslagen toevoegen en de geschiedenis van veranderingen van de volgende gebieden van de Planning van Workfront herzien:

   * Van de pagina met recorddetails.
   * Vanuit een weergave, in het vak met recorddetails.

### Opmerkingen over records beheren

{{step1-to-planning}}

1. Klik op de kaart van een werkruimte.

   De werkruimte wordt geopend en de recordtypen worden op kaarten weergegeven.

1. Klik op een opnametype.
De recordtypepagina wordt geopend en alle records van dat type worden weergegeven.

1. Kies een lijstmening van het **drop-down menu van de Mening**.
1. Klik op de naam van een record in de tabelweergave.

   De 1} pagina van de Details van het verslag **{opent.** Het gebied Opmerkingen wordt standaard in het rechtervenster geopend.

1. (Voorwaardelijk) als het juiste paneel niet door gebrek opent, klik **toon Commentaren** ![](assets/show-comments-icon.png) pictogram in de hoger-juiste hoek om de sectie van Commentaren te openen.

1. Begin een commentaar in de **Nieuwe commentaardoos** in te gaan.

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Als u weg navigeert uit de sectie Opmerkingen voordat u klaar bent met typen en verzenden, wordt de opmerking in conceptmodus op de pagina bewaard, zelfs nadat u zich hebt afgemeld en weer hebt aangemeld. Afbeeldingen die aan de opmerking worden toegevoegd, worden ook in het concept opgeslagen. Concepten worden 7 dagen bewaard waarna ze worden verwijderd en kunnen niet worden hersteld. Getekende opmerkingen zijn alleen zichtbaar voor de gebruiker die ze invoert.

1. (Optioneel) Als u een wijziging ongedaan wilt maken of opnieuw wilt uitvoeren, gebruikt u de volgende sneltoetsen:
   * CTRL + Z ( ⌘+z voor Mac) om een wijziging ongedaan te maken
   * CTRL + Y ( ⌘+y voor Mac) om een wijziging opnieuw uit te voeren
1. (Optioneel en voorwaardelijk) Als uw Workfront-instantie deel uitmaakt van de Adobe Unified Experience, voegt u **@** toe, gevolgd door de naam van een gebruiker om een tag toe te wijzen aan iemand in de update. Voor meer informatie, zie de sectie [ Overwegingen over het becommentariëren over een verslag ](#considerations-about-commenting-on-a-record) in dit artikel.

1. (Optioneel) Gebruik de opties op de werkbalk RTF om de tekst op te maken, emoties, koppelingen of afbeeldingen aan de update toe te voegen om de inhoud te verbeteren.

1. Voeg verder opmerkingen toe aan de record.

   Voor meer informatie over het bijwerken van voorwerpen, met inbegrip van de verslagen van de Planning van Workfront, zie [ het werk van de Update ](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

<!--
      >[!TIP]
      >
      >If another user submits a comment to the same item you are updating, there is a red line with a "New" indicator to inform you of the newer comments. 
      >
      >The indicator displays only after the comment was submitted on the item, and not when the comment is still composed. 
      >
      >![](assets/new-line-indicator-comments.png)

1. Click **Submit** to add the update to the record. 
1. (Optional) To edit a comment, click the **More** menu ![](assets/more-menu.png) in the upper-right corner of the comment, then click **Edit**.

   >[!IMPORTANT]
   >
   >You can edit your comment only within 15 minutes from submitting it.  

1. Edit the information in the comment, add or remove images or remove any of the tagged users. An "edited" indicator is added to the left of the comment.
   
      >[!TIP]
      >
      >Comments from the current year do not display the year in the date stamp. Hovering over a timestamp displays the full date, including the year.

1. (Optional and conditional) To search for an existing comment, start typing a keyword in the search box in the upper-right corner of the **Comments** area.     

   ![](assets/search-box-for-comments-area.png)
     
1. (Optional) Click **Reply** or start typing a comment in the **Add reply ...** area, to reply to an existing comment, then follow steps 4-8 above. (**************accurate??***********)

1. (Conditional and optional) If other users have added comments that display outside of the visible area in the Comments section while you were adding your comments, click **View** inside the **new comments banner** at the bottom of the screen  to display these comments.

    ![](assets/new-comments-banner-on-record.png)

    Additional comments display at the bottom of the screen.
  
1. (Optional) Click the **Like** icon to like an update or acknowledge that you read it. The icon updates with the number of likes.
1. (Conditional and optional) If you included additional people in your comment, click the avatars of the users included in the update to display a list of users that the comment is shared with. 
1. (Optional) Click the **More** icon ![](assets/more-menu.png) in the upper-right corner of the comment and click one of the following options, to copy a information from a comment: 

    * **Copy link**: This copies a link to the comment to your clipboard.
    * **Copy body text**: This copies the text of the comment to your clipboard.
    * **Quote reply**: This copies the content of your comment into a new reply. Images are not included in the copied reply. 

    For more information, see [Update work](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md). -->

1. (Optioneel) Klik op het **Meer** pictogram ![](assets/more-menu.png) in de rechterbovenhoek van de opmerking en klik vervolgens op **Verwijderen** om de opmerking te verwijderen.
1. (Optioneel) Klik op het **pictogram ![](assets/hide-comments-icon.png) Opmerkingen verbergen** om het rechterdeelvenster te sluiten.

## Overzicht van de sectie Historie

U kunt de wijzigingen in de record controleren in de sectie Historie van het rechterdeelvenster van een record.

Voor meer informatie, zie [ het sectieoverzicht van de Geschiedenis ](/help/quicksilver/planning/records/history-section-overview.md).
