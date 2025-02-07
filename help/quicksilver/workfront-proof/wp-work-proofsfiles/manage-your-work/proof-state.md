---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Proefstaat in Workfront Proof begrijpen
description: In  [!DNL Workfront Proof], bestaan de proefdrukken in verschillende staten. Deze staten bepalen welke acties u kunt ondernemen op het bewijs, zoals het maken van opmerkingen of het nemen van beslissingen.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cd120e53-d6c2-4929-904f-a9f72903f074
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Proefstaat in Workfront Proof begrijpen

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [ het Bewijzen ](../../../review-and-approve-work/proofing/proofing.md).

In [!DNL Workfront Proof] bestaan proeven in verschillende staten. Deze staten bepalen welke acties u kunt ondernemen op het bewijs, zoals het maken van opmerkingen of het nemen van beslissingen.

## Proefstatus

De vier staten zijn als volgt:

* [Actief](#active)
* [Vergrendeld](#locked)
* [Concept (alleen Dropzone)](#draft-dropzone-only)
* [Verzonden (alleen Dropzone)](#submitted-dropzone-only)

### Actief {#active}

Proefdrukken die via de pagina Nieuwe proef of de dropzone naar [!DNL Workfront Proof] zijn geüpload, worden na verwerking als actief weergegeven. Wanneer een proefdruk actief is, kunnen gebruikers opmerkingen maken en besluiten nemen over de proefdruk.

>[!NOTE]
>
>Proefdrukken die via de Dropzone worden geüpload, worden alleen als Actief weergegeven als de optie Proefdruk bij verzending activeren is ingeschakeld. Als deze optie niet is ingeschakeld, moet u de proefdruk handmatig activeren.

Voor meer informatie over montages Dropzone, zie [ dropzone in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md) vormen.

### Vergrendeld {#locked}

U kunt een proefdruk vergrendelen wanneer u deze hebt gecontroleerd. Een bewijs vergrendelen betekent dat er geen opmerkingen of besluiten meer op de bewijsmiddelen kunnen worden genomen, maar dat het bewijs nog kan worden geopend.

Gebruikers die bewerkingsrechten hebben op de proefdruk, kunnen deze ontgrendelen.

Voor meer informatie over rechten, zie [ Profielen van de Toestemmingen van de Bewijs in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
>E-mailberichten worden niet meer verzonden wanneer een proefdruk is vergrendeld. Als bijvoorbeeld een bewijs vóór de deadline is vergrendeld, wordt geen e-mailbericht verzonden wanneer de deadline is bereikt.

### Concept (alleen Dropzone) {#draft-dropzone-only}

Wanneer u een proef door Dropzone voorlegt, gaat het in de staat van het Ontwerp alvorens admin het activeert. Wanneer het zich in de ontwerpstreek bevindt, kunt u geen actie ondernemen met betrekking tot de proef.

### Verzonden (alleen Dropzone) {#submitted-dropzone-only}

Nadat de beheerder een concept heeft geactiveerd, wordt uw proefdruk weergegeven als Verzonden in de Dropzone. Nadat de proefdruk is verzonden, kunt u actie ondernemen.

## Proefstatus weergeven en wijzigen

Voor informatie over het bekijken van een lijst van alle proeven in een specifieke staat, zoals het bekijken van alle Actieve of Vergrendelde proeven, zie [ Punten op de Pagina van Bekijken in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) in artikel [ leiden Punten op de Pagina van Bekijken in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Open het [!DNL Workfront Proof] -dashboard.

   Voor meer informatie, zie [ Toegang  [!DNL Workfront Proof]  van Adobe Workfront ](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

1. Klik op de pijl **[!UICONTROL Dashboard]** naast de proefdruk die u wilt weergeven of wijzig de status van de proefdruk.**[!UICONTROL Expand]**

   ![ uitbreiden ](assets/screen-shot-2018-05-02-at-11.31.29-am-350x85.png)

   De sectie **[!UICONTROL Workflow process]** wordt weergegeven.

   ![ proces van het Werkschema ](assets/screen-shot-2018-05-02-at-11.33.20-am-350x226.png)

1. Bekijk **[!UICONTROL State]** in **[!UICONTROL Workflow process]**.

1. (Optioneel) Als u de status wilt wijzigen, plaatst u de muis boven de huidige status **[!UICONTROL State]** en klikt u op de vervolgkeuzelijst. Selecteer vervolgens een nieuwe status.

   ![ Nieuwe staat ](assets/screen-shot-2018-05-02-at-11.35.30-am.png)
