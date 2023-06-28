---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: AWS S3-modules
description: De [!DNL Adobe Workfront Fusion AWS] S3 modules laten u verrichtingen op uw S3 emmers uitvoeren.
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1254'
ht-degree: 0%

---

# AWS S3-modules

De [!DNL Adobe Workfront Fusion AWS] S3 modules laten u verrichtingen op uw S3 emmers uitvoeren.

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
   <p>Huidige vergunningsvereiste: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
   </td> 
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

Te gebruiken [!UICONTROL AWS S3] modules, moet u een [!DNL Amazon Web Service] account.

## Verbinden [!DNL AWS] tot [!DNL Workfront Fusion] {#connect-aws-to-workfront-fusion}

Verbinding maken [!DNL AWS S3] tot [!DNL Workfront Fusion] u moet verbinding maken met uw [!DNL AWS] account aan [!DNL Workfront Fusion]. Hiervoor moet u eerst een API-gebruiker maken in [!DNL AWS] [!UICONTROL IAM].

1. Aanmelden bij uw [!DNL AWS] [!UICONTROL IAM] account.
1. Ga naar **[!UICONTROL Identity and Access Management]** > **[!UICONTROL Access Management]** > **[!UICONTROL Users]**.

1. Klik op **[!UICONTROL Add User]**.
1. Voer de naam van de nieuwe gebruiker in en selecteer de **[!UICONTROL Programmatic access]** in de [!UICONTROL Access type] sectie.
1. Klikken **[!UICONTROL Attach existing policies directly]** en zoekt vervolgens naar **[!UICONTROL AmazonS3FullAccess]** in de zoekbalk. Klik op de knop wanneer deze wordt weergegeven en klik vervolgens op **[!UICONTROL Next]**.

1. Ga door de andere dialoogschermen te werk en klik vervolgens op **[!UICONTROL Create User]**.
1. Kopieer de opgegeven **[!UICONTROL Access key ID]** en **[!UICONTROL Secret access key]**.

1. Ga naar [!DNL Workfront Fusion] en opent u de [!DNL AWS S3] module **[!UICONTROL Create a connection]** .
1. Voer de [!UICONTROL Access key ID] en [!UICONTROL Secret access key] van stap 7 naar de desbetreffende velden en klik op **[!UICONTROL Continue]** om de verbinding tot stand te brengen.

De verbinding is tot stand gebracht. U kunt doorgaan met het instellen van de module.

## [!DNL AWS S3] modules en hun velden

Wanneer u [!DNL AWS S3] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL AWS S3] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Handelingen](#actions)
* [Zoekopdrachten](#searches)

### Handelingen

* [[!UICONTROL Create Bucket]](#create-bucket)
* [[!UICONTROL Get File]](#get-file)
* [[!UICONTROL Upload File]](#upload-file)
* [[!UICONTROL Make an API Call]](#make-an-api-call)

#### [!UICONTROL Create Bucket]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL AWS] account aan [!DNL Workfront Fusion], zie <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL AWS] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Voer de naam van het nieuwe emmertje in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Selecteer uw regionale eindpunt. Zie voor meer informatie de discussie over <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regionale eindpunten</a> in de documentatie van AWS.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get File]

Hiermee downloadt u een bestand van een emmertje.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL AWS] account aan [!DNL Workfront Fusion], zie <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL AWS] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Selecteer uw regionale eindpunt. Zie voor meer informatie de discussie over <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regionale eindpunten</a> in de [!DNL AWS] documentatie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Selecteer het emmertje waarvan u het bestand wilt downloaden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Path]</p> </td> 
   <td> <p>Voer het pad naar het bestand in. Voorbeeld: <code>/photos/2019/February/image023.jpg</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Upload File]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL AWS] account aan [!DNL Workfront Fusion], zie <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL AWS] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Selecteer uw regionale eindpunt. Zie voor meer informatie de discussie over <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regionale eindpunten</a> in de [!DNL AWS] documentatie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Folder] (optioneel) </p> </td> 
   <td> <p>Geef de doelmap op waarnaar u een bestand wilt uploaden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Headers] (optioneel)</p> </td> 
   <td> <p> Aanvraagkopteksten invoegen. Beschikbare kopteksten zijn te vinden in de <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">[!DNL AWS S3] documentatie - [!UICONTROL PUT] object</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Make an API Call]

Voor een uitvoerige bespreking van de [!DNL Amazon S3] API, zie [[!DNL Amazon S3] [!UICONTROL REST] API-introductie](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL AWS] account aan [!DNL Workfront Fusion], zie <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL AWS] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Region] </td> 
   <td> <p>Selecteer uw regionale eindpunt. Zie voor meer informatie de discussie over <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regionale eindpunten</a> in de [!DNL AWS] documentatie.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>URL Voer een host-URL in. Het pad moet relatief zijn ten opzichte van<code> https://s3.&lt;selected-region>.amazonaws.com/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Method]</td> 
   <td> <p>Selecteer [!UICONTROL HTTP] request method you need to configure the API call. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">[!UICONTROL HTTP] aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers]</td> 
   <td> <p>Voeg een aanvraagkoptekst toe. U kunt de volgende algemene aanvraagheaders gebruiken. Voor meer aanvraagheaders raadpleegt u <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">[!DNL AWS S3] API-documentatie</a>.</p> <p>[!DNL Workfront Fusion] voegt automatisch machtigingsheaders toe.</p> 
    <table style="table-layout:auto">
     <col> 
     <col> 
     <thead> 
      <tr> 
       <th>Naam koptekst</th> 
       <th> <p> Beschrijving</p> </th> 
      </tr> 
     </thead> 
     <tbody> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Length]</p> </td> 
       <td> <p>Lengte van het bericht (zonder de kopballen) volgens RFC 2616. Deze header is vereist voor [!UICONTROL PUT]s en verrichtingen die XML, zoals registreren en ACLs laden.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Type]</p> </td> 
       <td> <p>Het inhoudstype van de bron, voor het geval dat de aanvraaginhoud zich in de hoofdtekst bevindt. Voorbeeld: <code>text/plain</code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-MD5]</p> </td> 
       <td> <p>De base64 gecodeerde 128-bits MD5 samenvatting van het bericht (zonder de kopballen) volgens RFC 1864. Deze kopbal kan als controle van de berichtintegriteit worden gebruikt om te verifiëren dat de gegevens de zelfde gegevens zijn die oorspronkelijk werden verzonden. Hoewel dit optioneel is, raden we u aan de [!UICONTROL Content-MD5] mechanisme als integriteitscontrole van begin tot eind. Meer informatie over [!UICONTROL REST] aanvraagverificatie, ga naar <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">[!UICONTROL REST] Verificatie</a> in de <i>[!DNL Amazon] Simple Storage Service Developer Guide</i>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Date]</p> </td> 
       <td> <p>De huidige datum en tijd volgens de aanvrager. Voorbeeld: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. Wanneer u de <code>Authorization </code>header, moet u of <code>x-amz-date</code> of de <code>Date </code>header.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Expect]</p> </td> 
       <td> <p>Wanneer uw toepassing [!UICONTROL 100-continue], verzendt het de aanvraaginstantie pas nadat het een ontvangstbevestiging ontvangt. Als het bericht wordt verworpen gebaseerd op de kopballen, wordt het lichaam van het bericht niet verzonden. Deze koptekst kan alleen worden gebruikt als u een hoofdtekst verzendt.</p> <p>Geldige waarden: [!UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
       <td> <p>Voor padstijlverzoeken is de waarde <code>s3.amazonaws.com</code>. Voor aanvragen in virtuele stijl is de waarde <code>BucketName.s3.amazonaws.com</code>. Zie voor meer informatie <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">Virtueel hosten</a> in de <i>[!DNL Amazon] Simple Storage Service Developer Guide</i>.</p> <p>Deze header is vereist voor HTTP 1.1 (de meeste toolkits voegen deze header automatisch toe); optioneel voor HTTP/1.0-aanvragen.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>Wanneer het gebruiken van handtekeningsversie 4 om het verzoek voor authentiek te verklaren, verstrekt deze kopbal een knoeiboel van de verzoeklading. Wanneer u een object in blokken uploadt, stelt u de waarde in op <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> om aan te geven dat de handtekening alleen op kopteksten van toepassing is en dat er geen lading is. Zie voor meer informatie <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">Berekeningen van handtekening voor de machtigingsheader: Payload in meerdere blokken overbrengen (gesplitste bestanden uploaden) ([!DNL AWS] Handtekening versie 4)</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-date]</p> </td> 
       <td> <p>De huidige datum en tijd volgens de aanvrager. Voorbeeld: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. Wanneer u de <code>Authorization </code>header, moet u of <code>x-amz-date</code> of de <code>Date </code>header. Als u beide opgeeft, wordt de waarde opgegeven voor de <code>x-amz-date</code> header krijgt voorrang .</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>Deze kopbal kan in de volgende scenario's worden gebruikt:</p> 
        <ul> 
         <li>Beveiligingstokens opgeven voor [!DNL Amazon DevPay] bewerkingen. Elk verzoek dat gebruikt [!DNL Amazon DevPay] vereist twee <code>x-amz-security-token</code> kopteksten: één voor het productteken en één voor het gebruikerstoken. Wanneer [!DNL Amazon S3] ontvangt een voor authentiek verklaard verzoek, vergelijkt het de gegevens verwerkte handtekening met de verstrekte handtekening. Bij onjuist opgemaakte meerwaardekop voor het berekenen van een handtekening kunnen verificatieproblemen optreden.</li> 
         <li>Geef een beveiligingstoken op wanneer u tijdelijke beveiligingsreferenties gebruikt. Wanneer het maken van verzoeken gebruikend tijdelijke veiligheidsgeloofsbrieven u van IAM verwierf, moet u een veiligheidstoken verstrekken gebruikend deze kopbal. Ga voor meer informatie over tijdelijke beveiligingsreferenties naar Aanvragen indienen.</li> 
        </ul> <p>Deze header is vereist voor aanvragen die [!DNL Amazon DevPay] en aanvragen die zijn ondertekend met tijdelijke beveiligingsreferenties.</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query String]</td> 
   <td> <p>Voeg de gewenste querytekenreeksen toe, zoals parameters of formuliervelden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body]</td> 
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:   <p>Bij het gebruik van voorwaardelijke instructies zoals <code>if</code> in uw JSON, plaats de aanhalingstekens buiten de voorwaardelijke verklaring.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Zoekopdrachten

* [[!UICONTROL List Files]](#list-files)
* [[!UICONTROL List Folders]](#list-folders)

#### [!UICONTROL List Files]

Retourneert een lijst met bestanden van een opgegeven locatie.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL AWS] account aan [!DNL Workfront Fusion], zie <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL AWS] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Selecteer uw regionale eindpunt. Zie voor meer informatie de discussie over <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regionale eindpunten</a> in de [!DNL AWS] documentatie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Selecteer [!DNL Amazon S3] emmertje u naar dossiers wilt zoeken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix] (optioneel)</p> </td> 
   <td> <p> Pad naar een map waarin bestanden moeten worden opgezocht, bijvoorbeeld <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Folders]

Retourneert een lijst met mappen van een opgegeven locatie.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL AWS] account aan [!DNL Workfront Fusion], zie <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL AWS] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Selecteer uw regionale eindpunt. Zie voor meer informatie de discussie over <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regionale eindpunten</a> in de documentatie van AWS.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Selecteer [!DNL Amazon S3] emmertje dat u naar mappen wilt zoeken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix] (optioneel)</p> </td> 
   <td> <p> Pad naar een map om mappen in op te zoeken, bijvoorbeeld <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
