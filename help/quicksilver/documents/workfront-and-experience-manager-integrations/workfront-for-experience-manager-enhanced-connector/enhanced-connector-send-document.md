---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Een document verzenden met de verbeterde aansluiting
description: U kunt documenten van Workfront naar Experience Manager Assets verzenden. Documenten die van Workfront naar Experience Manager Assets zijn geüpload en verzonden, tellen nog steeds mee voor de totale opslag van documenten. Assets die vanuit Experience Manager Assets is gekoppeld, telt niet mee voor de totale opslag.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
source-git-commit: 3f9a824780f2ded914d461a473aef3b6ecfa8701
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---

# Een document verzenden met de verbeterde aansluiting

U kunt documenten van Workfront naar Experience Manager Assets verzenden. Documenten die van Workfront naar Experience Manager Assets zijn geüpload en verzonden, tellen nog steeds mee voor de totale opslag van documenten. Assets die vanuit Experience Manager Assets is gekoppeld, telt niet mee voor de totale opslag.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Medewerker of hoger</p>
   <p>Aanvraag of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aanvullende producten</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot documenten bewerken</p> s="MCXref xref"&gt;Aangepaste toegangsniveaus maken of wijzigen </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang of hoger weergeven op documenten</p></td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Vereisten

Voordat u begint, moet u

* Installeer de Workfront for Experience Manager Enhanced connector.

## Een document naar Experience Manager Assets verzenden

Wanneer een gebruiker een document van Workfront naar Experience Manager Assets verzendt, worden de metagegevens in kaart gebracht langs het document. Indien gevormd, de meta-gegevens syncs onophoudelijk telkens als een verandering wordt aangebracht.

Een document verzenden:

1. Ga naar het **gebied van Documenten** in Workfront, en selecteer het document u wilt verzenden.
1. Klik **verzenden naar**, dan kies de integratie van Experience Manager Assets uw beheerderopstelling.

   >[!NOTE]
   >
   >Voor deze integratie kan elke naam worden gekozen, dus Experience Manager Assets wordt niet specifiek vermeld.

   ![ verzendt naar ](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Kies waar u de activa wilt gaan, dan klik **Uitgezochte Omslag**.
1. Wanneer u uw gewenste bestemming vindt, klik **sparen**.

## Een nieuwe versie naar Experience Manager Assets sturen

U kunt een nieuwe versie toevoegen aan een document dat u eerder naar Workfront hebt geüpload. Voor meer informatie, zie [ een nieuwe versie van een document ](../../../documents/managing-documents/upload-new-document-version.md) uploaden. Nadat de laatste versie is geüpload, kunt u deze naar Experience Manager Assets verzenden. Als een toegewezen veld in Workfront is gewijzigd, werkt de nieuwe versie de metagegevens bij in Experience Manager Assets wanneer deze worden verzonden.

De meest recente versie verzenden:

1. Ga naar het **gebied van Documenten** in Workfront, en bepaal de plaats van het document.
1. Klik **verzenden naar**, dan kies de integratie van Experience Manager Assets uw beheerderopstelling.

   >[!NOTE]
   >
   >Voor deze integratie kan elke naam worden gekozen, dus Experience Manager Assets wordt niet specifiek vermeld.

   ![ verzendt naar ](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Klik **sparen**. De nieuwe versie slaat op dezelfde locatie op als de vorige versie.
