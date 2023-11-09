---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Workflows gebruiken in de integratie met Experience Manager Assets Essentials
description: Workflows gebruiken in de integratie met Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: 706e531be6f6269a927f94fee4d2c37d9367c9af
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 0%

---

# Workflows gebruiken in de Experience Manager Assets-integratie

Een werkstroom is een reeks acties die Workfront verbinden met Adobe Experience Manager as a Cloud Service. Een Workfront-beheerder kan workflows configureren in Workfront en deze vervolgens toewijzen aan projectsjablonen. Wanneer een Project wordt gecreeerd gebruikend een Malplaatje van het Project waaraan een werkschema wordt toegewezen, worden de acties die in het werkschema worden bepaald teweeggebracht.

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
   <td><p>U moet Experience Manager Assets hebben as a Cloud Service of Assets Essentials, en u moet aan het product als gebruiker in de Admin Console worden toegevoegd.</p><p>U moet schrijftoegang hebben tot de repository in Adobe Experience Manager.</p>
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
  <tr>
   <td><strong>Objectmachtigingen</strong>
   </td>
   <td>Toegang of hoger beheren voor het project 
<p>
Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <strong>Toegang tot objecten aanvragen </strong>.
   </td>
  </tr>
</table>

## Vereisten

Voordat u begint,

* Uw Workfront-beheerder moet workflows configureren in een Adobe Experience Manager-integratie. Zie voor meer informatie [De as a Cloud Service integratie met Experience Manager Assets configureren](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Een workflow toevoegen aan een sjabloon

U kunt een werkschema aan een projectmalplaatje toevoegen. De workflow wordt toegepast op alle projecten die op basis van de sjabloon zijn gemaakt.

1. Een sjabloon openen door te klikken **Sjablonen** in het Hoofdmenu selecteert u de sjabloon in de lijst.
1. Klikken **Experience Manager Assets** in het linkernavigatievenster.

   >[!NOTE]
   >
   >Als de sectie Experience Manager Assets niet wordt weergegeven in de linkernavigatie, heeft uw Workfront-beheerder geen workflows voor uw organisatie ingeschakeld. <!--Is this right?-->

1. In de **Een integratie selecteren voor het veld Automatische workflows**, selecteer de integratie met de werkschema&#39;s u voor projecten wilt gebruiken die van dit malplaatje worden gecreeerd.
1. (Optioneel) Bewerk de workflowwaarden die u wilt toepassen op projecten die op basis van deze sjabloon zijn gemaakt.

   Zie voor instructies over specifieke workflows [Werkstroomwaarden in een project bewerken](#edit-workflow-values-in-a-project) in dit artikel.

   Slechts zijn de werkschema&#39;s die op het gebied van de Experience Manager van Opstelling zijn geactiveerd beschikbaar in malplaatjes of projecten.

1. Uw wijzigingen worden automatisch opgeslagen. <!-- do they though??-->

## Een workflow toevoegen aan een project

U kunt een workflow toevoegen wanneer u een project maakt of een workflow toevoegen aan een bestaand project. In beide gevallen gebruikt u een projectsjabloon om de workflow toe te voegen.

### Een workflow toevoegen bij het maken van een project

1. Beginnen met het maken van een project.

   Zie voor instructies [Een project maken met een sjabloon](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Wanneer het selecteren van een malplaatje voor het project, selecteer het malplaatje dat de werkschema&#39;s bevat u voor dit project wilt gebruiken.
1. (Optioneel) Bewerk eventuele workflowwaarden voor het project, zoals beschreven in [Werkstroomwaarden in een project bewerken](#edit-workflow-values-in-a-project).

   Slechts zijn de werkschema&#39;s die op het gebied van de Experience Manager van Opstelling zijn geactiveerd beschikbaar in malplaatjes of projecten.


### Een workflow toevoegen aan een bestaand project

1. Begin een malplaatje aan het project toe te voegen.

   Zie voor instructies [Een sjabloon aan een project koppelen](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. Wanneer het selecteren van een malplaatje voor het project, selecteer het malplaatje dat de werkschema&#39;s bevat u voor dit project wilt gebruiken.
1. (Optioneel) Bewerk eventuele workflowwaarden voor het project, zoals beschreven in [Werkstroomwaarden in een project bewerken](#edit-workflow-values-in-a-project).

   Slechts zijn de werkschema&#39;s die op het gebied van de Experience Manager van Opstelling zijn geactiveerd beschikbaar in malplaatjes of projecten.

### Werkstroomwaarden in een project bewerken

U kunt werkstroomwaarden op projectniveau bewerken. Workflowwaarden op projectniveau overschrijven de waarden die zijn ingesteld in de projectsjabloon, die de standaardwaarden overschrijven die zijn ingesteld in de integratie van Adobe Experience Manager Assets.

Alle werkstroomwaarden vindt u in:

* De sectie Workflows van het Create project of geeft projectvenster uit.
* De sectie Adobe Experience Manager van de linkernavigatie.


  >[!NOTE]
  >
  >Als deze gebieden niet zichtbaar zijn, heeft uw Workfront-beheerder Workflows voor uw organisatie niet ingeschakeld.

#### Gekoppelde mappen

De workflow voor gekoppelde mappen bewerken:

1. Schakelen **[!UICONTROL Create Linked folder]** aan of uit naar wens.
1. (Voorwaardelijk) Als u gekoppelde mappen inschakelt, kiest u een mappad om aan te geven waar u alle gekoppelde mappen aan deze integratie wilt koppelen.
1. Klikken **[!UICONTROL Save]** als u de [!UICONTROL Create Project] of [!UICONTROL Edit project] venster.

   of

   Als u zich in de [!DNL Adobe Experience Manager area]worden de wijzigingen automatisch opgeslagen. <!--Do they though?-->


#### Elementen publiceren

De workflow voor het publiceren van elementen bewerken:

1. Schakelen **Elementen automatisch publiceren** aan of uit naar wens.
1. (Voorwaardelijk) Als u het publiceren toestaat, selecteer of u aan de publicatieservice, het merkportaal, of allebei wilt publiceren.
1. Klikken **[!UICONTROL Save]** als u de [!UICONTROL Create Project] of [!UICONTROL Edit project] venster.

   of

   Als u zich in de [!DNL Adobe Experience Manager area]worden de wijzigingen automatisch opgeslagen. <!--Do they though?-->


