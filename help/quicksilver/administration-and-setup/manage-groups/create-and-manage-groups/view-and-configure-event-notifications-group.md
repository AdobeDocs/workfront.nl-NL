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

Voor informatie over hoe een Workfront-beheerder een gebeurtenismelding ontgrendelt, raadpleegt u [Configuratie van gebeurtenismeldingen voor alle groepen ontgrendelen of vergrendelen](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

Voor informatie over de standaardmeldingsinstelling voor een gebeurtenis raadpleegt u [Typen gebeurtenismeldingen](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

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
   <td> <p>Plan </p> <p>U moet een groepsbeheerder van de groep of een beheerder van Workfront zijn. Zie voor meer informatie <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Groepbeheerders</a> en <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de Workfront-beheerder als u wilt weten welk abonnement- of licentietype u hebt.

## De gebeurtenismeldingen van een groep weergeven en configureren

1. (Voorwaardelijk en optioneel) Als u een Workfront-beheerder bent en u zich al op de pagina E-mailmeldingen bevindt (Setup > E-mail > Meldingen), kunt u het volgende doen en verdergaan met stap 6: Verwijderen **Systeemgebeurtenismeldingen** typ in het vak boven de lijst de naam van de groep in het vak en klik vervolgens op de naam wanneer deze wordt weergegeven.
1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Groepen** ![](assets/groups-icon.png).

1. Klik op de naam van de bovenste groep.
1. Klik in het linkermenu op **Gebeurtenismeldingen**.

   In de lijst die wordt weergegeven, **Actief** in de linkerkolom wordt aangegeven welke meldingen actief (blauw) en inactief (grijs) zijn voor de groep.

1. U activeert of deactiveert een ontgrendelde gebeurtenismelding door op de knop in het dialoogvenster <strong>Actief</strong> te activeren kolom <img src="assets/email-notification-enabled-unlocked.png"> of deactiveren <img src="assets/email-notification-disabled-unlocked.png"> het.

   >[!INFO]
   >
   >**Voorbeeld:** U kon de hoogste twee hieronder getoonde de de groepsgebeurtenisberichten van de Marketing vormen die voor groepen ontgrendeld zijn.</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* Als een knop in het dialoogvenster <strong>Actief</strong> de kolom is grijs en wordt grijs weergegeven <img src="assets/email-notification-disabled-locked.png">, wordt de gebeurtenismelding gedeactiveerd voor alle gebruikers en groepsbeheerders kunnen deze niet activeren of de onderwerpregel van de e-mail niet bewerken
   >* Als een knop in het dialoogvenster <strong>Actief</strong> de kolom is grijs en niet gedimd <img src="assets/email-notification-disabled-unlocked.png">, de gebeurtenis wordt gemeld <strong>gedeactiveerd voor alle gebruikers en</strong> groepsbeheerders kunnen deze activeren voor hun groepen.
   >* Als een knop in het dialoogvenster <strong>Actief</strong> kolom is blauw en is grijs <img src="assets/email-notification-enabled-locked.png">, wordt het gebeurtenisbericht geactiveerd voor alle gebruikers en groepsbeheerders kunnen het niet deactiveren of de e-mailonderwerpregel van het bericht voor hun groepen bewerken.
   >* Als een knop in het dialoogvenster <strong>Actief</strong> kolom is blauw en niet gedimd <img src="assets/email-notification-enabled-unlocked.png">, de gebeurtenis wordt gemeld <strong>geactiveerd voor alle gebruikers en</strong> groepsbeheerders kunnen deze voor hun groepen deactiveren.

<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

