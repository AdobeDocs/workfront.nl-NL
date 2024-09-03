---
title: Weergaven delen
description: U kunt een weergave delen met anderen om samenwerking te garanderen wanneer u Adobe Workfront Planning gebruikt.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 1e62d5c7eff86432b4914793d75cdf4f835f3d5d
workflow-type: tm+mt
source-wordcount: '1434'
ht-degree: 0%

---


# Weergaven delen

{{planning-important-intro}}

U kunt een weergave met anderen delen om samenwerking te garanderen wanneer u werkt met records in Adobe Workfront Planning.

>[!IMPORTANT]
>
>* Het verlenen van toestemmingen aan een werkruimte geeft andere gebruikers geen toestemmingen aan de meningen op de verslagtypepagina&#39;s. U moet machtigingen verlenen aan afzonderlijke weergaven in een recordtypepagina om deze te kunnen delen met andere gebruikers.
>
>* Als u machtigingen verleent aan een weergave, worden de machtigingen voor het weergeven van de records niet gewijzigd. De toestemmingen van het verslag worden verleend door werkruimten te delen.
>
>* Wanneer u een weergave deelt, geeft u anderen machtigingen om toegang te krijgen tot alle elementen van de weergave. Als u ze bijvoorbeeld de machtiging Beheren geeft aan een weergave, kunnen ze de weergave van de groepering, het filter, de sortering of de balk wijzigen.


U kunt een weergave delen met de volgende entiteiten:

* Intern, met Workfront-gebruikers en -groepen
* Openbaar, met gebruikers buiten Workfront

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

## Toegangsvereisten

+++ Breid uit om toegangsvereisten voor de Planning van Workfront te bekijken.

<!--at GA, check that the Workfront plans article linked below has Planning info-->

U moet het volgende hebben om tot de Planning van Workfront toegang te hebben:

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
<li>Eerste</li> 
<li>Ultieme</li></ul> 
<p>Workfront Planning is niet beschikbaar voor oudere Workfront-plannen</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Planning van Adobe Workfront*</p></td> 
   <td> 
<p>Alle </p> 
<p>Voor meer informatie over wat in elk Plan van de Planning van Workfront inbegrepen is, zie <a href="https://business.adobe.com/products/workfront/pricing.html"> Adobe Workfront tarifering en verpakking </a>. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-platform</p></td> 
   <td> 
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden genegeerd om tot alle mogelijkheden van de Planning van Workfront te kunnen toegang hebben.</p> 
<p>Uw organisatie moet aan de Adobe Verenigde Ervaring voor gebruikers worden bezet om toestemmingen aan een mening van een toestemmingsverzoek te kunnen verzoeken en verlenen. </p>
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td><p> Standaard</p>
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
   <td>  <p>Rechten beheren voor een weergave</p>  
   <p>Alleen gebruikers met de machtiging Beheren in een werkruimte kunnen een weergave openbaar delen.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--OLD: 

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
   <td> <p>Manage permissions to a view</p>  
   <p>Only users with Manage permissions to a workspace can share a view publicly.</p>
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

+++

## Overwegingen bij het delen van weergaven

* U kunt weergave- of beheermachtigingen aan interne Workfront-gebruikers geven.

* Gebruikers met de machtiging Beheren kunnen de weergave-instellingen wijzigen, deze delen, dupliceren of verwijderen.

* U kunt weergaven delen met personen buiten uw organisatie via een openbare koppeling.

* Wanneer u een mening openbaar deelt, is de verbinding toegankelijk door iedereen buiten uw bedrijf voor een beperkte tijd, die door de vervaldatum wordt vermeld. U hoeft zich niet aan te melden om de gedeelde weergave te kunnen weergeven.

* Personen buiten uw organisatie die toegang hebben tot een weergave, kunnen geen andere weergaven maken, de gedeelde weergave bewerken of recordgegevens in de weergave toevoegen, verwijderen of bewerken.

## Rechten delen met een weergave intern

U kunt weergaven die u hebt gemaakt of weergaven waarop u beheermachtigingen hebt, delen met gebruikers of groepen in Workfront.

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

   Het **Interne delende** lusje zou door gebrek moeten worden geselecteerd.

1. (Facultatief) op **die toegang** gebied heeft, selecteer van de volgende opties:

   * **slechts kunnen de uitgenodigde mensen tot** toegang hebben: U moet gebruikers of groepen specificeren die u de mening met wilt delen. Dit is de standaardoptie.
   * **iedereen in de werkruimte kan** bekijken: Alle gebruikers die Mening of hogere toestemmingen aan werkruimten hebben kunnen tot de mening toegang hebben.

1. In de **de meningstoegang van de Verlening tot** gebied, begin de naam van een gebruiker of een groep te typen, dan het te klikken wanneer het in de lijst toont.

   ![](assets/sharing-a-view-ui-with-groups.png)

1. Selecteer een van de volgende machtigingsniveaus in het keuzemenu:
   * Weergave
   * Beheren

     Voor informatie over toestemmingsniveaus en welke acties kunnen de gebruikers voor elk niveau uitvoeren, zie [ Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront ](/help/quicksilver/planning/access/sharing-permissions-overview.md).

     Systeembeheerders ontvangen altijd beheermachtigingen voor weergaven die met hen worden gedeeld.

1. Klik **verbinding van het Exemplaar** om een verbinding aan de mening aan uw klembord te kopiëren.
1. Klik **sparen**.

   De weergave wordt bijgewerkt met het pictogram voor personen ![](assets/view-shared-with-others-people-icon.png) om aan te geven dat de weergave nu wordt gedeeld met andere gebruikers.

   >[!TIP]
   >
   >Weergaven zonder personen of een globaal pictogram zijn weergaven die u hebt gemaakt en die niet met anderen worden gedeeld. Niet-gedeelde weergaven zijn alleen voor u zichtbaar.

1. Deel de gekopieerde koppeling met anderen. Gebruikers die de koppeling ontvangen, moeten actieve gebruikers zijn en zich aanmelden bij Workfront om de pagina met recordtypen te kunnen openen en weergeven in de geselecteerde weergave.

## Machtigingen delen voor een openbare weergave

U kunt weergaven die u hebt gemaakt of weergaven waarop u beheerdersmachtigingen hebt, delen met personen die geen Workfront-licentie hebben en die zich buiten uw organisatie bevinden.

>[!IMPORTANT]
>
>Alleen gebruikers met de machtiging Beheren in een werkruimte kunnen de weergaven van de werkruimte openbaar delen.


Een weergave openbaar delen in Workfront Planning:

{{step1-to-planning}}

1. Open de werkruimte waarvan u de weergave wilt delen en klik op een opnametype-kaart.

   Hierdoor wordt de pagina met recordtypen geopend.

1. Van het meningslusje, houd over de mening u **Meer** menu ![](assets/more-menu.png) aan het recht van de meningsnaam delen en wilt klikken, dan **Aandeel** klikken.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Klik **Openbaar het delen**.

   ![](assets/public-sharing-tab-for-views.png)

1. Laat **toe creeer openbare verbinding** plaatsen.

   Er wordt een koppeling beschikbaar. Dit is een openbare link. Als de koppeling wordt gedeeld, heeft iedereen met deze koppeling, dus ook mensen van buiten uw organisatie, toegang tot de pagina met recordtypen en kunnen records en velden op de pagina worden weergegeven.

1. Klik het **pictogram van de verbinding van het 0} Exemplaar ![](assets/copy-link-view.png) om de verbinding aan uw klembord te kopiëren.**

1. Voer manueel een datum in, of gebruik de kalender op het **gebied van de Vervaldatum van de Verbinding** om een vervaldatum voor de openbare verbinding te selecteren. De weergave van de recordpagina is na de geselecteerde datum niet toegankelijk.

1. Klik **sparen**.

   De weergave wordt bijgewerkt met een algemeen pictogram ![](assets/public-shared-view-icon-highlighted.png) om aan te geven dat de weergave openbaar wordt gedeeld.

   >[!TIP]
   >
   >Weergaven zonder personen of een globaal pictogram zijn weergaven die u hebt gemaakt en die niet met anderen worden gedeeld. Niet-gedeelde weergaven zijn alleen voor u zichtbaar.


1. (Optioneel) Plak de koppeling die u hebt gekopieerd naar een e-mail, chatbericht, document of Workfront-opmerking om deze met anderen te delen.

## Rechten verlenen aan een weergave vanuit een machtigingsverzoek

Gebruikers die een koppeling openen naar een weergave waarvoor zij geen machtigingen hebben, kunnen machtigingen aanvragen voor de weergave. Alle gebruikers met de machtiging Beheren voor de weergave ontvangen de aanvraag voor machtigingen en kunnen de machtigingen verlenen of weigeren.

1. (Voorwaardelijk) Als u de manager van een mening bent, zou u een verzoek van een andere gebruiker kunnen ontvangen om tot de mening op de volgende gebieden toegang te hebben:

   * Een melding in de app
     ![](assets/in-app-notification-for-access-request-for-view.png)
   * Een e-mailmelding
     ![](assets/in-app-notification-for-access-request-for-view.png)
1. (Voorwaardelijk) Klik in het systeemvak in Workfront op de melding in de app.
of
Van het e-mailbericht, klik **Mening alle berichten**, dan klik het bericht in de lijst.

   De **hangende toegangsverzoeken** vakvertoningen.

   ![](assets/notifications-list-approval-box.png)
1. (Optioneel) Voor de gebruiker wiens machtigingen u wilt goedkeuren, selecteert u een van de volgende opties in het vervolgkeuzemenu rechts van de gebruikersnaam:
   * **Mening**
   * **leiden**
1. Selecteer de gebruiker voor wie u de toestemming goedkeuren of wilt ontkennen, dan klik **allen** goedkeuren of **ontkennen allen**.
1. Klik de verlaten-richt pijl aan de linkerzijde van **Hangende toegangsverzoeken**, dan klik **sparen**.

   Als u het verzoek hebt goedgekeurd, worden de gebruikers toegevoegd aan het vak voor delen van de weergave. De gebruiker die de machtiging aanvraagt, ontvangt een e-mailbevestiging dat zijn aanvraag is goedgekeurd. <!--will they also get an in-app notification??-->

## Machtigingen verwijderen uit een weergave

{{step1-to-planning}}

1. Open de werkruimte waarvan u de weergave niet meer wilt delen en klik op een opnametype-kaart. Hierdoor wordt de pagina met recordtypen geopend.
1. Beweeg over de lusjenaam van de mening u het delen uit wilt verwijderen en **Meer** menu ![](assets/more-menu.png) klikken, dan **Aandeel** klikken.
1. Ga als volgt te werk om het interne delen van een weergave te verwijderen:

   1. Verzeker het **Interne delen** lusje wordt geselecteerd.
   1. Vind de gebruiker of de groep wat u wilt verwijderen, breid het toestemmingendrop-down menu rechts van de naam van de gebruiker of van de groep uit, dan klik **verwijdert**.

1. Ga als volgt te werk om het delen van een weergave door het publiek te verwijderen:

   1. Klik het **Openbare delen** tabel.
   1. Deselecteer **creeer openbare verbinding** optie.

1. Klik **sparen**.

   Personen hebben geen toegang meer tot de weergave. Er is geen bericht voor de gebruikers die zijn verwijderd van toegang tot de weergave, dat zij deze toegang niet meer hebben.
