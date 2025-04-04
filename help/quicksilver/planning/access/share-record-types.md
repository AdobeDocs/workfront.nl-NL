---
title: Recordtypen delen
description: U kunt een recordtype met anderen delen om samenwerking te verzekeren wanneer het gebruiken van de Planning van Adobe Workfront.
hide: true
hidefromtoc: true
exl-id: bf49db73-09f1-417e-836b-16c6062740d4
source-git-commit: 4df268c9b5a99991bee3f1862c83fe0079d162c1
workflow-type: tm+mt
source-wordcount: '1308'
ht-degree: 0%

---

<!-- add these to metadata on release:

author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog-->

<!-- take the Remove permissions section out, at the end - this is what Lilit said: Because of "Everyone in the workspace can view" wildcard, currently it's not possible to entirely remove access to a record type. Let's take out this section. -->

# Recordtypen delen

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

U kunt een recordtype met anderen delen om samenwerking te verzekeren wanneer het werken met verslagen in de Planning van Adobe Workfront.

>[!IMPORTANT]
>
>* Het verlenen van toestemmingen aan een werkruimte geeft gebruikers de zelfde toestemmingen aan de verslagtypes in de werkruimte, door gebrek.
>* Bovendien kunt u machtigingen voor afzonderlijke recordtypen aanpassen.
>* Nochtans, kunt u mensen geen hogere toestemmingen aan een verslagtype verlenen dan de toestemmingen zij aan de werkruimte hebben.
>* Personen met de machtiging Beheren voor de werkruimte hebben altijd toegang tot alle recordtypen in de werkruimte. Hun toestemmingen kunnen niet op verslagtypes worden verminderd, zelfs wanneer de Geërfte toestemmingen worden uitgezet.
> 
> Voor meer informatie, zie de [ Overwegingen wanneer het delen van verslagtypes ](#considerations-when-sharing-record-types) sectie in dit artikel.

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
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden bezeten om tot alle mogelijkheden van de Planning van Workfront toegang te hebben.</p> 
<p>Uw organisatie moet aan de Verenigde Ervaring van Adobe voor gebruikers worden bezet om toestemmingen aan een mening van een toestemmingsverzoek te kunnen verzoeken en verlenen. </p>
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
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het delen van recordtypen

* Voor algemene informatie over het delen van voorwerpen in de Planning van Workfront, zie ook [ Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront ](/help/quicksilver/planning/access/sharing-permissions-overview.md).

* Op dit moment kunt u het volgende bereiken wanneer u recordtypen deelt:
   * Geef mensen de toestemmingen van de Mening aan een werkruimte, wanneer u een verslagtype met hen voor het eerst deelt en zij hebben geen toestemmingen aan de werkruimte.

     Dit geeft hen ook de toestemmingen van de Mening aan alle verslagtypes in de werkruimte.

     Aangezien u hen toestemmingen aan het verslagtype geeft, is er een aanwijzing in het het delen vakje dat zij ook aan de werkruimte worden toegevoegd.
   * Maak het verslagtype mening-slechts voor iedereen in de werkruimte (behalve werkruimtemanagers), wanneer u Geërfte toestemmingen uitzet.

     Personen met de machtiging Beheren voor de werkruimte beschikken altijd over de machtiging Beheren voor de recordtypen, zelfs wanneer u de machtiging Geërfd voor het recordtype uitschakelt.
  <!-- checking with Lilit - this doesn't make much sense: * Add people with Contribute permission to the workspace, who will retain Contribute permission to the record type. This way, only the selected people can manage records in the record type, while others can only view them. -->
   * Minder bevoegdheden voor een recordtype. U kunt de toestemming van iemand aan een recordtype niet verhogen van wat hij op de werkruimte heeft.

     Als iemand bijvoorbeeld Contribute-machtigingen heeft voor de werkruimte, kunt u hun machtigingen wijzigen in een specifiek recordtype in Weergeven. Als ze echter over weergavemachtiging voor de werkruimte beschikken, kunt u ze geen Contribute-machtiging voor een recordtype verlenen.

* Het is niet mogelijk om toegang tot een recordtype voor mensen in de werkruimte te verwijderen. Iedereen heeft altijd minstens de toestemming van de Mening.

* U kunt een recordtype intern delen met de volgende entiteiten:

   * Workfront-gebruikers, -groepen, -teams, -bedrijven en -functies
* U kunt recordtypen niet extern delen met gebruikers buiten Workfront.
* Als u een gebruiker zonder werkruimtemachtigingen hoger wilt weergeven dan weergavemachtigingen, moet u de werkruimte eerst met deze gebruikers delen met een hogere machtiging dan Weergave.

## Machtigingen delen voor een recordtype

U kunt machtigingen aanpassen voor afzonderlijke recordtypen in een werkruimte als u beheerdersmachtigingen hebt voor de werkruimte.

{{step1-to-planning}}

1. Open de werkruimte waarvan recordtypen u wilt delen en klik vervolgens op een opnametype-kaart.

   Hierdoor wordt de pagina met recordtypen geopend.

1. Van het lusje van om het even welke mening, klik **Aandeel** in de hoger-juiste hoek van het verslagtype.

   Het **vakje van het Aandeel** opent.

   ![ Toestemmingen voor verslagtypes met geërfte toestemmingen op ](assets/permissions-for-record-types-with-inherited-permissions-on.png)

1. (Facultatief) op **die toegang** heeft, selecteer van de volgende opties: <!--the Only invited people is supposed to be removed - rewrite this - according to Vahan-->

   * **slechts kunnen de uitgenodigde mensen tot** toegang hebben: U moet gebruikers, groepen, team, bedrijf, of baanrollen specificeren die u de mening met wilt delen.
   * **iedereen in de werkruimte kan** bekijken: Alle gebruikers die Mening of hogere toestemmingen aan de werkruimte hebben kunnen tot de mening toegang hebben. Dit is de standaardoptie. <!--rewrite this based on what Lilit says in the proof: At this point, once the inherited permissions are disabled, everyone in the workspace except workspace managers will have View permission to the record type because the "Everyone in the workspace can view"  setting cannot be changed. -->

1. (Facultatief) breid **Geërfte toestemmingen** optie uit om gebruikers, teams, groepen, bedrijven, of baanrollen te bekijken die toestemmingen van de werkruimte erven.

   >[!TIP]
   >
   >U kunt afzonderlijke entiteiten niet verwijderen uit de lijst Geërfde machtigingen.


1. (Optioneel en voorwaardelijk) Als u het recordtype wilt delen met specifieke entiteiten en deze een andere toegang tot het recordtype wilt geven dan ze al hebben voor de werkruimte, gaat u als volgt te werk:

1. **Draai van** Geërfte toestemmingen.

   >[!TIP]
   >
   >Workspace-managers blijven beheerdersmachtigingen voor het recordtype hebben.

   1. In de **toegang van de Verlening tot dit verslagtype** gebied, voeg de gebruikers, de teams, de groepen, de bedrijven, of baanrollen toe die u een verschillend toestemmingsniveau aan wilt verlenen.
   1. Kies een machtigingsniveau.


   >[!IMPORTANT]
   >
   >* U kunt gebruikers nooit meer machtigingen geven voor een recordtype dan op een werkruimte.
   >* U kunt gebruikers niet minder bevoegdheden geven dan Beheren voor een recordtype, als zij beheerdersmachtigingen voor de werkruimte hebben.
   >* U kunt gebruikers minder bevoegdheden geven aan het recordtype als zij over Contribute-machtigingen voor de werkruimte beschikken.
   > Voor meer informatie, zie [ Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront ](/help/quicksilver/planning/access/sharing-permissions-overview.md).

1. Om gebruikers te geven die geen toestemmingen aan de werkruimtetoegang hebben om verslagtype, op de **toegang van de Verlening tot dit mening** gebied te bekijken, begin de naam van een gebruiker, een groep, een team, een bedrijf, of baanrol te typen, dan het te klikken wanneer het in de lijst toont.

   De entiteit u selecteerde wordt toegevoegd aan het verslagtype en aan de werkruimte met **toestemmingen van de Mening**.

   Systeembeheerders ontvangen altijd beheermachtigingen om gegevenstypen op te nemen die met hen worden gedeeld, en er is een indicatie dat een gebruiker een systeembeheerder is.

1. Klik **verbinding van het Exemplaar** om een verbinding aan het verslagtype aan uw klembord te kopiëren.
1. Klik **sparen**.

   Het recordtype wordt nu gedeeld met andere gebruikers.

1. Deel de gekopieerde koppeling met anderen. Gebruikers die de koppeling ontvangen, moeten actieve gebruikers zijn en zich aanmelden bij Workfront om de pagina met recordtypen te kunnen openen en weergeven in de geselecteerde weergave.

## Machtigingen verwijderen van een recordtype

{{step1-to-planning}}

1. Open de werkruimte waarvan recordtypen u wilt ophouden met delen en klik vervolgens op een opnametype-kaart. Hierdoor wordt de pagina met recordtypen geopend.

1. Van het lusje van om het even welke mening, klik **Aandeel** in de hoger-juiste hoek van het verslagtype.

   Het **vakje van het Aandeel** opent.
1. Vind de gebruiker, de groep, het team, het bedrijf, of de baanrol die de toestemmingen u wilt verwijderen, het drop-down menu van toestemmingen rechts van hun naam uitbreiden, dan **verwijderen** klikken. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![ verwijdert optie op verslagtype dat drop-down deelt ](assets/remove-option-on-record-type-sharing-drop-down.png)

1. Klik **sparen**.

   Personen hebben geen toegang meer tot het recordtype. Ze kunnen nog steeds machtigingen voor de werkruimte hebben, tenzij u ze ook verwijdert van werkruimtemachtigingen.

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

