---
title: Recordweergaven beheren
description: U kunt records in een tabel- of tijdlijnweergave weergeven wanneer u Adobe Maestro gebruikt.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 0%

---


# Recordweergaven beheren

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>Adobe Maestro maakt momenteel deel uit van een bètaprogramma dat voor een beperkt aantal klanten toegankelijk is.
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

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Overwegingen bij het werken met Maestro-weergaven

* Weergaven in Maestro zijn specifiek voor records. U kunt niet dezelfde weergave toepassen op twee verschillende recordtypen.
* Weergaven die u maakt, zijn zichtbaar voor iedereen die het gebied Maestro opent. <!-- edit this when we have permissions and the views will be shared only to be visible by others-->
  <!-- this is not yet possible: * You can share views with others if you want them to also apply them to the same record types.-->
* Het bouwen van meningen voor operationele verslagtypes is identiek aan het bouwen van meningen voor taxonomie verslagtypes.
* Wanneer u een weergave wijzigt of verwijdert, wordt deze gewijzigd en verwijderd voor alle gebruikers die toegang hebben tot het Maestro-gebied.
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
  <!--* [Share a view](#share-views) - not possible yet-->

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

<!--| Sort groupings                                                        | ✓          | ✓             |-->

<!--| Display a limited number of fields as columns, by default                      | ✓          |               |-->

<!--| Color-code records                     |           | ✓              |-->
<!--| Color-code groupings                     |           | ✓              |-->

## Weergaven maken of bewerken {#create-or-edit-views}

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-workfront.png) in de rechterbovenhoek <!--or the **Main Menu** icon ![](assets/main-menu-shell.png) in the upper-left corner, if available-->en klik vervolgens op **Maestro** ![](assets/maestro-icon.png).
De werkruimte die u het laatst hebt geopend, wordt standaard geopend. Zie voor informatie over het maken van werkruimten [Werkruimten maken](../architecture-and-fields/create-workspaces.md).
1. Klik op een opnametype. Zie voor informatie over het maken van een recordtype [Recordtypen maken](../architecture-and-fields/create-record-types.md).

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

1. Van de **Hoofdmenu** ![](assets/main-menu-workfront.png) in de rechterbovenhoek van het scherm, <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner of the screen, if available,--> klikken **Maestro** ![](assets/maestro-icon.png).

   De werkruimte die u het laatst hebt geopend, wordt standaard geopend. Zie voor informatie over het maken van werkruimten [Werkruimten maken](../architecture-and-fields/create-workspaces.md).
1. Klik op een opnametype.

   Zie voor informatie over het maken van een recordtype [Recordtypen maken](../architecture-and-fields/create-record-types.md).

   Standaard worden alle records van het geselecteerde type weergegeven in de tabelweergave.

1. Klik op het vervolgkeuzemenu Weergave, houd de muisaanwijzer boven een van de weergaven in de lijst en klik vervolgens op de knop **Meer** menu ![](assets/more-menu.png) > **Verwijderen**.
1. Klikken **Verwijderen** ter bevestiging. <!--ensure there is not another saving step here?!-->

   De weergave wordt verwijderd voor alle gebruikers die toegang hebben tot het Maestro-gebied en kan niet worden hersteld.

<!--not possible yet - August 30, 2023: 

## Duplicate views

If you want to keep multiple versions of a view and make slight changes between the version, you can duplicate a view. Duplicating a view creates identical copies of an existing view. 

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture-and-fields/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture-and-fields/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) to the right of the view name > **Duplicate**. (**********ensure there is not another saving step here?! also, add how this view is named; the button to duplicate was there but not the functionality yet************)
    
    The view is duplicated and visible to all users who can access the Maestro area. 

-->