---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Modules of scenario's kopiëren in [!DNL Adobe Workfront Fusion]
description: Modules of scenario's kopiëren in [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Modules of scenario&#39;s kopiëren in [!DNL Adobe Workfront Fusion]

U kunt modules, groepen modules, of volledige scenario&#39;s in kopiëren [!DNL Adobe Workfront Fusion]. Deze capaciteit staat u toe om scenario&#39;s of delen van scenario&#39;s opnieuw te gebruiken zonder het moeten hen opnieuw bouwen

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
  <td>
   <p>Huidige vergunningsvereiste: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor arbeidsautomatisering en -integratie],  [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereisten: Als u de [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Oudere productvereisten: Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

U moet modules aan een scenario toevoegen alvorens u hen kunt kopiëren.

## Een module of een groep modules kopiëren

Wanneer u een module kopieert, behoudt de kopie alle veldwaarden en instellingen van de originele module.

U kunt de module of modules in een ander gebied van het zelfde scenario, of in een verschillend scenario kleven.

Overweeg het volgende wanneer het kleven van modules in een verschillend scenario.

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* Veldwaarden die gegevens ophalen uit een andere module die u niet hebt gekopieerd, hebben geen toegang meer tot die gegevens. U moet deze gebieden plaatsen om informatie uit het nieuwe scenario te trekken.
* Als u de modules in een scenario kleeft dat door een ander team of een organisatie wordt bezeten, moeten alle verbindingen aan verbindingen worden bijgewerkt die door de groep of de organisatie worden bezeten die het nieuwe scenario bezit.

### Modules kopiëren

Het kopiëren van een groep modules is vergelijkbaar met het kopiëren van één module.

1. Klik met de rechtermuisknop op de module die u wilt kopiëren.

   >[!NOTE]
   >
   >U kunt meer dan één module selecteren door te houden [!UICONTROL shift] en klik op de modules die u wilt kopiëren. Het kopiëren van een groep modules kopieert ook om het even welke verbindende lijnen, filters, of het verpletteren van logica tussen hen.

1. Selecteren **[!UICONTROL Copy module]**.
1. Verplaats de curseur naar het gebied van het scenario waar u het exemplaar van het scenario wilt.
1. Klik met de rechtermuisknop en selecteer **[!UICONTROL Paste]**.
1. Sluit de geplakte modules aan op het scenario door deze naar de juiste locatie in het scenario te slepen.

   U kunt ook met sneltoetsen kopiëren en plakken.

## Een scenario kopiëren door klonen

Het klonen van een scenario leidt tot een exemplaar van het scenario, dat u dan kunt uitgeven.

1. Open de pagina met de details van het scenario:

   1. Klik op de knop **[!UICONTROL Scenario]** in het linkerpaneel, dan klik een scenario u details op zou willen.

      of

      Als u aan het scenario in werkt [De scenario-editor in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md), klikt u op de pijl naar links ![](assets/exit-editing-arrow.png) in de linkerbovenhoek van het venster.

1. Klikken met rechtermuisknop **[!UICONTROL Options]** rechtsboven op de pagina.
1. Selecteren **[!UICONTROL Clone]**.
1. (Optioneel) Voer een naam in voor het nieuwe scenario.
1. (Optioneel) Inschakelen **[!UICONTROL Keep the states of any new modules the same as those being duplicated]** om ervoor te zorgen dat het gekopieerde scenario ook informatie over de meest recente verslagen omvat die door het originele scenario worden verwerkt.
1. Klikken **[!UICONTROL Save]** om het scenario te maken.

## Een scenario kopiëren met behulp van blauwdrukken

Scenario-blauwdrukken vertegenwoordigen de rangschikking, toewijzing en veldwaarden van een bepaald scenario op een bepaald tijdstip. U kunt een scenario-blauwdruk naar een JSON-bestand op uw computer exporteren en het vervolgens importeren wanneer u een nieuw scenario maakt. Scenario&#39;s die uit een scenario-blauwdruk zijn geïmporteerd, kunnen worden bewerkt.

Een scenario blauwdruk vertegenwoordigt het volledige scenario. Als u slechts bepaalde modules van een scenario wilt kopiëren, zie [Een module of een groep modules kopiëren](#copy-a-module-or-a-group-of-modules) in dit artikel.

>[!NOTE]
>
>Voor informatie over blauwdrukken in de context van [!DNL Adobe Workfront], zie [Overzicht van blauwdrukken](../../administration-and-setup/blueprints/blueprints-overview.md).

### Een scenario-blauwdruk exporteren

1. Klik in het scenario op de knop **[!UICONTROL More]** in het gebied met scenario-instellingen.
1. Klik op **[!UICONTROL Export Blueprint]**.

   Er wordt een JSON-bestand gemaakt en gedownload naar de computer. U kunt dit bestand zoeken in uw [!DNL Downloads] map.

### Een blauwdruk importeren

>[!IMPORTANT]
>
>Als u een blauwdruk in een bestaand scenario invoert, vervangt het scenario blauwdruk het bestaande scenario. U kunt geen blauwdruk aan een bestaand scenario toevoegen.

1. Beginnen met het maken van een nieuw scenario.
1. Klik in het scenario op de knop **[!UICONTROL More]** in het gebied met scenario-instellingen.
1. Klik op **[!UICONTROL Import Blueprint]**.
1. Klik in het dialoogvenster dat wordt weergegeven op **[!UICONTROL Browse]**
1. Navigeer naar de blauwdruk die u wilt importeren en klik op **[!UICONTROL Open]**.
1. Klik op **[!UICONTROL Save]**.

   Er wordt een JSON-bestand gemaakt en gedownload naar de computer. U kunt dit bestand zoeken in uw [!UICONTROL Downloads] map.

## De scenario&#39;s van het exemplaar en hergebruik door malplaatjes te gebruiken

U kunt sjablonen maken als beginpunt voor uw [!DNL Workfront Fusion] scenario&#39;s. Wanneer u een scenario van een malplaatje creeert, kunt u het scenario wijzigen zonder het malplaatje te wijzigen. Veldwaarden worden niet opgeslagen in sjablonen.

Zie voor meer informatie over het maken en gebruiken van sjablonen [Scenario-sjablonen](../../workfront-fusion/scenarios/templates/fusion-templates.md).
