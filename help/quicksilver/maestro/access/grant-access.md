---
title: Toegang verlenen tot Adobe Maestro
description: Leer hoe u toegang verleent en informatie deelt in Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 85f499a429d4223c62b7b13dc0b1d10e8e79e9ed
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# Toegang verlenen tot Adobe Maestro

>[!IMPORTANT]
>
>De informatie in dit artikel verwijst naar Adobe Maestro, een nieuw aanbod van Adobe Workfront.
>
>Adobe Maestro maakt momenteel deel uit van een bètaprogramma dat voor een beperkt aantal klanten toegankelijk is. U moet een Workfront-klant zijn om toegang te hebben tot Maestro
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro-overview.md).

Alle gebruikers in uw organisatie kunnen toegang tot Maestro hebben, als de volgende eerste vereisten op zijn plaats zijn:

<!--the first requisite will be removed when we go to GA-->

* Uw organisatie is ingeschreven voor het afgesloten bètaprogramma van de Adobe Maestro.
* Als systeembeheerder, moet u het gebied van Maestro aan het Belangrijkste Menu toevoegen gebruikend een lay-outmalplaatje.

  Maestro wordt standaard niet weergegeven in het hoofdmenu voor een gebruiker, inclusief systeembeheerders.

  Zie voor meer informatie [Het hoofdmenu aanpassen met een lay-outsjabloon](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

<!-- take out the note below when we release permissions-->

>[!NOTE]
>
>Er zijn geen toegangsniveaus of toestemmingen verbonden aan gebruikers of de informatie in Maestro. Alle gebruikers die Maestro in hun omgeving hebben ingeschakeld, kunnen alle informatie die een andere gebruiker aan Maestro toevoegt, weergeven, bewerken en verwijderen.

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
   <td role="rowheader"><p>Toegangsniveau</p></td>
   <td> <p>Willekeurig gebruik van Maestro</p>
   <p>Systeembeheerder of -plan om het Maestro-gebied te delen in een lay-outsjabloon</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het Maestro-gebied aan uw lay-outmalplaatje toevoegen. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
When permissions is released:

* leave as is for Access levels (I think)
* Add a new row for Permissions: System admin or Manage access to the workspace to share a workspace with others
-->

## Het gebied Maestro in het hoofdmenu delen met anderen

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

Nadat uw organisatie is ingeschreven voor het bètaprogramma van Maestro, kunt u het Maestro-gebied toevoegen aan het Hoofdmenu van alle gebruikers door een lay-outsjabloon te gebruiken.

1. Aanmelden bij **Workfront** als Workfront-beheerder.

1. Voeg de **Maestro** pictogram ![](assets/maestro-icon.png) aan de **Hoofdmenu** met een **Lay-outsjabloon**.

   Zie voor meer informatie [Het hoofdmenu aanpassen met een lay-outsjabloon](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. Wijs het lay-outmalplaatje aan de gebruikers toe die u toegang tot Maestro wilt hebben.

   Zie voor meer informatie [Gebruikers toewijzen aan een lay-outsjabloon](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   Alle gebruikers die aan de sjabloon zijn toegewezen, hebben nu toegang tot Maestro in hun hoofdmenu.

   Gebruikers kunnen werkruimten, recordtypen, records en velden maken.

<!--

## Share permissions to a workspace

The following users can share a workspace with other users:

* System administrators can share all workspaces, including the ones that they did not create.
* All other users can share only workspaces for which they have Manage permissions to. 

To share a workspace with others: 

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner or Workfront, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (*************add screen shot when UI is finalized and maybe edit the steps*********)
1. In the field provided, start typing the name of a user or a group (******ensure you can share with groups*******), then click it when it displays in the list. 
1. Select one of the following permission levels from the drop-down menu: 
    * View
    * Contribute
    * Manage

        For information about permission levels and what actions users can perform for each level, see [Overview of sharing permissions in Adobe Maestro](../access/sharing-permissions-overview.md).
1. Click **Save**.


## Remove permissions to a workspace

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner of Workfront, if available, then click **Maestro**.
1. Open the workspace you want to remove permissions to, then click **Share** in the upper-right corner of the screen. (********add screen shot when UI is finalized and maybe edit the steps???****)
1. Click the drop-down menu to the right of a user or group name, then click **Remove**. 
1. Click **Save**.

    The user or the users that belong to the group removed no longer have access to the workspace or its objects. 

-->