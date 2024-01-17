---
title: Opnameopmerkingen beheren
description: U kunt samenwerken aan Adobe Maestro-records door opmerkingen of antwoorden toe te voegen in het gebied Opmerkingen van een record.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 5f3d5c93c2fc721dda2dd04adac22190ef6a3f29
workflow-type: tm+mt
source-wordcount: '991'
ht-degree: 0%

---


# Opnameopmerkingen beheren

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

U kunt samenwerken aan Adobe Maestro-records door opmerkingen of antwoorden toe te voegen in het gebied Opmerkingen van een record.

## Overwegingen bij opmerkingen in een record

* U kunt opmerkingen en antwoorden toevoegen aan de operationele records en taxonomieën in Maestro, in de sectie Opmerkingen van een record.

* Opmerkingen die zijn toegevoegd aan gekoppelde records, worden niet weergegeven op de records waarvan u een koppeling maakt. Als u bijvoorbeeld een opmerking maakt over een Maestro-productrecord die is gekoppeld aan een campagnerecord, wordt de opmerking alleen weergegeven in de productrecord in Maestro en niet in de campagnerecord van waaruit u een koppeling maakt.

* U kunt opmerkingen toevoegen aan Maestro-records die zijn gemaakt als gevolg van een verbinding tussen een Maestro-record en een object uit een andere toepassing.

  U kunt bijvoorbeeld opmerkingen plaatsen bij het projectmaestro-record nadat u Workfront-projecten hebt verbonden met Maestro-records. Zie voor meer informatie [Connect-records](/help/quicksilver/maestro/records/connect-records.md).

* Opmerkingen die zijn toegevoegd aan gekoppelde objecten in andere toepassingen, worden niet weergegeven in Maestro en opmerkingen die zijn toegevoegd aan gekoppelde objecten in Maestro worden niet weergegeven in andere toepassingen.

  Bijvoorbeeld, tonen de commentaren die aan projecten in Workfront worden toegevoegd niet op het zelfde project verbonden aan een campagne in Maestro, en de commentaren die aan het project Maestro- verslag worden toegevoegd tonen niet in Workfront.

* U kunt gebruikers tags toewijzen om hun aandacht te vestigen op een update. Gelabelde gebruikers ontvangen geen melding in de app of een e-mail over uw update. <!--this might change??-->

* U kunt een update aan verslagen van de volgende gebieden van Maestro toevoegen:

   * Van de pagina van Details.

  <!--* From the table view.-->

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
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles in Maestro. </p>  
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
   <td> <p>Uw Workfront of groepsbeheerder moet het Maestro-gebied aan uw lay-outsjabloon toevoegen. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

### Opmerkingen over records beheren

{{step1-to-maestro}}

De laatst geopende werkruimte wordt standaard geopend.
1. Kies een tabelweergave in het menu **Weergave** vervolgkeuzelijst.
1. Klik op de naam van een record in de tabelweergave.

   De record **Details** pagina wordt geopend. Het gebied Opmerkingen wordt standaard in het rechtervenster geopend.

1. Beginnen met een opmerking in het dialoogvenster **Nieuwe opmerking** doos.

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Als u weg navigeert uit de sectie Opmerkingen voordat u klaar bent met typen en verzenden, wordt de opmerking in conceptmodus op de pagina bewaard, zelfs nadat u zich hebt afgemeld en weer hebt aangemeld. Afbeeldingen die aan de opmerking worden toegevoegd, worden ook in het concept opgeslagen. Concepten worden 7 dagen bewaard waarna ze worden verwijderd en kunnen niet worden hersteld. Getekende opmerkingen zijn alleen zichtbaar voor de gebruiker die ze invoert.

1. (Optioneel) Als u een wijziging ongedaan wilt maken of opnieuw wilt uitvoeren, gebruikt u de volgende sneltoetsen:
   * CTRL + Z ( ⌘+z voor Mac) om een wijziging ongedaan te maken
   * CTRL + Y ( ⌘+y voor Mac) om een wijziging opnieuw uit te voeren
1. (Optioneel) Toevoegen **@** gevolgd door de naam van een gebruiker om iemand in de update van tags te voorzien.
1. (Optioneel) Gebruik de opties op de werkbalk RTF om de tekst op te maken, emoties, koppelingen of afbeeldingen aan de update toe te voegen om de inhoud te verbeteren. Zie de sectie &#39;Rijke tekst gebruiken in een Workfront-update&#39; in het artikel voor meer informatie [Werk bijwerken](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

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
   * **Platte tekst kopiëren** t: hiermee wordt de tekst van de opmerking naar het klembord gekopieerd.
   * **Offerteantwoord**: Hiermee kopieert u de inhoud van uw opmerking naar een nieuw antwoord. Afbeeldingen worden niet opgenomen in het gekopieerde antwoord.

   Zie voor meer informatie [Werk bijwerken](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Optioneel) Klik op de knop **Meer** pictogram ![](assets/more-menu.png) in de rechterbovenhoek van de opmerking klikt u op **Verwijderen** om de opmerking te verwijderen.

