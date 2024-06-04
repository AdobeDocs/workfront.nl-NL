---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Foutopsporingsscenario's met Adobe Workfront Fusion Devtool
description: Met Adobe Workfront Fusion Devtool kunt u scenario's begrijpen en problemen oplossen. Met het gereedschap Ontwikkelen voegt u een extra deelvenster toe aan Chrome Developer Tools. Gebruikend dit debugger paneel, kunt u alle handlooppas van uw scenario controleren, alle uitgevoerde verrichtingen herzien, en de details van elke uitgevoerde API vraag zien. U kunt zien welke module, verrichting, of enige reactie de fout veroorzaakte, en die kennis gebruiken om uw scenario te verfijnen.
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: 6edcb5b826bdcf37b62396a926c923875a3a1436
workflow-type: tm+mt
source-wordcount: '1700'
ht-degree: 0%

---

# Foutopsporingsscenario&#39;s met de [!DNL Adobe Workfront Fusion] Devtool

De [!DNL Adobe Workfront Fusion] Met Devtool kunt u scenario&#39;s begrijpen en problemen oplossen. Met het gereedschap Ontwikkelen voegt u een extra deelvenster toe aan het dialoogvenster [!DNL Chrome Developer Tools]. Gebruikend dit debugger paneel, kunt u alle handlooppas van uw scenario controleren, alle uitgevoerde verrichtingen herzien, en de details van elke uitgevoerde API vraag zien. U kunt zien welke module, verrichting, of enige reactie de fout veroorzaakte, en die kennis gebruiken om uw scenario te verfijnen.

>[!NOTE]
>
>Het registreren in het debugger paneel zal beperkt of niet beschikbaar voor vertrouwelijke scenario&#39;s, automatische uitvoeringen, en succesvolle verrichtingen zijn.

Ga voor een video-introductie en doorloop van het Fusion Devtool naar

* [Fusion Development Tool](https://video.tv.adobe.com/v/3427031/){target=_blank}.
* [Devtool doorloopt](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/troubleshooting-and-error-handling/dev-tool-walkthrough.html?lang=en)

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
   <p>Huidige vergunningsvereiste: Neen [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor arbeidsautomatisering en -integratie],  [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u beschikt over [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Vereisten voor verouderd product: uw organisatie moet het product kopen [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Toegang krijgen tot Workfront Fusion Devtool

De toegang tot het apparaat is afhankelijk van of u Fusion gebruikt in het dialoogvenster [!DNL Adobe Unified Experience].

* [Toegang tot het gereedschap Ontwikkelen in het dialoogvenster [!DNL Adobe Unified Experience]](#access-the-devtool-in-the-adobe-unified-experience)
* [Toegang tot het gereedschap Apparaat in de klassieke taal [!DNL Fusion] ervaring](#access-the-devtool-in-the-classic-fusion-experience)

### Toegang tot het gereedschap Ontwikkelen in het dialoogvenster [!DNL Adobe Unified Experience] of de nieuwe Fusion-ervaring

Als u Fusie in de Adobe verenigde Shell gebruikt, of aan de nieuwe ervaring van de Fusie bijgewerkt hebt, kunt u tot het Dev Hulpmiddel van de redacteur van het Scenario toegang hebben.

1. Klik op de knop **Helpgereedschappen** ![Helpgereedschappen](assets/debugger-icon.png) aan de onderkant van het scherm.

Of:

1. Ga naar de redacteur Scenario voor het scenario u wilt zuiveren.

   Ga voor de locatie van de Scenario-editor naar [Scenario-editor](/help/quicksilver/workfront-fusion/scenarios/scenario-editor.md).

1. Klik met de rechtermuisknop in een leeg gebied van de pagina (niet in een module).
1. Selecteren **Ontwikkelgereedschap openen**.

### Toegang tot het gereedschap Apparaat in de klassieke taal [!DNL Fusion] ervaring

Het gereedschap Ontwikkelen gebruiken in de klassieke [!DNL Fusion] ervaring, moet u een [!DNL Chrome] extensie. U kunt deze extensie vervolgens gebruiken vanuit het dialoogvenster [!DNL Chrome] Developer Tools.

* [Installeer het installatieprogramma [!DNL Chrome] Devtool-extensie](#install-the-chrome-devtool-extension)
* [Zoek de [!DNL Workfront Fusion] Devtool](#locate-the-workfront-fusion-devtool)

#### Installeer de [!DNL Chrome] Devtool-extensie

U kunt de [!DNL Workfront Fusion] Ontwikkelen naar [!DNL Chrome] via de [!UICONTROL [!DNL Chrome] Web Store].

1. Klikken [deze koppeling](https://chromewebstore.google.com/u/1/detail/workfront-fusion-devtool/hkimbmkkmmejdnhbhoaefggkpkndfjnn) om naar de [!DNL Workfront Fusion] Ontwikkelen op de [!UICONTROL [!DNL Chrome] Web Store].
1. Klik op **[!UICONTROL Add to [!DNL Chrome]]**.
1. Controleer de machtigingen in het venster dat wordt geopend. Als u akkoord gaat met de machtigingen, klikt u op **[!UICONTROL Add Extension]**.

De [!DNL Workfront Fusion] De extensie Devtool wordt toegevoegd aan uw [!DNL Chrome] extensies.


#### Zoek de [!DNL Workfront Fusion] Devtool

Als u de opdracht [!DNL Workfront Fusion] Ontwikkelen: u moet de opdracht [!DNL Workfront Fusion] Extensie Ontwikkelen voor uw [!DNL Chrome] browser, zoals beschreven in [De extensie Chrome Device installeren](#install-the-chrome-Devtool-extension).

1. Open uw [!DNL Workfront Fusion] scenario.
1. Openen [!DNL Chrome Developer Tools]:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Mac]</td> 
      <td>Command + Option + I</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Windows]</td> 
      <td> <p>Control + Shift + I</p> <p> of </p> <p>F12</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >We raden u aan de [!DNL Chrome Developer Console] onderaan om een betere mening van uw modules te handhaven.

1. Klik op de knop **[!DNL Workfront Fusion]** tab in [!DNL Chrome Dev Tools].

## Gebruik de [!DNL Workfront Fusion] Devtool

Workfront Fusion Devtool bestaat uit drie hoofdsecties. Deze vindt u in het linkerdeelvenster van het venster Ontwikkelen.

* [Live stream](#live-stream)
* [Scenario-foutopsporing](#scenario-debugger)
* [Gereedschappen](#tools)

### Live stream

Met Live stream kunt u zien wat er op de achtergrond gebeurt wanneer u eenmaal in uw scenario op Uitvoeren klikt.

1. Klik op de knop **[!UICONTROL Live Stream]** pictogram ![](assets/live-stream-icon.png) om de sectie Live stream te openen.
1. Voer een van de volgende handelingen uit:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Handeling</th> 
      <th>Instructies</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aanvraaggegevens weergeven</td> 
      <td> <p>U kunt de volgende informatie voor elke module in uw scenario bekijken</p> 
       <ul> 
        <li> <p>De Kopballen van het verzoek (API eindpunt URL, de methode van http, de tijd en de datum het verzoek werd geroepen, verzoekkopballen, en vraagkoord)</p> </li> 
        <li> <p>Indieningsinstantie</p> </li> 
        <li> <p>Antwoordheaders</p> </li> 
        <li> <p>Reactieorgaan</p> </li> 
       </ul> <p>Als u deze informatie wilt weergeven, klikt u op het desbetreffende tabblad in het rechterdeelvenster van het dialoogvenster [!DNL Workfront Fusion] Ontwikkelen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Verzoeken en antwoorden zoeken</p> </td> 
      <td> <p>Voer de zoekterm in het zoekveld in in het linkerdeelvenster van het dialoogvenster [!DNL Workfront Fusion] Ontwikkelen om alleen aanvragen weer te geven die de zoekterm bevatten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Lijst met aanvragen verwijderen </p> </td> 
      <td> <p>Klik op het prullenbakpictogram in de rechterbovenhoek van het linkerdeelvenster van het apparaat om de lijst met verzoeken te wissen die zijn opgenomen in het dialoogvenster [!DNL Workfront Fusion] Ontwikkelen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Logboekregistratie voor console inschakelen</p> </td> 
      <td> <p>Klik op het computerpictogram <img src="assets/console-computer-icon.png"> in de rechterbovenhoek van het linkerdeelvenster van het gereedschap Ontwikkelen.</p> <p>Aanmelden in de console wordt ingeschakeld wanneer het computerpictogram groen is.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>De aanvraag ophalen in de Raw JSON-indeling of cURL</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>Ruwe JSON</strong> </p> <p>Klikken <strong>[!UICONTROL Copy RAW]</strong> in de rechterbovenhoek van het rechterdeelvenster van het gereedschap Ontwikkelen.</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>Klikken <strong>[!UICONTROL Copy cURL]</strong> in de rechterbovenhoek van het rechterdeelvenster van het gereedschap Ontwikkelen.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Scenario-foutopsporing

Scenario Debugger is nuttig voor complexere scenario&#39;s. Het toont de geschiedenis van de scenario looppas en laat u toe om modules door hun naam of identiteitskaart te zoeken.

1. Klik op de knop **[!UICONTROL Scenario Debugger]** pictogram ![](assets/scenario-debugger-icon.png) om Scenario Debugger te openen.
1. (Optioneel) Voer de zoekterm (naam of module-id) in het zoekveld in het linkerdeelvenster van [!DNL Workfront Fusion] Ontwikkelen in het dialoogvenster [!UICONTROL Scenario Debugger] sectie.
1. Dubbelklik op de naam van de module om de instellingen in de scenarioeditor te openen.
1. Bekijk aanvraagdetails door op de gewenste bewerking te klikken.

### Gereedschappen

De [!DNL Workfront Fusion] Het apparaat is uitgerust met gereedschappen waarmee u uw scenario gemakkelijker kunt instellen.

1. Klik op de knop **[!UICONTROL Tools]** pictogram ![](assets/console-tools-icon.png) om de gereedschappen te openen.
1. Selecteer het gewenste gereedschap
1. Configureer de velden zoals hieronder wordt beschreven.
1. Klik op **[!UICONTROL Run]**.

Gereedschappen en de bijbehorende velden:

* [Een module activeren](#focus-a-module)
* [Modules zoeken op basis van toewijzing](#find-modules-by-mapping)
* [App-metagegevens ophalen](#get-app-metadata)
* [Toewijzing kopiëren](#copy-mapping)
* [Filter kopiëren](#copy-filter)
* [Verbinding wisselen](#swap-connection)
* [Variabele wisselen](#swap-variable)
* [App wisselen](#swap-app)
* [Basis 64](#base-64)
* [Naam module kopiëren](#copy-module-name)
* [Bron opnieuw toewijzen](#remap-source)
* [App markeren](#highlight-app)
* [GS migreren](#migrate-gs)

#### [!UICONTROL Focus a Module]

Hiermee opent u instellingen van de opgegeven module op ID.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Module ID]</td>
        <td>Voer de id in van de module waarvoor u instellingen wilt openen.</td>
    </tr>
</table>

#### [!UICONTROL Find Modules by Mapping]

Staat u toe om de waarden van modules voor een gespecificeerde termijn te zoeken. De output bevat IDs van modules die de termijn bevatten u naar hebt gezocht.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Keyword]</td> 
   <td> <p> Voer de term in waarnaar u wilt zoeken. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Use Only Values]</p> </td> 
   <td> <p>Schakel deze optie in als u alleen in de waarden van de modulevelden wilt zoeken.</p> <p>Schakel deze optie uit als u ook wilt zoeken in de namen van modulevelden.</p> <p>De zoekopdracht wordt uitgevoerd via de parameters name en label.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get App Metadata]

Hiermee worden metagegevens van de toepassing opgehaald op basis van de modulenaam of -id van de app. Dit is bijvoorbeeld handig wanneer u moet weten welke versie van de app in uw scenario wordt gebruikt.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Selecteer de module waarvoor u metagegevens wilt ophalen.</td>
    </tr>
</table>

#### [!UICONTROL Copy Mapping]

Hiermee kopieert u waarden uit de bronmodule naar de doelmodule.

>[!CAUTION]
>
>Zorg ervoor u de correcte bron en doelmodules plaatst. Als u een ander type module selecteert, worden de waarden in de doelmodule verwijderd.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Selecteer de module of voer de id in van de module waaruit u de veldwaarden wilt kopiëren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Selecteer de module of ga identiteitskaart van de module in waarin u de waarden van de bronmodule wilt opnemen.</p> <p>Belangrijk: waarden in de doelmodule worden overschreven.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copy Filter]

Hiermee kopieert u de filterinstellingen van de bronmodule naar de doelmodule.

>[!NOTE]
>
>De kopieeractie wordt uitgevoerd op het filter dat op de linkerkant van de geselecteerde module wordt geplaatst.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Selecteer de module of voer de id in van de module waaruit u filterwaarden wilt kopiëren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Selecteer de module of typ de id van de module waarin u de filterwaarden uit de bronmodule wilt invoegen.</p> <p>Belangrijk: waarden in de doelmodule worden overschreven.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Preserve Fallback Route setting]</p> </td> 
   <td> <p>De bronfilter wordt geplaatst als reserveroute. Schakel deze optie in om ook in te stellen dat het doelfilter is ingesteld als fallback-route.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Swap Connection]

Dupliceert een verbinding van de bronmodule aan elke module in het scenario van zelfde app.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Selecteer de module of voer de id in van de module waaruit u de verbinding wilt dupliceren.</td>
    </tr>
</table>

#### [!UICONTROL Swap Variable]

Zoekt naar opgegeven variabelen in het scenario en vervangt deze door een nieuwe variabele.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variable to Find]</td> 
   <td> <p> Zoek de variabele die u in uw scenario wilt vervangen en kopieer deze naar deze ([!UICONTROL Variable to Find]). In het veld wordt de markering weergegeven met dubbele accolades. Voorbeeld: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Replace With]</p> </td> 
   <td> <p>Zoek de variabele die u wilt vervangen door de variabele uit de module in uw scenario en kopieer deze naar deze ([!UICONTROL Variable to Find]). In het veld wordt de markering weergegeven met dubbele accolades. Voorbeeld: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module]</p> </td> 
   <td> <p>Selecteer de module waarin u de variabele wilt vervangen. Als geen module wordt geselecteerd, zal de variabele in het volledige scenario worden vervangen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Swap App]

Hiermee vervangt u de geselecteerde toepassingsversie in uw scenario door een andere toepassingsversie.

U kunt deze functie bijvoorbeeld gebruiken om de modules van Gmail- en E-mailapps te upgraden naar de meest recente versie.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL App to be Replaced]</td> 
   <td> <p> Selecteer de app die u wilt vervangen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Replace with]</p> </td> 
   <td> <p>Selecteer de app waarmee u deze wilt vervangen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Base 64]

Staat u toe om de ingegaan gegevens aan Base64 te coderen of Base64 te decoderen. Sommige verzoeken worden gecodeerd aan Base64. Dit hulpmiddel kan nuttig zijn wanneer u naar bepaalde gegevens in het gecodeerde verzoek wilt zoeken.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Operation] </td> 
   <td> <p>Selecteer of u de gegevens van wilt coderen [!UICONTROL Raw Data] veld naar Base64 of decoder Base64 naar Raw-gegevens.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Raw Data]</p> </td> 
   <td> <p> Voer de gegevens in die u wilt coderen naar Base64 of Base64 als u wilt decoderen naar onbewerkte gegevens, afhankelijk van de optie die in het dialoogvenster [!UICONTROL Operation] veld hierboven.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copy Module Name]

Hiermee kopieert u de naam van de geselecteerde module naar het klembord.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Module] </td> 
   <td> <p>Selecteer de module waarvan u de naam wilt kopiëren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remap Source]

Hiermee kunt u de toewijzingsbron wijzigen van de ene module in de andere.

U moet eerst de module toevoegen u als bronmodule aan de route in uw scenario wilt gebruiken.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module] </td> 
   <td> <p> Selecteer de module u als toewijzingsbron voor andere modules in uw scenario wilt worden vervangen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Selecteer de module die u als nieuwe toewijzingsbron wilt gebruiken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module to Edit]</p> </td> 
   <td> <p>Selecteer de module u de afbeelding voor wilt veranderen als u niet de afbeelding in het volledige scenario wilt veranderen. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Highlight App]

Hiermee worden de modules van de opgegeven app in uw scenario gemarkeerd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL App to be Highlighted] </td> 
   <td> <p> Selecteer de app die u wilt markeren in uw scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Version] </p> </td> 
   <td> <p>Selecteer de versie van de app die u wilt markeren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Highlight Color]</p> </td> 
   <td> <p> Voer de kleurhexadecimale kleur in die u voor markeringsmodules wilt gebruiken.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Migrate GS]

Dit gereedschap is speciaal bedoeld voor een upgrade [!DNL Google Sheets] (verouderde) modules tot de meest recente [!DNL Google Sheets] versie. Het voegt een nieuwe versie van de module net na de erfenisversie van de module in de scenario route toe.

Voor deze module hoeft u geen parameters in te stellen.
