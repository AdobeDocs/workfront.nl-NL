---
title: Weergaven delen
description: U kunt een weergave delen met anderen om samenwerking te garanderen wanneer u Adobe Workfront Planning gebruikt.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: fbf902196c9f5b55ddd1e20516e4237309dff2ed
workflow-type: tm+mt
source-wordcount: '1971'
ht-degree: 0%

---


# Weergaven delen

<!--take out preview and production references at production-->

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [&#x200B; snelle versies voor uw organisatie &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

U kunt een weergave met anderen delen om samenwerking te garanderen wanneer u werkt met records in Adobe Workfront Planning.

>[!IMPORTANT]
>
>* Het verlenen van toestemmingen aan een werkruimte geeft andere gebruikers geen toestemmingen aan de meningen op de verslagtypepagina&#39;s. U moet machtigingen verlenen aan afzonderlijke weergaven in een recordtypepagina om deze te kunnen delen met andere gebruikers.
>
>* Als u machtigingen verleent aan een weergave, worden de machtigingen voor het weergeven van de records niet gewijzigd. De toestemmingen van het verslag worden verleend door werkruimten te delen.
>
>* Wanneer u een weergave deelt, geeft u anderen machtigingen om toegang te krijgen tot alle elementen van de weergave. Als u ze bijvoorbeeld de machtiging Beheren geeft aan een weergave, kunnen ze de weergave van de groepering, het filter, de sortering of de balk wijzigen.


<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

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
<p>Het geval van Workfront van uw organisatie moet aan de Verenigde Ervaring van Adobe worden genegeerd om tot de Planning van Workfront te kunnen toegang hebben.</p> 
<p>Uw organisatie moet aan de Verenigde Ervaring van Adobe voor gebruikers worden bezet om toestemmingen aan een mening van een toestemmingsverzoek te kunnen verzoeken en verlenen. </p>
<p>Gebruikers moeten aan de Adobe Admin Console worden toegevoegd om machtigingen te verkrijgen voor de Workfront-planningsweergaven.</p>
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td><p> Standard</p>
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

</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het delen van weergaven

* U kunt een weergave op de volgende manieren delen:

   * Intern, met gebruikers, groepen, teams, bedrijven van Workfront, en baanrollen
   * Openbaar, met gebruikers buiten Workfront
   * Door een koppeling naar een weergave te kopiëren en vervolgens te delen
   * Door het naar Excel of een Csv- dossier uit te voeren. U kunt alleen de tabelweergave exporteren naar een bestand. Voor informatie, zie [&#x200B; de lijstmening &#x200B;](/help/quicksilver/planning/views/manage-the-table-view.md) leiden.

* Voor algemene informatie over het delen van voorwerpen in de Planning van Workfront, zie ook [&#x200B; Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront &#x200B;](/help/quicksilver/planning/access/sharing-permissions-overview.md).
* U kunt weergave- of beheermachtigingen aan interne Workfront-gebruikers geven.

* Gebruikers met de machtiging Beheren kunnen de weergave-instellingen wijzigen, deze delen, dupliceren of verwijderen.

* U kunt weergaven delen met personen buiten uw organisatie via een openbare koppeling.

* Wanneer u een mening openbaar deelt, is de verbinding toegankelijk door iedereen buiten uw bedrijf voor een beperkte tijd, die door de vervaldatum wordt vermeld. U hoeft zich niet aan te melden om de gedeelde weergave te kunnen weergeven.

* Personen buiten uw organisatie die toegang hebben tot een weergave, kunnen geen andere weergaven maken, de gedeelde weergave bewerken of recordgegevens in de weergave toevoegen, verwijderen of bewerken.

## Rechten delen met een weergave intern

U kunt weergaven delen die u hebt gemaakt of weergaven waarop u beheerdersmachtigingen hebt, met gebruikers, groepen, teams, bedrijven en taakrollen in Workfront Planning.

>[!NOTE]
>
>Systeembeheerders kunnen geen weergaven weergeven of delen die ze zelf niet hebben gemaakt. Ze kunnen alleen weergaven openen of delen die met hen worden gedeeld.
>
>Systeembeheerders kunnen alleen beheermachtigingen voor een weergave hebben.

{{step1-to-planning}}

1. Open de werkruimte waarvan u de weergave wilt delen en klik op een opnametype-kaart.

   Hierdoor wordt de pagina met recordtypen geopend.

1. Voer op het tabblad van de weergave een van de volgende handelingen uit:

   * Afhankelijk van de omgeving waarin u de weergave opent, voert u de volgende handelingen uit:

      * In het milieu van de Productie, houd over de lusjenaam van de mening u **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png) aan het recht van de meningsnaam delen en wilt klikken, dan **Aandeel** klikken.

      * <span class="preview"> In het milieu van de Voorproef, klik het lusje van de mening, over de mening in het drop-down menu, klik het **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png), dan klik **Aandeel**.</span>

     ![&#x200B; Meer menu voor een mening &#x200B;](assets/more-menu-for-views-expanded-with-share-option.png)

   * Klik **Aandeel** > **Aandeel de huidige mening**

     ![&#x200B; knoop van het Aandeel met verslagtype en mening die opties delen &#x200B;](assets/share-button-with-record-type-and-view-sharing-options.png)

   De **mening van het Aandeel** doos opent en het **Interne het delen** lusje zou door gebrek moeten worden geselecteerd.

1. (Facultatief) op **die toegang** gebied heeft, selecteer van de volgende opties:

   * **slechts kunnen de uitgenodigde mensen tot** toegang hebben: U moet gebruikers, groepen, team, bedrijf, of baanrol specificeren die u de mening met wilt delen. Dit is de standaardoptie.

   >[!NOTE]
   >
   >Naast teams, groepen, bedrijven, en baanrollen, kunt u slechts met gebruikers delen die aan Adobe Admin Console zijn toegevoegd. U kunt geen gebruikers met alleen Workfront toevoegen. Voor informatie, zie [&#x200B; gebruikers in Adobe Admin Console &#x200B;](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md) leiden.


   * **iedereen in de werkruimte kan** bekijken: Alle gebruikers die Mening of hogere toestemmingen aan werkruimten hebben kunnen tot de mening toegang hebben.

1. In de **toegang van de Verlening tot dit mening** gebied, begin de naam van een gebruiker, een groep, een team, een bedrijf, of baanrol te typen dan het te klikken wanneer het in de lijst toont.

   ![&#x200B; delend een mening met groepen &#x200B;](assets/sharing-a-view-ui-with-groups.png)

1. Selecteer een van de volgende machtigingsniveaus in het keuzemenu:
   * Weergave
   * Beheren

     Voor informatie over toestemmingsniveaus en welke acties kunnen de gebruikers voor elk niveau uitvoeren, zie [&#x200B; Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront &#x200B;](/help/quicksilver/planning/access/sharing-permissions-overview.md).

     Systeembeheerders ontvangen altijd beheermachtigingen voor weergaven die met hen worden gedeeld.

1. Klik **sparen**.

   De meningsupdates met een mensen pictogram ![&#x200B; Mening die met anderen pictogram &#x200B;](assets/view-shared-with-others-people-icon.png) wordt gedeeld om erop te wijzen dat de mening nu met andere gebruikers wordt gedeeld.

   De gebruikers die u de weergave hebt gedeeld, ontvangen zowel een melding in de app als een e-mailbericht over het hebben van machtigingen voor de weergave.

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

1. Voer op het tabblad Weergave een van de volgende handelingen uit:

   * Beweeg over de lusjenaam van de mening u **Meer** menu ![&#x200B; &#x200B;](assets/more-menu.png) aan het recht van de meningsnaam delen en wilt klikken, dan **Aandeel** klikken.

   ![&#x200B; Meer menu voor meningen die met aandeeloptie &#x200B;](assets/more-menu-for-views-expanded-with-share-option.png) worden uitgebreid
   * Klik **Aandeel** > **Aandeel de huidige mening**

   De **mening van het Aandeel** doos opent.

1. Klik **Openbaar het delen**.

   ![&#x200B; Openbaar delend lusje voor meningen &#x200B;](assets/public-sharing-tab-for-views.png)

1. Laat **toe creeer openbare verbinding** plaatsen.

   Er wordt een koppeling beschikbaar. Dit is een openbare link. Als de koppeling wordt gedeeld, heeft iedereen met deze koppeling, dus ook mensen van buiten uw organisatie, toegang tot de pagina met recordtypen en kunnen records en velden op de pagina worden weergegeven.

1. Klik de **pictogram van het 1&rbrace; verbinding van het Exemplaar** verbindingsmening van het Exemplaar ![&#x200B; om de verbinding aan uw klembord te kopiëren.](assets/copy-link-view.png)

1. Voer manueel een datum in, of gebruik de kalender op het **gebied van de Vervaldatum van de Verbinding** om een vervaldatum voor de openbare verbinding te selecteren. De weergave van de recordpagina is na de geselecteerde datum niet toegankelijk.

1. Klik **sparen**.

   De meningsupdates met een globaal pictogram ![&#x200B; Openbaar gedeeld meningspictogram benadrukte &#x200B;](assets/public-shared-view-icon-highlighted.png) om erop te wijzen dat de mening openbaar wordt gedeeld.

   >[!TIP]
   >
   >Weergaven zonder personen of een globaal pictogram zijn weergaven die u hebt gemaakt en die niet met anderen worden gedeeld. Niet-gedeelde weergaven zijn alleen voor u zichtbaar.


1. (Optioneel) Plak de koppeling die u hebt gekopieerd naar een e-mail, chatbericht, document of Workfront-opmerking om deze met anderen te delen.

## Een koppeling naar een weergave kopiëren

U kunt een koppeling naar een weergave naar het klembord kopiëren en deze opnemen in een andere toepassing of deze delen met anderen.

Om een verbinding aan een openbaar-gedeelde mening te kopiëren, zie de sectie [&#x200B; toestemmingen van het Aandeel aan een mening openbaar &#x200B;](#share-permissions-to-a-view-publicly) in dit artikel.

In deze sectie wordt beschreven hoe u een weergave intern deelt.

>[!IMPORTANT]
>
>U moet eerst de weergave met gebruikers delen voordat u de koppeling naar de weergave kunt delen. Anders kunt u de koppeling niet meer zien.


{{step1-to-planning}}

1. Open de werkruimte waarnaar u de koppeling wilt kopiëren en delen en klik vervolgens op een opnametype-kaart.

   Hierdoor wordt de pagina met recordtypen geopend.

1. Voer op het tabblad van een weergave een van de volgende handelingen uit:

   * Beweeg over het lusje van de mening u **Meer** menu ![&#x200B; &#x200B;](assets/more-menu.png) aan het recht van de meningsnaam wilt delen en klikken, dan **Aandeel** > **verbinding van het Exemplaar** in de **mening van het Aandeel** doos.
   * Klik **Aandeel** > **Kopieer de meningsverbinding** van de verslagtype pagina.

   Een koppeling naar de weergave wordt naar het klembord gekopieerd en u ontvangt een bevestiging onder aan het scherm.

   U kunt de koppeling nu naar een andere toepassing plakken of naar anderen verzenden.

## Rechten verlenen aan een weergave vanuit een machtigingsverzoek

Gebruikers die een koppeling openen naar een weergave waarvoor zij geen machtigingen hebben, kunnen machtigingen aanvragen voor de weergave. Alle gebruikers met de machtiging Beheren voor de weergave ontvangen de aanvraag voor machtigingen en kunnen de machtigingen verlenen of weigeren.

1. (Voorwaardelijk) Als u de manager van een mening bent, zou u een verzoek van een andere gebruiker kunnen ontvangen om tot de mening op de volgende gebieden toegang te hebben:

   * Een melding in de app
     ![&#x200B; In-app bericht voor toegangsverzoek voor mening &#x200B;](assets/in-app-notification-for-access-request-for-view.png)
   * Een e-mailmelding
     ![&#x200B; In-app bericht voor toegangsverzoek voor mening &#x200B;](assets/in-app-notification-for-access-request-for-view.png)
1. (Voorwaardelijk) Klik in het systeemvak in Workfront op de melding in de app.
of
Van het e-mailbericht, klik **Mening alle berichten**, dan klik het bericht in de lijst.

   De **hangende toegangsverzoeken** vakvertoningen.

   ![&#x200B; de lijstgoedkeuringsdoos van Meldingen &#x200B;](assets/notifications-list-approval-box.png)
1. (Optioneel) Voor de gebruiker wiens machtigingen u wilt goedkeuren, selecteert u een van de volgende opties in het vervolgkeuzemenu rechts van de gebruikersnaam:
   * **Mening**
   * **leiden**
1. Selecteer de gebruiker voor wie u de toestemming goedkeuren of wilt ontkennen, dan klik **allen** goedkeuren of **ontkennen allen**.
1. Klik de verlaten-richt pijl aan de linkerzijde van **Hangende toegangsverzoeken**, dan klik **sparen**.

   Als u het verzoek hebt goedgekeurd, worden de gebruikers toegevoegd aan het vak voor delen van de weergave. De gebruiker die de machtiging aanvraagt, ontvangt een e-mailbevestiging dat zijn aanvraag is goedgekeurd. <!--will they also get an in-app notification??-->

## Machtigingen verwijderen uit een weergave

{{step1-to-planning}}

1. Open de werkruimte waarvan u de weergave niet meer wilt delen en klik op een opnametype-kaart. Hierdoor wordt de pagina met recordtypen geopend.
1. Voer op het tabblad Weergave een van de volgende handelingen uit:

   * Beweeg over de lusjenaam van de mening u **Meer** menu ![&#x200B; &#x200B;](assets/more-menu.png) aan het recht van de meningsnaam delen en wilt klikken, dan **Aandeel** klikken.

   * Klik **Aandeel** > **Aandeel de huidige mening**

   De **mening van het Aandeel** doos opent.
1. Ga als volgt te werk om het interne delen van een weergave te verwijderen:

   1. Verzeker het **Interne delen** lusje wordt geselecteerd.
   1. Vind de gebruiker, de groep, het team, het bedrijf, of de baanrol wat u wilt verwijderen, breid het drop-down menu van toestemmingen rechts van de naam van de entiteit uit u de mening deelt met, dan klik **verwijdert**.

1. Ga als volgt te werk om het delen van een weergave door het publiek te verwijderen:

   1. Klik het **Openbare delen** tabel.
   1. Deselecteer **creeer openbare verbinding** optie.

1. Klik **sparen**.

   Personen hebben geen toegang meer tot de weergave. Er is geen bericht voor de gebruikers die zijn verwijderd van toegang tot de weergave, dat zij deze toegang niet meer hebben.
