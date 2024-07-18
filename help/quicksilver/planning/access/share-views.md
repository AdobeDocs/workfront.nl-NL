---
title: Weergaven delen
description: U kunt een weergave delen met anderen om samenwerking te garanderen wanneer u Adobe Workfront Planning gebruikt.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live-->

# Weergaven delen

{{planning-important-intro}}

U kunt een weergave met anderen delen om samenwerking te garanderen wanneer u werkt met records in Adobe Workfront Planning.

Het verlenen van toestemmingen aan een werkruimte geeft andere gebruikers geen toestemmingen aan de meningen op de verslagtypepagina&#39;s. U moet machtigingen verlenen aan afzonderlijke weergaven in een recordtypepagina om deze te kunnen delen met andere gebruikers.

Wanneer u een weergave deelt, geeft u anderen machtigingen om toegang te krijgen tot alle elementen van de weergave. Als u ze bijvoorbeeld de machtiging Beheren geeft aan een weergave, kunnen ze de weergave van de groepering, het filter, de sortering of de balk wijzigen.


U kunt een weergave delen met de volgende entiteiten:

* Workfront-gebruikers
* Workfront-groepen
<!--* Publicly, with users outside Workfront
-->

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

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
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td>
   <td>
   <p>Nieuw: Standaard</p>
   of
   <p>Huidig: Plan </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> Er zijn geen toegangscontroles voor de Planning van Adobe Workfront</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Rechten beheren voor een weergave</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p> <p>Voor informatie, zie <a href="/help/quicksilver/planning/access/access-overview.md"> overzicht van de Toegang </a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).



## Machtigingen delen naar een weergave <!--internally-->

U kunt weergaven delen die u hebt gemaakt of weergaven waarop u beheermachtigingen hebt. <!--with users or groups in Workfront-->

>[!NOTE]
>
>Systeembeheerders kunnen geen weergaven weergeven of delen die ze zelf niet hebben gemaakt. Ze kunnen alleen weergaven openen of delen die met hen worden gedeeld.
>
>Systeembeheerders kunnen alleen beheermachtigingen voor een weergave hebben.

{{step1-to-planning}}

1. Open de werkruimte waarvan u de weergave wilt delen en klik op een opnametype-kaart.

   Hierdoor wordt de pagina met recordtypen geopend.

1. Van het meningslusje, houd over de mening u **Meer** menu ![](assets/more-menu.png) aan het recht van de meningsnaam delen en wilt klikken, dan **Aandeel** klikken.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   <!--The Internal sharing tab should be selected by default.-->

1. (Optioneel) Selecteer een van de volgende opties om de weergave te delen:

   * **slechts kunnen de uitgenodigde mensen tot** toegang hebben: U moet gebruikers of groepen specificeren die u de mening met wilt delen. Dit is de standaardoptie.
   * **iedereen in de werkruimte kan** bekijken: Alle gebruikers die Mening of hogere toestemmingen aan werkruimten hebben kunnen tot de mening toegang hebben.

1. In de **de meningstoegang van de Verlening tot** gebied, begin de naam van een gebruiker of een groep te typen, dan het te klikken wanneer het in de lijst toont.  <!--***********replace screen shot below when public sharing is released***********-->

   ![](assets/sharing-a-view-ui-with-groups.png)

1. Selecteer een van de volgende machtigingsniveaus in het keuzemenu:
   * Weergave
   * Beheren

     Voor informatie over toestemmingsniveaus en welke acties kunnen de gebruikers voor elk niveau uitvoeren, zie [ Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront ](/help/quicksilver/planning/access/sharing-permissions-overview.md).

     Systeembeheerders ontvangen altijd beheermachtigingen voor weergaven die met hen worden gedeeld.

1. Klik **verbinding van het Exemplaar** om een verbinding aan de mening aan uw klembord te kopiëren.
1. Deel de gekopieerde koppeling met anderen. Gebruikers die de koppeling ontvangen, moeten actieve gebruikers zijn en zich aanmelden bij Workfront om de pagina met recordtypen te kunnen openen en weergeven in de geselecteerde weergave.
1. Klik **sparen**.

   >[!TIP]
   >
   >   Weergaven die met u worden gedeeld, hebben een personeels-indicator ![](assets/view-shared-with-others-people-icon.png) naast het weergavepictogram. Weergaven zonder de indicator Personen zijn weergaven die u hebt gemaakt.



<!--
## Share permissions to a view publicly

You can share views you created or views you have Manage permissions to with people that do not have a Workfront license and who might be external to your organization. 

Consider the following when publicly sharing a Workfront Planning view: 

* You can share a public link to a record type page that displays in the view you are sharing.
* People accessing the record type with the public link you provide have View permissions to the record page. They cannot modify the view, the records, or any of the fields that are visible in the view. 
* The shared public link must have an expiration date after which the link is no longer accessible. 

To share a view publicly in Workfront Planning: 

{{step1-to-planning}}

1. Open the workspace whose view you want to share, then click a record type card. 

   This opens the record type page.

1. From the view tab, hover over the view you want to share and click the **More** menu ![](assets/more-menu.png) to the right of the view name, then click **Share**. 

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Click **Public sharing**.

1. Enable the **Create public link** setting.

   A link becomes available. This is a public link. When shared, anyone with the link, including people from outside your organization can access the record type page, and view records and fields on the page. 

1. Click the **Copy link** icon ![](assets/copy-link-view.png) to copy the link to your clipboard. 

1. Manually enter a date, or use the calendar in the **Link expiration date** field to select an expiration date for the public link. The record page view will not be accessible after the selected date. 

1. Click **Save**.

1. Paste the link you copied to an email, chat message, document, or in a Workfront comment to share it with others. 

-->


## Machtigingen verwijderen uit een weergave

{{step1-to-planning}}

1. Open de werkruimte waarvan u de weergave niet meer wilt delen en klik op een opnametype-kaart. Hierdoor wordt de pagina met recordtypen geopend.
1. Beweeg over de lusjenaam van de mening u het delen uit wilt verwijderen en **Meer** menu ![](assets/more-menu.png) klikken, dan **Aandeel** klikken.
1. Vind de gebruiker of de groep wat u wilt verwijderen, dan **verwijderen** in het drop-down menu van toestemmingen rechts van de naam van de gebruiker of van de groep.
1. Klik **sparen**.
De gebruiker of de gebruikers die tot de verwijderde groep behoren, hebben geen toegang meer tot de weergave. Er is geen bericht voor de gebruikers die uit de toegang tot van mening zijn verwijderd dat zij deze toegang verloren.

<!--Replace the above instructions with the following when public sharing is released: 

{{step1-to-planning}}

1. Open the workspace whose view you want to stop sharing, then click a record type card. This opens the record type page.
1. Hover over the tab name of the view you want to remove sharing from and click the **More** menu ![](assets/more-menu.png), then click **Share**.
1. To remove the internal sharing of a view, do the following: 

   1. Ensure the **Internal sharing** tab is selected.
   1. Find the user or group what you want to remove, expand the permissions drop-down menu to the right of the user's or group's name, then click **Remove**.

1. To remove the public sharing of a view, do the following: 

   1. Click the **Public sharing** tab.
   1. Deselect the **Create public link** option. 

1. Click **Save**.
   
   People no longer have access to the view. There is no notification for the users that have been removed from accessing the view that they no longer have this access.-->