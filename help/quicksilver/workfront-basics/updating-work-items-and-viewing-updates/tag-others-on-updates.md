---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Andere tags toepassen op updates
description: Wanneer u updatecommentaren op een Adobe Workfront-object opgeeft, kunnen alle gebruikers van het project de verzonden informatie zien. Er kunnen zich echter situaties voordoen waarin gebruikers die zich niet bij het project bevinden, baat zouden hebben bij het bekijken van deze informatie. In plaats van deze gebruikers op te nemen in het project, kunt u ze labelen op de update om deze met hen te delen. Gelabelde gebruikers ontvangen een gebeurtenismelding.
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 886b5d9084cb1bfb63157152f05fa20128d34903
workflow-type: tm+mt
source-wordcount: '997'
ht-degree: 0%

---

# Andere tags toepassen op updates

<!--Audited: April, 2024-->

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process. </span> 
-->

U kunt gebruikers tags toewijzen wanneer u een update uitvoert naar een object als u de aandacht wilt vestigen op een object dat ze anders wellicht niet volgen.

In plaats van deze gebruikers op het object te plaatsen door ze eraan toe te wijzen of door ze ertoe te brengen zich erop te abonneren, kunt u ze in de update labelen om het met hen te delen. Getagde gebruikers ontvangen een Workfront-melding over de update die u invoert. Afhankelijk van hun meldingsinstellingen ontvangen zij ook een e-mail over de update die u invoert.

## Overwegingen over het coderen van gebruikers in updates

* Gebruikers die updates hebben gecodeerd, moeten een persoonlijke melding inschakelen in hun profiel om de e-mailmelding te ontvangen. Zie voor meer informatie [Uw eigen e-mailmeldingen wijzigen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  Voor informatie over het toevoegen van updates aan Workfront-objecten raadpleegt u [Werk bijwerken](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* Wanneer een kwestie in een project of een taak wordt omgezet, worden de updates gekopieerd aan het nieuwe project of de taak, maar de geëtiketteerde gebruikers niet. Om het gesprek voort te zetten, moet u de deelnemers opnieuw etiketteren.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie*</strong></td> 
   <td> <p>Nieuw: Medewerker of hoger voor uitgaven en documenten; licht of hoger voor alle andere objecten</p>
   <p>Huidig: Verzoek of hoger voor uitgaven en documenten; Controleren of hoger voor alle andere objecten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuratie op toegangsniveau</strong></td> 
   <td> <p>Toegang tot de objecten weergeven waar u het antwoord wilt plaatsen of vergroten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtiging</strong></td> 
   <td> <p>Machtigingen weergeven of hoger voor de objecten waar u het antwoord wilt plaatsen</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt. Zie voor meer informatie [Toegangsvereisten voor Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Andere tags toepassen op updates

U kunt op de volgende manieren tags toewijzen aan anderen bij updates:

* **Automatisch**: Wanneer een gebruiker een thread start, een opmerking toevoegt of een antwoord toevoegt, worden deze automatisch gelabeld en toegevoegd aan het gebied Tagpersonen of -teams van het opmerkingvak. <!--remove the tip below when the new commenting stream is the only stream and the legacy commenting is removed-->

* **Handmatig**: Wanneer u handmatig een gebruiker toevoegt aan het gebied Tagpersonen van het opmerkingsvak.

U kunt ook gebruikers verwijderen die per ongeluk zijn gelabeld wanneer u een opmerking bewerkt of erop reageert.

1. Beginnen met het bijwerken van een tijdelijk item, zoals beschreven in [Werk bijwerken](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). Als eigenaar van de opmerking wordt u automatisch gelabeld en toegevoegd aan het gebied Tagpersonen of -teams in het opmerkingvak.

   >[!TIP]
   >
   >De eigenaar van de opmerking kan zijn of haar eigen naam niet zien in het gebied Tagpersonen of -teams van het opmerkingvak.

1. In de **Tags toewijzen aan personen of teams** typt u de naam van de gebruiker of het team dat u wilt opnemen en klikt u op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.

   of

   Typ het @-symbool in het dialoogvenster **Een opmerking schrijven** typt u de naam van de gebruiker of het team dat u in de update wilt opnemen en klikt u vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.

   >[!TIP]
   > 
   >Als u de juiste gebruiker wilt identificeren wanneer er gebruikers met vergelijkbare of identieke namen zijn, ziet u de avatar, de primaire rol van de gebruiker of hun e-mailadres.
   > 
   >Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze in een update codeert.
   > 
   >De instelling Contactinfo weergeven moet zijn ingeschakeld op uw toegangsniveau zodat gebruikers de e-mails van gebruikers kunnen bekijken. Zie voor meer informatie [Toegang verlenen aan gebruikers](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![Tags toewijzen aan een gebruiker](assets/tag-others-unified-commenting-with-all-tab.png)

1. (Optioneel) Schakel de optie **Privé voor mijn bedrijf** in de rechterbenedenhoek van het updatevak. Hierdoor is de update alleen zichtbaar voor gebruikers in uw bedrijf. De **Privé voor mijn bedrijf** Deze optie is alleen beschikbaar wanneer een bedrijf is opgegeven in uw Workfront-profiel.

   >[!NOTE]
   >
   >* Deze optie toont slechts wanneer de gebruiker met een Bedrijf wordt geassocieerd.
   >* Gelabelde gebruikers buiten het bedrijf konden nog steeds een melding in de app of een e-mail ontvangen, ook al zullen ze de persoonlijke opmerkingen op het tabblad Updates niet zien. We raden u aan geen tags toe te wijzen aan externe gebruikers tijdens een update als u de gegevens niet met hen wilt delen.

1. (Optioneel) Herhaal stap 2 om meerdere gebruikers en teams toe te voegen. <!--insure this stays accurate-->

   >[!NOTE]
   >
   >Alle gebruikers en teamleden die in het veld &quot;Tagpersonen of -teams&quot; worden vermeld, ontvangen een melding in de app voor de update en ontvangen mogelijk een e-mail, afhankelijk van de configuratie van hun instellingen voor e-mailmeldingen. Gebruikers die zichzelf in een opmerking of antwoord labelen, ontvangen een melding voor die opmerking of reactie en kunnen hun naam als lid van de thread voor de rest van de thread zien, maar ontvangen geen andere melding tenzij ze zichzelf opnieuw labelen. Zie voor meer informatie [Uw eigen e-mailmeldingen wijzigen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) en [Gebeurtenismeldingen configureren voor iedereen in het systeem](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Klikken **Verzenden**.\
   Aan gebruikers die zijn opgenomen in de update, wordt automatisch weergavemachtiging toegekend aan het object en deze gebruikers kunnen updates die aan het object zijn toegevoegd, weergeven en erop reageren.

   De namen van de getagde entiteiten worden naast hun avatars (maximaal twee entiteiten) weergegeven. Als er meerdere entiteiten zijn gelabeld, wordt de naam van de eerste entiteit weergegeven, plus het aantal extra entiteiten dat is gelabeld.

   ![](assets/members-icons-expanded-unshimmed.png)

   Wanneer u in de opmerkingstekst bent gelabeld, wordt uw naam gemarkeerd in die opmerkingen.

   Voor informatie over de extra functionaliteit die beschikbaar is wanneer het bijwerken van een het werkpunt, zie [Werk bijwerken](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Optioneel) Klik op de knop **Meer** menu ![](assets/more-menu.png) in de rechterbovenhoek van de opmerking klikt u op **Bewerken**. Verwijder alle getagde gebruikers en klik vervolgens op **Verzenden**.

   >[!IMPORTANT]
   >
   >U kunt een opmerking pas bewerken binnen 15 minuten nadat u deze hebt ingevoerd. U kunt alleen de opmerkingen bewerken die u hebt toegevoegd.


<!--
   >[!TIP]
   >
   >When using the legacy commenting experience to add comments and replies, comment owners that were not specifically tagged cannot be manually removed by people who use the new commenting experience.
-->

<!--
### Tag others on updates in the legacy Updates section

You can manually tag users in the legacy Updates section. 

1. Begin updating a work item, as described in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In the **Notify** field, begin typing the name of the user or team you want to include, then click the name when it appears in the drop-down list.

   Or

   Type the @ symbol in the **Start a new update** area, begin typing the name of the user or team you want to include on the update, then click the name when it appears in the drop-down list.

   >[!TIP]
   >
   >To identify the correct user when there are users with similar or identical names, notice the avatar, the user's Primary Role, or their email address. 
   >
   >Users must be associated with at least one job role to view it as you tag them in an update. 
   >
   >You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-users-in-update.png)

1. (Optional) To make the update private, enable **Private to my company** in the lower-right corner of the update box. This makes the update visible just to users in your company. The **Private to my company** option is available only when a Company is specified in your Workfront profile. 

   >[!NOTE]
   >
   >Tagged users outside the company could still receive an in-app notification or email, even though they will not see the private comments on the Updates tab. We recommend not to tag external users on an update if you do not want to share the information with them.  

1. (Optional) To add multiple users and teams, repeat step 2.

   >[!NOTE]
   >
   >All users and team members listed in the Notify field receive an in-app notification for the update and might receive an email, depending on the configuration of their email notification settings. Users who tag themselves in a comment or reply receive a notification for that comment or reply and can see their name in the Notify field for the remainder of the thread, but they do not receive another notification unless they tag themselves again. For more information, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) and [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Click **Update**.  
   Users included in the update are automatically granted View permission to the object and can view and respond to updates made to the object.

   You can see who has been tagged in each reply at the top of the update thread. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object.

   ![](assets/tagging-transparency-350x192.png)
-->

Voor informatie over de extra functionaliteit die beschikbaar is wanneer het bijwerken van een het werkpunt, zie [Werk bijwerken](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).



