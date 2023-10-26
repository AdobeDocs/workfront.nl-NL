---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Door het systeem bijgehouden updates
description: Adobe Workfront legt de activiteit vast die plaatsvindt op bepaalde objecten door statusinformatie te registreren in de [!UICONTROL Updates] gebied.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: c2c09486756db021b6edaf380c5a54d531ffa723
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Door het systeem bijgehouden updates

<!--remove new experience and legacy notes when we remove legacy in the UI - Jan 24???-->

[!DNL Adobe Workfront] legt de activiteit vast die op bepaalde voorwerpen door statusinformatie in de objecten te registreren plaatsvindt [!UICONTROL Updates] gebied.

De [!UICONTROL Updates] omvat de volgende typen updates:

* **Gebruikers: updates:** Handmatig ingevoerd door gebruikers. Wordt ook opmerkingen, antwoorden en notities genoemd.

  Voor meer informatie over het configureren van gebruikersupdates raadpleegt u [Voorkeuren voor gebruikersupdates configureren](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![](assets/updates-qs-350x125.png)

* **Systeemupdates:** Automatisch gemaakt door het systeem. Een systeemupdate bevat een korte beschrijving van het type wijziging dat met het item is opgetreden.

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

* Hieronder ziet u de verschillen tussen de nieuwe en de oudere opmerkingervaring:

   * Wanneer u de nieuwe opmerkingervaring gebruikt, worden gebruikersupdates weergegeven op het tabblad Opmerkingen en worden systeemupdates weergegeven op het tabblad Systeemactiviteit.

     Ga voor meer informatie over de nieuwe opmerkingervaring naar [Nieuwe ervaring met opmerkingen](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

   * Als u de oudere opmerkingervaring gebruikt, worden het systeem en de gebruikersupdates in één doorlopende feed weergegeven.

   * Als gebruikers de oudere opmerkingervaring gebruiken, kunnen ze systeemupdates standaard bekijken of ze kunnen ervoor kiezen deze niet weer te geven. Het is niet mogelijk systeemupdates uit te schakelen wanneer u de nieuwe opmerkingervaring gebruikt.

     Zie de sectie voor informatie over het uitschakelen van de weergave van systeemupdates [Systeemupdates in- of uitschakelen](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) in het artikel [Werk bijwerken](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* Workfront registreert door het systeem bijgehouden updates voor de volgende objecten, maar er is geen optie om de weergave ervan uit te schakelen:

   * [!UICONTROL Portfolio]
   * [!UICONTROL Program]
   * [!UICONTROL Iteration]

* [!DNL Workfront] beheerders kunnen bepalen welk type van veranderingen het systeem in zou moeten volgen [!UICONTROL Updates] gebied. Niet alle objecten met een [!UICONTROL Updates] gebied ook configureerbaar [!UICONTROL update] feeds. De volgende objecten hebben een [!UICONTROL Updates] gebied dat door het systeem bijgehouden updateffeeds vastlegt, maar geen configureerbare bijwerkingsfeeds heeft:

   * [!UICONTROL Document]
   * [!UICONTROL Timesheet]
   * [!UICONTROL Iteration]
   * [!UICONTROL Goal]


