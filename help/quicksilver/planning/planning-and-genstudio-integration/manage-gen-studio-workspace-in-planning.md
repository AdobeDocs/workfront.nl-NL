---
title: GenStudio Workspace beheren in Adobe Workfront Planning
description: De werkruimte van GenStudio for Performance Marketing is beschikbaar in Adobe Workfront Planning wanneer uw bedrijf beide producten heeft aangeschaft en uw exemplaar van Workfront is geïntegreerd met het exemplaar van uw bedrijf GenStudio. U kunt de GenStudio-werkruimte vanuit plannings- en updategegevens weergeven in beide systemen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d6140b05-26c3-4298-a2f9-53695aa021cb
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1474'
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

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

De werkruimte van Adobe GenStudio for Performance Marketing is beschikbaar in Adobe Workfront Planning wanneer uw bedrijf beide producten heeft aangeschaft en uw exemplaar van Workfront is geïntegreerd met het exemplaar van uw bedrijf GenStudio.

U kunt de GenStudio-werkruimte vanuit plannings- en updategegevens weergeven in beide systemen.

Voor informatie over het gebruiken van en het beheren van de werkruimte van GenStudio van de Marketing van de Prestaties van GenStudio, zie {de Gids van de Gebruiker van 0} Adobe GenStudio for Performance Marketing [.](https://experienceleague.adobe.com/nl/docs/genstudio-for-performance-marketing/user-guide/home)

Voor algemene informatie over GenStudio aan de Planningsintegratie van Workfront, zie [&#x200B; begonnen met de Planning van Adobe Workfront en de integratie van Adobe GenStudio for Performance Marketing &#x200B;](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

>[!IMPORTANT]
>
>De stappen die in dit artikel worden beschreven, illustreren hoe u de GenStudio-werkruimte kunt bijwerken via Workfront Planning wanneer u beheerdersmachtigingen hebt.
> Niet alle mogelijkheden zijn beschikbaar wanneer u Contribute-machtigingen hebt voor de GenStudio-werkruimte.
>
>Als uw bedrijf meerdere exemplaren van Workfront heeft, krijgen alle gebruikers Contribute-machtigingen voor de GenStudio-werkruimte in Workfront Planning.

## Toegangsvereisten

+++ Breid uit om de toegangsvereisten voor de functionaliteit in dit artikel te bekijken. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Alle Workfront en alle planningspakketten</p>
<p>Willekeurige workflow en planningspakket</p>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
   <tr> 
<td> 
   <p> Aanvullende producten</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing-gebruikersrollen</p></td> 
   <td><p><ul><li>Elke GenStudio-gebruikersrol voor toegang tot campagnes, producten en persoonlijke instellingen</li>
   <li>GenSudio System Manager toegang tot activeringen <!--and Events--></li></ul>
   Voor informatie, zie <a href="https://experienceleague.adobe.com/nl/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles"> de rollen en de toestemmingen van de Gebruiker </a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Rechten voor de GenStudio-werkruimte beheren om nieuwe velden of recordtypen toe te voegen aan de GenStudio-werkruimte</p></li>
   <li><p>Contribute-machtigingen voor de GenStudio-werkruimte voor het toevoegen, bijwerken of verwijderen van records in de GenStudio-werkruimte</p> </li>  
   </ul>
   <p>Geen enkele gebruiker kan GenStudio for Performance Marketing-recordtypen of -velden verwijderen uit de GenStudio-werkruimte in Workfront Planning</p>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Eventuele machtigingen in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Machtigingen maken in Adobe GenStudio for Performance Marketing om items te maken</p></li></ul>
   </td>  
</tbody> 
</table>

Voor informatie over de toegang van de Planning van Adobe Workfront, zie [&#x200B; Adobe Workfront het toegangsoverzicht van de Planning &#x200B;](/help/quicksilver/planning/access/access-overview.md).

Voor meer informatie over Adobe GenStudio for Performance Marketing, zie {de Gids van de Gebruiker van 0} Adobe GenStudio for Performance Marketing [.](https://experienceleague.adobe.com/nl/docs/genstudio-for-performance-marketing/user-guide/home)

+++   

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront package</p>
<p>Any Planning package</p>  

   </td> </tr>
   <tr> 
<td> 
   <p> Additional products</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr> 
   
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
   <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
   <li>GenSudio System Manager to access Activations ****** and Events*********</li></ul>
   For information, see <a href="https://experienceleague.adobe.com/nl/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Manage permissions to the GenStudio workspace to add new fields or record types to the GenStudio workspace</p></li>
   <li><p>Contribute permissions to the GenStudio workspace to add, update, or delete records in the GenStudio workspace</p> </li>  
   </ul>
   <p>No users can remove GenStudio for Performance Marketing record types or fields from the GenStudio workspace in Workfront Planning</p>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Create permissions in Adobe GenStudio for Performance Marketing to create items</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table> -->

## Overwegingen bij het beheren van een GenStudio-werkruimte in Workfront Planning

* Uw organisatie moet Adobe GenStudio for Performance Marketing aanschaffen voordat u een GenStudio-werkruimte kunt weergeven in Workfront Planning.

* Afhankelijk van het aantal Workfront-instanties in uw organisatie, hebt u automatisch de volgende machtigingen voor de GenStudio-werkruimte in Planning:

  <!--this table is also in the Get started article-->

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
      <tr> 
      <td role="rowheader"><p>Eén exemplaar van Workfront</p></td> 
      <td> 
   <p>De GenStudio-werkruimte is zichtbaar in uw exemplaar van Workfront Planning</p>
   <p>Workfront-beheerders hebben beheerdersmachtigingen voor de GenStudio-werkruimte in Planning</p>
   <p>Alle andere gebruikers hebben Contribute toegang tot de GenStudio-werkruimte bij het plannen</p>
   </td> </tr>
      <tr> 
   <td> 
      <p> Meerdere versies van Workfront</p> </td> 
      <td> 
      <p>De GenStudio-werkruimte is zichtbaar vanuit alle Workfront-instanties</p>
   <p>Alle gebruikers met toegang tot GenStudio for Performance Marketing en Workfront Planning beschikken over Contribute-machtigingen voor de GenStudio in Planning</p> </td> 
   </tr>
      </tbody> 
   </table>

* Het bijwerken van de werkruimteconfiguratie, recordtypen, weergaven en velden voor een GenStudio-werkruimte is identiek aan het bijwerken van een Workfront-planningswerkruimte met de bijbehorende elementen.
<!--Is this just preview?? * You can build hierarchies for the record types in the GenStudio workspace. For more information, see [Create workspace hierarchies](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).
* You cannot include GenStudio Brands in a hierarchy. -->

<!--
## Manage GenStudio workspace from Workfront Planning

CAN YOU DO THIS?? 
- OPTIONS FROM THE WORKSPACE CARD ??
- OPTIONS FROM THE MORE MENU ON A WORKSPACE ??
-->

## De GenStudio-werkruimte beheren vanuit Workfront Planning

>[!NOTE]
>
>Alvorens de werkruimte van GenStudio te beheren, zie het artikel [&#x200B; begonnen worden met de Planning van Adobe Workfront en de integratie van Adobe GenStudio for Performance Marketing &#x200B;](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) voor meer informatie.
>

1. Meld u aan bij Workfront als een gebruiker die ook toegang heeft tot GenStudio.

{{step1-to-planning}}

De hoofdpagina Workfront Planning wordt geopend.

1. Klik **Andere werkruimten** en vind een werkruimte die een aanwijzing heeft die door het **Systeem** werd gecreeerd en de **GenStudio** markering op zijn kaart heeft.

   ![&#x200B; de werkruimtekaart van GenStudio met markering &#x200B;](assets/genstudio-card-with-tag-highlighted.png)

1. Klik de **werkruimtekaart van GenStudio** om de werkruimte van GenStudio in de Planning van Workfront te openen.
1. Standaard worden de volgende GenStudio-recordtypen gemaakt en zichtbaar in Workfront Planning:

   * Campagnes
   * Producten
   * Personas
   * Activering
   * Kanalen
   * Regio&#39;s

   Op de GenStudio-kaart met recordtype staat dat deze oorspronkelijk in GenStudio zijn gemaakt.

   <!--check screen shot-->

   ![&#x200B; GenStudio verslagtype kaart met markering &#x200B;](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)

1. Klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png) rechts van de werkruimtenaam, dan klik één van het volgende:

   * **geeft** uit

     Voor informatie, zie [&#x200B; werkruimten &#x200B;](/help/quicksilver/planning/architecture/edit-workspaces.md) uitgeven.
     <!--* **Delete** - this will generate an error message, per Iskuhi, so don't document as an option/ possibility-->

     <!--For information, see [Delete workspaces](/help/quicksilver/planning/architecture/delete-workspaces.md). -->

1. Klik **Aandeel** in de hoger-juiste hoek om de werkruimte met anderen te delen.

   Voor informatie, zie [&#x200B; werkruimten van het Aandeel &#x200B;](/help/quicksilver/planning/access/share-workspaces.md)

   >[!NOTE]
   >
   >De volgende beperkingen voor delen gelden:
   >
   >* U kunt GenStudio-gebruikers niet verwijderen uit de GenStudio-werkruimte nadat u de werkruimte met hen hebt gedeeld.
   >* Als een gebruiker machtigingen heeft in GenStudio, kan de toegang niet worden gewijzigd in Weergeven in Workfront Planning. Ze moeten ten minste Contribute-machtigingen hebben in de GenStudio-werkruimte in Planning.
   >* U kunt geërfte machtigingen voor GenStudio-recordtypen in de GenStudio-werkruimte niet uitschakelen.

1. Klik op een van de kaarten met recordtypen om records voor dat type weer te geven.

   Om het verslagtype, meningen, en gebieden te beheren, zie de sectie [&#x200B; GenStudio verslagtypes van de Planning van Workfront &#x200B;](#manage-genstudio-record-types-from-workfront-planning) in dit artikel beheren.


## Recordtypen, weergaven en records beheren vanuit de GenStudio-werkruimte in Workfront Planning

>[!NOTE]
>
>Alvorens de werkruimte van GenStudio te beheren, zie het artikel [&#x200B; begonnen worden met de Planning van Adobe Workfront en de integratie van Adobe GenStudio for Performance Marketing &#x200B;](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) voor meer informatie.
>

1. Ga naar de werkruimte van GenStudio in de Planning van Workfront en open een verslagtype pagina, zoals die in de sectie [&#x200B; wordt beschreven beheert de werkruimte van GenStudio van de Planning van Workfront &#x200B;](#manage-the-genstudio-workspace-from-workfront-planning) in dit artikel.

1. Klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png) rechts van een verslagtype naam, dan klik één van het volgende:

   * **geeft** uit

     Voor informatie, zie [&#x200B; recordtypes &#x200B;](/help/quicksilver/planning/architecture/edit-record-types.md) uitgeven.
   * **beheert automatiseringen**

     Voor informatie, zie [&#x200B; de automatisering van de Planning van Adobe Workfront &#x200B;](/help/quicksilver/planning/records/configure-automations-to-create-records.md) vormen.
   * **beheer aanvraagformulieren**

     U kunt meerdere aanvraagformulieren maken. De aanvraagformulieren zijn beschikbaar op het gebied Verzoeken van Workfront en u kunt ze ook openbaar of via een koppeling delen.

     Voor informatie, zie [&#x200B; creeer en beheer een verzoekvorm in de Planning van Adobe Workfront &#x200B;](/help/quicksilver/planning/requests/create-request-form.md).

1. Ga als volgt te werk om een weergave of het recordtype te delen:

   * Klik **Aandeel** in de hoger-juiste hoek van de verslagtype pagina, dan klik één van het volgende:
      * **Deel het verslagtype**
Voor informatie, zie [&#x200B; recordtypes van het Aandeel &#x200B;](/help/quicksilver/planning/access/share-record-types.md).
      * **Deel de huidige mening**
Voor informatie, zie [&#x200B; meningen van het Aandeel &#x200B;](/help/quicksilver/planning/access/share-views.md).
      * **Exemplaar de meningsverbinding**
Een koppeling naar de weergave wordt naar het klembord gekopieerd.
      * **Uitvoer de huidige mening**
Voor informatie, zie [&#x200B; verslagen van de Uitvoer van de lijstmening &#x200B;](/help/quicksilver/planning/records/export-records-from-the-table-view.md).

        >[!NOTE]
        >
        >U kunt GenStudio-gebruikers niet verwijderen uit recordtypen in de GenStudio-werkruimte nadat u die werkruimte of de recordtypen met hen hebt gedeeld.

1. Ga als volgt te werk om de recordtypeweergaven te beheren:

   * Klik op **+ View** om een weergave voor het GenStudio-recordtype te maken.

     Voor informatie, zie [&#x200B; verslagmeningen &#x200B;](/help/quicksilver/planning/views/manage-record-views.md) leiden.

   * Klik het **Volledige het schermpictogram** pictogram ![&#x200B; Open volledige mening in volledig het schermpictogram &#x200B;](assets/open-full-screen-icon.png) om het even welke mening op volledig-schermwijze te openen.

   * De elementen van een weergave vanuit elke weergave beheren.

     U kunt bijvoorbeeld het filter, de groepen, de sortering en de instellingen van een weergave wijzigen, indien beschikbaar.

     Voor informatie, zie [&#x200B; verslagmeningen &#x200B;](/help/quicksilver/planning/views/manage-record-views.md) leiden.

1. Voer een van de volgende handelingen uit om records toe te voegen:

   * Klik **Nieuw verslag** van om het even welke mening om verslagen van kras te creëren

   * Records importeren met een Excel- of CSV-bestand in de tabelweergave

   * Klik ergens in de tijdlijn- of kalenderweergave om records toe te voegen.

     Voor informatie, zie [&#x200B; verslagen &#x200B;](/help/quicksilver/planning/records/create-records.md) creëren.

     Records zijn zowel in Workfront als in GenStudio zichtbaar.

     >[!NOTE]
     >
     >U kunt geen records toevoegen voor het recordtype Activations.

1. Voer een van de volgende handelingen uit om records te bewerken:

   * Records inline bewerken vanuit de tabelweergave

   * Klik in een willekeurige weergave op een record om de detailpagina te openen.

     Voor informatie, zie [&#x200B; verslagen &#x200B;](/help/quicksilver/planning/records/edit-records.md) uitgeven.

     De wijzigingen die u aanbrengt in de GenStudio-werkruimte in Planning, zijn direct zichtbaar vanuit GenStudio.

1. Selecteer een verslag in de lijstmening, dan klik **Schrapping**.

   Voor informatie, zie [&#x200B; verslagen van de Schrapping &#x200B;](/help/quicksilver/planning/records/delete-records.md).

   Verwijderde records worden direct uit GenStudio verwijderd.

   >[!TIP]
   >
   >Verwijderde records kunnen worden hersteld uit de tabelweergave Onlangs verwijderd vak in Workfront Planning. Records die uit GenStudio zijn verwijderd, kunnen ook uit de recent verwijderde bin in Workfront Planning worden hersteld.

   Voor informatie, zie [&#x200B; schrapte verslagen &#x200B;](/help/quicksilver/planning/records/restore-deleted-records.md) herstellen

1. Klik op het pictogram + in de rechterbovenhoek van de tabelweergave om het volgende te maken:

   * Velden

     Voor informatie, zie [&#x200B; gebieden &#x200B;](/help/quicksilver/planning/fields/create-fields.md) creëren

   * Verbindingen

     Voor informatie, zie [&#x200B; Connect verslagtypes &#x200B;](/help/quicksilver/planning/architecture/connect-record-types.md)

     Velden die zijn gemaakt in de GenStudio-werkruimte, zijn zichtbaar in de volgende gebieden:

      * Weergaven Workfront Planning
      * Gegevens Workfront-planningsrecord
      * GenStudio-recorddetails

     >[!NOTE]
     >
     >* U kunt alleen meer velden toevoegen als u beheermachtigingen hebt in GenStudio.
     >* Velden die zijn gemaakt in Workfront Planning zijn niet zichtbaar in de lijstweergave in GenStudio.
     >
     >* U kunt elk GenStudio-recordtype verbinden met het Brands GenStudio-recordtype.
     >  De producten en de Persona&#39;s worden verbonden met Merken door gebrek.

1. Houd de muisaanwijzer boven een veld in de tabelweergave en klik op het vervolgkeuzemenu om een van de volgende handelingen uit te voeren:

   * Sorteren op
   * Verbergen
   * De instellingen bewerken

   <!--* Delete it - not possible now, per Iskuhi; the link is there but it will generate an error-->

   <!--GenStudio-native fields are note removed from GenStudio. -->

   >[!NOTE]
   >
   >* U kunt de configuratie van een GenStudio-veld alleen bewerken als u beheerdersmachtigingen hebt in GenStudio.
   >* U kunt een GenStudio-veld niet verwijderen.

<!--Is this just Preview?? Or direct to Prod?? 

## Create workspace hierarchies in the GenStudio workspace

Creating hierarchies in the GenStudio workspace is similar to creating hierarchies in any workspace. 

>[!NOTE]
>
>You cannot add GenStudio Brands to a hierarchy in the GenStudio workspace.

For information, see [Create workspace hierarchies](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md)
-->
