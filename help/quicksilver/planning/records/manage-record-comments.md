---
title: Opnameopmerkingen beheren
description: U kunt aan de verslagen van de Planning van Adobe Workfront samenwerken, door commentaren of antwoorden in het juiste paneel van een verslag toe te voegen. U kunt ook andere wijzigingen bekijken die in de record zijn aangebracht en door het systeem in dit gebied zijn opgenomen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: f5430d81f1914a3717130de3af54b4b84e0e2d06
workflow-type: tm+mt
source-wordcount: '1170'
ht-degree: 0%

---

# Opnameopmerkingen beheren

{{planning-important-intro}}

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

U kunt aan de verslagen van de Planning van Adobe Workfront samenwerken, door commentaren of antwoorden in het juiste paneel van een verslag toe te voegen. U kunt ook andere wijzigingen bekijken die in de record zijn aangebracht en door het systeem in dit gebied zijn opgenomen.

In het rechterdeelvenster van een record worden de volgende secties weergegeven:

* **Opmerkingen**: Hiermee geeft u opmerkingen en antwoorden weer die gebruikers aan records toevoegen.
* **Historie**: Hiermee geeft u door het systeem opgenomen wijzigingen weer die gebruikers in de recordvelden aanbrengen. Zie voor meer informatie [Overzicht van de sectie Historie](/help/quicksilver/planning/records/history-section-overview.md).

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
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td>
   <td>
   <p>Alle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td>
   <td> <p>Er zijn geen controles van het toegangsniveau in de Planning van Workfront. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Machtigingen voor een werkruimte weergeven of vergroten</a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Zie voor meer informatie <a href="/help/quicksilver/planning/access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


## Overwegingen bij opmerkingen in een record

* U kunt opmerkingen en antwoorden toevoegen aan records in Workfront Planning, in de sectie Opmerkingen van een record.

* Opmerkingen die zijn toegevoegd aan gekoppelde records, worden niet weergegeven op de records waarvan u een koppeling maakt. Bijvoorbeeld, als u op een verslag van het Product van de Planning van Workfront opmerkt dat met een verslag van de Campagne verbonden is, toont de commentaarvertoningen slechts op het verslag van het Product in de Planning van Workfront en niet op het verslag van de Campagne waarvan u koppelt.

* U kunt opmerkingen toevoegen aan Workfront Planning-records die zijn gemaakt als gevolg van een verbinding tussen een record en een object uit een andere toepassing.

  Bijvoorbeeld, kunt u op het verslag van de Planning van Workfront van het Project commentaar geven nadat u de projecten van Workfront met de verslagen van de Planning van Workfront verbindt. Zie voor meer informatie [Connect-records](/help/quicksilver/planning/records/connect-records.md).

* Opmerkingen die zijn toegevoegd aan gekoppelde objecten in andere toepassingen, worden niet weergegeven in Workfront Planning en opmerkingen die zijn toegevoegd aan gekoppelde objecten in Workfront Planning worden niet weergegeven in andere toepassingen.

  Bijvoorbeeld, tonen de commentaren die aan projecten in Workfront worden toegevoegd niet op het zelfde project verbonden aan een campagne in de Planning van Workfront, en de commentaren die aan het verslag van de Planning van Workfront van het project worden toegevoegd tonen niet in Workfront.

* U kunt gebruikers tags toewijzen om hun aandacht te vestigen op een update. Gelabelde gebruikers ontvangen geen melding in de app of een e-mail over uw update. <!--this might change??-->

<!--replace the bullet above with this: * You can tag users to bring their attention to an update. Tagged users receive an in-app notification or an email notification about your update. 
   The following scenario exists:   

   * Adobe Unified Experience users receive both an in-app notification and an email notification. 
   * Users who are not in the Adobe Unified Experience receive only an email notification. 

      For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md)
   
      To determine whether your company is using the Adobe Unified Experience, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
      -->

* U kunt een update aan verslagen toevoegen en de geschiedenis van veranderingen van de volgende gebieden van de Planning van Workfront herzien:

   * Van de pagina met recorddetails.
   * Vanuit een weergave, in het vak met recorddetails.

### Opmerkingen over records beheren

{{step1-to-planning}}

1. Klik op de kaart van een werkruimte.

   De werkruimte wordt geopend en de recordtypen worden op kaarten weergegeven.

1. Klik op een opnametype.
De recordtypepagina wordt geopend en alle records van dat type worden weergegeven.

1. Kies een tabelweergave in het menu **Weergave** vervolgkeuzelijst.
1. Klik op de naam van een record in de tabelweergave.

   De record **Details** pagina wordt geopend. Het gebied Opmerkingen wordt standaard in het rechtervenster geopend.

1. (Voorwaardelijk) Als het rechterdeelvenster niet standaard wordt geopend, klikt u op de knop **Opmerkingen tonen** ![](assets/show-comments-icon.png) in de rechterbovenhoek om de sectie Opmerkingen te openen.

1. Beginnen met een opmerking in het dialoogvenster **Nieuwe opmerking** doos.

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Als u weg navigeert uit de sectie Opmerkingen voordat u klaar bent met typen en verzenden, wordt de opmerking in conceptmodus op de pagina bewaard, zelfs nadat u zich hebt afgemeld en weer hebt aangemeld. Afbeeldingen die aan de opmerking worden toegevoegd, worden ook in het concept opgeslagen. Concepten worden 7 dagen bewaard waarna ze worden verwijderd en kunnen niet worden hersteld. Getekende opmerkingen zijn alleen zichtbaar voor de gebruiker die ze invoert.

1. (Optioneel) Als u een wijziging ongedaan wilt maken of opnieuw wilt uitvoeren, gebruikt u de volgende sneltoetsen:
   * CTRL + Z ( ⌘+z voor Mac) om een wijziging ongedaan te maken
   * CTRL + Y ( ⌘+y voor Mac) om een wijziging opnieuw uit te voeren
1. (Optioneel) Toevoegen **@** gevolgd door de naam van een gebruiker om iemand in de update van tags te voorzien.

   <!--Adobe Unified Experience users can receive an in-app and an email notification when they are tagged. All other users receive an email when they are tagged. For more information, see the section [Considerations about commenting on a record](#considerations-about-commenting-on-a-record) in this article. -->

1. (Optioneel) Gebruik de opties op de werkbalk RTF om de tekst op te maken, emoties, koppelingen of afbeeldingen aan de update toe te voegen om de inhoud te verbeteren. Zie de sectie &#39;Rijke tekst gebruiken in een Workfront-update&#39; in het artikel voor meer informatie [Werk bijwerken](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   >[!TIP]
   >
   >Als een andere gebruiker een opmerking verzendt naar hetzelfde item dat u bijwerkt, wordt er een rode lijn weergegeven met de indicator &quot;Nieuw&quot; om u op de hoogte te brengen van de nieuwere opmerkingen.
   >
   >De indicator wordt alleen weergegeven nadat de opmerking op het item is verzonden, en niet wanneer de opmerking nog steeds wordt samengesteld.
   >
   >![](assets/new-line-indicator-comments.png)

1. Klikken **Verzenden** om de update toe te voegen aan de record.
1. (Optioneel) Als u een opmerking wilt bewerken, klikt u op **Meer** menu ![](assets/more-menu.png) in de rechterbovenhoek van de opmerking klikt u op **Bewerken**.

   >[!IMPORTANT]
   >
   >Je kunt je opmerking alleen binnen 15 minuten bewerken nadat je deze hebt verzonden.

1. Bewerk de informatie in de opmerking, voeg afbeeldingen toe of verwijder afbeeldingen of verwijder een van de getagde gebruikers. Links van de opmerking wordt een indicator &quot;bewerkt&quot; toegevoegd.

   >[!TIP]
   >
   >Opmerkingen van het lopende jaar worden niet in het datumstempel weergegeven. Als u de muis boven een tijdstempel houdt, wordt de volledige datum weergegeven, inclusief het jaar.

1. (Optioneel en voorwaardelijk) Als u naar een bestaande opmerking wilt zoeken, typt u een trefwoord in het zoekvak rechtsboven in het dialoogvenster **Opmerkingen** gebied.

   ![](assets/search-box-for-comments-area.png)

1. (Optioneel) Klik op **Antwoord** of u begint een opmerking te typen in het dialoogvenster **Antwoord toevoegen...** om te reageren op een bestaande opmerking, volgt u stap 4-8 hierboven. <!--(**************accurate??***********)-->

1. (Voorwaardelijk en optioneel) Als andere gebruikers opmerkingen hebben toegevoegd die buiten het zichtbare gebied in de sectie Opmerkingen worden weergegeven terwijl u uw opmerkingen toevoegde, klikt u op **Weergave** in de **banner voor nieuwe opmerkingen** onder aan het scherm om deze opmerkingen weer te geven.

   ![](assets/new-comments-banner-on-record.png)

   Aanvullende opmerkingen worden onder in het scherm weergegeven.

1. (Optioneel) Klik op de knop **leuk** gebruiken om een update te volgen of te bevestigen dat u deze hebt gelezen. Het pictogram wordt bijgewerkt met het aantal ‘like’.
1. (Voorwaardelijk en optioneel) Als u extra personen hebt toegevoegd aan uw opmerking, klikt u op de avatars van de gebruikers die zijn opgenomen in de update om een lijst weer te geven met gebruikers waarmee de opmerking wordt gedeeld.
1. (Optioneel) Klik op de knop **Meer** pictogram ![](assets/more-menu.png) in de rechterbovenhoek van de opmerking en klik op een van de volgende opties om informatie van een opmerking te kopiëren:

   * **Koppeling kopiëren**: Hiermee wordt een koppeling naar de opmerking naar het klembord gekopieerd.
   * **Platte tekst kopiëren**: Hiermee wordt de tekst van de opmerking naar het klembord gekopieerd.
   * **Offerteantwoord**: Hiermee kopieert u de inhoud van uw opmerking naar een nieuw antwoord. Afbeeldingen worden niet opgenomen in het gekopieerde antwoord.

   Zie voor meer informatie [Werk bijwerken](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Optioneel) Klik op de knop **Meer** pictogram ![](assets/more-menu.png) in de rechterbovenhoek van de opmerking klikt u op **Verwijderen** om de opmerking te verwijderen.
1. (Optioneel) Klik op de knop **Opmerkingen verbergen** pictogram ![](assets/hide-comments-icon.png) om het rechterdeelvenster te sluiten.

## Overzicht van de sectie Historie

U kunt de wijzigingen in de record controleren in de sectie Historie van het rechterdeelvenster van een record.

Zie voor meer informatie [Overzicht van de sectie Historie](/help/quicksilver/planning/records/history-section-overview.md).
