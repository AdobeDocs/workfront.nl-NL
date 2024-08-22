---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: De Experience Manager Assets Essentials Integration configureren
description: Sluit uw werk aan op uw inhoud in Experience Manager Assets Essentials.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '620'
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

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table>
  <tr>
   <td>[!DNL Adobe Workfront] plan
   </td>
   <td>Alle
   </td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] licentie
   </td>
   <td><p>Huidige: [!UICONTROL Plan]</p>
   <p>Nieuw: [!UICONTROL Standard]</p></td>
  </tr>
  <tr>
   <td>[!DNL Experience Manager] licentie
   </td>
   <td>[!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td>Product
   </td>
   <td>U moet beschikken over Experience Manager Assets Essentials en u moet als gebruiker aan het product in de Admin Console worden toegevoegd.
   </td>
  </tr>
  <tr>
   <td>Configuraties op toegangsniveau
   </td>
   <td>U moet een [!DNL Workfront] beheerder zijn.
   </td>
  </tr>
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Integratie instellen

{{step-1-to-setup}}

1. Selecteer **Documenten** ![ documentenpictogram ](assets/document-icon.png) in het linkerpaneel, dan de uitgezochte **Integratie van de Experience Manager**.
1. Selecteer **toevoegen de Integratie van de Experience Manager**.
1. Geef het volgende op:

   <table>
   <tr>
      <td><strong> Naam </strong>
      </td>
      <td>Voer de naam in die gebruikers moeten zien in de knop Nieuwe toevoegen in het gebied Documenten.
      </td>
   </tr>
   <tr>
      <td><strong> Navigatie URL </strong>
      </td>
      <td>De navigatie-URL wordt automatisch door het systeem gevuld. Deze URL wordt gebruikt om aan de instantie van de Assets Essentials van uw organisatie van het Belangrijkste Menu voor snelle toegang te verbinden.
      </td>
   </tr>
   <tr>
      <td>
      <strong> de bewaarplaats van Experience Manager Assets </strong>
      </td>
      <td>
      Het systeem vult automatisch de opslagplaats voor Experience Managers in die aan uw organisatie-id is gekoppeld.
      </td>
   </tr>
   </table>

1. Klik **sparen** of beweging op de [ Opgestelde meta-gegevens (facultatief) ](#set-up-metadata-optional) sectie in dit artikel.


## Metagegevens instellen (optioneel)

Wijs Workfront-objectgegevens toe aan middelenmediavelden in Experience Manager Assets. Metagegevens worden toegewezen wanneer een element voor het eerst vanuit Workfront wordt geduwd.


### Vereisten

Voordat u begint, moet u

* Vorm een meta-gegevensschema in de Hoofdzaak van Experience Manager Assets zoals die in [ wordt verklaard vormt activa meta-gegevensafbeelding tussen Adobe Workfront en Experience Manager Assets ](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
* (Optioneel) Configureer aangepaste formuliervelden in Workfront. Workfront heeft veel ingebouwde aangepaste velden die u kunt gebruiken. U kunt echter ook uw eigen aangepaste velden maken. Voor meer informatie, zie [ Ontwerp een vorm met de vormontwerper ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Ondersteunde velden voor Workfront en Experience Manager Assets

### AEM trefwoord

U kunt elk door Workfront ondersteund veld toewijzen aan een trefwoord in Experience Manager Assets Essentials.

Als u een veld aan een trefwoord wilt koppelen, selecteert u `xcm:keywords` in de vervolgkeuzelijst Experience Manager Assets-veld in het gebied voor metagegevenstoewijzing.

Als u meerdere tekstvelden met één regel wilt toewijzen aan trefwoorden, voert u een door komma&#39;s gescheiden lijst van de trefwoordwaarden in aan de Workfront-zijde van de metagegevenstoewijzing en `xcm:keywords` aan de Experience Manager Assets-zijde. Elke veldwaarde wordt toegewezen aan een afzonderlijk trefwoord. U kunt een berekend veld gebruiken om meerdere Workfront-velden te combineren tot één door komma&#39;s gescheiden tekstveld.

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=en).
-->


### Assets

Metagegevens worden toegewezen wanneer een element voor het eerst vanuit Workfront wordt geduwd. Documenten met de ingebouwde of aangepaste velden worden automatisch toegewezen aan de opgegeven velden wanneer een element voor het eerst wordt verzonden naar Experience Manager Assets Essentials.

1. Op het **gebied van Workfront** kolom, kies een ingebouwd of gebied van douaneWorkfront.

   >[!NOTE]
   >
   >U kunt één Workfront-veld toewijzen aan meerdere Experience Manager Assets-velden. U kunt niet meerdere Workfront-velden toewijzen aan één Experience Manager Assets-veld.

1. Op het **Experience Manager** gebied, kies een gebied van Experience Manager Assets.

   Als u een Workfront-veld wilt toewijzen aan een Experience Manager Assets-tag, selecteert u `xcm:keywords` .

1. Herhaal stap 1 en 2 zo nodig.
   ![ laat meta-gegevens ](assets/metadata-assets-essentials.png) toe
1. Klik **sparen** of beweging op de [ Opstelling verbonden omslagen (facultatief) ](#set-up-linked-folders-optional) sectie in dit artikel.


## Gekoppelde mappen instellen (optioneel)

{{setup-linked-folder}}
