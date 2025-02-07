---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Objecten vergelijken tussen omgevingen
description: U kunt objecten in verschillende omgevingen vergelijken om ervoor te zorgen dat uw pakketten voor milieubescherming de objecten bevatten die u nodig hebt.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 085b0f04-5a9c-49b9-86d7-2363731ee067
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# Objecten vergelijken tussen omgevingen

U kunt objecten vergelijken tussen omgevingen om ervoor te zorgen dat uw pakketten voor milieubescherming de objecten bevatten die u nodig hebt.

U selecteert de omgevingen en typen objecten die u wilt vergelijken. Workfront vergelijkt alle objecten van de geselecteerde typen in beide omgevingen en geeft gegevens weer met betrekking tot de objectverschillen.

## Toegangsvereisten

U moet het volgende hebben:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan </strong>
   </td>
   <td> Prime of Ultimate (alleen nieuwe abonnementen)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenties </strong>
   </td>
   <td> [!UICONTROL Standard]
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

## Vereisten

Uw organisatie moet op het bedrijfsplatform van de Adobe zijn om voorwerpen tussen milieu&#39;s te vergelijken.

## Een objectvergelijking genereren

1. Ga naar een omgeving waarin u een object wilt vergelijken.
1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Setup]** ![ pictogram van de Opstelling ](/help/_includes/assets/gear-icon-setup.png).
1. Selecteer **Systeem** in de linkernavigatie, dan selecteren **Bevordering van het Milieu**.
1. Klik **vergelijken milieu&#39;s** dichtbij de hoger-juiste hoek van het scherm.
1. Op het **milieu van Source** gebied, selecteer het milieu dat u het pakket binnen wilt creëren. Dit is het milieu dat u voorwerpen **van** kopieert.
1. Op het **milieu van het Doel** gebied, selecteer het milieu waar u het pakket wilt installeren. Dit is het milieu dat u voorwerpen **aan** kopieert.
1. In de **Voorwerpen om** gebied te vergelijken, selecteer de objecten types die u tussen milieu&#39;s wilt vergelijken.
1. Klik **produceren vergelijking** dichtbij de hoger-juiste hoek van het scherm.

   Het kan enige tijd duren om de vergelijking te genereren, afhankelijk van het aantal en de grootte van de vergeleken objecten.

## Objectvergelijking weergeven

Nadat de vergelijking is voltooid, wordt de vergelijking weergegeven.

De lijst bevat objecten van de geselecteerde type(n) die in de bronomgeving aanwezig zijn, of die objecten ontbreken in de doelomgeving en of er veldverschillen zijn tussen de twee.

>[!BEGINSHADEBOX]

![ het voorbeeld van de Vergelijking ](assets/environment-promotion-comparison.png)

In dit voorbeeld:

* De eerste regel toont een object dat aanwezig is in de doelomgeving, maar verschilt van de bronomgeving.
* De tweede regel toont een object dat zich in de doelomgeving bevindt en dat hetzelfde is als in de bronomgeving.
* De derde regel toont een object dat niet aanwezig is in de doelomgeving.

>[!ENDSHADEBOX]

Specifieke objectverschillen weergeven:

1. Klik het vergrootglaspictogram ![ vergelijken pictogram ](assets/compare-icon.png) in de lijn voor dat voorwerp.

   Er wordt een venster geopend met alle velden van dat object. verschillen zijn rood.

## Een pakket maken op basis van een objectvergelijking

U kunt een pakket rechtstreeks op basis van een objectvergelijking maken.

Voor instructies, zie [ een pakket van een objecten vergelijking ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-a-package-from-an-object-comparison) in artikel creëren of uitgeven een pakket van de milieubevordering.
