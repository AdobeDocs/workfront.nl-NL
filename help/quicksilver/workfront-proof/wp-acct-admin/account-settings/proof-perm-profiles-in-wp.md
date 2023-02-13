---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Proefmachtigingenprofielen in Workfront Proef
description: Als Workfront-beheerder of beheerder van Workfront-proefdrukken kunt u een profiel met proefdrukmachtigingen toewijzen aan een gebruiker om de mogelijkheden voor proefdrukproeven op te geven die de gebruiker heeft voor alle proefdrukken in het systeem. Voor informatie over het vormen van het Profiel van de Toestemming van de Bewijs van een gebruiker, zie het Profiel van de Toestemming van de Bewijs van een Gebruiker in de Bewijs van Workfront vormen.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 249aa332-c051-49ac-be85-264d8babfcad
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '1763'
ht-degree: 0%

---

# Profielen met proefmachtigingen in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Als [!DNL Workfront] beheerder of [!DNL Workfront Proof] beheerder, kunt u een Profiel van de Toestemmingen van het Bewijs aan een gebruiker toewijzen om de het proefdrukken mogelijkheden te specificeren die de gebruiker voor alle proeven in het systeem zal hebben. Voor informatie over het configureren van het Proefmachtigingsprofiel van een gebruiker raadpleegt u [Het machtigingsprofiel van een proefversie van een gebruiker configureren in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/config-user-pref-in-wp.md).

>[!NOTE]
>
>U kunt ook het volgende doen:
>
>* Bied gebruikers specifieke rollen op individuele proefdrukken. Voor meer informatie over proefdrukrollen, zie [Proefrollen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).
>* Aangepaste profielen maken voor gebruikers in uw organisatie. Zie voor meer informatie [Aangepaste profielen configureren in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).
>


In de volgende tabel worden de machtigingen weergegeven die beschikbaar zijn bij elk profiel voor Proefmachtigingen.

| **Eigen items** |  |  |  |  | **Andere gebruikerstitems** |  |  | **Beheer** | **Facturering** |
|---|---|---|---|---|---|---|---|---|---|
|  | **Toevoegen** | **Weergave** | **Bewerken** | **Verwijderen** | **Weergave** | **Bewerken** | **Verwijderen** | **Bewerken en verwijderen** | **Bewerken** |
| Factureringsbeheer | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |
| Beheer | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |
| Supervisor | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |
| Manager | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |   |   |   |
| Waarnemer |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |
| Bezoeker |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

Overweeg het volgende over rollen en toestemmingen:

* Toegewezen profielmachtigingen hebben alleen betrekking op de gebruikers en items in uw eigen account. De uitzondering is in het geval van Satellietrekeningen, waar de Beheerder en de Facturerings Beheerder voor de belangrijkste (hub) rekeningen tot de rekeningsmontages en het factureren van die rekeningen van het niveau van de hubrekening kunnen toegang hebben en beheren.
* Factureringsbeheerders en -beheerders kunnen gebruikers verwijderen. Dit kan alleen worden gedaan in de accountinstellingen.
* Wanneer de Beheerders en de Beheerders van de Facturering bewijzen bekijken die door andere gebruikers in hun rekening worden bezeten, bekijken zij hen met de rol van Recensent.
* Met de rol Alleen-lezen hebben factureringsbeheerders en beheerders toegang tot proefdrukken in mappen die met hen worden gedeeld of in mappen die door hen worden gemaakt.

In de volgende secties worden elk profiel en de machtigingen die aan het profiel zijn gekoppeld, in een standaard beschreven [!DNL Workfront Proof] instellen:

* [Factureringsbeheerder](#billing-administrator)
* [Beheerder](#administrator)
* [Supervisor](#supervisor)
* [Manager](#manager)
* [Waarnemer](#observer)
* [Bezoeker](#visitor)
* [Gast](#guest)

## Factureringsbeheerder {#billing-administrator}

Factureringsbeheerders hebben toegang tot [Accountinstellingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) and [The [!DNL Workfront Proof] Factureringspagina](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)en beschikken over de volgende machtigingen:

![](assets/cleaner2.png)Kan proefdrukken genereren, bestanden uploaden en mappen maken. Zie voor meer informatie [Proefdrukken genereren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Bestanden en webinhoud uploaden naar [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md), en [Mappen maken in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Kan eigen proefdrukken en bestanden die ze maken, weergeven, bewerken en verwijderen.

![](assets/cleaner2.png)Kan proefdrukken en bestanden die door alle gebruikers in de organisatie zijn gemaakt, weergeven, bewerken en verwijderen.

![](assets/cleaner2.png)Kan de openbare mappen van andere gebruikers verwijderen. Zie voor meer informatie [Mappen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Heeft bewerkingsrechten voor alle proefdrukken die in de account zijn gemaakt.

![](assets/cleaner2.png)Kan worden ingesteld als eigenaar van de dropzone. Zie voor meer informatie [De dropzone configureren in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Kan de facturatiepagina openen en de factureringsgegevens bewerken. Zie voor meer informatie [De [!DNL Workfront Proof] Factureringspagina](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

![](assets/cleaner2.png)Kan de pagina Accountinstellingen openen en de accountgegevens bewerken. Zie voor meer informatie [Accountinstellingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)Kan de prullenbak leeg maken. Zie voor meer informatie [De prullenbak herstellen en leegmaken [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)Kan gebruikers toevoegen, bewerken en verwijderen.

![](assets/cleaner2.png)Kan groepen maken en nieuwe contactpersonen toevoegen.

![](assets/cleaner2.png)Kan contactpersonen verwijderen.

![](assets/cleaner2.png)Proefdrukken kunnen worden bewerkt als er geen reacties op zijn.

![](assets/no2.png)Kan de reacties op proefdrukken niet bewerken.

![](assets/no2.png)Kan de privémappen van andere gebruikers niet verwijderen. Zie voor meer informatie [Mappen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

Voor informatie over accountinstellingen raadpleegt u [Accountinstellingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

Voor informatie over facturering raadpleegt u [De [!DNL Workfront Proof] Factureringspagina](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Beheerder {#administrator}

Beheerders hebben toegang tot [Accountinstellingen](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings)en beschikken over de volgende machtigingen:

![](assets/cleaner2.png)Kan proefdrukken maken, bestanden uploaden en mappen maken. Zie voor meer informatie [Proefdrukken genereren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Bestanden en webinhoud uploaden naar [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md), en [Mappen maken in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Kan gemaakte proefdrukken en bestanden weergeven, bewerken en verwijderen.

![](assets/cleaner2.png)Kan proefdrukken en bestanden die door alle gebruikers in de organisatie zijn gemaakt, weergeven, bewerken en verwijderen.

![](assets/cleaner2.png)Kan de openbare mappen van andere gebruikers verwijderen. Zie voor meer informatie [Mappen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Heeft bewerkingsrechten voor alle proefdrukken die in de account zijn gemaakt.

![](assets/cleaner2.png)Kan worden ingesteld als eigenaar van de dropzone. Zie voor meer informatie [De dropzone configureren in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Kan de pagina Accountinstellingen openen en de accountgegevens bewerken. Zie voor meer informatie [Accountinstellingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)Kan de prullenbak leeg maken. Zie voor meer informatie [De prullenbak herstellen en leegmaken [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)Kan gebruikers toevoegen, bewerken en verwijderen.

![](assets/cleaner2.png)Kan groepen maken en nieuwe contactpersonen toevoegen.

![](assets/cleaner2.png)Kan contactpersonen verwijderen.

![](assets/cleaner2.png)Proefdrukken kunnen worden bewerkt als er geen reacties op zijn.

![](assets/no2.png)Kan de reacties op proefdrukken niet bewerken.

![](assets/no2.png)Kan de privémappen van andere gebruikers niet verwijderen. Zie voor meer informatie [Mappen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Kan de pagina Facturering niet openen of de factureringsdetails uitgeven. Zie voor meer informatie [De [!DNL Workfront Proof] Factureringspagina](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Supervisor {#supervisor}

De toezichthouders hebben de volgende toestemmingen:

![](assets/cleaner2.png)Kan proefdrukken maken, bestanden uploaden en mappen maken. Zie voor meer informatie [Proefdrukken genereren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Bestanden en webinhoud uploaden naar [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md), en [Mappen maken in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Kan eigen proefdrukken en bestanden die ze hebben gemaakt, weergeven, bewerken en verwijderen.

![](assets/cleaner2.png)Kan proefdrukken en bestanden die door alle gebruikers in de organisatie zijn gemaakt, weergeven, bewerken en verwijderen.

![](assets/cleaner2.png)Kan de openbare mappen van andere gebruikers verwijderen. Zie voor meer informatie [Mappen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Heeft bewerkingsrechten voor alle proefdrukken die in de account zijn gemaakt.

![](assets/cleaner2.png)Kan worden ingesteld als eigenaar van de dropzone. Zie voor meer informatie [De dropzone configureren in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Kan groepen maken en nieuwe contactpersonen toevoegen.

![](assets/cleaner2.png)Kan contactpersonen verwijderen.

![](assets/cleaner2.png)Proefdrukken kunnen worden bewerkt als er geen reacties op zijn.

![](assets/no2.png)Kan de reacties op proefdrukken niet bewerken.

![](assets/no2.png)Kan de privémappen van andere gebruikers niet verwijderen. Zie voor meer informatie [Mappen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/folders.md).

![](assets/no2.png)Kan geen toegang krijgen tot de instellingen voor de facturatiepagina of account. Zie voor meer informatie [De [!DNL Workfront Proof] Factureringspagina](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) en [Accountinstellingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Kan gebruikers niet toevoegen, bewerken of verwijderen.

![](assets/no2.png)Kan de prullenbak niet leegmaken. Zie voor meer informatie [De prullenbak herstellen en leegmaken [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

### Manager {#manager}

Managers hebben de volgende machtigingen:

![](assets/cleaner2.png)Kan proefdrukken maken, bestanden uploaden en mappen maken. Zie voor meer informatie [Proefdrukken genereren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Bestanden en webinhoud uploaden naar [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md), en [Mappen maken in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Kan eigen proefdrukken en bestanden die ze maken of bezitten, weergeven, bewerken en verwijderen.

![](assets/cleaner2.png)Kan proefdrukken van andere gebruikers zien, controleren en goedkeuren die expliciet met hen worden gedeeld (alleen-lezen rechten op alles in een gedeelde map). Zie voor meer informatie [Proefrollen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Kan groepen maken en een nieuwe contactpersoon toevoegen.

![](assets/no2.png)Kan proofs en bestanden die door andere gebruikers in de organisatie zijn gemaakt, niet weergeven, bewerken of verwijderen.

![](assets/no2.png)Kan geen proefdrukken of antwoorden bewerken.

![](assets/no2.png)Kan de privémappen van andere gebruikers niet verwijderen. Zie voor meer informatie [Mappen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Kan de openbare mappen van andere gebruikers niet verwijderen. Zie voor meer informatie [Mappen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Kan geen toegang krijgen tot de instellingen voor de facturatiepagina of account. Zie voor meer informatie [De [!DNL Workfront Proof] Factureringspagina](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) en [Accountinstellingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Kan niet instellen als eigenaar van de dropzone. Zie voor meer informatie [De dropzone configureren in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Kan de prullenbak niet leegmaken. Zie voor meer informatie [De prullenbak herstellen en leegmaken [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Kan gebruikers niet toevoegen, bewerken of verwijderen.

![](assets/no2.png)Kan contacten niet schrappen.

### Waarnemer {#observer}

Waarnemers hebben de volgende machtigingen:

![](assets/cleaner2.png)Kan proefdrukken van andere gebruikers zien, controleren en goedkeuren die expliciet met hen worden gedeeld (alleen-lezen rechten op alles in een gedeelde map). Zie voor meer informatie [Proefrollen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Kan bestanden weergeven die expliciet met deze bestanden worden gedeeld.

![](assets/cleaner2.png) Kan contacten en groepen bekijken

![](assets/no2.png)Kan geen proefdrukken maken, bestanden uploaden en mappen maken. Zie voor meer informatie [Bestanden en webinhoud uploaden naar [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)Kan proofs en bestanden die door andere gebruikers in de organisatie zijn gemaakt, niet weergeven, bewerken of verwijderen.

![](assets/no2.png)Kan geen proefdrukken of antwoorden bewerken.

![](assets/no2.png)Kan geen items verwijderen die in de organisatie zijn gemaakt.

![](assets/no2.png)Kan geen toegang krijgen tot de instellingen voor de facturatiepagina of account. Zie voor meer informatie [De [!DNL Workfront Proof] Factureringspagina](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) en [Accountinstellingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Kan niet instellen als eigenaar van de dropzone. Zie voor meer informatie [De dropzone configureren in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Kan de prullenbak niet leegmaken. Zie voor meer informatie [De prullenbak herstellen en leegmaken [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Kan gebruikers niet toevoegen, bewerken of verwijderen.

![](assets/no2.png)Kan geen groepen maken of nieuwe contactpersonen toevoegen.

![](assets/no2.png)Kan contacten niet schrappen.

>[!NOTE]
>
>De menu&#39;s en functies die beschikbaar zijn voor waarnemers zijn beperkt.
>
>* Waarnemers zien het menu Koptekst of het groene menu Nieuw niet in het dashboard
>* De volgende koppelingen worden niet weergegeven door waarnemers in hun instellingen: Accountinstellingen, facturering
>


### Bezoeker {#visitor}

Bezoekers hebben de volgende machtigingen:

![](assets/cleaner2.png)Kan proefdrukken van andere gebruikers zien, controleren en goedkeuren die expliciet met hen worden gedeeld (alleen-lezen rechten op alles in een gedeelde map). Zie voor meer informatie [Proefrollen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Kan bestanden weergeven die expliciet met deze bestanden worden gedeeld.

![](assets/no2.png) Kan geen contacten en groepen bekijken

![](assets/no2.png)Kan geen proefdrukken maken, bestanden uploaden en mappen maken. Zie voor meer informatie [Bestanden en webinhoud uploaden naar [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)Kan proofs en bestanden die door andere gebruikers in de organisatie zijn gemaakt, niet weergeven, bewerken of verwijderen.

![](assets/no2.png)Kan geen proefdrukken of antwoorden bewerken.

![](assets/no2.png)Kan geen items verwijderen die in de organisatie zijn gemaakt.

![](assets/no2.png)Kan geen toegang krijgen tot de instellingen voor de facturatiepagina of account. Zie voor meer informatie [De [!DNL Workfront Proof] Factureringspagina](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) en [Accountinstellingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Kan niet instellen als eigenaar van de dropzone. Zie voor meer informatie [De dropzone configureren in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Kan de prullenbak niet leegmaken. Zie voor meer informatie [De prullenbak herstellen en leegmaken [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Kan gebruikers niet toevoegen, bewerken of verwijderen.

![](assets/no2.png)Kan geen groepen maken of nieuwe contactpersonen toevoegen.

![](assets/no2.png)Kan contacten niet schrappen.

>[!NOTE]
>
>Voor bezoekers zijn slechts beperkte menu&#39;s en functies beschikbaar.
>
>* Bezoekers zien het menu Koptekst of het groene menu Nieuw niet in hun dashboard
>* Bezoekers zien de volgende koppelingen niet in hun instellingen: Accountinstellingen, facturering
>


### Gast {#guest}

Met het gastprofiel krijgt u toegang tot proefdrukken voor revisoren die geen eigen Workfront-proefaccount hebben. Gasten hebben rechtstreeks toegang tot proefdrukken die met hen worden gedeeld via hun persoonlijke e-mailberichten.

![](assets/cleaner2.png)Kan proefdrukken weergeven, bekijken en goedkeuren die expliciet met deze proefdrukken worden gedeeld.

![](assets/cleaner2.png)Kan bestanden weergeven die expliciet met deze bestanden worden gedeeld.

![](assets/no2.png)Kan het dashboard niet openen.

![](assets/no2.png)Kan geen mappen met hen laten delen. Zie voor meer informatie [Mappen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Kan niet als Auteurs of Moderatoren aan de proefdrukken worden toegevoegd. Zie voor meer informatie [Proefrollen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

>[!NOTE]
>
>Gasten zijn geen Workfront-proefgebruikers, zodat ze niet alle proefdrukken kunnen zien die met hen worden gedeeld in hun eigen dashboard.

## Bewijs van machtigingsprofiel van een gebruiker bewerken

Beheerders en factureringsbeheerders kunnen de machtigingsprofielen van alle gebruikers in de account bewerken.

1. Voer een van de volgende handelingen uit om te zoeken naar de gebruiker die u wilt bewerken:

   * Navigeren naar **[!UICONTROL Account Settings]** klikt u op de knop **[!UICONTROL Users]** tab.

   * Ga naar de **[!UICONTROL Contacts]** pagina.

1. Klik op de naam van de gebruiker wiens machtigingen u wilt bewerken. ![](assets/screenshot-2018-03-30-14-16-05a-350x69.png)

1. Klik op de knop **[!UICONTROL Permissions profile]** en selecteer een nieuw machtigingsprofiel. :

   ![Screenshot_2018-03-30_14-18-03.png](assets/screenshot-2018-03-30-14-18-03a.png)

   De profielen van de toestemming zijn Beheerder, Supervisor, Manager, en Waarnemer.

1. Klik ergens buiten het menu om op te slaan.

>[!NOTE]
>
>Beheerders kunnen het profiel Factureringsbeheerder niet toewijzen. Een lijst met profielwijzigingen vindt u in de volgende logboeken:
>
>* De activiteitenlogboeken van de account
>* Het profiellogboek van de Gebruiker (toegankelijk slechts voor die Gebruiker)
>


Voor meer informatie over activiteitenlogboeken, zie [De [!DNL Workfront Proof] Activiteit Audit Trail](../../../workfront-proof/wp-work-proofsfiles/basic-features/activity-audit-trail.md).
