---
title: Recordtypen delen
description: U kunt een recordtype met anderen delen om samenwerking te verzekeren wanneer het gebruiken van de Planning van Adobe Workfront.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: bf49db73-09f1-417e-836b-16c6062740d4
source-git-commit: a4bb3582eb476acbefa5d11db1f2c06eafc13cdd
workflow-type: tm+mt
source-wordcount: '1540'
ht-degree: 0%

---


<!-- take the Remove permissions section out, at the end - this is what Lilit said: Because of "Everyone in the workspace can view" wildcard, currently it's not possible to entirely remove access to a record type. Let's take out this section. -->

# Recordtypen delen

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

U kunt een recordtype met anderen delen om samenwerking te verzekeren wanneer het werken met verslagen in de Planning van Adobe Workfront.

>[!IMPORTANT]
>
>Gebruikers met toegang tot een werkruimte krijgen automatisch minstens weergavemachtigingen voor alle recordtypen in de werkruimte.
>&#x200B;>Als u weergaven deelt, geeft u gebruikers geen machtigingen om gegevenstypen op te nemen. Alleen werkruimten delen kan gebruikers machtigingen verlenen om gegevenstypen op te nemen.
>
>* Voor algemene informatie over het delen van voorwerpen in de Planning van Workfront, zie ook [ Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront ](/help/quicksilver/planning/access/sharing-permissions-overview.md).
>* Voor meer informatie, zie de [ Overwegingen wanneer het delen van verslagtypes ](#considerations-when-sharing-record-types) sectie in dit artikel.

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.

<!--at GA, check that the Workfront plans article linked below has Planning info-->

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
<p>Het geval van Workfront van uw organisatie moet aan de Verenigde Ervaring van Adobe worden genegeerd om tot de Planning van Workfront te kunnen toegang hebben.</p> 
<p>Gebruikers moeten aan de Adobe Admin Console worden toegevoegd om machtigingen te verkrijgen voor de Workfront-planningsweergaven.</p>
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
   <td>  <p>Machtigingen beheren voor een recordtype</p>  
   <p>Alleen gebruikers met de machtiging Beheren in een werkruimte kunnen beheermachtigingen delen met een recordtype</p></td> 
  </tr>

</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het delen van recordtypen

* Het verlenen van toestemmingen aan een werkruimte geeft gebruikers de zelfde toestemmingen aan de verslagtypes in de werkruimte, door gebrek.

  Bovendien kunt u machtigingen voor afzonderlijke recordtypen aanpassen.

  Nochtans, kunt u mensen geen hogere toestemmingen aan een verslagtype verlenen dan de toestemmingen zij aan de werkruimte hebben.
* U kunt gebruikers lagere machtigingen verlenen voor het recordtype dan in de werkruimte. Ze kunnen bijvoorbeeld beschikken over Contribute-machtigingen voor de werkruimte en weergavemachtigingen voor een recordtype.
* Personen met de machtiging Beheren voor de werkruimte hebben altijd toegang tot alle recordtypen in de werkruimte. Hun toestemmingen kunnen niet op verslagtypes worden verminderd, zelfs wanneer de Geërfte toestemmingen worden uitgezet.

* Op dit moment kunt u het volgende bereiken wanneer u recordtypen deelt:

   * Geef mensen de toestemmingen van de Mening aan een werkruimte, wanneer u een verslagtype met hen voor het eerst deelt en zij hebben geen toestemmingen aan de werkruimte.

     Dit geeft hen ook de toestemmingen van de Mening aan alle verslagtypes in de werkruimte.

     Aangezien u hen toestemmingen aan het verslagtype geeft, is er een aanwijzing in het het delen vakje dat zij ook aan de werkruimte worden toegevoegd.
   * Maak het verslagtype mening-slechts voor iedereen in de werkruimte (behalve werkruimtemanagers), wanneer u Geërfte toestemmingen onbruikbaar maakt.

     Personen met de machtiging Beheren voor de werkruimte beschikken altijd over de machtiging Beheren voor de recordtypen, zelfs wanneer u de machtiging Geërfd voor het recordtype uitschakelt.
   * Minder bevoegdheden voor een recordtype. U kunt de toestemming van iemand aan een recordtype niet verhogen van wat hij op de werkruimte heeft.

     Als iemand bijvoorbeeld Contribute-machtigingen heeft voor de werkruimte, kunt u hun machtigingen wijzigen in een specifiek recordtype in Weergeven. Als ze echter over weergavemachtiging voor de werkruimte beschikken, kunt u ze geen Contribute-machtiging voor een recordtype verlenen.

* Het is niet mogelijk om toegang tot een recordtype voor mensen in de werkruimte te verwijderen. Iedereen heeft altijd minstens de toestemming van de Mening aan alle verslagtypes als zij minstens de toestemmingen van de Mening aan de werkruimte hebben.

* U kunt een recordtype intern delen met de volgende entiteiten:

  Workfront-gebruikers, -groepen, -teams, -bedrijven en -functies
* U kunt recordtypen niet extern delen met gebruikers buiten Workfront.
* Als u een gebruiker zonder werkruimtemachtigingen hoger wilt weergeven dan weergavemachtigingen, moet u de werkruimte eerst met deze gebruikers delen met een hogere machtiging dan Weergave. De hogere toestemmingen voor de werkruimte zullen dan op de verslagtypes van toepassing zijn.

## Machtigingen delen voor een recordtype

U kunt machtigingen aanpassen voor afzonderlijke recordtypen in een werkruimte als u beheerdersmachtigingen hebt voor de werkruimte.

{{step1-to-planning}}

1. Open de werkruimte waarvan u de recordtypen wilt delen.

1. Voer een van de volgende handelingen uit:

   * <span class="preview"> van de kaart van het verslagtype, klik **Meer** menu > **Aandeel**.</span>
   * Klik een kaart van het verslagtype om de pagina van het verslagtype te openen, dan klik **Aandeel** > **Deel het verslagtype** van om het even welke verslagtypemening.

   Het **vakje van het Aandeel** opent.

   ![ Toestemmingen voor verslagtypes met geërfte toestemmingen op ](assets/permissions-for-record-types-with-inherited-permissions-on.png)

1. (Facultatief) in **die toegang** heeft, kan **iedereen in de werkruimte** optie bekijken door gebrek worden geselecteerd.  Alle gebruikers met de machtiging Weergave of hoger voor de werkruimte kunnen het recordtype weergeven.

1. (Facultatief) klik het aantal gebruikers onder de **Geërfte toestemmingen** optie om gebruikers, teams, groepen, bedrijven, of baanrollen te bekijken die toestemmingen van de werkruimte erven.

   >[!TIP]
   >
   >U kunt afzonderlijke entiteiten niet verwijderen uit de lijst Geërfde machtigingen.

1. (Optioneel en voorwaardelijk) Als u het recordtype wilt delen met specifieke entiteiten en deze een andere toegang tot het recordtype wilt geven dan ze al hebben voor de werkruimte, gaat u als volgt te werk:

   1. Selecteer **onbruikbaar maken** van **Geërfte toestemmingen** drop-down menu.

   >[!TIP]
   >
   >Workspace-managers blijven beheerdersmachtigingen voor het recordtype hebben.

   1. In de **toegang van de Verlening tot dit verslagtype** gebied, voeg de gebruikers, de teams, de groepen, de bedrijven, of baanrollen toe die u een verschillend toestemmingsniveau aan wilt verlenen dan zij voor de werkruimte hebben.
   1. Kies een machtigingsniveau.

   >[!IMPORTANT]
   >
   >* Naast teams, groepen, bedrijven, en baanrollen, kunt u slechts met gebruikers delen die aan Adobe Admin Console zijn toegevoegd. U kunt geen gebruikers met alleen Workfront toevoegen. Voor informatie, zie [ gebruikers in Adobe Admin Console ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md) leiden.
   >* U kunt gebruikers nooit meer machtigingen geven voor een recordtype dan op een werkruimte.
   >* U kunt gebruikers niet minder bevoegdheden geven dan Beheren voor een recordtype, als zij beheerdersmachtigingen voor de werkruimte hebben.
   >* U kunt gebruikers minder bevoegdheden geven aan het recordtype als zij over Contribute-machtigingen voor de werkruimte beschikken.
   > Voor meer informatie, zie [ Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront ](/help/quicksilver/planning/access/sharing-permissions-overview.md).

1. Om gebruikers te geven die geen toestemmingen aan de werkruimtetoegang hebben om een verslagtype, op de **toegang van de Verlening tot dit mening** gebied te bekijken, begin de naam van een gebruiker, een groep, een team, een bedrijf, of baanrol te typen, dan het te klikken wanneer het in de lijst toont.

   De entiteit u selecteerde wordt toegevoegd aan het verslagtype en aan de werkruimte met **toestemmingen van de Mening**.

   Systeembeheerders ontvangen altijd beheermachtigingen om gegevenstypen op te nemen die met hen worden gedeeld, en er is een indicatie dat een gebruiker een systeembeheerder is.

1. (Facultatief) klik **verbinding van het Exemplaar** om een verbinding aan het verslagtype aan uw klembord te kopiëren en het met anderen te delen.
1. Klik **sparen**.

   Het recordtype wordt nu gedeeld met andere gebruikers.
De gebruikers die u het recordtype hebt gedeeld, ontvangen zowel een melding in de app als een e-mailmelding dat zij machtigingen hebben verleend aan de volgende entiteiten:

   * Het recordtype
   * De werkruimte, als zij geen toestemmingen aan de werkruimte hadden alvorens het verslagtype met hen werd gedeeld.

1. Deel de gekopieerde koppeling met anderen. Gebruikers die de koppeling ontvangen, moeten actieve gebruikers zijn en zich aanmelden bij Workfront om de pagina met recordtypen te kunnen openen en weergeven in de geselecteerde weergave. Zij moeten toestemmingen aan het verslagtype hebben om het te kunnen bekijken.

## Machtigingen verwijderen van een recordtype

U kunt gebruikersmachtigingen verwijderen uit een recordtype. Ze behouden echter ten minste weergavemachtigingen voor de werkruimte die hun ten minste weergavemachtigingen voor het recordtype geven. U moet hun toegang uit de werkruimte verwijderen als u wilt dat zij geen machtigingen hebben voor de recordtypen in de werkruimte.

{{step1-to-planning}}

1. Open de werkruimte waarvan recordtypen u wilt ophouden met delen en klik vervolgens op een opnametype-kaart. Hierdoor wordt de pagina met recordtypen geopend.

1. Van het lusje van om het even welke mening, klik **Aandeel** in de hoger-juiste hoek van het verslagtype.
1. Klik **Deel het verslagtype**.

   Het **vakje van het Aandeel** opent.
1. Vind de gebruiker, de groep, het team, het bedrijf, of de baanrol die de toestemmingen u wilt verwijderen, het drop-down menu van toestemmingen rechts van hun naam uitbreiden, dan **verwijderen** klikken. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![ verwijdert optie op verslagtype dat drop-down deelt ](assets/remove-option-on-record-type-sharing-drop-down.png)

1. Klik **sparen**.

   Personen beschikken niet meer over de aangegeven machtigingen voor het recordtype. Ze hebben echter nog steeds machtigingen voor de werkruimte, tenzij u ze ook verwijdert uit de werkruimtemachtigingen.

   Er is geen bericht voor de gebruikers die zijn verwijderd van toegang tot de weergave, dat zij deze toegang niet meer hebben.

<!-- This is not working yet: *************************** edit this before publishing, because this was not tested with record types - this section came from sharing views *******************: 

## Grant permissions to a record type from a permission request

Users who access a link to a record type to which they do not have permissions can request permissions to the record type. All users with Manage permissions to the view receive the permission request and can grant or deny the permissions. 

1. (Conditional) If you are are the manager of a view, you might receive a request from another user to access the view in the following areas:
   
   * An in-app notification
      ![In-app notification for access request for view](assets/in-app-notification-for-access-request-for-view.png)
   * An email notification
      ![In-app notification for access request for view](assets/in-app-notification-for-access-request-for-view.png)
1. (Conditional) From the notification area in Workfront, click the in-app notification
   Or
   From the email notification, click **View all notifications**, then click the notification in the list.

   The **Pending access requests** box displays. 

      ![Notifications list approval box](assets/notifications-list-approval-box.png)
1. (Optional) For the user whose permissions you want to approve, select one of the following options from the drop-down menu to the right of the user's name: 
   * **View**
   * **Manage**
1. Select the user for whom you want to approve or deny the permission, then click **Approve all** or **Deny all**. 
1. Click the left-pointing arrow to the left of **Pending access requests**, then click **Save**.

   If you approved the request, the users are added to the sharing box of the view. The user requesting the permission receives an email confirmation that their request was approved. <!--will they also get an in-app notification??-->

