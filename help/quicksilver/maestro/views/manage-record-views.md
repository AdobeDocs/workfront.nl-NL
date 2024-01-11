---
title: Recordweergaven beheren
description: U kunt records in een tabel- of tijdlijnweergave weergeven wanneer u Adobe Maestro gebruikt.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 0%

---

# Recordweergaven beheren

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>De informatie in dit artikel verwijst naar Adobe Maestro, een nieuw aanbod van Adobe Workfront.
>
>Adobe Maestro maakt momenteel deel uit van een bètaprogramma dat voor een beperkt aantal klanten toegankelijk is. U moet een Workfront-klant zijn om Maestro-mogelijkheden te kunnen gebruiken.
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro-overview.md).

Nadat u een recordtype hebt geselecteerd in Adobe Maestro, kunt u alle records van dat type weergeven in de volgende weergaven:

* Tabel

  Zie voor meer informatie [De tabelweergave beheren](../views/manage-the-table-view.md).
* Tijdlijn

  Zie voor meer informatie [De tijdlijnweergave beheren](../views/manage-the-timeline-view.md).

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
   <td role="rowheader">Configuratie op toegangsniveau</td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor Maestro</p>  
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

## Overwegingen bij het werken met Maestro-weergaven

* Weergaven in Maestro zijn specifiek voor records. U kunt niet dezelfde weergave toepassen op twee verschillende recordtypen.
* Weergaven die u maakt, zijn alleen zichtbaar voor u en gebruikers met wie u de weergaven deelt.
* Het bouwen van meningen voor operationele verslagtypes is identiek aan het bouwen van meningen voor taxonomie verslagtypes.
* Wanneer u een weergave wijzigt of verwijdert, wordt deze gewijzigd en verwijderd voor alle gebruikers die machtigingen hebben voor de weergave.
* De volgende elementen zijn uniek voor elke weergave in Maestro:

   * Filter
   * Groepering
   * Sorteren

  <!-- some of these are not available in all of the views - edit above-->

  Wanneer u bijvoorbeeld een filter maakt in een tabelweergave, zijn de filterresultaten alleen zichtbaar in de geselecteerde weergave en niet in alle weergaven die worden vermeld in het vervolgkeuzemenu Weergave.

  >[!NOTE]
  >
  > Omdat Maestro zich momenteel in een bètastatus bevindt, zijn sommige weergave-elementen mogelijk niet beschikbaar voor beide weergaven.

In dit artikel wordt de volgende informatie over Maestro-weergaven beschreven:

* [Een weergave maken en bewerken](#create-or-edit-record-views)
* [Een weergave verwijderen](#delete-views)
  <!--* [Duplicate a view](#duplicate-views)-->
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
* [Een weergave delen](#share-a-view)

## Gelijkaardigheden en verschillen tussen de tabel- en tijdlijnweergaven

In de volgende tabel worden de overeenkomsten en verschillen tussen de tabel- en tijdlijnweergaven in Maestro weergegeven:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Functie | Tabelweergave | Tijdlijnweergave |
|-----------------------------------------------------------------------|------------|---------------|
| Records in een lijst of tabel weergeven | ✓ |              |
| Alle velden standaard weergeven als kolommen in de tabel | ✓ |              |
| Velden (of kolommen) verbergen of weergeven | ✓ |               |
| Veldwaarden bewerken voor elke record | ✓ |               |
| Records toevoegen als nieuwe rijen in de weergave | ✓ |               |
| Velden toevoegen als nieuwe kolommen in de weergave | ✓ |               |
| Rijen kopiëren uit een externe lijst en deze in een tabel plakken | ✓ |               |
| Records in een tijdlijn weergeven |            | ✓ |
| Filterrecords | ✓ | ✓ |
| Groepsrecords |           | ✓ |
| Records sorteren | ✓ |              |
| Kleurcoderecords |           | ✓ |
| Kleurcodegroepen |           | ✓ |
| Zoeken in records | ✓ | ✓ |

<!--| Sort groupings                                                        | ✓          | ✓             |-->
<!--| Display a limited number of fields as columns, by default                      | ✓          |               |-->

## Weergaven maken of bewerken {#create-or-edit-views}

{{step1-to-maestro}}


De werkruimte die u het laatst hebt geopend, wordt standaard geopend. Zie voor informatie over het maken van werkruimten [Werkruimten maken](../architecture/create-workspaces.md).
1. Klik op een opnametype. Zie voor informatie over het maken van een recordtype [Recordtypen maken](../architecture/create-record-types.md).

   Standaard worden alle records van het geselecteerde type weergegeven in de tabelweergave.

1. Klik op de knop **Weergave** en selecteert u een bestaande **Tabelweergave** ![](assets/table-view-icon.png) of klik op **Weergave maken > Tabel** een tabelweergave maken

   of

   Bestaande selecteren **Tijdlijnweergave** ![](assets/timeline-view-icon.png) weergeven of klikken **Weergave maken > Tijdlijn** om een tijdlijnweergave te maken.

   ![](assets/view-types-drop-down-from-record-type-list.png)

   >[!NOTE]
   >
   >    Als u een tijdlijnweergave wilt maken, moet het recordtype waarvoor u de weergave maakt, ten minste twee datumvelden hebben. Anders wordt de optie Tijdlijn grijs weergegeven.

1. (Optioneel) Werk de naam van de weergave bij en klik vervolgens op **Maken** opslaan.

   Standaard krijgt Maestro de naam van de weergave &quot;Tabel &lt; nummer >&quot; of &quot;Tijdlijn &lt; nummer >&quot;. Het getal is een automatisch gegenereerde toename.

1. (Optioneel) Als u de naam van een weergave wilt wijzigen nadat deze is gemaakt, klikt u op de vervolgkeuzelijst Weergave en vervolgens op de knop **Meer** menu ![](assets/more-menu.png) > **Naam wijzigen** om de weergavenaam bij te werken. <!--ensure there is not another saving step here?!-->
1. (Optioneel) Raadpleeg de volgende artikelen voor meer informatie om een weergave te beheren:

   * [De tabelweergave beheren](../views/manage-the-table-view.md)
   * [De tijdlijnweergave beheren](../views/manage-the-timeline-view.md)


<!--# Add a view as a favorite - this is not possible yet-->

<!-- ## Share views - not possible yet-->

## Weergaven verwijderen

{{step1-to-maestro}}

De werkruimte die u het laatst hebt geopend, wordt standaard geopend. Zie voor informatie over het maken van werkruimten [Werkruimten maken](../architecture/create-workspaces.md).

1. Klik op een opnametype.

   Zie voor informatie over het maken van een recordtype [Recordtypen maken](../architecture/create-record-types.md).

   Standaard worden alle records van het geselecteerde type weergegeven in de tabelweergave.

1. Klik op het vervolgkeuzemenu Weergave, houd de muisaanwijzer boven een van de weergaven in de lijst en klik vervolgens op de knop **Meer** menu ![](assets/more-menu.png) > **Verwijderen**.
1. Klikken **Verwijderen** ter bevestiging. <!--ensure there is not another saving step here?!-->

   De weergave wordt verwijderd voor alle gebruikers die toegang hebben tot het Maestro-gebied en kan niet worden hersteld.

## Een weergave delen

Zie voor informatie over het delen van weergaven [Een weergave delen](/help/quicksilver/maestro/access/share-views.md).


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
