---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: http-modules
title: HTTP &gt; een aanvraagmodule voor clientcertificaten maken
description: Dit [!DNL Adobe Workfront Fusion] kunt u een HTTP-aanvraag configureren met HTTP-clientcertificaatautorisatie en deze verzenden naar een server. De ontvangen HTTP-respons wordt vervolgens opgenomen in de uitvoerbundel.
author: Becky
feature: Workfront Fusion
exl-id: c0b0057f-3db0-4c10-a274-ebaec1a5b87b
source-git-commit: 45540ccc3b9fca98f8aaae86ac4d6574a067a6e4
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---

# HTTP >[!UICONTROL Make a Client Certificate Authorization request] module

>[!NOTE]
>
>Adobe Workfront Fusion vereist een [!DNL Adobe Workfront Fusion] naast een Adobe Workfront-licentie.

Dit [!DNL Adobe Workfront Fusion] kunt u een HTTP-aanvraag configureren met HTTP-clientcertificaatautorisatie en deze verzenden naar een server. De ontvangen HTTP-respons wordt vervolgens opgenomen in de uitvoerbundel.

>[!NOTE]
>
>Als u verbinding maakt met een product van de Adobe dat momenteel geen speciale aansluiting heeft, raden we u aan de Adobe Authenticator-module te gebruiken.
>
>Zie voor meer informatie [Adobe Authenticator-module](/help/quicksilver/workfront-fusion/apps-and-their-modules/adobe-authenticator-modules.md).

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

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!UICONTROL HTTP] >[!UICONTROL Make a Client Certificate Authorization request] moduleconfiguratie

Wanneer u vormt [!UICONTROL HTTP] >[!UICONTROL Make a Client Certificate Authorization request] module, [!DNL Adobe Workfront Fusion] geeft de onderstaande velden weer. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<img src="assets/map-toggle-350x74.png" style="width: 350;height: 74;" data-mc-conditions="QuicksilverOrClassic.Draft mode">

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Credentials]</td> 
   <td> <p>Selecteer de sleutel die de verificatiereferenties van uw clientcertificaat bevat of klik op <strong>[!UICONTROL Add]</strong> om uw referenties aan een nieuwe sleutel toe te voegen. </p> <p>Opmerking: u kunt meer referenties toevoegen om gemakkelijk tussen elke verbinding te kunnen schakelen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Evaluate all states as errors (except for 2xx and 3xx )] </td> 
   <td> <p>Gebruik deze optie om foutafhandeling in te stellen.</p> <p>Zie voor meer informatie <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Foutafhandeling in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Voer de URL in waarnaar u een aanvraag wilt verzenden, zoals een API-eindpunt, website, enzovoort.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers] </td> 
   <td> <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object. Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Voer de gewenste sleutel-waardeparen voor de query in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Body type]</p> </td> 
   <td> <p>De hoofdtekst van HTTP is de gegevensbytes die in een HTTP- transactiebericht onmiddellijk na de kopballen worden overgebracht als er om het even welk zijn om worden gebruikt.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>Het type Raw-hoofdtekst is over het algemeen geschikt voor de meeste HTTP-hoofdtekstaanvragen, zelfs in situaties waarin in de documentatie van de ontwikkelaar geen gegevens zijn opgegeven die moeten worden verzonden.</p> <p>Geef een vorm op voor het parseren van de gegevens in het dialoogvenster [!UICONTROL Content type] veld.</p> <p>Ondanks het geselecteerde inhoudstype, gaat de module gegevens in om het even welk formaat in dat door de ontwikkelaardocumentatie wordt bepaald of wordt vereist.</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>Dit lichaamstype is: [!UICONTROL POST] gegevens gebruiken <code>application/x-www-form-urlencoded</code>.</p> <p>Voor <code>[!UICONTROL application/x-www-form-urlencoded]</code>, is de hoofdtekst van het HTTP-bericht dat naar de server wordt verzonden, in wezen één queryreeks. De toetsen en waarden worden gecodeerd in sleutelwaardeparen, gescheiden door <code>&amp;</code> en met <code>=</code> tussen de toets en de waarde. </p> <p>Voor binaire gegevens, gebruik <code>[!UICONTROL multipart/form-data]</code> in plaats daarvan.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>Voorbeeld: </b></span></span> 
       <p>Voorbeeld van de resulterende HTTP-aanvraagindeling:</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>De [!UICONTROL Multipart/form-data] is een multipart HTTP-aanvraag die wordt gebruikt om bestanden en gegevens te verzenden. Het wordt doorgaans gebruikt om bestanden naar de server te uploaden.</p> <p>Voeg velden toe die in de aanvraag moeten worden verzonden. Elk veld moet een sleutelwaardepaar bevatten.</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Text]</strong> </p> <p>Voer de sleutel en waarde in die binnen de aanvraaginstantie moeten worden verzonden.</p> </li> 
       <li> <p><strong>[!UICONTROL File]</strong> </p> <p>Voer de sleutel in en geef het bronbestand op dat u wilt verzenden in de hoofdtekst van de aanvraag.</p> <p>Wijs het bestand toe dat u uit de vorige module wilt uploaden (bijvoorbeeld [!UICONTROL HTTP] &gt;[!UICONTROL Get a File] of [!UICONTROL Google Drive] &gt;[!UICONTROL Download a File)]of voer de bestandsnaam en de bestandsgegevens handmatig in.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Parse response]</p> </td> 
   <td> <p>Schakel deze optie in om reacties automatisch te parseren en JSON- en XML-reacties om te zetten zodat u deze niet hoeft te gebruiken [!UICONTROL JSON] &gt; [!UICONTROL Parse JSON] of [!UICONTROL XML] &gt; [!UICONTROL Parse XML] modules.</p> <p>Voordat u geparseerde JSON- of XML-inhoud kunt gebruiken, voert u de module één keer handmatig uit, zodat de module de inhoud van de reactie herkent en deze in volgende modules kunt toewijzen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timeout] </td> 
   <td> <p>Geef de time-out van het verzoek op in seconden (1-300). De standaardwaarde is 40 seconden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Share cookies with other HTTP modules]</td> 
   <td> <p> Schakel deze optie in om cookies van de server te delen met alle HTTP-modules in uw scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Self-signed certificate]</td> 
   <td> <p> Upload uw certificaat als u TLS wilt gebruiken met uw zelfondertekende certificaat.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reject connections that are using unverified (self-signed) certificates] </td> 
   <td> <p>Schakel deze optie in om verbindingen die niet-geverifieerde TLS-certificaten gebruiken, te weigeren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Follow redirect]</td> 
   <td> <p> Schakel deze optie in om de URL-omleidingen te volgen met 3xx-reacties.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Follow all redirects] </td> 
   <td> <p>Schakel deze optie in om de URL-omleidingen te volgen met alle antwoordcodes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Disable serialization of multiple same query string keys as arrays]</p> </td> 
   <td> <p>Standaard, [!DNL Workfront Fusion] Verwerkt meerdere waarden voor dezelfde URL-querytekenreeks-parametersleutel als arrays. Bijvoorbeeld: <code>www.test.com?foo=bar&amp;foo=baz</code> wordt omgezet in <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. Activeer deze optie om deze functie uit te schakelen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Request compressed content]</td> 
   <td> <p> Schakel deze optie in om een gecomprimeerde versie van de website aan te vragen.</p> <p>Hiermee voegt u een <code>[!UICONTROL Accept-Encoding]</code> om gecomprimeerde inhoud aan te vragen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Use Mutual TLS]</td> 
   <td> <p>Schakel deze optie in om Wederzijdse TLS te gebruiken in de HTTP-aanvraag.</p> <p>Zie voor meer informatie over wederzijdse TLS <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Gebruik wederzijds TLS in HTTP-modules in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
