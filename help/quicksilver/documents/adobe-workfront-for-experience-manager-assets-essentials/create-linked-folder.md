---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Een map maken die is gekoppeld met Experience Manager Assets of Assets Essentials
description: U kunt in Workfront een map maken die is gekoppeld met Experience Manager Assets of Assets Essentials.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: e9c6a01e80d34bc873c9a06ae0782dc65afb2445
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# Een map maken die is gekoppeld met Experience Manager Assets of Assets Essentials

U kunt in Workfront een map maken die is gekoppeld met Experience Manager Assets of Assets Essentials. Omdat de map is gekoppeld, worden alle aan de map toegevoegde middelen automatisch weergegeven in zowel Workfront als Experience Manager. U hoeft het middel niet handmatig te verzenden als het zich in een gekoppelde map bevindt.

Als een element wordt verwijderd of verplaatst uit een gekoppelde map in Experience Manager Assets of Assets Essentials, behoudt Workfront een kopie van het element in het gebied Project > Documenten.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben:

<table>
  <tr>
   <td><strong> plan* van Adobe Workfront </strong>
   </td>
   <td>Alle
   </td>
  </tr>
  <tr>
   <td><strong> Adobe Workfront vergunningen* </strong>
   </td>
   <td>Plan
   </td>
  </tr>
  <tr>
   <td><strong> Product </strong>
   </td>
   <td>U moet Experience Manager Assets as a Cloud Service of Assets Essentials hebben en u moet als gebruiker aan het product worden toegevoegd.
   </td>
  </tr>
  <tr>
   <td><strong> de toestemmingen van Experience Manager </strong>
   </td>
   <td>U moet schrijftoegang tot de bestemmingsomslag in de integratie van de Manager van de Ervaring hebben.
   </td>
  </tr>
  <tr>
   <td><strong> het niveauconfiguraties van de Toegang </strong>
   </td>
   <td>U moet een Workfront-beheerder zijn om een Experience Manager-integratie te configureren. Nadat het wordt gevormd, kunnen de gebruikers met een vergunning van het Plan opstelling verbonden omslagen op individuele projecten.
   </td>
  </tr>
</table>


*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

+++

## Vereisten

Voordat u begint,

* Uw Workfront-beheerder moet een Experience Manager-integratie configureren. Voor meer informatie, zie [ de integratie van Experience Manager Assets as a Cloud Service ](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) vormen of [ vormen de integratie van de Hoofdzaak van Experience Manager Assets ](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Een gekoppelde map maken

De gekoppelde map wordt gemaakt op de locatie die door de Workfront-beheerder is opgegeven bij het instellen van de integratie. Elke integratie kan slechts één maplocatie voor gekoppelde mappen hebben.

De naam voor de gekoppelde map wordt automatisch gemaakt op basis van de Portfolio, het programma, het project waaraan de map is gekoppeld en kan niet worden gewijzigd. Als het project niet aan een Portfolio of Programma wordt geassocieerd, zal de verbonden omslag de projectnaam en de aanmaakdatum tonen.

>[!NOTE]
>
>U kunt geen nieuw document of proefdrukversie maken in een gekoppelde map.


Een gekoppelde map maken:

1. Ga naar het project waar u de omslag wilt.
1. Selecteer **toevoegen Nieuw**, dan ga naar de integratie van de Manager van de Ervaring uw beheerderopstelling.

   >[!NOTE]
   >
   >De Workfront-beheerder kan een willekeurige naam voor deze integratie kiezen, dus Experience Manager Assets of Assets Essentials wordt niet specifiek genoemd.

1. Selecteer **creeer verbonden omslag**. Het systeem maakt automatisch een map in Experience Manager op basis van de locatie die is opgegeven bij het instellen van de integratie.
   ![ creeer een verbonden omslag ](assets/linked-folder.png)
