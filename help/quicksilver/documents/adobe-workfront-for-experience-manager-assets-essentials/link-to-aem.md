---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Elementen en mappen koppelen vanuit Experience Manager Assets of Assets Essentials
description: U kunt een middel of een omslag van Experience Manager Assets of Assets Essentials met om het even welk voorwerp van Adobe Workfront verbinden dat documenten steunt. Elementen die vanuit Assets Essentials worden verzonden, tellen niet mee voor de totale opslag van documenten in Workfront. Documenten die van Workfront naar Assets Essentials zijn geüpload en verzonden, tellen wel mee voor de totale opslag.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 8ecbca4d5d09b1f696f489148e960e0eeba2119e
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Elementen en mappen koppelen vanuit Experience Manager Assets of Assets Essentials

U kunt een middel of een omslag van Experience Manager Assets of Assets Essentials met om het even welk voorwerp van Adobe Workfront verbinden dat documenten steunt. Elementen die vanuit Assets Essentials worden verzonden, tellen niet mee voor de totale opslag van documenten in Workfront. Documenten die van Workfront naar Assets Essentials zijn geüpload en verzonden, tellen wel mee voor de totale opslag.

Metagegevensvelden worden eerst toegewezen wanneer u een element verzendt van Workfront naar Experience Manager Assets of Assets Essentials. Als uw Workfront-beheerder heeft ingesteld dat objectmetagegevenssynchronisatie is ingeschakeld, blijven de velden up-to-date als deze in een van beide toepassingen zijn gewijzigd.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p> Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenties*</td> 
   <td> <p>Aanvraag of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>U moet Experience Manager as a Cloud Service of Assets Essentials hebben, en u moet aan het product als gebruiker in de Admin Console worden toegevoegd.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Machtigingen Experience Manager</td> 
    <td>U moet schrijftoegang tot de map hebben.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot documenten bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang weergeven of hoger</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

Voordat u begint,

* Uw Workfront-beheerder moet een Experience Manager-integratie configureren. Zie voor meer informatie [De as a Cloud Service integratie met Experience Manager Assets configureren](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) of [De integratie met Experience Manager Assets Essentials configureren](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Middelen van Experience Manager Assets of Assets Essentials koppelen

U kunt middelen van Experience Manager Assets of Assets Essentials koppelen aan Workfront. Als het element eenmaal is gekoppeld, kunt u

* [Een gekoppeld element proefdrukken voor Experience Manager Assets of Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [Een nieuwe versie van een document uploaden](../../documents/managing-documents/upload-new-document-version.md)

1. Ga naar de **Documenten** in Workfront waar u het document wilt toevoegen.
1. Selecteren **Nieuwe toevoegen** en selecteert u vervolgens de Experience Manager-integratie die uw beheerdersinstelling heeft ingesteld.

   >[!NOTE]
   >
   >De Workfront-beheerder kan een willekeurige naam voor deze integratie kiezen, dus wordt niet specifiek verwezen naar Middelen of Assets Essentials.

1. Selecteer de gewenste elementen.

   ![](assets/select-an-asset.png)

1. Klikken **Selecteren**.

## Een map koppelen vanuit Experience Manager Assets of Assets Essentials

Rechten om afzonderlijke elementen in een map weer te geven, zijn afhankelijk van Experience Manager Assets- of Assets Essentials-machtigingen.

1. Ga naar de **Documenten** in Workfront waar u de map wilt plaatsen.
1. Selecteren **Nieuwe toevoegen** en selecteert u vervolgens de Experience Manager-integratie die uw beheerdersinstelling heeft ingesteld.

   >[!NOTE]
   >
   >De Workfront-beheerder kan een willekeurige naam voor deze integratie kiezen, dus in dit programma wordt mogelijk niet specifiek verwezen naar Middelen of Assets Essentials.

1. Selecteer de gewenste mappen.

   ![](assets/select-a-folder.png)

1. Klikken **Selecteren**.

## Een nieuwe versie koppelen vanuit Experience Manager Assets of Assets Essentials

U kunt een nieuw element uit Assets Essentials halen en het als een nieuwe versie toevoegen aan een bestaand element. Als het document al is gekoppeld en een nieuwe versie wordt toegevoegd in Assets Essentials, wordt de nieuwe versie automatisch weergegeven in Workfront.

Een nieuwe versie koppelen vanuit Assets Essentials:

1. Ga naar de **Documenten** in Workfront waar u het document wilt toevoegen.
1. Selecteer het element dat u wilt vervangen door een nieuwe versie. U kunt geen nieuwe versie van een middel in een verbonden omslag tot stand brengen.
1. Selecteren **Nieuwe toevoegen** > **Versie** en selecteert u vervolgens de Experience Manager-integratie die uw beheerdersinstelling heeft ingesteld.

   >[!NOTE]
   >
   >De Workfront-beheerder kan een willekeurige naam voor deze integratie kiezen, dus in dit programma wordt mogelijk niet specifiek verwezen naar Middelen of Assets Essentials.

1. Selecteer het gewenste element.

   ![](assets/select-an-asset.png)

1. Klikken **Selecteren**.

>[!TIP]
>
>U kunt alle versies van een element weergeven als u naar **Documentdetails** > **Versies**.
