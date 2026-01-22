---
title: Werkruimten delen
description: U kunt een werkruimte met anderen delen om samenwerking te verzekeren wanneer het werken in de Planning van Adobe Workfront.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 54a6e633e903c73a78b36e90fb27edb445dc8d47
workflow-type: tm+mt
source-wordcount: '894'
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

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Alle Workfront- en planningspakketten</p> 
of
<p>Willekeurig workflowpakket en planningspakket</p> 
 </tr>
<tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr>

<td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>  <p>Machtigingen beheren in een werkruimte</p>  </td> 
  </tr>

</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
<p>Your organization must be onboarded to the Adobe Unified Experience for users to be able to request and grant permissions to a workspace from a permission request. </p> 
<p>Users must be added to the Adobe Admin Console in order to gain permissions to Workfront Planning workspaces.</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
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
   <td>  <p>Manage permissions to a workspace</p>  </td> 
  </tr> 

</tbody> 
</table> -->

## Overwegingen bij het delen van werkruimten

* Voor algemene informatie over het delen van voorwerpen in de Planning van Workfront, zie ook [ Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront ](/help/quicksilver/planning/access/sharing-permissions-overview.md).
* U kunt werkruimten delen met gebruikers, teams, rollen, groepen, of bedrijven binnen uw organisatie.
* Naast teams, groepen, bedrijven, en baanrollen, kunt u slechts met gebruikers delen die aan Adobe Admin Console zijn toegevoegd.
* U kunt werkruimten niet delen met gebruikers buiten uw organisatie.
* Wanneer u een werkruimte deelt, worden ook alle recordtypen, records en velden gedeeld die aan de werkruimten zijn gekoppeld.
* Als u een werkruimte deelt, worden de weergaven niet gedeeld. U moet de weergaven afzonderlijk delen.
* Workspace-machtigingen worden weergegeven als Geërfde machtigingen voor recordtypen.

## Machtigingen delen naar een werkruimte

De volgende gebruikers kunnen een werkruimte delen met andere gebruikers:

* Systeembeheerders kunnen alle werkruimten delen, inclusief de werkruimten die ze niet hebben gemaakt.
* Alle andere gebruikers kunnen alleen werkruimten delen waarvoor zij beheerdersmachtigingen hebben.

Een werkruimte delen met anderen:

{{step1-to-planning}}

1. Open de werkruimte u wilt delen, dan **Aandeel** in de hoger-juiste hoek van het scherm klikken.

   ![ knoop van het Aandeel op werkruimte het hoogste recht ](assets/share-button-on-workspace-top-right.png)

1. In de **toegang van de Verlening tot dit werkruimte** gebied, begin de naam van een gebruiker, een groep, een team, een bedrijf, of baanrol te typen dan het te klikken wanneer het in de lijst toont.

   ![ delend UI met groepen ](assets/sharing-ui-with-groups.png)

   >[!NOTE]
   >
   >* Naast teams, groepen, bedrijven, en baanrollen, kunt u slechts met gebruikers delen die aan Adobe Admin Console zijn toegevoegd. U kunt geen gebruikers met alleen Workfront toevoegen. Voor informatie, zie [ gebruikers in Adobe Admin Console ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md) leiden.
   >
   >* Wanneer u een werkruimte met een gebruiker deelt, hun primaire baanrol <span class="preview"> en hun e-mail </span> ook tonen op het gebied. U moet de instelling Contactgegevens weergeven hebben ingeschakeld voor het object Users in uw toegangsniveau om de e-mail van de gebruiker te kunnen zien.


1. Selecteer een van de volgende machtigingsniveaus in het keuzemenu:
   * Weergave
   * Contribute
   * Beheren

     Voor informatie over toestemmingsniveaus en welke acties kunnen de gebruikers voor elk niveau uitvoeren, zie [ Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront ](/help/quicksilver/planning/access/sharing-permissions-overview.md).
1. Klik **verbinding van het Exemplaar** om een verbinding aan de werkruimte aan uw klembord te kopiëren.
1. Deel de gekopieerde koppeling met anderen. Gebruikers die de koppeling ontvangen, moeten actieve gebruikers zijn en zich aanmelden bij Workfront om toegang te krijgen tot de werkruimte.
1. Klik **sparen**.

   De gebruikers die u de werkruimte hebt gedeeld, ontvangen zowel een melding in de app als een e-mailbericht over het hebben van machtigingen voor de werkruimte.

## Machtigingen verlenen aan een werkruimte uit een machtigingsverzoek

Gebruikers die een koppeling openen naar een werkruimte waarvoor zij geen machtigingen hebben, kunnen machtigingen aanvragen bij de werkruimte. Alle gebruikers met de machtiging Beheren voor de werkruimte ontvangen de aanvraag voor machtigingen en kunnen de machtigingen verlenen of weigeren.

1. (Voorwaardelijk) Als u de manager van een werkruimte bent, zou u een verzoek van een andere gebruiker kunnen ontvangen om tot de mening op de volgende gebieden toegang te hebben:

   * Een melding in de app
     ![ In-app bericht voor toegangsverzoek ](assets/in-app-notification-for-access-request.png)
   * Een e-mailmelding
     ![ E-mailbericht voor toegangsverzoek ](assets/email-notification-for-access-request.png)
1. (Voorwaardelijk) Klik in het systeemvak in Workfront op de melding in de app.
of
Van het e-mailbericht, klik **Mening alle berichten**, dan klik het bericht in de lijst.

   De **hangende toegangsverzoeken** vakvertoningen.

   ![ de lijstgoedkeuringsdoos van Meldingen ](assets/notifications-list-approval-box.png)

1. (Optioneel) Voor de gebruiker wiens machtigingen u wilt goedkeuren, selecteert u een van de volgende opties in het vervolgkeuzemenu rechts van de gebruikersnaam:
   * **Mening**
   * **draagt** bij
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

   Er is geen melding voor de gebruikers die uit de toegang tot de werkruimte zijn verwijderd, dat zij niet langer over deze machtigingen beschikken.