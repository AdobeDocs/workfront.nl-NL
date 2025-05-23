---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Workfront Fusion gebruiken om een Workfront-project te maken met Adobe Experience Manager-workflows
description: Als u een project via Workfront Fusion maakt en Adobe Experience Manager-workflows wilt opnemen in het project, moet u een specifieke Fusion-moduleconfiguratie gebruiken, zoals in dit artikel wordt beschreven.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
exl-id: b8132d5e-234d-47f6-a09c-ca46018a2d77
source-git-commit: cb38223c4dd8048fd2ab105abce2c9a79b84c43f
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---

# Workfront Fusion gebruiken om een Workfront-uitgave om te zetten in een project dat Adobe Experience Manager-workflows bevat

Als u een project via Workfront Fusion maakt en Adobe Experience Manager-workflows wilt opnemen in het project, moet u een specifieke Fusion-moduleconfiguratie gebruiken, zoals in dit artikel wordt beschreven.

>[!NOTE]
>
>Workflows zijn alleen beschikbaar in een Adobe Experience Manager as a Cloud Service-integratie. Ze zijn niet beschikbaar in integraties met Adobe Experience Manager Assets Essentials.


## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben:

<table>
  <tr>
    <td><strong>Adobe Workfront-abonnement*</strong></td>
    <td>Alle</td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront-licenties*</strong></td>
   <td>Aanvraag of hoger</td>
  </tr>
  <tr>
   <td><strong>Product</strong></td>
   <td>
     <p><b>Adobe Experience Manager:</b></p>
     <ul>
       <li>
         <p>U moet Experience Manager Assets as a Cloud Service Assets Essentials hebben, en u moet aan het product als gebruiker in de Admin Console worden toegevoegd.</p>
       </li>
       <li>
        <p>U moet schrijftoegang hebben tot de repository in Adobe Experience Manager.</p>
       </li>
     </ul>
     <p><b>Workfront Fusion:</b></p>
     <p>Nieuw:</p>
     <ul>
       <li>
         <p>Selecteer of Prime Workfront Plan: Uw organisatie moet Adobe Workfront Fusion aanschaffen.</p>
       </li>
       <li> 
         <p>Ultimate Workfront Plan: Workfront Fusion is inbegrepen.</p>
       </li>
     </ul>
     <p>of</p>
     <p>Huidig: Uw organisatie moet Adobe Workfront Fusion aanschaffen.</p>
   </td>
  </tr>
  <tr>
   <td><strong> het niveauconfiguraties van de Toegang* </strong>
   </td>
   <td>Toegang tot documenten bewerken
     <p>
       <strong> Nota: </strong> als u nog geen toegang hebt, vraag uw beheerder van Workfront als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <strong> tot douanetoegangsniveaus </strong> leiden of wijzigen.
     </p>
   </td>
  </tr>
</table>

+++

## Vereisten

Voordat u begint,

* Uw Workfront-beheerder moet workflows configureren in een Adobe Experience Manager-integratie. Voor meer informatie, zie [ de as a Cloud Service integratie van Experience Manager Assets ](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional) vormen.
* U moet een projectmalplaatje hebben dat met een Adobe Experience Manager integratie verbonden omslagwerkschema wordt gevormd.
* U moet een toepassing OAuth in Workfront hebben gecreeerd om de verbinding voor deze module te vormen.

  Voor instructies, zie [ tot een toepassing OAuth ](#create-an-oauth-application) in dit artikel leiden.

## Moduleconfiguratie

Als u in Workfront Fusion een project wilt maken dat Adobe Experience Manager-workflows bevat, moet u de module Workfront > Misc Action gebruiken.

1. Voeg de **Workfront** > **Diverse module van de Actie** aan uw scenario toe.
1. Op het **gebied van de Verbinding**, selecteer de verbinding van Workfront die met de rekening verbindt deze module zal gebruiken.

   Voor instructies bij het creëren van een verbinding, zie [  [!DNL Workfront]  verbinden  [!DNL Workfront Fusion] ](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion) in de modules van artikelWorkfront.

   Voor instructies bij het creëren van identiteitskaart van de Cliënt en Geheime cliënt zult u een verbinding moeten creëren, zie [ een toepassing OAuth ](#create-an-oauth-application) in dit artikel creëren.

1. Op het **gebied van het Type van Verslag**, uitgezochte `Issue`.
1. Op het **gebied van de Actie**, uitgezochte `convertToProject`.
1. Op het **gebied van identiteitskaart**, ga of kaart identiteitskaart van de kwestie in die u in een project omzet.
1. Laat **toe tonen geavanceerde montages**.
1. De rol aan de bodem van de module en bepaalt de plaats van het **Project (Geavanceerde Inzameling)** gebied.
1. Plak de volgende tekst in het **Project (Geavanceerde Inzameling)** gebied.

   ```
   {
       "aemNativeFolderTreeIDs": ["Folder Tree ID here"],
       "aemNativeFolderWorkflowEnabled": "true",
       "name": "New project name here",
       "templateID": "Template ID here"
   }
   ```

1. Vervang `Folder tree ID here` door de map-id&#39;s.

   Om van omslagboom IDs de plaats te bepalen, zie [ plaats omslagboom IDs ](#locate-folder-tree-ids) in dit artikel.

   Als u meerdere mapstructuren wilt gebruiken, scheidt u de id&#39;s met een komma:

   `"aemNativeFolderTreeIDs": ["Folder tree ID here","Second folder tree ID here"],`
1. Vervang `New project name here` door de naam die het nieuwe project krijgt.
1. Vervang `Template ID here` door de id van de sjabloon die u voor het nieuwe project gebruikt.

   U kunt de sjabloon-id uit een vorige module (zoals een Workfront > Zoekmodule) toewijzen of deze zoeken in de URL van de sjabloonpagina in Workfront.

1. Klik **O.K.** om de moduleconfiguratie te bewaren.

## Locatie mapstructuur-id&#39;s

De mapstructuur-id&#39;s zoeken:

>[!NOTE]
>
>Deze instructies gebruiken de Chrome browser.

1. Open in Workfront de sjabloon die u voor dit project wilt gebruiken. Deze sjabloon moet de Adobe Experience Manager-configuratie bevatten die u voor het project wilt gebruiken.
1. Open de ontwikkelaarsgereedschappen voor uw browser.
1. Open het **lusje van het Netwerk** in de ontwikkelaarshulpmiddelen.
1. In de **doos van de Filter**, ga `object-workflow` in.
1. Klik in de kolom Naam op de alfanumerieke id die wordt weergegeven.

   ![ Locating folder ID 1 ](assets/finding-folder-id-1.png)

1. Klik het **lusje van de Voorproef** rechts van alfanumerieke identiteitskaart
1. Open de volgende samengevouwen secties:
   1. `data`
   1. `objectWorkflow`
   1. `workflows`
   1. `enhancedLinkedFolderCreationWorkflow`
   1. `enhancedLinkedFolderCreationWorkflowConfigurations`

   Elke mappenstructuur wordt aangeduid met een getal. 0 (nul) staat voor de eerste map in de lijst, 1 voor de tweede, enzovoort. Als de sjabloon maar één mapstructuur bevat, is de waarde 0.

1. Open de mappenstructuur die u voor het nieuwe project wilt gebruiken. Noteer de veldwaarde van `_id` . Als u meer dan één mapstructuur wilt gebruiken, moet u alle `_id` -veldwaarden noteren voor de mapstructuren die u wilt gebruiken.

   ![ Locating folder ID 2 ](assets/finding-folder-id-2.png)

   Dit zijn de `aemNativeFolderTreeIDs` waarden die u in het **Project (Geavanceerde Inzameling)** gebied op **Workfront** > **Diverse Module van de Fusie van Acties** zult ingaan.

## Een OAuth-toepassing maken

Voor de verbinding van deze module moet u in Workfront een OAuth-toepassing instellen. U hoeft dit slechts één keer te doen voor een bepaalde Workfront-verbinding in Fusion.

1. In Workfront, begin creërend een toepassing OAuth, zoals die in [ wordt beschreven creeer een toepassing OAuth2 gebruikend gebruikersgeloofsbrieven (de stroom van de code van de Vergunning) ](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow) in het artikel leidt toepassingen OAuth2 voor [!DNL Workfront] integratie.
1. Kopieer de client-id en het clientgeheim naar een beveiligde locatie.
1. Op het **Redirect URIs** gebied, ga het volgende in:

   ```
   http://app.workfrontfusion.com/oauth/cb/workfront-workfront
   ```

1. Klik **sparen**.

U zult deze identiteitskaart van de Cliënt en het geheim van de Cliënt gebruiken wanneer het vormen van de verbinding van de module in Fusion.

Voor instructies bij het creëren van een verbinding, zie [  [!DNL Workfront]  verbinden  [!DNL Workfront Fusion] ](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion) in de modules van artikelWorkfront.
