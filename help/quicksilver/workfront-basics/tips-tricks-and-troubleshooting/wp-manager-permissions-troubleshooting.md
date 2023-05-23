---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Problemen met Workfront Proofing Manager-machtigingen oplossen
description: De machtigingsprofielen beschikbaar in [!DNL Adobe] Workfront voor het proefdrukken van gebruikers is Beheerder, Supervisor, en Manager.
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# [!UICONTROL [!DNL Workfront] Proof Manager] problemen met machtigingen

Hieronder vindt u de machtigingsprofielen die beschikbaar zijn in [!DNL Adobe Workfront] voor proefdrukgebruikers:

* [!UICONTROL Administrator]
* [!UICONTROL Supervisor]
* [!UICONTROL Manager]

<!--For detailed information about these options and how to configure them, see .-->

Wanneer een gebruiker een [!UICONTROL Manager] toestemmingen, is de volgende het oplossen van problemeninformatie beschikbaar:

* **PROBLEEM:** Gebruikers met [!UICONTROL Manager] rechten kunnen geen proefdrukken weergeven die door andere gebruikers zijn gemaakt. In plaats daarvan zien ze de [!UICONTROL Access Denied] scherm.

   ![](assets/access-denied-350x161.png)

   **OPLOSSING:** Gebruikers met [!UICONTROL Manager] rechten moeten expliciet aan de proefdrukken worden toegevoegd. Proefdrukken moeten altijd worden gemaakt via de [!UICONTROL Advanced proofing options] venster en gebruikers moeten altijd via deze optie worden toegevoegd.

* **PROBLEEM:** Gebruikers met [!UICONTROL Manager] met machtigingen kunnen geen proefversies worden toegevoegd aan de proefdrukken die door andere gebruikers zijn gemaakt (ze kunnen mogelijk een proefdruk indienen in de set documenten, maar de versies zouden NIET verbonden zijn met de oorspronkelijke set die door een andere gebruiker is gemaakt).\
   **OPLOSSING:** Gebruikers met [!UICONTROL Manager] machtigingen kunnen de versies alleen naar de proefdruk van een andere gebruiker verzenden als de gebruiker met [!UICONTROL Manager] machtigingen als aan beide volgende voorwaarden wordt voldaan:

   * Expliciet toegevoegd aan de proefdrukken
   * Instellen als [!UICONTROL Authors] (proefrol) op proefdrukken

* **PROBLEEM:** Gebruikers met [!UICONTROL Manager] machtigingen kunnen opmerkingen van andere gebruikers niet bewerken op een proefdruk die ze niet hebben of niet hebben gemaakt.\
   **OPLOSSING:** Als gebruikers met [!UICONTROL Manager] rechten zijn niet de eigenaar van de proefdrukken, maar ze moeten opmerkingen kunnen bewerken en toevoegen als [!UICONTROL Authors] (of [!UICONTROL Moderators]).\
   Deze drie typen machtigingen zijn beschikbaar in [!DNL Workfront] for [!UICONTROL Planner], [!UICONTROL Worker], [!UICONTROL Requester], [!UICONTROL Reviewer] type licenties. Systeembeheerder of -beheerder in [!DNL Workfront] kan gebruikersprofielen bewerken en aanpassen [!DNL Workfront Proof] rechten van daar.
