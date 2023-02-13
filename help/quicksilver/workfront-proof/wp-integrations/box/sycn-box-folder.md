---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: box
title: Mappen synchroniseren met [!DNL Workfront Proof]
description: U kunt een Box-map synchroniseren met een map in Workfront Proof. Elke wijziging die u aanbrengt in de map Box, wordt doorgevoerd in Workfront Proof (dus het uploaden van een nieuw bestand, het toevoegen van een nieuwe versie, het wijzigen van de bestandsnaam, enzovoort).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d85577f5-6aa0-40a3-a6e3-45555a3124db
source-git-commit: a6c79166c50af5bfe4c0341d003052179ce78373
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---

# Synchroniseren [!DNL Box] Mappen met [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

U kunt een [!DNL Box] map met een map in [!DNL Workfront Proof]. Elke wijziging die u aanbrengt in de map Box, wordt doorgevoerd in Workfront Proof (dus het uploaden van een nieuw bestand, het toevoegen van een nieuwe versie, het wijzigen van de bestandsnaam, enzovoort).

Zie voor meer informatie over mappen [Mappen en de inhoud ervan beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

>[!NOTE]
>
>Alleen gebruikers met profielen van [!UICONTROL Managers] of hoger kunnen mappen synchroniseren. De [!DNL Box] gebruiker die het bestand uploadt naar een map die is gesynchroniseerd met [!DNL Workfront Proof]wordt de eigenaar van het in [!DNL Workfront Proof] (als ze een gebruiker zijn binnen dezelfde [!DNL Workfront Proof] account). Als de [!DNL Box] gebruiker is een gebruiker in een andere [!DNL Workfront Proof] account of geen account heeft met [!DNL Workfront Proof]De persoon die de synchronisatie tussen de mappen heeft gemaakt, wordt de eigenaar van de proefdruk. Zie voor meer informatie *&quot;Gebruikersprofielen en machtigingen bewerken.&quot;*

Een [!DNL Box] map met een map in [!DNL Workfront Proof]:

1. In uw [!DNL Box] account, ga naar [!UICONTROL All Files and Folders] pagina.
1. Klik op de knop **[!UICONTROL More options]** menu naast de map waarmee u wilt synchroniseren [!DNL Workfront Proof] (1)
1. Selecteren **[!UICONTROL More Actions]** (2)
1. Klikken **[!UICONTROL Sync with [!DNL Workfront Proof]]** (3)
1. In de [!UICONTROL Sync folder] doos die verschijnt (als u het programma opent [!DNL Workfront Proof]), voert u een van de volgende handelingen uit:

   * Klik op een [!DNL Workfront Proof] mapnaam om deze te synchroniseren met de bijbehorende map in vak (4).
   * Klikken **[!UICONTROL New folder]** om een nieuwe map te maken in [!DNL Workfront Proof] (5).\

      ![map_sync_2.jpg](assets/folder-sync-2-350x231.jpg)Als u ervoor kiest een nieuwe map te maken, wordt u gevraagd gegevens over de nieuwe map op te geven.

1. Klik op **[!UICONTROL Save]**.\
   De [!UICONTROL Folder details] pagina voor de gesynchroniseerde map wordt geopend in [!DNL Workfront Proof]. Deze pagina bevat informatie over de map.\
   Op deze pagina kunt u het synchroniseren ook pauzeren en uitschakelen. Als u de synchronisatie onderbreekt, wordt de map niet meer bijgewerkt met de wijzigingen van [!DNL Box], maar de synchronisatie kan op elk gewenst moment worden hervat. Als u de synchronisatie uitschakelt, wordt de verbinding tussen de mappen verbroken en moet de synchronisatie opnieuw worden ingesteld via het [!DNL Box] account.\
   De [!UICONTROL Folder details] bevat de volgende informatie en functies met betrekking tot uw map in [!DNL Box]:

   * **[!UICONTROL Pause syncing]**: De [!DNL Workfront Proof] wordt niet meer bijgewerkt met de wijzigingen in het vak. Synchronisatie kan op elk gewenst moment worden hervat (1).
   * **[!UICONTROL Disable folder sync]**: De verbinding tussen de mappen gaat verloren en de synchronisatie moet opnieuw worden ingesteld vanuit het dialoogvenster [!DNL Box] rekening (2).

   * Alleen de gebruiker die de mapsynchronisatie heeft gestart, kan deze uitschakelen of pauzeren. Zie voor meer informatie  [Mappen en de inhoud ervan beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).
   * **Ga naar [!DNL Box] map**: Als u de map URL (in het dialoogvenster [!DNL Box] (mapopties), wordt deze optie beschikbaar en gaat u rechtstreeks naar de [!DNL Box] map (3).
   * **[!UICONTROL Folder sync details]**: Deze sectie bevat informatie over de [!DNL Box] map (4).
   * **[!UICONTROL [!DNL Box] folder link]**: URL naar de [!DNL Box] map (5).
   * **[!UICONTROL Activity]:** Hiermee geeft u de activiteitenlogs weer van de [!DNL Workfront Proof] , hier kunt u controleren wie de mapsynchronisatie heeft gestart (6).
   * ![folder_details__1_.jpg](assets/folder-details--1--350x324.jpg)

>[!NOTE]
>
>* U kunt ook de [!DNL Box] uit de [!UICONTROL Folder options] -menu.
>* Als u uw eigen merk hebt [!DNL Workfront Proof] aanmeldingspagina, wordt u doorgestuurd naar die pagina in plaats van naar de standaardpagina [!DNL Workfront Proof] aanmeldingspagina. Zie de artikelen onder [Branding](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) voor meer informatie.
>* Als u de optie [!UICONTROL Single Sign-On (SSO)] in uw [!DNL Workfront Proof] -account, wordt u naar de aanmeldingspagina van de SSO geleid en wordt u gevraagd uw SSO-aanmeldgegevens in te voeren, maar alleen als u hetzelfde e-mailadres gebruikt voor uw [!DNL Box] rekening en [!DNL Workfront Proof]. Voor meer informatie, zie [[!UICONTROL Single Sign-On] in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).
>* Als u niet hetzelfde e-mailadres gebruikt voor beide [!DNL Box] account en uw [!DNL Workfront Proof] rekening, zal u altijd aan de norm worden gehouden [!DNL Workfront Proof] aanmeldingspagina.
>



