---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Workflows gebruiken in de integratie met Experience Manager Assets Essentials
description: Workflows gebruiken in de integratie met Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: 9080dfe7e46a3780d493b59c8f2a3c4efbc011e7
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Workflows gebruiken in de Experience Manager Assets-integratie

<span class="preview">De informatie op deze pagina verwijst naar functionaliteit die nog niet algemeen beschikbaar is. Deze optie is alleen beschikbaar in de omgeving van de voorvertoningssandbox.</span>

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
   <td><p>U moet Experience Manager Assets as a Cloud Service of Assets Essentials hebben, en u moet als gebruiker in de Admin Console aan het product worden toegevoegd.</p><p>U moet schrijftoegang hebben tot de opslagplaats in Adobe Experience Manager om gekoppelde mappen te maken.</p>&gt;
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

1. <!-- main menu snippet??--> Een sjabloon openen door te klikken **Sjablonen** in het Hoofdmenu selecteert u de sjabloon in de lijst.
1. Klikken **Experience Manager Assets** in het linkernavigatievenster.

   >[!NOTE]
   >
   >Als de sectie Experience Manager Assets niet wordt weergegeven in de linkernavigatie, heeft uw Workfront-beheerder geen workflows voor uw organisatie ingeschakeld. <!--Is this right?-->

1. In de **Een integratie selecteren voor het veld Automatische workflows**, selecteer de integratie met de werkschema&#39;s u voor projecten wilt gebruiken die van dit malplaatje worden gecreeerd.
1. (Optioneel) Bewerk de workflowwaarden die u wilt toepassen op projecten die op basis van deze sjabloon zijn gemaakt.

   Als u bijvoorbeeld een gekoppelde map wilt maken op een andere locatie dan de standaardwaarde, voert u de locatie van de gekoppelde map in.

   Slechts zijn de werkschema&#39;s die op het gebied van de Experience Manager van Opstelling zijn geactiveerd beschikbaar in malplaatjes of projecten.

1. Uw wijzigingen worden automatisch opgeslagen. <!-- do they though??-->

## Een workflow toevoegen aan een project

U kunt een werkschema toevoegen wanneer het creëren van een project, of een werkschema toevoegen aan een bestaand project. In beide gevallen gebruikt u een projectsjabloon om de workflow toe te voegen.

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

1. Schakelen tussen **[!UICONTROL Create Linked folder]** op.
1. Kies een mappad om aan te geven waar u alle gekoppelde mappen aan deze integratie wilt koppelen.
1. Klik op Opslaan als u het projectvenster Project maken of Bewerken gebruikt.

   of

   Als u zich in het Adobe Experience Manager-gebied bevindt, worden de wijzigingen automatisch opgeslagen. <!--Do they though?-->
