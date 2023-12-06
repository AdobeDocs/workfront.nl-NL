---
title: Opnameopmerkingen beheren
description: U kunt samenwerken aan Adobe Maestro-records door updates toe te voegen en vragen of antwoorden te stellen in het gebied Opmerkingen van een record.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 3ffb6fdebb54682abc737e55186850458a133f7c
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Opnameopmerkingen beheren

U kunt samenwerken aan Adobe Maestro-records door updates toe te voegen en vragen of antwoorden te stellen in het gebied Opmerkingen van een record.

## Overwegingen bij opmerkingen in een record

* U kunt opmerkingen en antwoorden toevoegen aan de operationele records en taxonomieën in Maestro, in de sectie Opmerkingen van een record.

* Opmerkingen die zijn toegevoegd aan gekoppelde records, worden niet weergegeven op de records waarvan u een koppeling maakt. Bijvoorbeeld, als u op een Project opmerkt dat met een verslag van de Campagne verbonden is, toont de commentaarvertoningen slechts op het projectverslag in Maestro en niet op het campagneverslag waarvan u koppelt.

* Opmerkingen die zijn toegevoegd aan gekoppelde objecten in andere toepassingen, worden niet weergegeven in Maestro.
Opmerkingen die zijn toegevoegd aan gekoppelde objecten in Maestro, worden niet weergegeven in andere toepassingen.\
  Bijvoorbeeld, tonen de commentaren die aan projecten in Workfront worden toegevoegd niet op het zelfde project verbonden aan een campagne in Maestro.

* U kunt gebruikers tags toewijzen om hun aandacht te vestigen op een update. Gelabelde gebruikers ontvangen geen melding in de app of een e-mail over uw update. U kunt geen tags toewijzen aan teams in een Maestro-commentaar.

  >[!TIP]
  >
  >* Eigenaars van opmerkingen worden niet automatisch gelabeld in een update.
  >
  >* U kunt getagde gebruikers niet verwijderen uit een update wanneer u erop reageert.

* U kunt een update aan verslagen van de volgende gebieden van Maestro toevoegen:

   * Van de pagina van Details.

  <!--* From the table view.-->

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe</p> </td>
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
   <td role="rowheader">Toegangsniveau</td>
   <td> <p>Alle</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Lay-outsjabloon</td>
   <td> <p>Uw systeembeheerder moet het gebied Maestro in uw lay-outmalplaatje toevoegen. Zie voor meer informatie <a href="../access/grant-access.md">Toegang verlenen tot Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permissions - replace the table with: **************CHECK ON THE VIEW PERMISSIONS TO THE WORKSPACE; RIGHT NOW, WE SAY THAT VIEW USERS CAN COMMENT BUT THE PAGE BLOWS OUT WHEN I TRY - ASKED PM TO CONFIRM*****************

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

### Opmerkingen over records beheren

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](assets/dots-main-menu.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](assets/lines-main-menu.png) in de linkerbovenhoek klikt u op **[!UICONTROL Maestro]**.

   De laatst geopende werkruimte wordt standaard geopend.
1. Kies een tabelweergave in het menu **Weergave** vervolgkeuzelijst.
1. Klik op de naam van een record in de tabelweergave.

   De record **Details** pagina wordt geopend.

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

