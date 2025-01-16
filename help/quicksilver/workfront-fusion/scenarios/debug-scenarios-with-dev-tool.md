---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Foutopsporingsscenario's met Adobe Workfront Fusion Devtool
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1703'
ht-degree: 0%

---

# Foutopsporingsscenario&#39;s met het gereedschap [!DNL Adobe Workfront Fusion] Ontwikkelen

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ zuivert een scenario ](https://experienceleague.adobe.com/docs/workfront-fusion/using/manage-scenarios/debug-a-scenario.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

Met het gereedschap [!DNL Adobe Workfront Fusion] Ontwikkelen kunt u scenario&#39;s begrijpen en problemen oplossen. Met het gereedschap Ontwikkelen voegt u een extra deelvenster toe aan de [!DNL Chrome Developer Tools] . Gebruikend dit debugger paneel, kunt u alle handlooppas van uw scenario controleren, alle uitgevoerde verrichtingen herzien, en de details van elke uitgevoerde API vraag zien. U kunt zien welke module, verrichting, of enige reactie de fout veroorzaakte, en die kennis gebruiken om uw scenario te verfijnen.

>[!NOTE]
>
>Het registreren in het debugger paneel zal beperkt of niet beschikbaar voor vertrouwelijke scenario&#39;s, automatische uitvoeringen, en succesvolle verrichtingen zijn.

Ga voor een video-introductie en doorloop van het Fusion Devtool naar

* [ het Hulpmiddel van de Ontwikkeling van de Fusie ](https://video.tv.adobe.com/v/3427031/){target=_blank}.
* [ Devtool walkthrough ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/troubleshooting-and-error-handling/dev-tool-walkthrough.html)

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
   </td>    </tr> 
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

## Toegang krijgen tot Workfront Fusion Devtool

De toegang tot het gereedschap Ontwikkelen is afhankelijk van het feit of u Fusion gebruikt in de [!DNL Adobe Unified Experience] .

* [Heb toegang tot Devtool in  [!DNL Adobe Unified Experience]](#access-the-devtool-in-the-adobe-unified-experience)
* [Heb toegang tot Devtool in de klassieke  [!DNL Fusion]  ervaring](#access-the-devtool-in-the-classic-fusion-experience)

### Toegang tot het gereedschap Ontwikkelen in de [!DNL Adobe Unified Experience] of de nieuwe Fusion-ervaring

Als u Fusie in de Adobe verenigde Shell gebruikt, of aan de nieuwe ervaring van de Fusie bijgewerkt hebt, kunt u tot het Dev Hulpmiddel van de redacteur van het Scenario toegang hebben.

1. Klik het **hulpmiddel van de Helper** ![ Hulpmiddelen ](assets/debugger-icon.png) pictogram dichtbij de bodem van het scherm.

Of:

1. Ga naar de redacteur Scenario voor het scenario u wilt zuiveren.

   Om van de redacteur van het Scenario de plaats te bepalen, zie {de redacteur van 0} Scenario ](/help/quicksilver/workfront-fusion/scenarios/scenario-editor.md).[

1. Klik met de rechtermuisknop in een leeg gebied van de pagina (niet in een module).
1. Selecteer **Open Devtool**.

### Toegang tot het gereedschap Apparaat in de klassieke [!DNL Fusion] ervaring

Als u het gereedschap Ontwikkelen wilt gebruiken in de klassieke [!DNL Fusion] -ervaring, moet u een [!DNL Chrome] -extensie installeren. U kunt deze extensie vervolgens gebruiken via de [!DNL Chrome] Developer Tools.

* [Installeer installeer  [!DNL Chrome]  Devtool uitbreiding](#install-the-chrome-devtool-extension)
* [Bepaal de plaats van  [!DNL Workfront Fusion]  Devtool](#locate-the-workfront-fusion-devtool)

#### De extensie [!DNL Chrome] DeviceTool installeren

U kunt [!DNL Workfront Fusion] Devtool toevoegen aan [!DNL Chrome] via [!UICONTROL [!DNL Chrome] Web Store] .

1. Klik [ deze verbinding ](https://chromewebstore.google.com/u/1/detail/workfront-fusion-devtool/hkimbmkkmmejdnhbhoaefggkpkndfjnn) om naar [!DNL Workfront Fusion] Devtool op [!UICONTROL [!DNL Chrome] Web Store] te gaan.
1. Klik op **[!UICONTROL Add to [!DNL Chrome]]**.
1. Controleer de machtigingen in het venster dat wordt geopend. Klik op **[!UICONTROL Add Extension]** als u akkoord gaat met de machtigingen.

De extensie [!DNL Workfront Fusion] Device wordt toegevoegd aan uw [!DNL Chrome] -extensies.


#### Zoek het gereedschap [!DNL Workfront Fusion] Ontwikkelen

Om [!DNL Workfront Fusion] Devtool te gebruiken, moet u de [!DNL Workfront Fusion] Devtool uitbreiding aan uw [!DNL Chrome] browser toevoegen, zoals die in [ wordt beschreven installeer de uitbreiding van Chrome Devtool ](#install-the-chrome-Devtool-extension).

1. Open uw [!DNL Workfront Fusion] -scenario.
1. Openen [!DNL Chrome Developer Tools] :

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
   >We raden u aan [!DNL Chrome Developer Console] onderaan te koppelen om een betere weergave van uw modules te behouden.

1. Klik op de tab **[!DNL Workfront Fusion]** in [!DNL Chrome Dev Tools] .

## Het gereedschap [!DNL Workfront Fusion] Ontwikkelen gebruiken

Workfront Fusion Devtool bestaat uit drie hoofdsecties. Deze vindt u in het linkerdeelvenster van het venster Ontwikkelen.

* [ Levende Stroom ](#live-stream)
* [ Foutopsporing van het Scenario ](#scenario-debugger)
* [Gereedschappen](#tools)

### Live stream

Met Live stream kunt u zien wat er op de achtergrond gebeurt wanneer u eenmaal in uw scenario op Uitvoeren klikt.

1. Klik op het pictogram **[!UICONTROL Live Stream]** ![](assets/live-stream-icon.png) om de sectie Live stream te openen.
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
       </ul> <p>Klik op het desbetreffende tabblad in het rechterdeelvenster van het gereedschap [!DNL Workfront Fusion] Ontwikkelen om deze informatie weer te geven.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Verzoeken en antwoorden zoeken</p> </td> 
      <td> <p>Typ de zoekterm in het zoekveld in het linkerdeelvenster van het gereedschap [!DNL Workfront Fusion] Ontwikkelen om alleen aanvragen weer te geven die de zoekterm bevatten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Lijst met aanvragen verwijderen </p> </td> 
      <td> <p>Klik op het prullenbakpictogram in de rechterbovenhoek van het linkerdeelvenster van het apparaat om de lijst met verzoeken te wissen die is opgenomen in het gereedschap [!DNL Workfront Fusion] Ontwikkelen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Logboekregistratie voor console inschakelen</p> </td> 
      <td> <p>Klik op het computerpictogram <img src="assets/console-computer-icon.png"> in de rechterbovenhoek van het linkerdeelvenster van het apparaat.</p> <p>Aanmelden in de console wordt ingeschakeld wanneer het computerpictogram groen is.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>De aanvraag ophalen in de Raw JSON-indeling of cURL</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong> Ruwe JSON </strong> </p> <p>Klik op <strong>[!UICONTROL Copy RAW]</strong> in de rechterbovenhoek van het rechterdeelvenster van het gereedschap Ontwikkelen.</p> </li> 
        <li> <p><strong> cURL </strong> </p> <p>Klik op <strong>[!UICONTROL Copy cURL]</strong> in de rechterbovenhoek van het rechterdeelvenster van het gereedschap Ontwikkelen.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Scenario-foutopsporing

Scenario Debugger is nuttig voor complexere scenario&#39;s. Het toont de geschiedenis van de scenario looppas en laat u toe om modules door hun naam of identiteitskaart te zoeken.

1. Klik op het pictogram **[!UICONTROL Scenario Debugger]** ![](assets/scenario-debugger-icon.png) om Scenario Debugger te openen.
1. (Optioneel) Typ de zoekterm (naam of module-id) in het zoekveld in het linkerdeelvenster van [!DNL Workfront Fusion] Gereedschap ontwikkelen in de sectie [!UICONTROL Scenario Debugger] .
1. Dubbelklik op de naam van de module om de instellingen in de scenarioeditor te openen.
1. Bekijk aanvraagdetails door op de gewenste bewerking te klikken.

### Gereedschappen

In [!DNL Workfront Fusion] Devtool zijn gereedschappen beschikbaar waarmee u uw scenario gemakkelijker kunt instellen.

1. Klik op het pictogram **[!UICONTROL Tools]** ![](assets/console-tools-icon.png) om de gereedschappen te openen.
1. Selecteer het gewenste gereedschap
1. Configureer de velden zoals hieronder wordt beschreven.
1. Klik op **[!UICONTROL Run]**.

Gereedschappen en de bijbehorende velden:

* [ Focus een Module ](#focus-a-module)
* [ vind Modules door Afbeelding ](#find-modules-by-mapping)
* [ krijg Meta-gegevens van de App ](#get-app-metadata)
* [ Toewijzing van het Exemplaar ](#copy-mapping)
* [ de Filter van het Exemplaar ](#copy-filter)
* [ Verbinding van het Wisselen ](#swap-connection)
* [ Veranderlijke van het Wisselen ](#swap-variable)
* [ Wisselen App ](#swap-app)
* [ Basis 64 ](#base-64)
* [ Naam van de Module van het Exemplaar ](#copy-module-name)
* [ Remap Source ](#remap-source)
* [ Benadruk App ](#highlight-app)
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
   <td> <p> Bepaal de plaats van de veranderlijke pil die u van de module in uw scenario wilt vervangen en kopieer het aan dit ([!UICONTROL Variable to Find]) gebied. In het veld wordt de markering weergegeven met dubbele accolades. Voorbeeld: <code>&#123;&#123;5.value&#125;&#125;</code> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Replace With]</p> </td> 
   <td> <p>Bepaal de plaats van de veranderlijke pil die u de variabele met van de module in uw scenario wilt vervangen en het kopiëren aan dit ([!UICONTROL Variable to Find]) gebied. In het veld wordt de markering weergegeven met dubbele accolades. Voorbeeld: <code>&#123;&#123;5.value&#125;&#125;</code> .</p> </td> 
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
   <td> <p>Selecteer of u de gegevens van het [!UICONTROL Raw Data] gebied aan Base64 wilt coderen of Base64 aan Ruwe Gegevens decoderen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Raw Data]</p> </td> 
   <td> <p> Voer de gegevens in die u wilt coderen naar Base64 of Base64 als u wilt decoderen naar onbewerkte gegevens, afhankelijk van de optie die is geselecteerd in het bovenstaande veld [!UICONTROL Operation] .</p> </td> 
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

Dit gereedschap is vooral bedoeld om [!DNL Google Sheets] (verouderde) modules bij te werken naar de nieuwste [!DNL Google Sheets] -versie. Het voegt een nieuwe versie van de module net na de erfenisversie van de module in de scenario route toe.

Voor deze module hoeft u geen parameters in te stellen.
