---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: De integratie met Experience Manager Assets Essentials configureren
description: Sluit uw werk aan op uw inhoud in Experience Manager Assets Essentials.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: a729c134ce3d9c565fac18fea80ea7c49471182b
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 0%

---

# De integratie met Experience Manager Assets Essentials configureren

Sluit uw werk aan op uw inhoud in Experience Manager Assets Essentials &#x200B;:

* Elementen en metagegevens van Adobe Workfront naar Experience Manager Assets Essentials &#x200B;
* Elementen van Experience Manager Assets Essentials koppelen aan uw projecten en taken in Workfront &#x200B;
* Workflows voor versiebeheer vereenvoudigen voor middelen die naar Experience Manager Assets Essentials worden geduwd

>[!NOTE]
>
>U kunt ook verschillende Experience Manager Assets-opslagruimten verbinden met één Workfront-omgeving of met verschillende Workfront-omgevingen met één Experience Manager Assets-opslagplaats voor alle organisatie-id&#39;s. Volg de configuratieinstructies in dit artikel voor elke integratie u opstelling zou willen.

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
   <td>U moet een Workfront-beheerder zijn. Zie voor informatie over Workfront-beheerders <strong>Volledige administratieve toegang verlenen aan een gebruiker</strong>.
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
      <td>De navigatie-URL wordt automatisch door het systeem gevuld. Deze URL wordt gebruikt om aan de instantie van de Assets Essentials van uw organisatie van het Belangrijkste Menu voor snelle toegang te verbinden.
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

Wijs Workfront-objectgegevens toe aan middelenmediavelden in Experience Manager Assets. Metagegevens worden toegewezen wanneer een element voor het eerst vanuit Workfront wordt geduwd.


### Vereisten

Voordat u begint, moet u

* Een metagegevensschema configureren in Experience Manager Assets Essentials, zoals wordt uitgelegd in [Metagegevenstoewijzing tussen Adobe Workfront en Experience Manager Assets configureren](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
* (Optioneel) Configureer aangepaste formuliervelden in Workfront. Workfront heeft veel ingebouwde aangepaste velden die u kunt gebruiken. U kunt echter ook uw eigen aangepaste velden maken. Zie voor meer informatie [Een aangepast formulier maken of bewerken](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Ondersteunde velden voor Workfront en Experience Manager Assets

### AEM trefwoord

U kunt elk door Workfront ondersteund veld toewijzen aan een trefwoord in Experience Manager Assets Essentials.

Als u een veld wilt koppelen aan een trefwoord, selecteert u `xcm:keywords` in de vervolgkeuzelijst Experience Manager Assets-veld in het gebied voor metagegevenstoewijzing.

Als u meerdere tekstvelden met één regel wilt toewijzen aan trefwoorden, voert u een door komma&#39;s gescheiden lijst van de trefwoordwaarden in aan de Workfront-zijde van de metagegevenstoewijzing, en `xcm:keywords` aan de zijde van Experience Manager Assets. Elke veldwaarde wordt toegewezen aan een afzonderlijk trefwoord. U kunt een berekend veld gebruiken om meerdere Workfront-velden te combineren tot één door komma&#39;s gescheiden tekstveld.

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=en).
-->

+++


### Activa

Metagegevens worden toegewezen wanneer een element voor het eerst vanuit Workfront wordt geduwd. Documenten met de ingebouwde of aangepaste velden worden automatisch toegewezen aan de opgegeven velden wanneer een element voor het eerst wordt verzonden naar Experience Manager Assets Essentials.

1. In de **Workfront-veld** kiest u een ingebouwd of aangepast Workfront-veld.
   >[!NOTE]
   >
   >U kunt één Workfront-veld toewijzen aan meerdere Experience Manager Assets-velden. U kunt niet meerdere Workfront-velden toewijzen aan één Experience Manager Assets-veld.
1. In de **Experience Manager** een Experience Manager Assets-veld kiezen.

   Als u een Workfront-veld wilt toewijzen aan een Experience Manager Assets-tag, selecteert u `xcm:keywords`.
1. Herhaal stap 1 en 2 zo nodig.
   ![metagegevens inschakelen](assets/metadata-assets-essentials.png)
1. Klikken **Opslaan** of ga naar de [Gekoppelde mappen instellen (optioneel)](#set-up-linked-folders-optional) in dit artikel.


## Gekoppelde mappen instellen (optioneel)

{{setup-linked-folder}}
