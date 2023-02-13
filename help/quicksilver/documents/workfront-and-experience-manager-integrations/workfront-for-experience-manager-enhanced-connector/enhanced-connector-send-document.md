---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Een document verzenden met de verbeterde aansluiting
description: U kunt documenten van Workfront naar Experience Manager Assets verzenden. Documenten die van Workfront naar Experience Manager Assets zijn geüpload en verzonden, tellen nog steeds mee voor de totale opslag van documenten. Middelen die via Experience Manager Assets zijn gekoppeld, tellen niet mee voor de totale opslag.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# Een document verzenden met de verbeterde aansluiting

U kunt documenten van Workfront naar Experience Manager Assets verzenden. Documenten die van Workfront naar Experience Manager Assets zijn geüpload en verzonden, tellen nog steeds mee voor de totale opslag van documenten. Middelen die via Experience Manager Assets zijn gekoppeld, tellen niet mee voor de totale opslag.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Pro of hoger</p> </td> 
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
   <td> <p>Toegang of hoger weergeven op documenten</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

Voordat u begint, moet u

* Installeer de Workfront for Experience Manager Enhanced connector.

## Een document naar Experience Manager Assets verzenden

Wanneer een gebruiker een document van Workfront naar Experience Manager Assets verzendt, worden de metagegevens in kaart gebracht langs het document. Indien geconfigureerd, worden de metagegevens voortdurend gesynchroniseerd telkens wanneer een wijziging wordt aangebracht.

Een document verzenden:

1. Ga naar de **Documenten** in Workfront en selecteer het document dat u wilt verzenden.
1. Klikken **Verzenden naar** en kiest u vervolgens de Experience Manager Assets-integratie die uw beheerder heeft ingesteld.

   >[!NOTE]
   >
   >Voor deze integratie kan elke naam worden gekozen, dus Experience Manager Assets wordt niet specifiek vermeld.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Kies waar u het element wilt plaatsen en klik op **Map selecteren**.
1. Wanneer u het gewenste doel hebt gevonden, klikt u op **Opslaan**.

## Een nieuwe versie naar Experience Manager Assets sturen

U kunt een nieuwe versie toevoegen aan een document dat u eerder naar Workfront hebt geüpload. Zie voor meer informatie [Een nieuwe versie van een document uploaden](../../../documents/managing-documents/upload-new-document-version.md). Nadat de laatste versie is geüpload, kunt u deze naar Experience Manager Assets verzenden. Als een toegewezen veld in Workfront is gewijzigd, werkt de nieuwe versie de metagegevens bij in Experience Manager Assets wanneer deze worden verzonden.

De meest recente versie verzenden:

1. Ga naar de **Documenten** in Workfront en zoek het document.
1. Klikken **Verzenden naar** en kiest u vervolgens de Experience Manager Assets-integratie die uw beheerder heeft ingesteld.

   >[!NOTE]
   >
   >Voor deze integratie kan elke naam worden gekozen, dus Experience Manager Assets wordt niet specifiek vermeld.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Klikken **Opslaan**. De nieuwe versie slaat op dezelfde locatie op als de vorige versie.
