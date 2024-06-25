---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Photoshop-modules
description: Met de Adobe Photoshop-modules kunt u een Adobe Workfront Fusion-scenario starten op basis van gebeurtenissen in uw Adobe Photoshop-account, overeenkomsten en andere records maken, lezen of bijwerken, records zoeken aan de hand van criteria die u hebt ingesteld en documenten uploaden.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: f20192ea-e363-4fba-8bd2-b1d50443918d
source-git-commit: 6bcf404432129a812b5e4d840b59e72f036ec723
workflow-type: tm+mt
source-wordcount: '1317'
ht-degree: 0%

---

# [!DNL Adobe Photoshop] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL Adobe Photoshop]en deze verbinding maken met meerdere toepassingen en services van derden.


Als u instructies bij het creëren van een scenario nodig hebt, zie [Een scenario maken](../../workfront-fusion/scenarios/create-a-scenario.md).

Voor informatie over modules, zie [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
      <td>
        <p>[!UICONTROL Pro] of hoger</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licentie*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td>
      <td >
        <p>[!UICONTROL Workfront Fusion for Work Automation and Integration]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Product</td>
      <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;Neem contact op met uw [!DNL Workfront] beheerder.

&#42;&#42;Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Vereisten

Voordat u de [!DNL Adobe Photoshop] -aansluiting, moet u ervoor zorgen dat aan de volgende voorwaarden wordt voldaan:

* U moet een actieve [!DNL Adobe Photoshop] account.

## Verbinding maken met [!DNL Adobe Photoshop]

Als u een verbinding wilt maken voor uw [!DNL Adobe Photoshop] modules:

1. Klikken **[!UICONTROL Add]** naast het vak Verbinding.

1. Vul de volgende velden in:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>Voer een naam in voor deze verbinding.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Voer uw [!UICONTROL Adobe] [!UICONTROL Client ID]. Dit vindt u in het gedeelte [!UICONTROL Credentials] sectie details van de [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Voer uw [!DNL Adobe] [!UICONTROL Client Secret]. Dit vindt u in het gedeelte [!UICONTROL Credentials] sectie details van de [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Technical account ID]</td>
        <td>Voer uw [!DNL Adobe] [!UICONTROL Technical account ID]. Dit vindt u in het gedeelte [!UICONTROL Credentials] sectie details van de [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Organization ID]</td>
        <td>Voer uw [!DNL Adobe] [!UICONTROL Organization ID]. Dit vindt u in het gedeelte [!UICONTROL Credentials] sectie details van de [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Private key]</td>
        <td>
          <p>Voer de persoonlijke sleutel in die is gegenereerd toen uw referenties werden gemaakt in het dialoogvenster [!DNL Adobe Developer Console]. </p>
          <p>Uw persoonlijke sleutel of certificaat uitnemen:</p>
          <ol>
            <li value="1">
              <p>Klik op <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Selecteer het type bestand dat u extraheert.</p>
            </li>
            <li value="3">
              <p>Selecteer het bestand dat de persoonlijke sleutel of het certificaat bevat.</p>
            </li>
            <li value="4">
              <p>Voer het wachtwoord voor het bestand in.</p>
            </li>
            <li value="5">
              <p>Klikken <b>Opslaan</b> om het bestand uit te pakken en terug te keren naar[!UICONTROL ]e verbinding instellen.</p>
            </li>
          </ol>
        </td>
        </tr>
      </tbody>
    </table>

1. Klikken **[!UICONTROL Continue]** om de verbinding op te slaan en terug te keren naar de module.

## [!DNL Adobe Photoshop] modules en hun velden

Wanneer u [!DNL Adobe Photoshop] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Adobe Photoshop] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


### Handelingen

* [Een nieuwe PSD maken](#create-a-new-psd)
* [Tekstlagen bewerken](#edit-text-layers)
* [Diepte vervagen uitvoeren](#execute-depth-blur)
* [Photoshop-handelingen uitvoeren](#execute-photoshop-actions)
* [Uitsnijden van product uitvoeren](#execute-product-crop)
* [Laaginfo ophalen](#get-layer-info)
* [Een aangepaste API-aanroep maken](#make-a-custom-api-call)

#### Een nieuwe PSD maken

Deze actiemodule maakt een nieuwe PSD met optionele lagen en genereert uitvoeringen of slaat op als een PSD.

Voor velden die betrekking hebben op deze module, raadpleegt u [Een nieuwe PSD maken](https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/documentCreate) in de documentatie van Adobe Photoshop.

#### Tekstlagen bewerken

In deze actiemodule worden tekstlagen bewerkt in een Photoshop-bestand.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Photoshop], zie <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Verbinding maken met [!DNL Adobe Photoshop]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Selecteer de bestandsservice waarin het bestand dat u wilt bewerken is opgeslagen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Voer de URL of het pad in of wijs deze toe aan het bestand dat u wilt bewerken. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Manage missing fonts]</td>
      <td>
        <p>Selecteer de actie die u wilt uitvoeren als het document een of meer ontbrekende lettertypen bevat. Als het lettertype niet wordt opgegeven, gebruikt de module het standaardlettertype.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Default font]  </td>
      <td>
        <p>Voer de volledige postscriptnaam in van het lettertype dat als algemene standaardinstelling voor het document moet worden gebruikt. Dit lettertype wordt gebruikt voor alle tekstlagen met een ontbrekend lettertype en er is geen specifiek lettertype voor die laag opgegeven. Als dit lettertype ontbreekt, wordt de optie voor het beheren van ontbrekende lettertypen van kracht.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Layers]</td>
   <td> <p>Zie voor meer informatie over laagopties <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/text">Tekstlaag bewerken</a> in de documentatie van Adobe Photoshop.</p>  </td>     </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Output file storage]</td>
      <td>
        <p>Selecteer de bestandsservice waar het bewerkte bestand moet worden opgeslagen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file URL]</p>
      </td>
   <td> Voer de URL of het pad in of wijs deze toe waar het bewerkte bestand wordt opgeslagen. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file type]</p>
      </td>
   <td> Selecteer het bestandstype voor het bewerkte bestand. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Selecteer of het zojuist bewerkte bestand alle uitvoerbestanden overschrijft die al bestaan.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Selecteer het compressieniveau voor het uitvoerbestand. </td> 
    </tr>
  </tbody>
</table>

#### Diepte vervagen uitvoeren

Deze actiemodule voert Diepte vervagen op het geselecteerde bestand uit.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Photoshop], zie <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Verbinding maken met [!DNL Adobe Photoshop]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Selecteer de bestandsservice waarin het bestand dat u wilt bewerken is opgeslagen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Voer de URL of het pad in of wijs deze toe aan het bestand dat u wilt bewerken. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Output file storage]</td>
      <td>
        <p>Selecteer de bestandsservice waar het bewerkte bestand moet worden opgeslagen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file URL]</p>
      </td>
   <td> Voer de URL of het pad in of wijs deze toe waar het bewerkte bestand wordt opgeslagen. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file type]</p>
      </td>
   <td> Selecteer het bestandstype voor het bewerkte bestand. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Other fields]</td>
      <td>
        <p>Voor meer informatie over andere opties voor Diepte vervagen raadpleegt u <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/depthBlur">Diepte vervagen uitvoeren </a>in de Adobe Photoshop API-documentatie.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Selecteer of het zojuist bewerkte bestand alle uitvoerbestanden overschrijft die al bestaan.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Selecteer het compressieniveau voor het uitvoerbestand. </td> 
    </tr>
  </tbody>
</table>

#### Photoshop-handelingen uitvoeren

Deze actiemodule voert een Photoshop-actie uit op de geselecteerde afbeelding.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Photoshop], zie <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Verbinding maken met [!DNL Adobe Photoshop]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Selecteer de bestandsservice waarin het bestand dat u wilt bewerken is opgeslagen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Voer de URL of het pad in of wijs deze toe aan het bestand dat u wilt bewerken. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Actions file storage]</td>
      <td>
        <p>Selecteer de bestandsservice waarin het actiebestand is opgeslagen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Actions file URL]</p>
      </td>
   <td> Voer de URL of het pad van het actiebestand in of wijs deze toe. </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Action name]</p>
      </td>
   <td> Als u alleen een bepaalde handeling wilt uitvoeren, kunt u opgeven welke handeling in de ActionSet moet worden afgespeeld. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Font / Pattern / Brush storage]</td>
      <td>
        <p>Selecteer de bestandsservice waar het bestand dat u wilt gebruiken, is opgeslagen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Font / Pattern / Brush file URL]</p>
      </td>
   <td> Voer de URL of het pad in of wijs deze toe aan het bestand dat u wilt gebruiken. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Output file storage]</td>
      <td>
        <p>Selecteer de bestandsservice waar het bewerkte bestand moet worden opgeslagen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file URL]</p>
      </td>
   <td> Voer de URL of het pad in of wijs deze toe waar het bewerkte bestand wordt opgeslagen. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file type]</p>
      </td>
   <td> Selecteer het bestandstype voor het bewerkte bestand. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Selecteer of het zojuist bewerkte bestand alle uitvoerbestanden overschrijft die al bestaan.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Selecteer het compressieniveau voor het uitvoerbestand. </td> 
    </tr>
  </tbody>
</table>

#### Uitsnijden van product uitvoeren

Deze actiemodule voert het Uitsnijden van het Product op het geselecteerde beeld uit.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Photoshop], zie <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Verbinding maken met [!DNL Adobe Photoshop]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Selecteer de bestandsservice waar het bestand dat u wilt uitsnijden, is opgeslagen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Voer de URL of het pad in of wijs deze toe aan het bestand dat u wilt uitsnijden. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Unit]</p>
      </td>
   <td> Selecteer of u de hoogte- en breedteaanpassing wilt beschrijven in pixels of als een percentage. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Width]</p>
      </td>
   <td> Voer de hoeveelheid breedte-opvulling in die u wilt toevoegen of wijs deze toe. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Height]</p>
      </td>
   <td> Voer de hoeveelheid opvulling voor de hoogte in die u wilt toevoegen of wijs deze toe. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Output file storage]</td>
      <td>
        <p>Selecteer de bestandsservice waar het bewerkte bestand moet worden opgeslagen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file URL]</p>
      </td>
   <td> Voer de URL of het pad in of wijs deze toe waar het bewerkte bestand wordt opgeslagen. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file type]</p>
      </td>
   <td> Selecteer het bestandstype voor het bewerkte bestand. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Selecteer of het zojuist bewerkte bestand alle uitvoerbestanden overschrijft die al bestaan.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Selecteer het compressieniveau voor het uitvoerbestand. </td> 
    </tr>
  </tbody>
</table>

#### Laaginfo ophalen

Deze actiemodule wint laaginformatie van het gespecificeerde dossier van PSD terug.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Photoshop], zie <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Verbinding maken met [!DNL Adobe Photoshop]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Selecteer de bestandsservice waar het bestand waarvan u laaggegevens wilt ophalen, is opgeslagen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Typ of wijs de URL of het pad toe van het bestand waaruit u laaggegevens wilt ophalen. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Thumbnails]</p>
      </td>
   <td> </td> 
    </tr>
  </tbody>
</table>

#### Een aangepaste API-aanroep maken

Deze actiemodule maakt een aangepaste aanroep naar de Photoshop API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Photoshop], zie <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Verbinding maken met [!DNL Adobe Photoshop]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Een pad invoeren ten opzichte van <code>https://image.adobe.io/pie/psdService</code>. Voorbeeld: <code>/photoshopActions</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p>
        <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] voegt automatisch machtigingsheaders toe.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Voer de queryreeks voor de aanvraag in.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:  <p>Bij het gebruik van voorwaardelijke instructies zoals <code>if</code> in uw JSON, plaats de aanhalingstekens buiten de voorwaardelijke verklaring.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>
