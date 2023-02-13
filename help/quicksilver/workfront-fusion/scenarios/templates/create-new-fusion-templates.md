---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Nieuwe sjablonen maken in [!DNL Adobe Workfront Fusion]
description: U kunt nieuwe scenario-sjablonen maken in [!DNL Adobe] Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# Nieuwe sjablonen maken in [!DNL Adobe Workfront Fusion]

U kunt nieuwe scenario-sjablonen maken in [!DNL Adobe] Workfront Fusion.

>[!TIP]
>
>Voordat u een nieuwe sjabloon maakt, kunt u de opdracht [!UICONTROL Public templates] om ervoor te zorgen dat de sjabloon die u wilt maken, nog niet beschikbaar is.

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] of hoger</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licentie**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p><p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Een nieuwe sjabloon maken

1. Klikken **[!UICONTROL Templates]** ![](assets/fusion-template-icon.png) in het linkernavigatievenster.
1. Klikken **[!UICONTROL Create a new template]** in de rechterbovenhoek.
1. (Optioneel) Wijzig de naam van de sjabloon door de standaardnaam te vervangen **[!UICONTROL New template name]** in de linkerbovenhoek.
1. (Optioneel) Als u de taal van de sjabloon wilt wijzigen, klikt u op **[!UICONTROL Set up a template]** ![](assets/fusion-scenario-settings-icon.png) en selecteert u de taal in het keuzemenu Taal.

   >[!IMPORTANT]
   >
   >De taalselectie komt overeen met de talen die beschikbaar zijn in de systeeminstellingen en heeft alleen betrekking op de naam van de openbare sjabloon en de beschrijving ervan. U kunt een sjabloontaal niet wijzigen nadat de sjabloon is opgeslagen.

1. (Optioneel) Als u een beschrijving van de sjabloon wilt invoeren, klikt u op **[!UICONTROL Set up a template]** ![](assets/fusion-scenario-settings-icon.png) en voert u de beschrijving in.
1. U kunt toepassingen, modules en gereedschappen op dezelfde manier toevoegen als wanneer u een standaardscenario maakt.

   Als u contextafhankelijke Help wilt toevoegen aan de modules, raadpleegt u [Instellen [!UICONTROL Wizard] functionaliteit](#set-up-wizard-functionality) in dit artikel.

   Voor meer informatie bij het bouwen van een scenario, zie [Een scenario maken in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >Als uw malplaatje modules omvat die vereisen toevoegend de verbinding, geloofsbrieven, of andere privacy-gevoelige informatie, wordt deze informatie niet gedeeld met de malplaatjegebruikers.

1. (Optioneel) Klik op **[!UICONTROL Run once]** om de sjabloon te testen.
1. Klik op de knop **[!UICONTROL Save]** pictogram ![](assets/save-icon.png).

>[!NOTE]
>
>Door uw sjabloon op te slaan maakt u deze zichtbaar voor al uw teamleden. Als u uw malplaatje buiten uw team toegankelijk wilt zijn moet u het publiceren en dan een gedeelde verbinding gebruiken, of uw beheerder vragen om het malplaatje goed te keuren en te publiceren.

## Instellen [!UICONTROL Wizard] functionaliteit {#set-up-wizard-functionality}

De [!DNL Workfront Fusion template] [!UICONTROL Wizard] Hiermee kunt u toekomstige gebruikers van de sjabloon instructies of informatie geven over de specifieke velden die in modules worden gebruikt.

1. Klik op de module die aan de sjabloon is toegevoegd om de velden van de module weer te geven.
1. Zoek het veld waaraan u wilt toevoegen [!UICONTROL Wizard] informatie en **[!UICONTROL Use in Wizard]** voor dat veld.
1. Voer de informatie die u voor gebruikers zichtbaar wilt maken in het dialoogvenster [!UICONTROL Help] veld.
1. (Optioneel) Schakel **[!UICONTROL Use as default value]**.
1. Herhaal stap 2-4 voor elk veld waarvoor u informatie wilt opgeven.
1. Klikken **[!UICONTROL OK]** om de wijzigingen op te slaan en de module te sluiten.
