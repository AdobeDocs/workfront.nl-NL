---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Workfront Fusion gebruiken om een Workfront-project te maken met Adobe Experience Manager-workflows
description: Als u een project via Workfront Fusion maakt en Adobe Experience Manager-workflows wilt opnemen in het project, moet u een specifieke Fusion-moduleconfiguratie gebruiken, zoals in dit artikel wordt beschreven.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
exl-id: b8132d5e-234d-47f6-a09c-ca46018a2d77
source-git-commit: 1677ed676a5ccb4f519cc81bf3b31cc90b8326b4
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# Workfront Fusion gebruiken om een Workfront-uitgave om te zetten in een project dat Adobe Experience Manager-workflows bevat

Als u een project via Workfront Fusion maakt en Adobe Experience Manager-workflows wilt opnemen in het project, moet u een specifieke Fusion-moduleconfiguratie gebruiken, zoals in dit artikel wordt beschreven.

>[!NOTE]
>
>Workflows zijn alleen beschikbaar in een Adobe Experience Manager as a Cloud Service-integratie. Ze zijn niet beschikbaar in integraties met Adobe Experience Manager Assets Essentials.


## Toegangsvereisten

U moet het volgende hebben:

<table>
  <tr>
   <td><strong>Adobe Workfront-abonnement*</strong>
   </td>
   <td>Alle
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront-licenties*</strong>
   </td>
   <td>Aanvraag of hoger
   </td>
  </tr>
  <tr>
   <td><strong>Product</strong>
   </td>
   <td><b>Adobe Experience Manager<b>:
   <ul>
   <li>
   <p>U moet Experience Manager Assets hebben as a Cloud Service of Assets Essentials, en u moet aan het product als gebruiker in de Admin Console worden toegevoegd.</p>
   </li
   ><li>
   <p>U moet schrijftoegang hebben tot de repository in Adobe Experience Manager.</p>
   </li>
   </ul>
  <b>Workfront Fusion</b>:<p>Nieuw:</p>
   <ul>
   <li>
   <p>Select or Prime Workfront Plan: Uw organisatie moet Adobe Workfront Fusion aanschaffen.</p>
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
   <td><strong>Configuraties op toegangsniveau*</strong>
   </td>
   <td>Toegang tot documenten bewerken
<p>
<strong>Opmerking: </strong>Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <strong>Aangepaste toegangsniveaus maken of wijzigen</strong>.
   </td>
  </tr>
</table>

## Vereisten

Voordat u begint,

* Uw Workfront-beheerder moet workflows configureren in een Adobe Experience Manager-integratie. Zie voor meer informatie [De as a Cloud Service integratie met Experience Manager Assets configureren](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).
* U moet een projectmalplaatje hebben dat met een Adobe Experience Manager integratie verbonden omslagwerkschema wordt gevormd.
* U moet een toepassing OAuth in Workfront hebben gecreeerd om de verbinding voor deze module te vormen.

  Zie voor instructies [Een OAuth-toepassing maken](#create-an-oauth-application) in dit artikel.

## Moduleconfiguratie

Als u in Workfront Fusion een project wilt maken dat Adobe Experience Manager-workflows bevat, moet u de module Workfront > Misc Action gebruiken.

1. Voeg de **Workfront** > **Handeling Misc** aan uw scenario.
1. In de **Verbinding** in het veld selecteert u de Workfront-verbinding die verbinding maakt met de account die deze module gebruikt.

   Zie voor instructies over het maken van een verbinding [Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#connect-workfront-to-workfront-fusion) in de Workfront-modules.

   Voor instructies voor het creëren van identiteitskaart van de Cliënt en Geheim u een verbinding zult moeten creëren, zie [Een OAuth-toepassing maken](#create-an-oauth-application) in dit artikel.

1. In de **Recordtype** veld, selecteren `Issue`.
1. In de **Handeling** veld, selecteren `convertToProject`.
1. In de **ID** Voer de id in van de uitgave die u naar een project converteert.
1. Inschakelen **Geavanceerde instellingen tonen**.
1. Ga naar de onderkant van de module en zoek de **Project (geavanceerde verzameling)** veld.
1. Plak de volgende tekst in de **Project (geavanceerde verzameling)** veld.

   ```
   {
       "aemNativeFolderTreeIDs": ["Folder Tree ID here"],
       "aemNativeFolderWorkflowEnabled": "true",
       "name": "New project name here",
       "templateID": "Template ID here"
   }
   ```

1. Vervangen `Folder tree ID here` met de map-id&#39;s.

   Ga naar [Locatie mapstructuur-id&#39;s](#locate-folder-tree-ids) in dit artikel.

   Als u meerdere mapstructuren wilt gebruiken, scheidt u de id&#39;s met een komma:

   `"aemNativeFolderTreeIDs": ["Folder tree ID here","Second folder tree ID here"],`
1. Vervangen `New project name here` met de naam die het nieuwe project zal hebben.
1. Vervangen `Template ID here` met identiteitskaart van het malplaatje dat u voor het nieuwe project gebruikt.

   U kunt de sjabloon-id uit een vorige module (zoals een Workfront > Zoekmodule) toewijzen of deze zoeken in de URL van de sjabloonpagina in Workfront.

1. Klikken **OK** om de moduleconfiguratie te bewaren.

## Locatie mapstructuur-id&#39;s

De mapstructuur-id&#39;s zoeken:

>[!NOTE]
>
>Deze instructies gebruiken Chrome-browser.

1. Open in Workfront de sjabloon die u voor dit project wilt gebruiken. Deze sjabloon moet de Adobe Experience Manager-configuratie bevatten die u voor het project wilt gebruiken.
1. Open de ontwikkelaarsgereedschappen voor uw browser.
1. Open de **Netwerk** in de ontwikkelaarsgereedschappen.
1. In de **Filter** box, enter `object-workflow`.
1. Klik in de kolom Naam op de alfanumerieke id die wordt weergegeven.

   ![Map-id 1 zoeken](assets/finding-folder-id-1.png)

1. Klik op de knop **Voorvertoning** rechts van de alfanumerieke id.
1. Open de volgende samengevouwen secties:
   1. `data`
   1. `objectWorkflow`
   1. `workflows`
   1. `enhancedLinkedFolderCreationWorkflow`
   1. `enhancedLinkedFolderCreationWorkflowConfigurations`

   Elke mappenstructuur wordt aangeduid met een getal. 0 (nul) staat voor de eerste map in de lijst, 1 voor de tweede, enzovoort. Als de sjabloon maar één mapstructuur bevat, is de waarde 0.

1. Open de mappenstructuur die u voor het nieuwe project wilt gebruiken. Noteer de `_id` veldwaarde. Als u meer dan één mapstructuur wilt gebruiken, noteert u alle `_id` veldwaarden voor de mapstructuren die u wilt gebruiken.

   ![Map-id 2 zoeken](assets/finding-folder-id-2.png)

   Dit zijn de `aemNativeFolderTreeIDs`  de waarden die u in de **Project (geavanceerde verzameling)** in het veld **Workfront** > **Diverse handelingen** Fusiemodule.

## Een OAuth-toepassing maken

Voor de verbinding van deze module moet u in Workfront een OAuth-toepassing instellen. U hoeft dit slechts één keer te doen voor een bepaalde Workfront-verbinding in Fusion.

1. Maak in Workfront een OAuth-toepassing zoals beschreven in [Een OAuth2-toepassing maken met gebruikersgegevens (doorloop machtigingscode)](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow) in het artikel OAuth2-toepassingen maken voor [!DNL Workfront] integratie.
1. Kopieer de client-id en het clientgeheim naar een beveiligde locatie.
1. In de **URI&#39;s omleiden** veld, voert u het volgende in:

   ```
   http://app.workfrontfusion.com/oauth/cb/workfront-workfront
   ```

1. Klikken **Opslaan**.

U zult deze identiteitskaart van de Cliënt en het geheim van de Cliënt gebruiken wanneer het vormen van de verbinding van de module in Fusion.

Zie voor instructies over het maken van een verbinding [Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#connect-workfront-to-workfront-fusion) in de Workfront-modules.

