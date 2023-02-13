---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Door het systeem bijgehouden updates
description: Adobe Workfront legt de activiteit vast die plaatsvindt op bepaalde objecten door statusinformatie te registreren in de [!UICONTROL Updates] gebied.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---

# Door het systeem bijgehouden updates

[!DNL Adobe Workfront] legt de activiteit vast die op bepaalde voorwerpen door statusinformatie in de objecten te registreren plaatsvindt [!UICONTROL Updates] gebied.

De [!UICONTROL Updates] omvat de volgende typen updates:

* **Gebruikersupdates:** Handmatig ingevoerd door gebruikers. Wordt ook opmerkingen, antwoorden en notities genoemd.

   ![](assets/updates-qs-350x125.png)

* **Systeemupdates:** Automatisch gemaakt door het systeem. Een systeemupdate bevat een korte beschrijving van het type wijziging dat met het item is opgetreden.

   <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

De volgende objecten kunnen updates hebben:

* Project
* Taak
* Probleem
* Portfolio
* Programma
* Gebruiker
* Sjablonen
* Sjabloontaken
* Documenten
* Timesheets

Uw [!DNL Workfront] de licentie bepaalt of systeemupdates standaard worden weergegeven in de [!UICONTROL Updates] gebied met objecten. [!DNL Workfront] gebruikers met een [!UICONTROL Plan] licentie systeemupdates worden weergegeven in het dialoogvenster [!UICONTROL Updates] gebied standaard. Gebruikers kunnen systeemupdates echter uitfilteren, zoals beschreven in het dialoogvenster [[!UICONTROL Enable] of systeemupdates uitschakelen](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) sectie in [Werk bijwerken](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). Alle andere [!DNL Workfront] licenties filteren systeemupdates standaard.

[!DNL Workfront] beheerders kunnen bepalen welk type van veranderingen het systeem in zou moeten volgen [!UICONTROL Updates] gebied. Niet alle objecten kunnen worden geconfigureerd [!UICONTROL update] statusfeeds. De volgende objecten hebben een [!UICONTROL Updates] gebied dat door het systeem bijgehouden updateffeeds vastlegt, maar geen configureerbare statusfeeds voor updates heeft:

* Sjablonen
* Sjabloontaken
* Documenten
* Timesheets

Voor meer informatie over de feeds van systeemupdates en hoe te om hen toe te laten, zie [Systeemupdates configureren](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md). Voor meer informatie over het configureren van gebruikersupdates raadpleegt u [Voorkeuren voor gebruikersupdates configureren](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
