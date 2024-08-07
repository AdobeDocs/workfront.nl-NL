---
user-type: administrator
product-area: system-administration;user-management
keywords: weergave,groep,gebeurtenis,meldingen,configureren,inschakelen,uitschakelen
navigation-topic: create-and-manage-groups
title: Gebeurtenismeldingen voor een groep weergeven en configureren
description: Als groepsbeheerder kunt u de gebeurtenismeldingen weergeven die zijn geactiveerd voor een groep die u beheert. Ook, als een beheerder van Adobe Workfront een gebeurtenisbericht ontgrendelt, kunt u het voor een top-level groep vormen die u beheert. Configuratie van een gebeurtenismelding bestaat uit het activeren of deactiveren ervan.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Gebeurtenismeldingen voor een groep weergeven en configureren

Als groepsbeheerder kunt u de gebeurtenismeldingen weergeven die zijn geactiveerd voor een groep die u beheert.

Ook, als een beheerder van Adobe Workfront een gebeurtenisbericht ontgrendelt, kunt u het voor een top-level groep vormen die u beheert. Configuratie van een gebeurtenismelding bestaat uit het activeren of deactiveren ervan.

Een Workfront-beheerder kan dit ook voor elke groep doen.

Het vormen van een gebeurtenisbericht voor een groep beïnvloedt gebruikers voor wie die groep, of één van zijn subgroepen, hun Groep van het Huis is. In hun gebruikersprofielen zien deze gebruikers de gebeurtenismeldingen die voor hun thuisgroep zijn geactiveerd in plaats van de gebeurtenismeldingen die voor het hele systeem zijn geactiveerd.

Voor informatie over hoe een beheerder van Workfront een gebeurtenisbericht ontgrendelt, zie [ configuratie van gebeurtenisberichten voor alle groepen ](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) ontgrendelen of sluiten.

Voor informatie over het standaardbericht dat voor een gebeurtenis plaatst, zie [ de berichttypes van de Gebeurtenis ](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> <p>U moet een groepsbeheerder van de groep of een beheerder van Workfront zijn. Voor meer informatie, zie <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref"> de beheerders van de Groep </a> en <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> verlenen een gebruiker volledige administratieve toegang </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; als u moet weten welk plan of licentietype u hebt, contacteer uw beheerder van Workfront.

## De gebeurtenismeldingen van een groep weergeven en configureren

1. (Voorwaardelijk en facultatief) als u een beheerder van Workfront bent en u reeds op de E-mailmeldingspagina (Opstelling > E-mail > Meldingen) bent, kunt u het volgende doen en dan overslaan aan stap 6: De Berichten van de Gebeurtenis van het Systeem van de Schrapping **in de doos boven de lijst, beginnen de naam van de groep in de doos te typen, dan het te klikken wanneer het verschijnt.**
1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Opstelling** ![](assets/gear-icon-settings.png).

1. In het linkerpaneel, klik **Groepen** ![](assets/groups-icon.png).

1. Klik op de naam van de bovenste groep.
1. In het linkermenu, klik **de berichten van de Gebeurtenis**.

   In de lijst die toont, toont de **Actieve** kolom op de linkerzijde welke berichten actief (blauw) en inactief (grijs) voor de groep zijn.

1. Om een ontgrendeld gebeurtenisbericht te activeren of onbruikbaar te maken: klik de knoop in de <strong> Actieve </strong> kolom om te activeren <img src="assets/email-notification-enabled-unlocked.png"> of deactiveren <img src="assets/email-notification-disabled-unlocked.png"> it.

   >[!INFO]
   >
   >**Voorbeeld:** u kon de hoogste twee hieronder getoonde de de groepsgebeurtenisberichten van de Marketing vormen die voor groepen zijn ontgrendeld.</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* Als een knoop in de <strong> Actieve </strong> kolom grijs en verduisterd is <img src="assets/email-notification-disabled-locked.png"> , wordt de gebeurtenismelding gedeactiveerd voor alle gebruikers en groepsbeheerders kunnen deze niet activeren of de e-mailonderwerpregel ervan bewerken
   >* Als een knoop in de <strong> Actieve </strong> kolom grijs is en niet gedimd <img src="assets/email-notification-disabled-unlocked.png">, wordt het gebeurtenisbericht <strong> gedeactiveerd voor alle gebruikers en </strong> groepsbeheerders kunnen het voor hun groepen activeren.
   >* Als een knoop in de <strong> Actieve </strong> kolom blauw en verduisterd is <img src="assets/email-notification-enabled-locked.png"> , wordt de gebeurtenismelding geactiveerd voor alle gebruikers en groepsbeheerders kunnen deze niet deactiveren of de e-mailonderwerpregel van deze gebruiker voor hun groepen bewerken.
   >* Als een knoop in de <strong> Actieve </strong> kolom blauw en niet gedimd is <img src="assets/email-notification-enabled-unlocked.png">, wordt het gebeurtenisbericht <strong> geactiveerd voor alle gebruikers en </strong> groepsbeheerders kunnen het voor hun groepen deactiveren.

<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

