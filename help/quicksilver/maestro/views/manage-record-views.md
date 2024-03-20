---
title: Recordweergaven beheren
description: U kunt records weergeven in een tabel-, tijdlijn- of kalenderweergave wanneer u de Adobe Workfront-planningsmogelijkheden gebruikt.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: e881aa57b5175ce5b559180a2713de0c607b3b1d
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 0%

---

# Recordweergaven beheren

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

Nadat u een recordtype hebt geselecteerd in het gedeelte met planningsmogelijkheden van Adobe Workfront, kunt u alle records van dat type weergeven in de volgende weergaven:

* Tabel

  Zie voor meer informatie [De tabelweergave beheren](../views/manage-the-table-view.md).

* Tijdlijn

  Zie voor meer informatie [De tijdlijnweergave beheren](../views/manage-the-timeline-view.md).

* Kalender

  Zie voor meer informatie [De kalenderweergave beheren](/help/quicksilver/maestro/views/manage-the-calendar-view.md).

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
<p>Uw organisatie moet zijn ingeschreven voor het gesloten bètaprogramma voor Adobe Workfront-planningsmogelijkheden. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
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
   <td role="rowheader">Configuratie op toegangsniveau</td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor de planningsmogelijkheden van Workfront</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Rechten voor de weergave beheren</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Lay-outsjabloon</td>
   <td> <p>Uw systeembeheerder moet het gebied Maestro in uw lay-outmalplaatje toevoegen. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Overwegingen bij het werken met recordweergaven

* Weergaven in het gedeelte met Workfront-planningsmogelijkheden zijn specifiek voor records. U kunt niet dezelfde weergave toepassen op twee verschillende recordtypen.
* Weergaven die u maakt, zijn alleen zichtbaar voor u en gebruikers met wie u de weergaven deelt.
* Het bouwen van meningen voor operationele verslagtypes is identiek aan het bouwen van meningen voor taxonomie verslagtypes.
* Wanneer u een weergave wijzigt of verwijdert, wordt deze gewijzigd en verwijderd voor alle gebruikers die machtigingen hebben voor de weergave.
* De volgende elementen zijn uniek voor elke recordweergave:

   * Filter
   * Groepering
   * Sorteren

  <!-- some of these are not available in all of the views - edit above-->

  Wanneer u bijvoorbeeld een filter maakt in een tabelweergave, zijn de filterresultaten alleen zichtbaar in de geselecteerde weergave en niet in alle weergaven die worden vermeld in het vervolgkeuzemenu Weergave.

  >[!NOTE]
  >
  > Omdat de Adobe Workfront-planningsmogelijkheden zich momenteel in een bètastatus bevinden, zijn sommige weergave-elementen mogelijk niet beschikbaar voor alle weergaven.

In dit artikel wordt de volgende informatie over recordweergaven beschreven:

* [Een weergave maken en bewerken](#create-or-edit-record-views)
* [Een weergave verwijderen](#delete-views)
  <!--* [Duplicate a view](#duplicate-views)-->
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
* [Een weergave delen](#share-a-view)

## Gelijksoortigheid en verschillen tussen recordweergaven

In de volgende tabel worden de overeenkomsten en verschillen tussen de tabel-, tijdlijn- en kalenderweergave weergegeven:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Functie | Tabelweergave | Tijdlijnweergave | Kalenderweergave |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| Records in een lijst of tabel weergeven | ✓ |              | |
| Alle velden standaard weergeven als kolommen in de tabel | ✓ |              |    |
| Velden (of kolommen) verbergen of weergeven | ✓ |               |    |
| Veldwaarden bewerken voor elke record | ✓ |               |             |
| Records toevoegen als nieuwe rijen in de weergave | ✓ |               |        |
| Velden toevoegen als nieuwe kolommen in de weergave | ✓ |               |         |
| Rijen kopiëren uit een externe lijst en deze in een tabel plakken | ✓ |               |          |
| Records in een tijdlijn weergeven |            | ✓ |             |
| Filterrecords | ✓ | ✓ | ✓ |
| Records weergeven op een kalender |           |              | ✓ |
| Groepsrecords | ✓ | ✓ |
| Records sorteren | ✓ |              |
| Kleurcoderecords |           | ✓ | ✓ |
| Kleurcodegroepen |           | ✓ |
| Specifieke records zoeken | ✓ | ✓ |
| Weergave delen | ✓ | ✓ | ✓ |
| Open de pagina Details van de record vanuit de weergave | ✓ | ✓ |    |


## Weergaven maken of bewerken {#create-or-edit-views}

{{step1-to-maestro}}


De werkruimte die u het laatst hebt geopend, wordt standaard geopend. Zie voor informatie over het maken van werkruimten [Werkruimten maken](../architecture/create-workspaces.md).

1. Klik op een opnametype. Zie voor informatie over het maken van een recordtype [Recordtypen maken](../architecture/create-record-types.md).

   Standaard worden alle records van het geselecteerde type weergegeven in de tabelweergave.

1. Klikken **+ Weergave** om een nieuwe weergave toe te voegen.
1. Selecteer een van de volgende typen weergaven:

   * Tabel
   * Tijdlijn
   * Kalender

   Er wordt een nieuw tabblad gemaakt met de geselecteerde weergave.

   Afhankelijk van de breedte van het scherm kunnen aanvullende weergaven worden weergegeven in het dialoogvenster **Meer** menu ![](assets/more-menu.png).


>[!TIP]
>
>Wanneer u een recordtype maakt, wordt de tabelweergave ook standaard gemaakt.
>
>Als u een tijdlijn of een kalenderweergave wilt maken, moet het recordtype waarvoor u de weergave maakt, ten minste twee datumvelden hebben. Anders worden de opties Tijdlijn en Kalender grijs weergegeven.
>

![](assets/view-types-drop-down-from-record-type-list.png)

>[!NOTE]
>
>    Als u een tijdlijn of een kalenderweergave wilt maken, moet het recordtype waarvoor u de weergave maakt, ten minste twee datumvelden hebben. Anders worden de tijdlijn of de kalenderopties gedimd weergegeven.

1. (Voorwaardelijk) Klik **Volgende**, wanneer u een tijdlijn- of kalenderweergave maakt.

   Standaard geeft Workfront de weergave een van de volgende namen:

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   Het getal is een automatisch gegenereerde toename.

1. (Voorwaardelijk) Selecteer **Start** en **Einddata** voor de records die worden weergegeven in de tijdlijn of de kalenderweergave.
1. Klikken **Maken**.

   De weergave wordt weergegeven als een nieuw tabblad. De weergaven worden in chronologische volgorde weergegeven vanaf het moment waarop ze zijn gemaakt of met u zijn gedeeld.
1. (Optioneel) Klik op de knop **Meer** menu ![](assets/more-caret-down-icon-views.png) naast de laatste weergave om alle weergaven voor het geselecteerde recordtype weer te geven.

   Aanvullende weergaven worden weergegeven onder de **Meer** na het laatste weergavetabblad. Het getal naast de **Meer** wordt het aantal extra weergaven weergegeven.
1. (Optioneel) Als u de naam van een weergave wilt wijzigen nadat deze is gemaakt, klikt u op de vervolgkeuzelijst Weergave en vervolgens op de knop **Meer** menu ![](assets/more-menu.png) > **Naam wijzigen** de weergavenaam bijwerken

   of

   Dubbelklik op de weergavenaam en typ de nieuwe naam.  <!--ensure there is not another saving step here?!-->

1. (Optioneel) Raadpleeg de volgende artikelen voor informatie over het beheren van een bepaald weergavetype:

   * [De tabelweergave beheren](../views/manage-the-table-view.md)
   * [De tijdlijnweergave beheren](../views/manage-the-timeline-view.md)
   * [De kalenderweergave beheren](/help/quicksilver/maestro/views/manage-the-calendar-view.md)


## Weergaven verwijderen

{{step1-to-maestro}}

De werkruimte die u het laatst hebt geopend, wordt standaard geopend. Zie voor informatie over het maken van werkruimten [Werkruimten maken](../architecture/create-workspaces.md).

1. Klik op een opnametype.

   Zie voor informatie over het maken van een recordtype [Recordtypen maken](../architecture/create-record-types.md).

   Standaard worden alle records van het geselecteerde type weergegeven in de tabelweergave.

1. Houd de muis boven een van de namen van de weergave op het tabblad Weergave en klik vervolgens op **Meer** ![](assets/more-menu.png) links van de weergavenaam klikt u op **Verwijderen**.
Eerst moet u mogelijk op **Meer** links van de laatste tab om de weergave te zoeken die u wilt verwijderen.

1. Klikken **Verwijderen** ter bevestiging. <!--ensure there is not another saving step here?!-->

   De weergave wordt verwijderd voor alle gebruikers die toegang hebben tot het recordgebied en kan niet worden hersteld.

## Een weergave delen

Zie voor informatie over het delen van weergaven [Weergaven delen](/help/quicksilver/maestro/access/share-views.md).

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: 

## Duplicate views

If you want to keep multiple versions of a view and make slight changes between the version, you can duplicate a view. Duplicating a view creates identical copies of an existing view. 

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) to the right of the view name > **Duplicate**. (**********ensure there is not another saving step here?! also, add how this view is named; the button to duplicate was there but not the functionality yet************)
    
    The view is duplicated and visible to all users who can access the Maestro area. 

-->
