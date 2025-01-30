---
title: Werkruimten delen
description: U kunt een werkruimte met anderen delen om samenwerking te verzekeren wanneer het werken in de Planning van Adobe Workfront.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: cf3b5d3f8e3a8a1922da757a41b4c5e0ee84e6fd
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 0%

---

# Werkruimten delen

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

U kunt een werkruimte met anderen delen om samenwerking te verzekeren wanneer het werken in de Planning van Adobe Workfront.

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

>[!NOTE]
>
>Het verlenen van toestemmingen aan een werkruimte geeft andere gebruikers geen toestemmingen aan de meningen op de verslagtypepagina&#39;s. U moet machtigingen verlenen aan afzonderlijke weergaven in een recordtypepagina om deze te kunnen delen met andere gebruikers. Voor informatie, zie [ een mening ](/help/quicksilver/planning/access/share-views.md) delen.


## Toegangsvereisten

+++ Breid uit om toegangsvereisten voor de Planning van Workfront te bekijken.

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
   <p> Producten</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-abonnement*</p></td> 
   <td> 
<p>Een van de volgende Workfront-plannen:</p> 
<ul><li>Selecteren</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is niet beschikbaar voor oudere Workfront-plannen</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-planningspakket*</p></td> 
   <td> 
<p>Alle </p> 
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningsplan is opgenomen. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-platform</p></td> 
   <td> 
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden genegeerd om tot alle mogelijkheden van de Planning van Workfront te kunnen toegang hebben.</p>
<p>Uw organisatie moet aan de Adobe Verenigde Ervaring voor gebruikers worden bezet om toestemmingen aan een werkruimte van een toestemmingsverzoek te kunnen verzoeken en verlenen. </p> 
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td><p> Standaard </p>
   <p>Workfront Planning is niet beschikbaar voor oudere Workfront-licenties</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td> 
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>  <p>Machtigingen beheren in een werkruimte</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--

OLD: 
 
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
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->



## Machtigingen delen naar een werkruimte

De volgende gebruikers kunnen een werkruimte delen met andere gebruikers:

* Systeembeheerders kunnen alle werkruimten delen, inclusief de werkruimten die ze niet hebben gemaakt.
* Alle andere gebruikers kunnen alleen werkruimten delen waarvoor zij beheerdersmachtigingen hebben.

Een werkruimte delen met anderen:

{{step1-to-planning}}

1. Open de werkruimte u wilt delen, dan **Aandeel** in de hoger-juiste hoek van het scherm klikken.

   ![](assets/share-button-on-workspace-top-right.png)

1. In de **werkruimtetoegang van de Verlening tot** gebied, begin de naam van een gebruiker, een groep, <span class="preview"> team, een bedrijf, of baanrol </span> dan het te typen wanneer het in de lijst toont.

   <div class="preview">

   ![](assets/sharing-ui-with-groups.png)

   </div>

1. Selecteer een van de volgende machtigingsniveaus in het keuzemenu:
   * Weergave
   * Contribute
   * Beheren

     Voor informatie over toestemmingsniveaus en welke acties kunnen de gebruikers voor elk niveau uitvoeren, zie [ Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront ](/help/quicksilver/planning/access/sharing-permissions-overview.md).
1. Klik **verbinding van het Exemplaar** om een verbinding aan de werkruimte aan uw klembord te kopiëren.
1. Deel de gekopieerde koppeling met anderen. Gebruikers die de koppeling ontvangen, moeten actieve gebruikers zijn en zich aanmelden bij Workfront om toegang te krijgen tot de werkruimte.
1. Klik **sparen**.

## Machtigingen verlenen aan een werkruimte uit een machtigingsverzoek

Gebruikers die een koppeling openen naar een werkruimte waarvoor zij geen machtigingen hebben, kunnen machtigingen aanvragen bij de werkruimte. Alle gebruikers met de machtiging Beheren voor de werkruimte ontvangen de aanvraag voor machtigingen en kunnen de machtigingen verlenen of weigeren.

1. (Voorwaardelijk) Als u de manager van een werkruimte bent, zou u een verzoek van een andere gebruiker kunnen ontvangen om tot de mening op de volgende gebieden toegang te hebben:

   * Een melding in de app
     ![](assets/in-app-notification-for-access-request.png)
   * Een e-mailmelding
     ![](assets/email-notification-for-access-request.png)
1. (Voorwaardelijk) Klik in het systeemvak in Workfront op de melding in de app.
of
Van het e-mailbericht, klik **Mening alle berichten**, dan klik het bericht in de lijst.

   De **hangende toegangsverzoeken** vakvertoningen.

   ![](assets/notifications-list-approval-box.png)

1. (Optioneel) Voor de gebruiker wiens machtigingen u wilt goedkeuren, selecteert u een van de volgende opties in het vervolgkeuzemenu rechts van de gebruikersnaam:
   * **Mening**
   * **Contribute**
   * **leiden**
1. Selecteer de gebruiker voor wie u de toestemming goedkeuren of wilt ontkennen, dan klik **allen** goedkeuren of **ontkennen allen**.
1. Klik de verlaten-richt pijl aan de linkerzijde van **Hangende toegangsverzoeken**, dan klik **sparen**.

   Als u het verzoek hebt goedgekeurd, worden de gebruikers toegevoegd aan het vak voor delen van de werkruimte. De gebruiker die de machtiging aanvraagt, ontvangt een e-mailbevestiging dat zijn aanvraag is goedgekeurd. <!--will they also get an in-app notification??-->


## Machtigingen verwijderen uit een werkruimte


{{step1-to-planning}}

1. Open de werkruimte u toestemmingen aan wilt verwijderen, dan **Aandeel** in de hoger-juiste hoek van het scherm klikken.
1. Klik het drop-down menu rechts van de naam van een entiteit u de werkruimte met deelt, dan klik **verwijderen**.
1. Klik **sparen**.

   De verwijderde gebruikers hebben geen toegang meer tot de werkruimte of de bijbehorende objecten.
