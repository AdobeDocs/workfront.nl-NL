---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: De uitvoeringsgeschiedenis van een scenario weergeven in Adobe Workfront Fusion
description: U kunt informatie over alle looppas voor een scenario tonen, of u kunt alle uitvoeringen van het scenario voor specifieke gegevens zoeken.
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: 1b729960a23e43252bda16d9bfb7ca9656a115a1
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 0%

---

# De uitvoeringsgeschiedenis van een scenario weergeven in [!DNL Adobe Workfront Fusion]

U kunt informatie over alle looppas voor een scenario tonen, of u kunt alle uitvoeringen van het scenario voor specifieke gegevens zoeken.

De uitvoeringshistorie van een scenario toont alle executies van een scenario voor de laatste 30 dagen.

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
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor verouderde licentie: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie], [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u het [!UICONTROL Select] - of [!UICONTROL Prime] [!DNL Adobe Workfront] -abonnement hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Alle uitvoeringen van een scenario weergeven

### De uitvoeringshistorie van scenario&#39;s weergeven op de [!UICONTROL Scenario Detail] -pagina

1. Klik op de tab **[!UICONTROL Scenario]** in het linkerdeelvenster en klik vervolgens op het scenario.

   of

   Als u aan het scenario in de redacteur Scenario werkt, klik de linkerpijl ![](assets/exit-editing-arrow.png) dichtbij de upper-left hoek van het venster.

1. Bekijk de informatie in de lijst aan de rechterkant.

   U kunt ook klikken om een volledige paginaweergave van deze gegevens te bekijken. In de weergave van de volledige pagina kunt u de geschiedenis filteren om bepaalde uitvoeringen weer te geven.

   De volgende details zijn vermeld voor elke uitvoering van het scenario:

   * Datum waarop de bewerking is uitgevoerd **[!UICONTROL Started]**
   * **[!UICONTROL Status]** (geslaagd of mislukt)
   * Uitvoeren **[!UICONTROL Duration]**
   * Aantal **[!UICONTROL Operations]**
   * Grootte van **[!UICONTROL Data Transfer]**
   * Koppeling naar **[!UICONTROL Details]**

>[!NOTE]
>
>De scenario-geschiedenis toont a **badge van de a** Verwerking naast scenario&#39;s die onlangs hebben uitgevoerd, terwijl de uitvoeringsdetails aan opslag worden geschreven. De verwerking vindt onmiddellijk plaats nadat het scenario wordt uitgevoerd. en mag niet langer duren dan een paar minuten. Details van de uitvoering van het scenario zijn mogelijk niet zichtbaar terwijl de uitvoering wordt verwerkt.

### De uitvoeringshistorie van scenario&#39;s weergeven op het tabblad [!UICONTROL History]

Het tabblad [!UICONTROL History] bevat meer details dan beschikbaar zijn op de pagina van [!UICONTROL Scenario detail] . U kunt de uitvoeringen ook filteren en sorteren op het tabblad [!UICONTROL History] .

1. Klik op de tab **[!UICONTROL Scenario]** in het linkerdeelvenster en klik vervolgens op het scenario.

   of

   Als u aan het scenario in de redacteur Scenario werkt, klik de linkerpijl ![](assets/exit-editing-arrow.png) dichtbij de upper-left hoek van het venster.

1. Klik op de tab **[!UICONTROL History]** in de linkerbovenhoek van de pagina
1. (Optioneel) Klik op de koppeling **[!UICONTROL Details]** voor meer informatie over een geselecteerd scenario dat wordt uitgevoerd, inclusief de bundels die zijn verwerkt.

   Voor meer informatie bij verwerkingsbundels, zie [ de uitvoeringsstroom van het Scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >* De koppeling [!UICONTROL details] is alleen zichtbaar als er details beschikbaar zijn voor de uitvoering.
   >
   >* De de geschiedenisvertoningen van het scenario a **Verwerkingsgeschiedenis** badge naast scenario&#39;s die onlangs hebben uitgevoerd, terwijl de uitvoeringsdetails aan opslag worden geschreven. De verwerking vindt onmiddellijk plaats nadat het scenario wordt uitgevoerd. en mag niet langer duren dan een paar minuten. Details van de uitvoering van het scenario zijn mogelijk niet zichtbaar terwijl de uitvoering wordt verwerkt.

## De uitvoeringshistorie van het scenario filteren

U kunt de uitvoeringshistorie filteren om alleen uitvoeringen met de opgegeven waarden weer te geven.

1. Open de full-page geschiedenis voor een scenario zoals die in [ de uitvoeringshistorie van het scenario van de Mening op het [!UICONTROL History] lusje ](#view-scenario-execution-history-on-the-history-tab) in dit artikel wordt beschreven.
1. Klik op het pictogram [!UICONTROL filter] ![](assets/fusion-scenario-filter-icon.png) in de koptekst van de kolom waarop u wilt filteren.
1. Voer in het dialoogvenster [!UICONTROL filter] de waarden in waarop u wilt filteren.
1. Klik op **[!UICONTROL Save]**.

Het filterpictogram is oranje in kolommen met een momenteel actief filter.

## De uitvoeringshistorie van het scenario sorteren

U kunt de geschiedenis van de uitvoering van het scenario sorteren.

1. Open de full-page geschiedenis voor een scenario zoals die in [ de uitvoeringshistorie van het scenario van de Mening op het [!UICONTROL History] lusje ](#view-scenario-execution-history-on-the-history-tab) in dit artikel wordt beschreven.
1. Klik op het pictogram [!UICONTROL Sort] in de koptekst van de kolom waarop u wilt filteren.
1. Optioneel: klik nogmaals op het pictogram [!UICONTROL Sort] om de sorteervolgorde om te keren.

## Alle uitvoeringen van een scenario doorzoeken

1. Klik op het pictogram **[!UICONTROL Scenario]** ![](assets/scenarios-icon.png) in het linkerdeelvenster en klik vervolgens op het scenario.

   of

   Als u aan het scenario in de redacteur Scenario werkt, klik de linkerpijl ![](assets/exit-editing-arrow.png) dichtbij de upper-left hoek van het venster.

1. Klik op de tab **[!UICONTROL History]** in de linkerbovenhoek van het scherm.
1. Klik op **[!UICONTROL Fulltext search]** boven aan de lijst met uitvoeringen.

   of

   Het type **Ctrl+Shift+F** (Vensters) of **Cmd+Shift+F** (Mac)
Het venster [!UICONTROL Search in history] wordt geopend.

1. (Optioneel) Als u wilt zoeken naar uitvoeringen die specifieke tekst bevatten, voert u de tekst in de zoekbalk van het venster **[!UICONTROL Search in history]** in.

   Als u naar exacte tekst wilt zoeken, plaatst u dubbele aanhalingstekens in de tekst (&quot;voorbeeld&quot;).

   >[!INFO]
   >
   >**Voorbeeld:** als u de uitvoering wilt vinden die tot een specifiek project leidde, ga projectidentiteitskaart in de [!UICONTROL Fulltext search] bar in.
   >
   >&quot;625ef2ef006036bd1794b6e52d737c5&quot;

1. (Optioneel) Als u uw zoekopdracht wilt beperken tot een datumbereik, selecteert u de begin- en einddatum van de gewenste zoekopdracht in het gebied [!UICONTROL By date range] .

   >[!NOTE]
   >
   >* Uitvoeringen zijn alleen beschikbaar gedurende de afgelopen 30 dagen.
   >
   >* In [!DNL Workfront Fusion] worden de payloads van de webhaak 30 dagen opgeslagen. De toegang tot van een Web-haaklading meer dan 30 dagen nadat het werd gecreeerd resulteert in de fout &quot;[!UICONTROL Failed to read file from storage.]&quot;


1. (Optioneel) Als u uw zoekopdracht wilt beperken tot status, selecteert u de gewenste status in het vervolgkeuzemenu **[!UICONTROL By status]** .


   Beschikbare statussen zijn:

   * [!UICONTROL All]

   * [!UICONTROL Error]

   * [!UICONTROL Warning]

   * [!UICONTROL Success]

1. (Optioneel) Wijzig de volgorde die wordt weergegeven in de vervolgkeuzelijst **[!UICONTROL Sort by dates]** .

1. (Optioneel) Klik op het pictogram **[!UICONTROL Copy execution ID]** om een scenario-uitvoerings-id te kopiëren <img src="assets/copy-fusion-execution-id-icon.png"> in de rij van de gewenste uitvoering

1. (Optioneel) Klik op een resultaat van de [!UICONTROL Fulltext search] om de uitvoerbundel van de scenariomodule met de informatie te bekijken.
