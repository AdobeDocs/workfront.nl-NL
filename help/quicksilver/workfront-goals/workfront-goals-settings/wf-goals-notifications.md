---
content-type: reference
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Meldingen voor Adobe Workfront-doelen inschakelen
description: Adobe Workfront Goals wordt geleverd met een set vooraf gedefinieerde gebeurtenismeldingen die u kunt inschakelen voor uw account. Deze gebeurtenismeldingen activeren e-mailcommunicatie telkens wanneer aan de door de gebeurtenis gedefinieerde voorwaarde wordt voldaan.
author: Alina
feature: Workfront Goals
exl-id: 40f9b9a3-c829-480b-9897-099b68389cd4
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---

# Meldingen voor Adobe Workfront-doelen inschakelen

>[!IMPORTANT]
>
>Uw organisatie moet het volgende hebben om de functionaliteit te gebruiken die in dit artikel wordt beschreven:
>
>* Voor het nieuwe plan en de nieuwe licentiestructuur:
>
>   * Het Ultimate Workfront-plan
>    
>* Voor het huidige plan en de licentiestructuur:
>
>   * Een Pro- of hoger Workfront-abonnement
>   * Een Adobe Workfront Goals-licentie in aanvulling op een Workfront-licentie.
>
>Neem contact op met uw Workfront-accountmanager voor meer informatie over een Workfront Goals-licentie.
> 
>Voor extra informatie over toegang tot de Doelen van Workfront, zie [&#x200B; Vereisten om de Doelen van Workfront &#x200B;](/help/quicksilver/workfront-goals/goal-management/access-needed-for-wf-goals.md) te gebruiken.

De Doelen van Adobe Workfront komt met een reeks gebeurtenisberichten die u voor uw rekening kunt toelaten. Deze gebeurtenismeldingen activeren e-mailcommunicatie telkens wanneer aan de door de gebeurtenis gedefinieerde voorwaarde wordt voldaan.

Voor informatie over welke berichten u voor de Doelen van Workfront kunt toelaten, zie [&#x200B; Meldingen: Doelen &#x200B;](../../workfront-basics/using-notifications/notifications-goals.md).

Voor informatie over het beheren van berichten in Adobe Workfront, zie [&#x200B; uw eigen e-mailberichten wijzigen &#x200B;](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Access requirements</h2>
<p>(NOTE: drafted, no longer available from WF Goals proper. Documented at the links above.) </p>
<p>You must have the following access to perform the actions described in this article:</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Adobe Workfront plan*</td>
<td> <p>Pro or higher</p> </td>
</tr>
<tr>
<td role="rowheader">Adobe Workfront license*</td>
<td> <p>Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
</tr>
<tr>
<td role="rowheader">Product</td>
<td> <p>You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
</tr>
<tr>
<td role="rowheader">Access level*</td>
<td> <p>View or higher access to&nbsp;Goals</p> <note type="note">
<p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
<ul>
<li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
<li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
</ul>
</note> </td>
</tr>
<tr data-mc-conditions="">
<td role="rowheader">Object permissions</td>
<td>
<div>
<p>View or higher permissions on goals</p>
<p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
</div> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
<h2>Prerequisites: </h2>
<p>You must have the following before you can start:</p>
<ul>
<li> <p>A Layout Template that includes the Goals area in the Main&nbsp;Menu.</p> </li>
</ul>
<h2>Understand Workfront Goals notifications settings</h2>
<p>Consider the following when configuring and receiving Workfront Goals notifications:</p>
<ul>
<li>They are personal notifications which means that each user can manage their own notifications.</li>
<li>The Workfront administrator does not need to enable event notifications before each user can select which ones they want to receive. </li>
<li>They trigger as soon as the defined events happen on goals, activities, or results and cannot be part of a daily digest. </li>
<li>They trigger regardless of the status of the goal. </li>
<li>They do not trigger when you are the initiator of the event described in the notification setting. </li>
</ul>
<h2>Configure email notifications for Workfront Goals</h2>
<ol>
<li value="1"> <p>Log in to Workfront and ensure that your Workfront administrator gave you access to&nbsp;Workfront Goals.</p> <p>For information about access to&nbsp;Workfront Goals, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>.</p> </li>
<li value="2"> <p> <p>Click the <strong>Main Menu icon</strong> <img src="assets/main-menu-icon.png"> in the upper-right corner of your screen, then click <strong>Goals</strong>.</p> <p>This opens the Workfront Goals area. </p> </p> </li>
<li value="3"> <p>Click <strong>Goal Settings</strong> in the left panel.</p> <p> <img src="assets/notifications-settings-list-highlighted-350x124.png" style="width: 350;height: 124;"> </p> </li>
<li value="4"> <p>Select any of the check boxes below to enable notifications for the following events:</p>
<table style="table-layout:auto">
<col>
<thead>
<tr>
<th>Notification </th>
</tr>
</thead>
<tbody>
<tr>
<td> <p>Someone created a new personal Goal for you.</p> <p>This is enabled by default.</p> <note type="tip">
A personal goal is a goal where you are designated as the owner.
</note> </td>
</tr>
<tr>
<td> <p>Someone assigned a Result/ an Activity to you.</p> <p>This is enabled by default. </p> </td>
</tr>
<tr>
<td>Someone left a comment on your Goal </td>
</tr>
<tr>
<td>Someone liked updates on your Goal</td>
</tr>
<tr>
<td>Someone liked a comment you left on a Goal</td>
</tr>
<tr>
<td>Someone liked your Aligned Goal</td>
</tr>
</tbody>
</table> </li>
<li value="5"> <p>Click <strong>Save Settings</strong>. </p> </li>
</ol>
</div>
-->

## Voorbeeld van e-mailkennisgeving voor Workfront Goals

Wanneer de gebeurtenis plaatsvindt die wordt gedefinieerd door het bericht dat u hebt ingeschakeld, ontvangt u een e-mail met een beschrijving van de gebeurtenis. Hieronder ziet u een voorbeeld van een e-mail met de kennisgeving dat u bent toegewezen als eigenaar van een nieuw doel:

![&#x200B; het bericht van Doelen e-mail &#x200B;](assets/wf-align-notification-email-350x164.png)
