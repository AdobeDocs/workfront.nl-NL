---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Overzicht van door het systeem bijgehouden updates
description: Adobe Workfront legt de activiteit vast die plaatsvindt op bepaalde objecten door statusinformatie in het gebied [!UICONTROL Updates] van het object te registreren.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# Overzicht van door het systeem bijgehouden updates

<!-- Audited: 08/2025-->

[!DNL Adobe Workfront] legt de activiteit vast die op bepaalde objecten plaatsvindt door statusinformatie in de [!UICONTROL Updates] -sectie van het object te registreren.

Voor informatie over de sectie van Updates, zie [ overzicht van de sectie van Updates ](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

Het gebied [!UICONTROL Updates] bevat de volgende typen updates:

* **de updates van de Gebruiker:** manueel ingegaan door gebruikers. Wordt ook opmerkingen, antwoorden en notities genoemd. De updates van de gebruiker tonen in de Commentaren en Alle lusjes van de sectie van Updates van een voorwerp.

  Voor meer informatie over het vormen van gebruikersupdates, zie [ voorkeur voor gebruikersupdates ](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md) vormen.

  ![ Updates ](assets/updates-qs-350x125.png)

* **de updates van het Systeem:** automatisch gemaakt door het systeem. Een systeemupdate bevat een korte beschrijving van het type wijziging dat met het item is opgetreden. De updates van het systeem tonen in de Activiteit van het Systeem en de Alle lusjes van de sectie van Updates van een voorwerp.

  Voor meer informatie over de feeds van de systeemupdate en hoe te om hen toe te laten, zie [ systeemupdates ](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md) vormen.

  ![ het updatevoorbeeld van het Systeem ](assets/system-updates-example-unified-stream.png)


  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## Overwegingen bij systeembijgehouden updates

Door het systeem bijgehouden updates zijn niet beschikbaar voor alle objecten die het gebied Updates hebben.

* Het gebied [!UICONTROL Updates] is beschikbaar voor de volgende objecten:

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

     In [!DNL Workfront] is een artikel een taak.
   * [!UICONTROL Iteration]
   * [!UICONTROL Goal]

     Niet alle Workfront-pakketten bevatten Workfront Goals. Voor informatie, zie [ Vereisten om de Doelen van Workfront ](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md) te gebruiken.
   * [!UICONTROL Card] op een bord

     Voor meer informatie over updates op kaarten, zie [ Gebruik verbonden kaarten op raad ](../../../agile/get-started-with-boards/connected-cards.md).

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

  Voor een lijst van voorwerpen die niet de Activiteit van het Systeem of Alle lusjes hebben, zie [ overzicht van de sectie van de Update ](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)

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

* [!DNL Workfront] beheerders kunnen bepalen welk type wijzigingen het systeem in het [!UICONTROL Updates] -gebied moet bijhouden. Niet alle objecten met een [!UICONTROL Updates] -gebied hebben configureerbare [!UICONTROL update] -feeds. De volgende objecten hebben een [!UICONTROL Updates] -gebied dat door het systeem bijgehouden bijwerkingsfeeds vastlegt, maar geen configureerbare bijwerkingsfeeds hebben:

   * [!UICONTROL Document]
   * [!UICONTROL Timesheet]
   * [!UICONTROL Iteration]
   * [!UICONTROL Goal]


