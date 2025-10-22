---
title: Records delen
description: U kunt records met anderen delen om de samenwerking te verbeteren.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 0%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

<!--take out preview and production references at release-->

# Records delen

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->

{{planning-important-intro}}

Als u met andere gebruikers wilt samenwerken, kunt u records met anderen delen.

U kunt een Adobe Workfront-planningsrecord op de volgende manieren delen:

* Kopieer de koppeling van de recordpagina vanuit uw browser wanneer de pagina is geopend.

* Kopieer een koppeling naar de pagina van de record wanneer u records bekijkt in de tabelweergave van het recordtype.

* U kunt alle records in een werkruimte met andere gebruikers delen door de werkruimte en het recordtype te delen.

  Zie de volgende artikelen voor meer informatie:

   * [Een werkruimte delen](/help/quicksilver/planning/access/share-workspaces.md)

   * [Een recordtype delen](/help/quicksilver/planning/access/share-record-types.md)

In dit artikel wordt beschreven hoe u een koppeling naar de pagina van een record kunt kopiëren vanuit de tabelweergave van een recordtype.

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
<p>Alle Workfront en alle planningspakketten</p> <p>Willekeurige workflow en planningspakket</p>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Medewerker of hoger</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>  <p>Machtigingen voor een werkruimte weergeven of hoger en recordtype opnemen om een record te delen met een koppeling</p>
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> De gebruikers met een Licht of de vergunning van de Medewerker moeten een lay-outmalplaatje worden toegewezen dat Planning omvat.
   <p>De standaardgebruikers en de Beheerders van het Systeem hebben de Gebieden van de Planning die door gebrek worden toegelaten.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  


<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Contributor or higher license </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  <p>View or higher permissions to a workspace and record typeto share   a record using a link </p>
   <p>Manage permissions to a workspace and record type to share the records in the workspace </p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table> -->


## Recordkoppelingen delen vanuit de tabelweergave van het recordtype

{{step1-to-planning}}

De werkruimte die u het laatst hebt geopend.

1. Klik op een opnametype.

   De pagina met recordtypen wordt geopend.

1. (Voorwaardelijk) van **Mening** drop-down menu in de hoger-juiste hoek van de lijst, selecteer een lijstmening. Dit moet de standaardweergave zijn, tenzij u het recordtype in de tijdlijnweergave hebt bekeken toen u het als laatste opende.

   De records die aan het geselecteerde recordtype zijn gekoppeld, worden in de tabelweergave weergegeven.

1. Klik met de rechtermuisknop op een recordrij

   of

   Beweeg over de naam van een verslag, klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png), dan klik **verbinding van het Exemplaar**.

   ![&#x200B; Contextueel menu voor verslagrij &#x200B;](assets/contextual-menu-for-record-row.png)

   De koppeling wordt naar het klembord gekopieerd.

1. Plak de koppeling in een e-mail- of chatvenster om deze met andere gebruikers te delen. Wanneer gebruikers de koppeling ontvangen, wordt de recordpagina geopend.

   >[!TIP]
   >
   >De velden op de recordpagina zijn dezelfde velden die beschikbaar zijn in de tabelweergave van de record.


   <!--add there when it will be available: if they have access to this record-->

## Alle records in een werkruimte delen door de werkruimte te delen

U kunt alle records in een werkruimte delen wanneer u de werkruimte deelt met anderen.

Recordtypen en records nemen dezelfde machtigingen over van de werkruimte.

Alleen gebruikers met de machtiging Beheren in een werkruimte kunnen deze delen met anderen.

Voor meer informatie, zie [&#x200B; een werkruimte &#x200B;](/help/quicksilver/planning/access/share-workspaces.md) delen.

## Alle records in een recordtype delen door het recordtype te delen

Records nemen machtigingen over van het recordtype.

Standaard nemen recordtypen machtigingen van de werkruimte over.

U kunt echter een van de volgende handelingen uitvoeren:

* Schakel overgeërfde machtigingen van de werkruimte op een recordtype uit. Dit verwijdert hogere toestemmingen aan de verslagen, maar houdt de toestemmingen van de Mening aan de werkruimte, verslagtype, en verslagen.
* Hiermee geeft u gebruikers handmatig machtigingen voor een recordtype, zelfs als ze geen machtigingen voor de werkruimte hebben. Dit geeft hen automatisch de toestemmingen van de Mening aan de werkruimte. Hierdoor krijgen gebruikers machtigingen voor de records.

Alleen gebruikers met de machtiging Beheren in een werkruimte kunnen hun recordtypen en records delen met anderen.

Voor meer informatie, zie [&#x200B; recordtypes van het Aandeel &#x200B;](/help/quicksilver/planning/access/share-record-types.md).

