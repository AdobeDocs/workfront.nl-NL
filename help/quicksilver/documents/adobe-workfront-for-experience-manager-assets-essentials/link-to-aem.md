---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Elementen en mappen van Experience Manager Assets of Elementen koppelen
description: U kunt middelen of een omslag van Experience Manager Assets of de Hoofdzaak van Activa aan om het even welk voorwerp van Adobe Workfront verbinden dat documenten steunt. Assets die vanuit Assets Essentials wordt verzonden, telt niet mee voor uw totale documentopslag in Workfront. Documenten die van Workfront naar Assets Essentials zijn geüpload en verzonden, tellen wel mee voor de totale opslag.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 85a2f154b3b561cdf53c68d50e66b8945f9f9823
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# Elementen en mappen van Experience Manager Assets of Elementen koppelen

U kunt middelen of een omslag van Experience Manager Assets of de Hoofdzaak van Activa aan om het even welk voorwerp van Adobe Workfront verbinden dat documenten steunt. Assets die vanuit Assets Essentials wordt verzonden, telt niet mee voor uw totale documentopslag in Workfront. Documenten die van Workfront naar Assets Essentials zijn geüpload en verzonden, tellen wel mee voor de totale opslag.

Metagegevensvelden worden eerst toegewezen wanneer u een element verzendt van Workfront naar Experience Manager Assets of Elementen. Als uw Workfront-beheerder heeft ingesteld dat objectmetagegevenssynchronisatie is ingeschakeld, blijven de velden up-to-date als deze in een van beide toepassingen zijn gewijzigd.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <td>U moet Experience Manager as a Cloud Service of Assets Essentials hebben en u moet als gebruiker aan het product worden toegevoegd in de Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager-machtigingen</td> 
    <td>U moet schrijftoegang tot de map hebben.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot documenten bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang weergeven of hoger</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

+++

## Vereisten

Voordat u begint,

* Uw Workfront-beheerder moet een Experience Manager-integratie configureren. Voor meer informatie, zie [ de integratie van Experience Manager Assets as a Cloud Service ](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) vormen of [ vormen de integratie van de Hoofdzaak van Experience Manager Assets ](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Middelen van Experience Manager Assets of Elementen koppelen

U kunt middelen van Experience Manager Assets of Elementen aan Workfront koppelen. Als het element eenmaal is gekoppeld, kunt u

* [ Bewijs van een verbonden activa voor Experience Manager Assets of de Hoofdzaak van Activa ](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [Een nieuwe versie van een document uploaden](../../documents/managing-documents/upload-new-document-version.md)

1. Ga naar het **gebied van Documenten** in Workfront waar u het document wilt toevoegen.
1. Selecteer **toevoegen Nieuw**, dan selecteren de integratie van Experience Manager uw beheerderopstelling.

   >[!NOTE]
   >
   >De Workfront-beheerder kan een willekeurige naam voor deze integratie kiezen, dus Assets of Assets Essentials wordt niet specifiek vermeld.

1. Selecteer de gewenste elementen.

   ![ Uitgezocht een activa ](assets/select-an-asset.png)

1. Klik **Uitgezocht**.

## Een map koppelen vanuit Experience Manager Assets of Assets Essentials

Machtigingen om afzonderlijke elementen in een map weer te geven, zijn afhankelijk van Experience Manager Assets- of Assets Essentials-machtigingen.

1. Ga naar het **gebied van Documenten** in Workfront waar u de omslag wilt.
1. Selecteer **toevoegen Nieuw**, dan selecteren de integratie van Experience Manager uw beheerderopstelling.

   >[!NOTE]
   >
   >De Workfront-beheerder kan een willekeurige naam voor deze integratie kiezen, dus Assets of Assets Essentials wordt niet specifiek genoemd.

1. Selecteer de gewenste mappen.

   ![ selecteer een omslag ](assets/select-a-folder.png)

1. Klik **Uitgezocht**.

## Een nieuwe versie koppelen vanuit Experience Manager Assets of Assets Essentials

U kunt een nieuw element ophalen van Elementen en het als een nieuwe versie toevoegen aan een bestaand element. Als het document al is gekoppeld en er een nieuwe versie wordt toegevoegd aan de Elementen, wordt de nieuwe versie automatisch weergegeven in Workfront.

Een nieuwe versie koppelen van Elementen:

1. Ga naar het **gebied van Documenten** in Workfront waar u het document wilt toevoegen.
1. Selecteer het element dat u wilt vervangen door een nieuwe versie. U kunt geen nieuwe versie van een middel in een verbonden omslag tot stand brengen.
1. Selecteer **Nieuwe** toevoegen > **Versie**, dan de integratie van Experience Manager uw beheerderopstelling selecteren.

   >[!NOTE]
   >
   >De Workfront-beheerder kan een willekeurige naam voor deze integratie kiezen, dus Assets of Assets Essentials wordt niet specifiek genoemd.

1. Selecteer het gewenste element.

   ![ Uitgezocht een activa ](assets/select-an-asset.png)

1. Klik **Uitgezocht**.

>[!TIP]
>
>U kunt alle versies van activa bekijken als u **Details van het Document** > **Versies** gaat.
