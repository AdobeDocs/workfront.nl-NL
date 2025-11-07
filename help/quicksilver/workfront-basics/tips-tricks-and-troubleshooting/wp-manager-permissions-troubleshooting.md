---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Problemen met Workfront Proof Manager-machtigingen oplossen
description: De toestemmingsprofielen beschikbaar in  [!DNL Adobe]  Workfront voor het proefdrukken van gebruikers zijn Beheerder, Supervisor, en Manager.
feature: Get Started with Workfront
auhor: Courtney
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# [!UICONTROL [!DNL Workfront] Proof Manager] problemen met machtigingen oplossen

Hier volgen de machtigingsprofielen die beschikbaar zijn in [!DNL Adobe Workfront] voor het maken van proefdrukken van gebruikers:

* [!UICONTROL Administrator]
* [!UICONTROL Supervisor]
* [!UICONTROL Manager]

<!--For detailed information about these options and how to configure them, see .-->

Bij het verlenen van [!UICONTROL Manager] gebruikersmachtigingen zijn de volgende informatie over probleemoplossing beschikbaar:

* **PROBLEEM:** De gebruikers met [!UICONTROL Manager] toestemmingen kunnen geen proeven bekijken die door andere gebruikers worden gecreeerd. In plaats daarvan zien ze het scherm [!UICONTROL Access Denied] .

  ![](assets/access-denied-350x161.png)

  **OPLOSSING:** Gebruikers met [!UICONTROL Manager] toestemmingen moeten uitdrukkelijk aan de proeven worden toegevoegd. Proefbestanden moeten altijd worden gemaakt via het venster [!UICONTROL Advanced proofing options] en gebruikers moeten altijd via deze optie worden toegevoegd.

* **PROBLEM:** De gebruikers met [!UICONTROL Manager] toestemmingen kunnen proefversies aan de proeven niet toevoegen die door andere gebruikers worden gecreeerd (zij konden potentieel een proef in de documentenreeks voorleggen, maar de versies zouden NIET met de originele reeks worden verbonden die door een andere gebruiker wordt gecreeerd).\
   **OPLOSSING:** De gebruikers met [!UICONTROL Manager] toestemmingen kunnen de versies naar de proef van een andere gebruiker voorleggen slechts als de gebruiker met [!UICONTROL Manager] toestemmingen wanneer allebei van het volgende:

   * Expliciet toegevoegd aan de proefdrukken
   * Instellen als [!UICONTROL Authors] (proefdrukrol) op proefdrukken

* **PROBLEEM:** De gebruikers met [!UICONTROL Manager] toestemmingen kunnen geen commentaren van andere gebruikers op een proef uitgeven zij niet bezitten of zij niet creeerden.\
   **OPLOSSING:** als de gebruikers met [!UICONTROL Manager] toestemmingen niet de proeven bezitten, maar zij zouden commentaren moeten kunnen uitgeven, hen toevoegen als [!UICONTROL Authors] (of [!UICONTROL Moderators]).\
   Deze drie typen machtigingen zijn beschikbaar in [!DNL Workfront] voor [!UICONTROL Planner] -, [!UICONTROL Worker] -, [!UICONTROL Requester] - [!UICONTROL Reviewer] tekstlicenties. Systeembeheerder of Gebruikersbeheerder in [!DNL Workfront] kan gebruikersprofielen bewerken en [!DNL Workfront Proof] -machtigingen van daaruit aanpassen.
