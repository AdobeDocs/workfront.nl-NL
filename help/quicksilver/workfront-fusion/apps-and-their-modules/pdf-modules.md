---
title: Adobe PDF Services
description: Adobe PDF Services
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: e0a5736b-dbdb-43c6-83ff-e88a5625a5bf
source-git-commit: ba161761acfc57e271f8593f534a5f7510187559
workflow-type: tm+mt
source-wordcount: '3222'
ht-degree: 0%

---

# [!DNL Adobe PDF Services]

Met de [!DNL Adobe Workfront Fusion] [!DNL Adobe PDF Services]kunt u gegevens uit een PDF-bestand extraheren of een nieuw PDF-bestand genereren op basis van de gegevens die u opgeeft. Daarnaast kunt u verschillende bestandstypen omzetten in PDF of PDF in andere bestandstypen. Met PDF Services kunt u ook metagegevens voor een PDF-bestand combineren, comprimeren of lezen, en wachtwoordbeveiliging voor het bestand instellen.

Als u instructies bij het creëren van een scenario nodig hebt, zie [Een scenario maken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Voor informatie over modules, zie [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

Voor informatie over API die voor de Diensten van PDF wordt gebruikt, zie [Adobe van API voor documentgeneratie](https://www.adobe.io/apis/documentcloud/dcsdk/doc-generation.html).

## Beveiligingsoverwegingen bij gebruik [!DNL Adobe PDF Services]

<!--

* [You do not need an [!DNL Adobe] account](#you-do-not-need-an-adobe-account) 
* [[!DNL Workfront Fusion] does not store your files](#workfront-fusion-does-not-store-your-files)

### You do not need an [!DNL Adobe] account 

Because [!DNL Workfront Fusion] is part of the [!DNL Adobe] product suite, you don't need a separate [!DNL Adobe] account to use these tools. Each tool accesses [!DNL Adobe] PDF functionality without using a connection.

Although [!DNL Workfront Fusion] does not require an [!DNL Adobe] account to use the PDF Services, the modules do require a connection. There are no credentials involved in this connection, and you provide only a name for the connection itself.

### [!DNL Workfront Fusion] does not store your files 

-->

De [!DNL Adobe PDF Services] kan uw bestanden lezen, converteren of wijzigen, maar geen van beide [!DNL Adobe] noch [!DNL Workfront Fusion] Sla uw bestanden of gegevens op. Dit betekent dat:

* U behoudt de controle over uw bestanden, inclusief de beveiliging ervan
* U hoeft geen [!UICONTROL Adobe] opslag- of cloudopslagaccount voor gebruik van de PDF Services.

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] of hoger</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige vergunningsvereiste: Neen [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
   </td> 
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

## Vereisten

Als u een OAuth Server-to-Server wilt maken, moet u de Adobe PDF Services API toevoegen in uw Adobe Developers Console. Selecteer bij het toevoegen van de API de optie OAuth Server-to-Server.

Zie voor instructies [API aan project toevoegen gebruikend OAuth](https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/) In de documentatie van de ontwikkelaar van de Adobe.

## Verbinding maken met [!DNL Adobe PDF Services]

Als u een verbinding wilt maken voor uw [!DNL Adobe PDF Services] modules:

1. In alle [!DNL Adobe PDF Services] module, klikt u op **[!UICONTROL Add]** naast het vak Verbinding.

1. Vul de volgende velden in:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Connection type]</td>
          <td>
            <p>Selecteer of u een server-aan-server verbinding of een verbinding wilt tot stand brengen JWT.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Connection name]</td>
          <td>
            <p>Voer een naam in voor deze verbinding.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client ID]</td>
          <td>Voer uw [!DNL Adobe] [!UICONTROL Client ID]. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].<p>Zie voor instructies over het zoeken naar referenties <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Credentials</a> in de Adobe Developer documentation.</p></td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]</td>
          <td>Voer uw [!DNL Adobe] [!UICONTROL Client Secret]. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].<p>Zie voor instructies over het zoeken naar referenties <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Credentials</a> in de Adobe Developer documentation.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Technical account ID] (alleen JWT)</td>
          <td>Voer uw [!DNL Adobe] [!UICONTROL Technical account ID]. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].<p>Zie voor instructies over het zoeken naar referenties <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Credentials</a> in de Adobe Developer documentation.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Organization ID] (alleen JWT)</td>
          <td>Voer uw [!DNL Adobe] [!UICONTROL Organization ID]. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].<p>Zie voor instructies over het zoeken naar referenties <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Credentials</a> in de Adobe Developer documentation.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Meta scopes] (alleen JWT)</td>
          <td>
            Voer het metabereik in dat nodig is voor de verbinding.
          </td>
        </tr>
       </tbody>
    </table>
1. Klikken **[!UICONTROL Continue]** om de verbinding op te slaan en terug te keren naar de module.


## [!DNL Adobe PDF Services] modules en hun velden

Wanneer u [!DNL PDF Services], [!DNL Workfront Fusion] geeft de onderstaande velden weer. Afhankelijk van factoren zoals uw toegangsniveau in de app of service, kunnen er naast deze velden mogelijk extra velden worden weergegeven. Een vetgedrukte titel in een module geeft een verplicht veld aan.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Generate document]](#generate-document)
* [[!UICONTROL Extract Text / Table]](#extract-text--table)
* [[!UICONTROL Combine PDF files]](#combine-pdf-files)
* [[!UICONTROL Compress PDF files]](#compress-pdf-files)
* [[!UICONTROL Convert document to PDF file]](#convert-document-to-pdf-file)
* [[!UICONTROL Convert HTML to PDF file]](#convert-html-to-pdf-file)
* [[!UICONTROL Convert image to PDF file]](#convert-image-to-pdf-file)
* [[!UICONTROL Convert PDF to document]](#convert-pdf-to-document)
* [[!UICONTROL Convert PDF to image]](#convert-pdf-to-image)
* [[!UICONTROL Linearize a PDF file]](#linearize-a-pdf-file)
* [[!UICONTROL OCR for PDF file]](#ocr-for-pdf-file)
* [[!UICONTROL Page manipulation]](#page-manipulation)
* [[!UICONTROL PDF accessibility auto-tag]](#pdf-accessibility-auto-tag)
* [[!UICONTROL PDF file properties]](#pdf-file-properties)
* [[!UICONTROL Protect PDF file]](#protect-pdf-file)
* [[!UICONTROL Remove protection of a PDF file]](#remove-protection-of-a-pdf-file)
* [Een PDF-bestand splitsen](#split-a-pdf-file)

### [!UICONTROL Generate document]

De [!UICONTROL Generate document] is een krachtige manier om een PDF te maken die gegevens bevat die u selecteert. U kunt het formatteren door te gebruiken [!DNL Microsoft Word] of door gegevens in JSON-indeling op te geven.

Voor meer informatie over de [!UICONTROL [!DNL Adobe PDF Services] Generate document] functionaliteit, zie [Overzicht van het genereren van documenten](https://www.adobe.io/apis/documentcloud/dcsdk/docs.html) in de [!DNL Adobe Document Services] documentatie.

* [Gebruik de [!UICONTROL Generate document] met een [!DNL Microsoft Word] template](#use-the-generate-document-module-with-a-microsoft-word-template)
* [Gebruik de [!UICONTROL Generate document] module met JSON](#use-the-generate-document-module-with-json)

#### Gebruik de [!UICONTROL Generate document] met een [!DNL Microsoft Word] template

<!--
>[!NOTE]
>
>For a discussion of Microsoft Word templates, see [Microsoft Word Template modules](../../workfront-fusion/apps-and-their-modules/microsoft-word-templates-modules.md). 
>
>You do not need to use Microsoft Word template modules to use a Microsoft Word template with the PDF Services Generate document module.
-->

Als u de opdracht [!UICONTROL Generate document] met een [!UICONTROL Microsoft Word] sjabloon, moet u eerst de sjabloon maken. Zoek naar &quot;Een sjabloon maken&quot; in het dialoogvenster [!DNL Microsoft Office] documentatie.

Vul de [!UICONTROL Generate document] Modulevelden als volgt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source File]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> <p>Dit bronbestand is het [!DNL Microsoft Word ]sjabloon die de module gebruikt om de nieuwe PDF te genereren.</p> <p>We raden u aan een project te maken in [!DNL Workfront] voor de [!DNL Microsoft Word] sjablonen die u gebruikt in [!DNL Workfront Fusion]. U kunt dan de [!DNL Workfront] &gt; [!UICONTROL Download document] om de aangewezen malplaatje in uw scenario te trekken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format]</td> 
   <td> <p>Selecteer de indeling voor het gegenereerde document.</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data for merge]</td> 
   <td> <p>Vul voor elke waardetag in de sjabloon die u door tekst wilt vervangen het volgende in:</p> 
    <ul> 
     <li> <p>[!UICONTROL Key]</p> <p>Voer een toets in. In de sjabloon is de sleutel de tekst die wordt weergegeven in de tag value. Als u bijvoorbeeld tekst wilt plaatsen in de tag value <code>&#123;&#123;name&#125;&#125;</code>, enter <code>name </code>in het sleutelveld.</p> </li> 
     <li> <p>Type waarde</p> <p>Selecteer of de gegevens in het waardeveld een waarde, een object of een array van objecten zijn.</p> </li> 
     <li> <p>[!UICONTROL Value]</p> <p>Typ of wijs de tekst toe die u in het gegenereerde document wilt weergeven in plaats van de waardetag.</p> </li> 
    </ul> <p> <img src="assets/generate-with-template-350x241.png" style="width: 350;height: 241;"> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Gebruik de [!UICONTROL Generate document] module met JSON

Als u de opdracht [!UICONTROL Generate document] Vul de velden als volgt in met JSON:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source File]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format]</td> 
   <td> <p>Selecteer de indeling voor het gegenereerde document.</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data for merge]</td> 
   <td> <p>Als u JSON in deze module wilt gebruiken, moet u de toewijzing in dit veld inschakelen.</p> <p>Typ of wijs de JSON toe waaruit u het document wilt genereren. </p> <p>U kunt JSON rechtstreeks in dit veld typen of JSON-uitvoer vanuit een JSON-module toewijzen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Extract Text / Table]

Met deze actiemodule kunt u gegevens uit een PDF-bestand extraheren. De module voert afzonderlijke tekstelementen uit, zoals een alinea of de tekst in één cel van een tabel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elements that should be extracted as JSON]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Text]</p> </li> 
     <li> <p>[!UICONTROL Tables]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Extract Bounding boxes?]</td> 
   <td>Schakel deze optie in om gegevens over het selectiekader van de tekst op te halen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include styling information for output?]</td> 
   <td>Schakel deze optie in om opmaakgegevens toe te voegen aan de uitvoer-JSON.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Combine PDF files]

Deze actiemodule neemt meerdere PDF-bestanden en combineert deze tot één PDF-bestand. In deze module kunnen bijvoorbeeld alle documenten in een [!UICONTROL Workfront] in één enkele PDF na voltooiing van het project.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documents]</td> 
   <td> <p>U kunt een aggregatormodule gebruiken om documenten te verzamelen die in een PDF moeten worden gecombineerd, of u kunt de documenten handmatig toevoegen. </p> <p>We raden u aan een [!UICONTROL Array Aggregator] aan gezamenlijke output van een vorige module. Door een aggregator te gebruiken, te hoeven u niet de namen, de plaatsen, of de aantallen dossiers te kennen om te combineren. Het gebruik van een aggregator is daarom veel flexibeler en schaalbaarder dan het handmatig invoeren van de te combineren documenten.</p> <p>Als u de opdracht [!UICONTROL Combine PDF] bestandsmodule met een aggregator, moet u toewijzing inschakelen op de [!UICONTROL Documents] veld. </p> <p>In dit voorbeeld wordt [!UICONTROL Read Related Records] identificeert documenten verbonden aan een project, en [!UICONTROL Download Documents] elke module wordt gedownload. Alle PDF worden geaggregeerd in een array die wordt doorgegeven aan de [!UICONTROL Combine PDF] bestandenmodule.</p> <p> <img src="assets/combine-example-350x104.png" style="width: 350;height: 104;"> </p> <p>U kunt documenten ook handmatig invoeren.</p> <p>Voor elk document dat in de gecombineerde PDF moet worden opgenomen:</p> 
    <ol> 
     <li value="1"> <p>Klikken [!UICONTROL Add a Document]</p> </li> 
     <li value="2"> <p>In de [!UICONTROL Source file] , selecteert u de module die het document uitvoert dat u wilt opnemen, of wijst u de naam en gegevens van het bronbestand toe. </p> </li> 
     <li value="3"> <p>(Optioneel) Als u alleen bepaalde pagina's uit het bronbestand wilt opnemen, klikt u voor elk paginabereik dat u wilt toevoegen op <strong>[!UICONTROL Add item]</strong> in de [!UICONTROL Pages] veld, voert u vervolgens de eerste en laatste pagina in van het paginabereik dat u wilt opnemen, en klikt u op <strong>[!UICONTROL Add]</strong>. U kunt meerdere paginabereiken uit één document opnemen.</p> </li> 
     <li value="4"> <p>Klik op <strong>[!UICONTROL Add]</strong>. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Compress PDF files]

Deze actiemodule maakt een PDF-bestand en comprimeert dit. Dit kan handig zijn om bandbreedte of geheugen te besparen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> <p>Het bronbestand moet de indeling PDF hebben. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compression level]</td> 
   <td>Selecteer het compressieniveau dat u wilt gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convert document to PDF file]

Met dit gereedschap wordt een document geconverteerd naar een PDF-bestand. Het bronbestand moet een van de volgende documentindelingen hebben:

* DOC
* XLS
* PPT
* TXT
* RTF

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> <p>Het bronbestand moet een van de volgende indelingen hebben:</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>XLS</p> </li> 
     <li> <p>PPT</p> </li> 
     <li> <p>TXT</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td> <p>Selecteer de standaardtaal voor het brondocument. Zo kan de module een geschikt lettertype selecteren als het bronbestand geen lettertype bevat.</p> <p>Selecteer een van de volgende talen:</p> 
    <ul> 
     <li> <p>en-US (Default): English (United States of America)</p> </li> 
     <li> <p>ca-ES: Catalaans (Spanje)</p> </li> 
     <li> <p>cs-CZ: Tsjechisch (Tsjechische Republiek)</p> </li> 
     <li> <p>DK: Deens (Denemarken)</p> </li> 
     <li> <p>de-DE: Duits (Duitsland)</p> </li> 
     <li> <p>en-AE: Engels (Verenigde Arabische Emiraten)</p> </li> 
     <li> <p>en-GB: Engels (Verenigd Koninkrijk)</p> </li> 
     <li> <p>en-IL: Engels (Israël)</p> </li> 
     <li> <p>en-US: Engels (Verenigde Staten van Amerika)</p> </li> 
     <li> <p>es-ES: Spaans (Spanje)</p> </li> 
     <li> <p>es-MX: Spaans (Mexico)</p> </li> 
     <li> <p>EU-ES: Baskisch (Spanje)</p> </li> 
     <li> <p>fi-FI: Fins (Finland)</p> </li> 
     <li> <p>fr-CA: Frans (Canada)</p> </li> 
     <li> <p>fr-FR: Frans (Frankrijk)</p> </li> 
     <li> <p>fr-MA: Frans (Marokko)</p> </li> 
     <li> <p>HR: Kroatisch (Kroatië)</p> </li> 
     <li> <p>hu-HU: Hongaars (Hongarije)</p> </li> 
     <li> <p>IT: Italiaans (Italië)</p> </li> 
     <li> <p>ja-JP: Japans (Japan)</p> </li> 
     <li> <p>kr-KR: Koreaans (Zuid-Korea)</p> </li> 
     <li> <p>nb-NO: Noors Bokmål (Noorwegen)</p> </li> 
     <li> <p>NL: Nederlands (Nederland)</p> </li> 
     <li> <p>pl-PL: Pools (Polen)</p> </li> 
     <li> <p>pt-BR: Portugees (Brazilië)</p> </li> 
     <li> <p>pt-PT: Portugees</p> </li> 
     <li> <p>RO: Roemeens (Roemenië)</p> </li> 
     <li> <p>Ru-RU: Russisch (Rusland)</p> </li> 
     <li> <p>sk-SK: Slowakije (Slowakije)</p> </li> 
     <li> <p>sl-SI: Slovenië (Slovenië)</p> </li> 
     <li> <p>sv-SE: Zweeds (Zweden)</p> </li> 
     <li> <p>tr-TR: Turks (Turkije)</p> </li> 
     <li> <p>uk-UA: Oekraïens (Oekraïne)</p> </li> 
     <li> <p>zh-CN: Chinees (continentaal China)</p> </li> 
     <li> <p>zh-TW: Chinees (Taiwan)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convert HTML to PDF file]

Met dit gereedschap wordt een HTML-bestand geconverteerd naar een PDF-bestand.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> <p>Belangrijk: bronbestand moet de HTML- of ZIP-indeling hebben. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON]</td> 
   <td> <p>Als uw HTML verwijst naar JavaScript-variabelen, kunt u deze variabelen hier opnemen. </p> <p>Voor elke variabele klikt u op <strong>[!UICONTROL Add item]</strong> en neemt de sleutel en de waarde van de variabele op.</p> <p>Opmerking:   
     <ul> 
      <li> <p>Wanneer u een PDF maakt van een ZIP-bestand, moet het bronelement een scriptelement bevatten, zoals: <code> &lt;script src='./json.js' type='text/javascript'&gt;&lt;/script&gt;</code> </p> </li> 
      <li> <p>Wanneer u een PDF maakt van een URL, wordt de inhoud van dit JSON-object in de browser-VM geïnjecteerd voordat de pagina wordt weergegeven. </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include header and footer]</td> 
   <td> <p>Schakel deze optie in om kop- en voetteksten te maken voor het PDF-document.</p> 
    <ul> 
     <li> <p>De koptekst bevat een datum en de documenttitel.</p> </li> 
     <li> <p>De voettekst bevat de bestandsnaam en een paginanummer.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Page width]</td> 
   <td>Voer de breedte van het papier in inches in. De module gebruikt deze informatie om de pagina's in het gemaakte PDF-bestand op te maken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Page height]</td> 
   <td>Voer de hoogte van het papier in inches in. De module gebruikt deze informatie om de pagina's in het gemaakte PDF-bestand op te maken.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convert image to PDF file]

Met dit gereedschap zet u een afbeelding om in een PDF-bestand.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en het afbeeldingsbestand van het bronbestand toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convert PDF to document]

Met dit gereedschap wordt een PDF-bestand geconverteerd naar een document. U kunt een van de volgende indelingen selecteren voor het uitvoerbestand.

* DOC
* DOCX
* PPTX
* XLSX
* RTF

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> <p>Het bronbestand moet de indeling PDF hebben. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Files Format]</td> 
   <td> <p>Selecteer de indeling waarin u de bestanden wilt uitvoeren:</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>DOCX</p> </li> 
     <li> <p>PPTX</p> </li> 
     <li> <p>XLSX</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convert PDF to image]

Met dit gereedschap zet u een PDF om in een afbeelding in de PNG- of JPEG-indeling. Dit wordt vervolgens uitgevoerd als een ZIP-bestand. De PDF wordt omgezet in één afbeelding per pagina en elke afbeelding eindigt met het paginanummer. De afbeeldingsbestanden worden vervolgens gecombineerd tot een ZIP-bestand.

Een bestand met de naam &#39;TestFile&#39; met 8 pagina&#39;s zou bijvoorbeeld 8 afbeeldingen produceren met de naam &#39;TestFile_1&#39; tot en met &#39;TestFile_8&#39;. De uitvoer van de module is een ZIP-bestand met de 8 afbeeldingen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> <p>Het bronbestand moet de indeling PDF hebben. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Files Format]</td> 
   <td> <p>Selecteer de indeling waarin u de bestanden wilt uitvoeren:</p> 
    <ul> 
     <li>PNG</li> 
     <li>JPEG</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Linearize a PDF file]

Met dit gereedschap lineariseert u een PDF-document om een voor het web geoptimaliseerd PDF-document te maken. Een gelineariseerd PDF-document kan per pagina worden weergegeven zonder dat het gehele document hoeft te worden gedownload.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL OCR for PDF file]

Met dit gereedschap wordt OCR (Optical Character Recognition) op een bestand uitgevoerd en wordt een PDF gemaakt.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL OCR type]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Modified original image] tekst zorgt ervoor dat de tekst doorzoekbaar en selecteerbaar is, maar wijzigt de oorspronkelijke afbeelding tijdens het opschoonproces (bijvoorbeeld het schuintrekken van de tekst) voordat een onzichtbare tekstlaag erop wordt geplaatst. Dit type verwijdert ongewenste artefacten en kan in sommige scenario's resulteren in een beter leesbaar document. </p> </li> 
     <li> <p>[!UICONTROL Unchanged original image] tekst bedekt ook een doorzoekbare tekstlaag boven de oorspronkelijke afbeelding, maar in dit geval blijft de oorspronkelijke afbeelding ongewijzigd. Met dit type krijgt u een maximale getrouwheid ten opzichte van de oorspronkelijke afbeelding.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td>Selecteer de taal van dit document.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Page manipulation]

In deze module kunt u pagina&#39;s in een PDF-document selectief roteren of verwijderen. U kunt bijvoorbeeld de staande weergave wijzigen in de liggende weergave of bepaalde pagina&#39;s uit het PDF-document verwijderen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td> <p>Selecteer de handeling die u op het bestand wilt uitvoeren.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Delete]</b> </p> <p>Selecteer deze optie als u pagina's uit het document wilt verwijderen.</p> </li> 
     <li> <p><b>[!UICONTROL Rotate]</b> </p> <p>Selecteer deze optie als u pagina's wilt roteren en voer vervolgens in graden rechtsom de hoek in die u de documentpagina's wilt roteren ten opzichte van de beginoriëntatie.</p> <p>Als u de pagina wilt roteren van Staand naar Liggend of andersom, roteert u de pagina 90 of 270 graden.</p> <p>Als een pagina ondersteboven is, roteert u deze 180 graden.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pages]</td> 
   <td> <p>Klik voor elk paginabereik dat u wilt verwijderen op <strong>[!UICONTROL Add]</strong> en voer vervolgens de eerste en laatste pagina van het paginabereik in. </p> <p>Opmerking:   
     <ul> 
      <li> <p>U kunt negatieve getallen gebruiken om terug te tellen vanaf het einde van het document. De laatste pagina van een document is -1, de tweede tot de laatste pagina is -2, enzovoort.</p> </li> 
      <li> <p>Als u één pagina wilt verwijderen, stelt u hetzelfde paginanummer in als het begin en het einde van het bereik.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module wilt werken met tijdens elke cyclus van de scenariouitvoering.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDF accessibility auto-tag]

In deze actiemodule wordt een PDF gemaakt die is gelabeld voor gebruik door toegankelijkheid. Het leidt ook tot een facultatief rapport van Microsoft Excel dat van problemen een lijst maakt en oplossingen voorstelt.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Shift Headings]</td> 
   <td> <p>Schakel deze optie in om koppen in het document te verplaatsen.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Generate Report]</b> </p> <p>Schakel deze optie in om een rapport te genereren met toegankelijkheidsproblemen in de PDF en hun locatie, en suggesties voor het oplossen van deze problemen.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDF file properties]

Dit hulpmiddel haalt basisinformatie over het document, zoals:

* Aantal pagina&#39;s
* PDF-versie
* Of het bestand is versleuteld
* Of het bestand lineair is
* Of het bestand ingesloten bestanden bevat

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Protect PDF file]

Met dit gereedschap beveiligt u een PDF-document met een gebruikers- of eigenaarwachtwoord. Er worden ook beperkingen ingesteld voor bepaalde functies, zoals afdrukken, bewerken en kopiëren in het PDF-document. U selecteert het type inhoud dat moet worden gecodeerd en het versleutelingsalgoritme.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> <p>Het bronbestand moet de indeling PDF hebben. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Password Protection Type]</td> 
   <td> <p>Schakel deze optie in als u wachtwoorden wilt gebruiken om het invoer-PDF-document te versleutelen. Als u deze optie inschakelt, moet u een waarde opgeven en invoeren voor een van de volgende opties of beide: </p> 
    <ul> 
     <li> <p>[!UICONTROL userPassword]</p> </li> 
     <li> <p>[!UICONTROL ownerPassword] </p> </li> 
    </ul> <p>Elk wachtwoord kan maximaal 128 tekens lang zijn.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encryption Algorithm]</td> 
   <td> <p>Selecteer het versleutelingsalgoritme. </p> 
    <ul> 
     <li> <p>[!UICONTROL AES-128 encryption]</p> <p>Het wachtwoord ondersteunt alleen LATIN-I-tekens. </p> </li> 
     <li> <p>[!UICONTROL AES-256 encryption]</p> <p>Het wachtwoord ondersteunt Unicode-tekenset</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content to Encrypt]</td> 
   <td> <p>Selecteer het type inhoud dat u wilt versleutelen.</p> 
    <ul> 
     <li> <p>[!UICONTROL All content]</p> </li> 
     <li> <p>[!UICONTROL All content except metadata]</p> </li> 
     <li> <p>[!UICONTROL Only embedded data] </p> </li> 
    </ul> <p>Selecteren "[!UICONTROL Only embedded data]" geeft alle verleende toegangsmachtigingen als ineffectief weer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Permissions]</td> 
   <td> <p>Selecteer de machtigingen die u wilt opnemen om het afdrukken, bewerken of kopiëren van inhoud toe te staan.</p> <p>Machtigingsinstellingen worden alleen gebruikt als de [!UICONTROL ownerPassword] wordt ingesteld in het dialoogvenster [!UICONTROL Password Protection Type] veld.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Remove protection of a PDF file]

Met dit gereedschap verwijdert u beveiliging (wachtwoordbeveiliging) uit een PDF-document.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> <p>Het bronbestand moet de indeling PDF hebben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Password]</td> 
   <td>Voer het wachtwoord in dat het bestand momenteel beveiligt.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Split a PDF file]

In deze actiemodule wordt een PDF-document in meerdere kleinere documenten gesplitst. U geeft op of het bestand moet worden gesplitst op basis van het aantal bestanden, pagina&#39;s per bestand of paginabereiken.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> <p>Het bronbestand moet de indeling PDF hebben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split option]</td> 
   <td>Selecteer hoe u het bestand wilt splitsen. 
   <ul>
   <li><p><b>Paginabereik</b></p><p>Voor elk paginabereik dat u in een afzonderlijk document wilt splitsen, klikt u op <b>Toevoegen</b> en voert u de pagina in waarop u wilt beginnen en de pagina waarop u wilt eindigen.</p></li>
   <li><p><b>Aantal pagina's</b></p><p>Voer het aantal pagina's in dat u in de nieuwe documenten wilt opnemen.</p></li>
   <li><p><b>Aantal bestanden</b></p><p>Voer het aantal bestanden van gelijke grootte in waarin u het document wilt splitsen.</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

## Een aangepaste API-aanroep maken

Deze actie module een verzoek van douaneHTTP aan de PDF Diensten API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecteer de verbinding die u voor deze module wilt gebruiken.</p> Voor instructies over het maken van een verbinding met [!DNL Adobe PDF Services], zie <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Verbinding maken met [!DNL Adobe PDF Services]</a> in dit artikel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> Voer een relatief pad of een URL in. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion voegt de machtigingsheaders automatisch toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Voeg de query voor de API-aanroep toe als een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td> <p>Voor elk gebied dat u aan de API vraag wilt toevoegen, klik <b>Item toevoegen</b> en voert u de sleutel en optionele waarde van het veld in.</p> <p>Opmerking:  <p>Bij het gebruik van voorwaardelijke instructies zoals <code>if</code> in uw JSON, plaats de aanhalingstekens buiten de voorwaardelijke verklaring.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

