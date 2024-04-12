---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Door het systeem bijgehouden updates
description: Adobe Workfront legt de activiteit vast die plaatsvindt op bepaalde objecten door statusinformatie te registreren in de [!UICONTROL Updates] gebied.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: 18dfb67626982d73ad33871b8afce4a3f0d4cdb3
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# Door het systeem bijgehouden updates

<!-- Audited: April, 2024-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>-->

[!DNL Adobe Workfront] legt de activiteit vast die op bepaalde voorwerpen door statusinformatie in de objecten te registreren plaatsvindt [!UICONTROL Updates] sectie.

Voor informatie over de sectie van Updates, zie [Overzicht van de sectie Updates](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

De [!UICONTROL Updates] omvat de volgende typen updates:

* **Gebruikers: updates:** Handmatig ingevoerd door gebruikers. Wordt ook opmerkingen, antwoorden en notities genoemd. De updates van de gebruiker tonen in de Commentaren en Alle lusjes van de sectie van Updates van een voorwerp.

  Voor meer informatie over het configureren van gebruikersupdates raadpleegt u [Voorkeuren voor gebruikersupdates configureren](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![](assets/updates-qs-350x125.png)

* **Systeemupdates:** Automatisch gemaakt door het systeem. Een systeemupdate bevat een korte beschrijving van het type wijziging dat met het item is opgetreden. De updates van het systeem tonen in de Activiteit van het Systeem en de Alle lusjes van de sectie van Updates van een voorwerp.

  Voor meer informatie over de feeds van systeemupdates en hoe te om hen toe te laten, zie [Systeemupdates configureren](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  ![](assets/system-updates-example-unified-stream.png)


  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## Overwegingen bij systeembijgehouden updates

Door het systeem bijgehouden updates zijn niet beschikbaar voor alle objecten die het gebied Updates hebben.

* De [!UICONTROL Updates] is beschikbaar voor de volgende objecten:

   * [!UICONTROL Project]
   * [!UICONTROL Task]
   * [!UICONTROL Issue]
   * [!UICONTROL Portfolio]
   * [!UICONTROL Program]
   * [!UICONTROL User]
   * [!UICONTROL Template]
   * [!UICONTROL Template Task]
   * [!UICONTROL Team]
   * [!UICONTROL Document]
   * [!UICONTROL Timesheet]
   * [!UICONTROL Story]

     In [!DNL Workfront]Een verhaal is een taak.
   * [!UICONTROL Iteration]
   * [!UICONTROL Goal]

     U moet een extra licentie hebben om toegang te hebben tot de [!UICONTROL Goals] gebied. Zie voor meer informatie [Vereisten voor het gebruik van Workfront-doelen](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL Card] aan boord

     Voor meer informatie over updates van kaarten raadpleegt u [Gekoppelde kaarten op borden gebruiken](../../../agile/get-started-with-boards/connected-cards.md).

* [!DNL Workfront] houdt geen systeemupdates bij voor de volgende objecten:

   * [!UICONTROL Team]
   * [!UICONTROL Template]
   * [!UICONTROL Template Task]
   * Ad hoc [!UICONTROL Card]
   * [!UICONTROL Iterations]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* De updates van de gebruiker tonen op het lusje van Commentaren en systeemupdates tonen in de Activiteit van het Systeem en de Alle lusjes.

  Voor een lijst met objecten die niet over de tabbladen Systeemactiviteit of Alle beschikken, raadpleegt u [Overzicht van de sectie Bijwerken](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)

* U kunt geen antwoord toevoegen aan een systeemupdate. Alle antwoorden die vóór 11 april 2024 in de oudere opmerkingervaring naar de systeemactiviteitenrecords zijn verzonden, worden echter als alleen-lezen ingevuld op het tabblad Systeemactiviteit.

<!--
* The following are differences between the new and the legacy commenting experience: 

   * When using the new commenting experience, user updates display in the Comments tab and system updates display in the System Activity <span class="preview">and the All</span> tabs.  

      For more information about the new commenting experience, see [New commenting experience](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

      <span class="preview">For a list of objects that do not have the System Activity or the All tabs, see [Update section overview](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)</span>

   * <span class="preview">When using the new commenting experience, you cannot add a comment to a system update. However, any replies made to system activity records in the legacy commenting experience are populated on the System Activity tab as read-only in the new commenting experience.</span>
   * When using the legacy commenting experience, the system and user updates display in one continuous feed. 

   * When using the legacy commenting experience, users can view system updates by default or they can choose to not display them. Disabling system updates is not possible when using the new commenting experience. 

      For information about disabling the display of system updates, see the section [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) in the article [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).  

   * <span class="preview">The legacy commenting experience has been disabled in the Preview environment. For more information, see [Second Quarter 2024 Update stream and notification enhancements](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md).</span>
-->

* [!DNL Workfront] beheerders kunnen bepalen welk type van veranderingen het systeem in zou moeten volgen [!UICONTROL Updates] gebied. Niet alle objecten met een [!UICONTROL Updates] gebied ook configureerbaar [!UICONTROL update] feeds. De volgende objecten hebben een [!UICONTROL Updates] gebied dat door het systeem bijgehouden updateffeeds vastlegt, maar geen configureerbare bijwerkingsfeeds heeft:

   * [!UICONTROL Document]
   * [!UICONTROL Timesheet]
   * [!UICONTROL Iteration]
   * [!UICONTROL Goal]


