---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Webhaken
description: Een webhaak is een HTTP-aanroep die door een gebeurtenis wordt geactiveerd. U kunt webhaken gebruiken om onmiddellijk triggermodules te activeren. Elke toepassing die is verbonden met internet en HTTP-aanvragen toestaat, kan webhooks naar Adobe Workfront Fusion verzenden.
author: Becky
feature: Workfront Fusion
exl-id: 987544a4-5840-40d4-9438-41a000aa22ee
source-git-commit: 34d7edb6a3f9cb1e818f6c234a8dda88d01c5fc4
workflow-type: tm+mt
source-wordcount: '1322'
ht-degree: 0%

---

# Webhaken



<!--This information moved to the webhooks article in the create scenarios folders in the new repo-->

Een webhaak is een HTTP-aanroep die door een gebeurtenis wordt geactiveerd. U kunt webhaken gebruiken om onmiddellijk triggermodules te activeren. Elke toepassing die is verbonden met internet en HTTP-aanvragen toestaat, kan webhooks naar Adobe Workfront Fusion verzenden.

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
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en integratie] </p>
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

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

&#42;&#42; voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Webhaak gebruiken in [!DNL Workfront Fusion]

>[!NOTE]
>
>Als u een webhaak van derden (een uitgaande webhaak) wilt aanroepen, gebruikt u een van de HTTP-modules. Voor meer informatie, zie [ modules van HTTP ](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

Een webhaak gebruiken om een app te verbinden met [!DNL Workfront Fusion] :

1. Voeg de **[!UICONTROL Webhooks]** > **[!UICONTROL Custom Webhook]** onmiddellijke trekkermodule aan uw scenario toe.

1. Klik op **[!UICONTROL Add]** naast het veld Webhaak en voer een naam voor de nieuwe webhaak in.
1. (Optioneel) Klik op **[!UICONTROL Advanced Settings]** .
1. Voer in het veld **[!UICONTROL IP restrictions]** een door komma&#39;s gescheiden lijst in met de IP-adressen waaruit de module gegevens kan accepteren.
1. Klikken **[!UICONTROL Save]**

Nadat u een webhaak hebt gemaakt, wordt een unieke URL weergegeven. Dit is het adres waar de webhaak gegevens verzendt. Workfront Fusion valideert de gegevens die naar dit adres worden verzonden en geeft deze vervolgens door voor verwerking in het scenario.

>[!NOTE]
>
>Als u een webhaak hebt gemaakt, kunt u deze in meerdere scenario&#39;s tegelijk gebruiken.

### De gegevensstructuur van de webhaak configureren {#configure-the-webhook-s-data-structure}

[!DNL Workfront Fusion] parseert voorbeeldgegevens die u naar het weergegeven adres verzendt om de gegevensstructuur van de inkomende lading te herkennen. U kunt de voorbeeldgegevens opgeven door een wijziging aan te brengen in de service of app die ervoor zorgt dat die service of toepassing de webhaak oproept. U kunt bijvoorbeeld een bestand verwijderen.

U kunt ook de onderstaande stappen volgen om de voorbeeldgegevens via de module [!UICONTROL HTTP] > [!UICONTROL Make a request] te verzenden.

1. Een nieuw scenario maken met de module **[!UICONTROL HTTP]** > **[!UICONTROL Make a request]**

1. Configureer de module met de volgende waarden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><p>[!UICONTROL URL] </p></td> 
      <td>Voer de URL van de webhaak in. U vindt deze URL in de module [!UICONTROL Webhooks] die u hebt gebruikt om de webhaak in te stellen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Method] </td> 
      <td><p>[!UICONTROL POST]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Body type]</td> 
      <td><p> [!UICONTROL Raw]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Content type]</td> 
      <td><p> JSON (application/json)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request content]</td> 
      <td><p>Ruwe JSON verwacht in de webhaak</p></td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-scenario-set-up-like-this-350x446.png)

1. Open het scenario met de module [!UICONTROL Webhooks] in een afzonderlijk browsertabblad of venster.
1. Klik in de module Webhooks op **[!UICONTROL Redetermine data structure]** .

   U hoeft andere modules niet los te koppelen van de module Webhooks.

1. Schakel over naar het scenario met de module [!UICONTROL HTTP] en voer het uit.
1. Schakel terug naar het scenario met de module Webhooks.

   Een &quot;[!UICONTROL Successfully determined]&quot;bericht betekent dat de module met succes de gegevensstructuur heeft bepaald.

   ![](assets/successfully-determined-350x175.png)

1. Klik op **[!UICONTROL OK]** om de gegevensstructuur op te slaan.

   De items van de webhaak zijn nu beschikbaar in het deelvenster Toewijzing voor gebruik met volgende modules in het scenario.

## De webshaakwachtrij

Als een website gegevens ontvangt en er geen actief scenario is dat dat gegevens verwacht, worden de gegevens opgeslagen in de rij. Zodra u het scenario activeert, verwerkt het alle bundels die in de rij opeenvolgend wachten.

>[!IMPORTANT]
>
>Webhaak-wachtrijen worden gedeeld door scenario&#39;s waarin dezelfde webhaak wordt gebruikt. Als één van de scenario&#39;s gehandicapt is, worden alle inkomende gegevens gehouden in de rij.

## Ondersteunde binnenkomende gegevensindelingen

[!DNL Workfront Fusion] ondersteunt 3 binnenkomende gegevensindelingen: [!UICONTROL Query String] , [!UICONTROL Form Data] en [!UICONTROL JSON] .

[!DNL Workfront Fusion] valideert alle binnenkomende gegevens op basis van de geselecteerde gegevensstructuur. Afhankelijk van de instellingen van het scenario worden de gegevens vervolgens in de wachtrij opgeslagen voor verwerking of onmiddellijk verwerkt.

Als een deel van de gegevens niet voor de validatie zorgt, retourneert [!DNL Workfront Fusion] een 400 HTTP-statuscode en wordt in de hoofdtekst van de HTTP-reactie aangegeven waarom de binnenkomende gegevens de validatiecontroles niet hebben doorstaan. Als de bevestiging van de inkomende gegevens slaagt, keert Workfront Fusion &quot;[!UICONTROL 200 Accepted]&quot;status terug.

* [[!UICONTROL Query String]](#query-string)
* [[!UICONTROL Form Data]](#form-data)
* [[!UICONTROL JSON]](#json)

### [!UICONTROL Query String]

```
GET https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>?name=<yourname>&job=automate
```

### [!UICONTROL Form Data]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/x-www-form-urlencoded

name=<yourname>&job=automate
```

#### Multipart-formuliergegevens

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>


Content-Type: multipart/form-data; boundary=---generatedboundary

---generatedboundary

Content-Disposition: form-data; name="file"; filename="file.txt"


Content-Type: text/plain


Content of file.txt


---generatedboundary

Content-Disposition: form-data; name="name"

Workfront Fusion

---generatedboundary
```

Als u bestanden wilt ontvangen die zijn gecodeerd met `multipart/form-data` , moet u een gegevensstructuur configureren met een `collection` tekstveld dat de geneste velden `name` , `mime` en `data` bevat. Het veld `name` is een `text` -type en bevat de naam van het geüploade bestand. `mime` is een `text` -type en bevat een bestand in de MIME-indeling. Het veld `data` is een `buffer` -type en bevat binaire gegevens voor het bestand dat wordt overgedragen.

Voor meer informatie over formaat MIME, zie [ MIME modules ](../../workfront-fusion/apps-and-their-modules/mime.md).

### [!UICONTROL JSON]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/json

{"name": "Workfront Fusion", "job": "automate"}
```

>[!TIP]
>
>Als u toegang wilt krijgen tot de oorspronkelijke JSON, schakelt u JSON-pass-through in wanneer u de webhaak instelt.
>
>1. Klik op **[!UICONTROL Add]** om een nieuwe webhaak toe te voegen.
>1. Klik op **[!UICONTROL Show advanced settings]**.
>1. Klik op **[!UICONTROL JSON pass-through]**.
>

## WebHaakkoppen

Als u de koppen van de webhaak wilt openen, schakelt u aanvraagheaders ophalen in wanneer u de webhaak instelt.

1. Klik op **[!UICONTROL Add]** om een nieuwe webhaak toe te voegen.
1. Klik op **[!UICONTROL Show advanced settings]**.
1. Klik op **[!UICONTROL Get request headers]**.

U kunt een bepaalde headerwaarde extraheren met de combinatie van `map()` - en `get()` -functies.

>[!INFO]
>
>**Voorbeeld:**
>
>In het onderstaande voorbeeld ziet u een formule die de waarde van de header `authorization` extraheert uit de array `Headers[]` . De formule wordt gebruikt in een filter dat de geëxtraheerde waarde met de gegeven tekst vergelijkt om slechts webhooks over te gaan als er een gelijke is.
>
>![](assets/set-up-a-filter-350x169.png)
>
>Voor verdere informatie bij het verkrijgen van het element van een serie met een bepaalde sleutel, zie [ het element van een serie met een bepaalde sleutel ](../../workfront-fusion/mapping/map-information-between-modules.md#mapping) in de artikel [ informatie van de Kaart van één module aan een andere in de Fusie van Adobe Workfront ](../../workfront-fusion/mapping/map-information-between-modules.md) in kaart brengen.

## Reageren op webhaken

De standaardreactie op een webshaanroep is de tekst &quot;Geaccepteerd&quot;. De reactie wordt geretourneerd aan de toepassing die de webhaak heeft aangeroepen tijdens de uitvoering van de aangepaste module Webhaak.

* [ Test de reactie op een webhaak ](#test-the-response-to-a-webhook)
* [ het voorbeeld van de Reactie van HTML ](#html-response-example)
* [Voorbeeld van omleiding](#redirect-example)

### De reactie op een webhaak testen

1. Neem de module **[!UICONTROL Custom Webhook]** op in uw scenario.
1. Voeg een nieuwe webhaak aan de module toe.
1. Kopieer de URL van de webhaak naar het klembord.
1. Voer het scenario uit.

   Het bliksempictogram in de module [!UICONTROL Custom Webhook] verandert in draaiende stippen. Dit toont aan dat de module nu op de webhaakvraag wacht.

1. Open een nieuw browservenster, plak de gekopieerde URL in de adresbalk en druk op **[!UICONTROL Enter]** .

   De module [!UICONTROL Custom Webhook] wordt geactiveerd en de browser geeft een nieuwe pagina weer.

Als u de reactie van de webhaak wilt aanpassen, gebruikt u de module Reactie Webhaak.

De configuratie van de module bevat twee velden: [!UICONTROL Status] en [!UICONTROL Body] .

* Het veld [!UICONTROL Status] bevat statuscodes voor HTTP-reacties, zoals 2xx voor succes (bijvoorbeeld `200` voor OK), 3xx voor Omleiding (bijvoorbeeld `307` voor Tijdelijke omleiding), 4xx voor Clientfouten (bijvoorbeeld `400` voor Onjuiste aanvraag), enzovoort.

* Het veld [!UICONTROL Body] bevat alles wat wordt geaccepteerd door de aanroep van de website. Het kan eenvoudige tekst zijn, HTML, XML, JSON enzovoort.

  >[!TIP]
  >
  >We raden u aan de header `Content-Type` in te stellen op het corresponderende MIME-type: `text/plain` voor onbewerkte tekst, `text/html` voor HTML, `application/json` voor JSON, `application/xml` voor XML enzovoort. Voor meer informatie over types MIME, zie [ MIME modules ](../../workfront-fusion/apps-and-their-modules/mime.md).

De time-out voor het verzenden van een reactie is 40 seconden. Als de reactie niet beschikbaar is binnen die periode, retourneert Workfront Fusion de status &#39;200 Accepted&#39;.

### HTML-voorbeeld

>[!INFO]
>
>**Voorbeeld:**
>
>Configureer de module [!UICONTROL Webhook Response] als volgt:
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Status] </td> 
&gt;   <td> <p>2xx de statuscode van succesHTTP, b.v. 200</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Body] </td> 
&gt;   <td> <p>HTML-code</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL Custom headers]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong> Sleutel </strong>: Inhoud-type</li> 
&gt;     <li><strong> Waarde </strong>: text/html</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/custom-headers-350x235.png)
>
>Hierdoor wordt een HTML-reactie gegenereerd die in een webbrowser wordt weergegeven:
>
>![](assets/html-response-350x70.png)

### Voorbeeld van omleiding

>[!INFO]
>
>**Voorbeeld:** vorm de [!UICONTROL Webhook Response] module als volgt:
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Status] </td> 
&gt;   <td> <p>3xx HTTP-statuscode voor omleiding, bijvoorbeeld 303</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL Custom headers]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>[!UICONTROL Key]</strong>: Locatie</li> 
&gt;     <li><strong>[!UICONTROL Value]</strong>: De URL waarnaar u wilt omleiden.</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/webhook-response-350x279.png)

## Webhaak-deactivering

Webhaken worden automatisch gedeactiveerd als een van de volgende twee situaties van toepassing is:

* De webhaak is langer dan 5 dagen niet verbonden met een scenario
* De webhaak wordt alleen gebruikt in inactieve scenario&#39;s, die al meer dan 30 dagen inactief zijn.

gedeactiveerde webhaken worden automatisch verwijderd en niet geregistreerd als ze niet zijn aangesloten op scenario&#39;s en meer dan 30 dagen in de gedeactiveerde status zijn geweest.


## Problemen oplossen

### Ontbrekende items in het deelvenster Toewijzing

Als sommige items ontbreken in het deelvenster Toewijzing tijdens het instellen van de modules na de module [!UICONTROL Webhooks] > [!UICONTROL Custom Webhook] , klikt u op de module **[!UICONTROL Webhooks]>[!UICONTROL Custom Webhook]** om de installatie te openen en klikt u op **[!UICONTROL Re-determine data structure]** :

![](assets/redetermine-data-structure-btn-350x195.png)

Dan volg de stappen die in de sectie [ worden beschreven vormen de de gegevensstructuur van de webhaak ](#configure-the-webhook-s-data-structure) in dit artikel.
