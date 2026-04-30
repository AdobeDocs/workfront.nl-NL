---
product-area: documents
navigation-topic: manage-documents
title: Documentopslaglimieten controleren
description: Als Adobe Workfront-beheerder geeft u het gebruik en de quota voor documentopslag weer op de pagina Klantgegevens. De manier waarop opslag wordt weergegeven, hangt af van het feit of uw organisatie oude Workfront-opslag of Adobe Enterprise-opslag gebruikt.
author: Courtney
feature: Digital Content and Documents
exl-id: f5d1963e-b205-44b9-b2b6-b7de465c6977
last-update: 2026-04-29T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: e25be455e16beee813e612b983bca1302f129e6f
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Documentopslaglimieten controleren

{{highlighted-preview}}

Hoewel er geen beperkingen gelden voor de typen en formaten van afzonderlijke bestanden die gebruikers naar uw Workfront-exemplaar kunnen uploaden, bevat uw Workfront-abonnement een totale opslaglimiet. Als beheerder van Workfront, controleert u gebruik en quota van het gebied van de Opstelling op de pagina van de Info van de Klant.

De manier waarop opslag wordt weergegeven, hangt af van het feit of uw organisatie oude Workfront-opslag of Adobe Enterprise-opslag gebruikt:

* Als u de opslag van erfenisWorkfront gebruikt, zie &lbrace;de opslag van Workfront van de Verouderde [&#128279;](#legacy-workfront-storage) in dit artikel.
* Als u de ondernemingsopslag van Adobe gebruikt, zie [&#x200B; de ondernemingsopslag van Adobe &#x200B;](#adobe-enterprise-storage) in dit artikel.

  Voor meer informatie over ondernemingsopslag, zie [&#x200B; overzicht van de ondernemingsopslag van Adobe &#x200B;](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Workfront-plan</td> 
   <td> <p>Elk Workfront-pakket voor het beheer van documenten die gebruikmaken van oude opslagsystemen</p>
      <p>Elk workflowpakket voor het beheer van documenten met behulp van Adobe Enterprise Storage</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Legacy Workfront-opslag

Als uw organisatie gebruikmaakt van verouderde Workfront-opslag, wordt op de pagina Klantgegevens één opslagquotum weergegeven voor documenten die rechtstreeks naar Workfront worden geüpload.

Verouderde Workfront-documentopslag controleren:

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Systeem** > **Info van de Klant**.
1. In de **Basis Info** sectie, vind **Quota van de Opslag**. Hier kunt u zien hoeveel opslagruimte u momenteel gebruikt en hoeveel opslagruimte uw Workfront-abonnement bevat.

Het opslagquotum wordt dagelijks vernieuwd om het meest actuele aantal weer te geven.

>[!NOTE]
>
>Deze limiet geldt niet voor documenten die u via een andere externe serviceprovider (SharePoint, Google Drive, Webdam, Box, Dropbox of een andere leverancier van documentmiddelen) met Workfront verbindt.

<div class="preview">

## Adobe Enterprise-opslag

Als uw organisatie gebruikmaakt van Adobe Enterprise-opslag, geeft Klantgegevens een opslagoverzicht dat het gebruik in verschillende secties opsplitst voor oudere Workfront-opslag, Adobe Enterprise-opslag en Frame.io. Workfront past ook een soft cap toe op uploads wanneer het gebruik uw quota overschrijdt, zodat kunnen de gebruikers nog documenten uploaden.

### Opslaggebruik weergeven op klantgegevens

Adobe Enterprise-documentopslag controleren:

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Systeem** > **Info van de Klant**.
1. Ga naar de **sectie van het Overzicht van de Opslag**.
1. Bekijk het gebruik voor Adobe Enterprise Storage.
   <!--Both Workfront and Frame.io usage are broken down separately, but roll up to the total usage for Adobe enterprise storage.-->

![&#x200B; het gebruik van de ondernemingsopslag van Adobe op Info van de Klant &#x200B;](assets/storage-usage.png)

De cijfers van het gebruik verfrissen zich regelmatig zodat ziet u een bijgewerkt aantal.

### E-mailmeldingen voor beheerders

Wanneer het gebruik 75%, 85%, of 100% van uw opslagquota overschrijdt, verzendt Workfront een e-mailbericht naar de Beheerders van het Systeem.

</div>