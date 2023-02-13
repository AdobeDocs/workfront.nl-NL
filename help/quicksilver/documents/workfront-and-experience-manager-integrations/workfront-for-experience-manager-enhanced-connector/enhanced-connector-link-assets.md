---
title: Elementen en mappen koppelen met de verbeterde aansluiting
description: U kunt een middel of een omslag van Experience Manager Assets aan om het even welk voorwerp van Workfront verbinden dat documenten steunt.
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Elementen en mappen koppelen met de verbeterde aansluiting

U kunt een middel of een omslag van Experience Manager Assets aan om het even welk voorwerp van Workfront verbinden dat documenten steunt. Elementen die vanuit Experience Manager Assets worden verzonden, tellen niet mee voor de totale opslag van documenten in Workfront. Documenten die van Workfront naar Experience Manager Assets zijn geüpload en verzonden, tellen wel mee voor de totale opslag.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Aanvraag of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot documenten bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang of hoger weergeven op een document</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

Voordat u begint, moet u

* De Workfront for Experience Manager Enhanced-aansluiting installeren

## Middelen van Experience Manager Assets koppelen

U kunt middelen van Experience Manager Assets aan Workfront koppelen. Als het element eenmaal is gekoppeld, kunt u

* [Een gekoppeld element proefdrukken voor Experience Manager Assets](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md)
* [Een nieuwe versie van een document uploaden](../../../documents/managing-documents/upload-new-document-version.md)

Een element koppelen aan Experience Manager Assets:

1. Ga naar de **Documenten** in Workfront waar u het document wilt toevoegen.
1. Klikken **Nieuw toevoegen** en kiest u vervolgens de Experience Manager Assets-integratie die uw beheerder heeft ingesteld.

   >[!NOTE]
   >
   >Voor deze integratie kan elke naam worden gekozen, dus Experience Manager Assets wordt niet specifiek vermeld.

1. Selecteer de gewenste elementen.

   ![](assets/select-an-asset.png)

1. Klikken **Koppeling**.

## Een map koppelen vanuit Experience Manager Assets

Rechten om afzonderlijke elementen in een map weer te geven, zijn afhankelijk van Experience Manager Assets-machtigingen.

Een map koppelen aan Experience Manager Assets:

1. Ga naar de **Documenten** in Workfront waar u het document wilt toevoegen.
1. Klikken **Nieuw toevoegen** en kiest u vervolgens de Experience Manager Assets-integratie die uw beheerder heeft ingesteld.

   >[!NOTE]
   >
   >Voor deze integratie kan elke naam worden gekozen, dus Experience Manager Assets wordt niet specifiek vermeld.

1. Selecteer de gewenste mappen.

   ![](assets/select-a-folder.png)

1. Klikken **Koppeling**.

## Een nieuwe versie koppelen vanuit Experience Manager Assets

U kunt een nieuw element uit Experience Manager Assets halen en het aan een bestaand element toevoegen als een nieuwe versie in Workfront. Als het document al is gekoppeld en een nieuwe versie wordt toegevoegd in Experience Manager Assets, wordt de nieuwe versie automatisch weergegeven in Workfront.

>[!TIP]
>
>U kunt alle versies van een element weergeven als u naar **Documentdetails** > **Versies**.

Een nieuwe versie koppelen vanuit Experience Manager Assets:

1. Ga naar de **Documenten** in Workfront waar u het document wilt toevoegen.
1. Selecteer het element dat u wilt vervangen door een nieuwe versie. U kunt geen nieuwe versie van een middel in een verbonden omslag tot stand brengen.
1. Klikken **Nieuw toevoegen** en kiest u vervolgens de Experience Manager Assets-integratie die uw beheerder heeft ingesteld.

   >[!NOTE]
   >
   >Voor deze integratie kan elke naam worden gekozen, dus Experience Manager Assets wordt niet specifiek vermeld.

1. Selecteer het gewenste element.

   ![](assets/select-an-asset.png)

1. Klikken **Koppeling**.
