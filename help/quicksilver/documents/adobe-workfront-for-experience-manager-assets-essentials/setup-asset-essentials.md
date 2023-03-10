---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: De integratie met Experience Manager Assets Essentials configureren
description: Sluit uw werk aan op uw inhoud in Experience Manager Assets Essentials - BEWERK ME.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 059cfa79c57f071b3c7efd690b583099f46c99fb
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# De integratie met Experience Manager Assets Essentials configureren

Sluit uw werk aan op uw inhoud in Experience Manager Assets Essentials &#x200B;:

* Elementen en metagegevens van Adobe Workfront naar Experience Manager Assets Essentials &#x200B;
* Elementen van Experience Manager Assets Essentials koppelen aan uw projecten en taken in Workfront &#x200B;
* Workflows voor versiebeheer vereenvoudigen voor middelen die naar Experience Manager Assets Essentials worden geduwd


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
   <td>Plan
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager</strong>
   </td>
   <td>Standaard
   </td>
  </tr>
  <tr>
   <td><strong>Product</strong>
   </td>
   <td>U moet beschikken over Experience Manager Assets Essentials en u moet als gebruiker aan het product in de Admin Console worden toegevoegd.
   </td>
  </tr>
  <tr>
   <td><strong>Configuraties op toegangsniveau</strong>
   </td>
   <td>U moet een Workfront-beheerder zijn. Voor informatie over Workfront-beheerders raadpleegt u <strong>Volledige administratieve toegang verlenen aan een gebruiker</strong>.
   </td>
  </tr>
</table>


*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.


## Integratie instellen

1. Klik op de knop **Hoofdmenu** in de rechterbovenhoek van Adobe Workfront en klik vervolgens op **Instellen**.
1. Selecteren  **Documenten** ![documentpictogram](assets/document-icon.png) in het linkerdeelvenster selecteert u vervolgens **Experience Manager-integratie**.
1. Selecteren **Integratie van Experience Manager toevoegen**.
1. Geef het volgende op:

   <table>
   <tr>
      <td><strong>Naam</strong>
      </td>
      <td>Voer de naam in die gebruikers moeten zien in de knop Nieuwe toevoegen in het gebied Documenten.
      </td>
   </tr>
   <tr>
      <td><strong>Navigatie-URL</strong>
      </td>
      <td>De navigatie-URL wordt automatisch door het systeem gevuld. Deze URL wordt gebruikt om via het hoofdmenu een koppeling te maken naar het Assets Essentials-exemplaar van uw organisatie, zodat u deze snel kunt openen.
      </td>
   </tr>
   <tr>
      <td>
      <strong>Experience Manager Assets-opslagplaats</strong>
      </td>
      <td>
      Het systeem vult automatisch de opslagplaats voor Experience Managers in die aan uw organisatie-id is gekoppeld.
      </td>
   </tr>
   </table>

1. Klikken **Opslaan** of ga naar de [Metagegevens instellen (optioneel)](#set-up-metadata-optional) in dit artikel.


## Metagegevens instellen (optioneel)

Workfront-objectgegevens toewijzen aan middelenmediavelden in Experience Manager Assets. Metagegevens worden toegewezen wanneer een element voor het eerst vanuit Workfront wordt geduwd.


### Vereisten

Voordat u begint, moet u

* Een metagegevensschema configureren in Experience Manager Assets Essentials, zoals wordt uitgelegd in [Metagegevenstoewijzing tussen Adobe Workfront en Experience Manager Assets configureren](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
* (Optioneel) Configureer aangepaste formuliervelden in Workfront. Workfront heeft veel ingebouwde aangepaste velden die u kunt gebruiken. U kunt echter ook uw eigen aangepaste velden maken. Zie voor meer informatie [Een aangepast formulier maken of bewerken](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).


### Activa

Metagegevens worden toegewezen wanneer een element voor het eerst vanuit Workfront wordt geduwd. Documenten met de ingebouwde of aangepaste velden worden automatisch toegewezen aan de opgegeven velden wanneer een element voor het eerst wordt verzonden naar Experience Manager Assets Essentials.

1. In de **Workfront-veld** kiest u een ingebouwd of aangepast Workfront-veld.
   >[!NOTE]
   >
   >U kunt ????n Workfront-veld toewijzen aan meerdere Experience Manager Assets-velden. U kunt niet meerdere Workfront-velden toewijzen aan ????n Experience Manager Assets-veld.
1. In de **Experience Manager** een Experience Manager Assets-veld kiezen.
1. Herhaal stap 1 en 2 zo nodig.
   ![metagegevens inschakelen](assets/metadata-assets-essentials.png)
1. Klikken **Opslaan** of ga naar de [Gekoppelde mappen instellen (optioneel)](#set-up-linked-folders-optional) in dit artikel.


## Gekoppelde mappen instellen (optioneel)

{{setup-linked-folder}}
