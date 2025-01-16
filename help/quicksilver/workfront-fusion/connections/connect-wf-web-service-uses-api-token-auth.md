---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Verbind  [!DNL Adobe Workfront Fusion]  met de Webdienst die de tokenvergunning van API gebruikt
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 0%

---

# Verbind [!DNL Adobe Workfront Fusion] met een Webdienst die API tokenvergunning gebruikt

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ verbind de Fusie van Adobe Workfront met de Webdienst die API tokenvergunning gebruikt ](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-wf-web-service-uses-api-token-auth.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

Bij sommige services is het niet mogelijk om met integratieoplossingen zoals [!DNL Adobe Workfront Fusion] een app te maken die u eenvoudig kunt gebruiken in uw scenario.

Er is een oplossing voor deze situatie. U kunt de gewenste service (app) verbinden met [!DNL Workfront Fusion] via de module [!DNL Workfront Fusion] s [!UICONTROL HTTP] .

In dit artikel wordt uitgelegd hoe u bijna elke webservice kunt verbinden met [!DNL Workfront Fusion] via een API-token voor sleutel en API.

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

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Verbinding maken met een webservice die een API-token gebruikt

De procedure voor het verbinden van de service via een API-token is vergelijkbaar voor de meeste webservices.

1. Creeer een toepassing op de website van de Webdienst, zoals verklaard in de sectie [ creeer een nieuwe toepassing en verkrijg het API teken ](#create-a-new-application-and-obtain-the-api-token) in dit artikel.
1. Haal de API-sleutel of API-token op.
1. Voeg de module [!UICONTROL HTTP] > [!UICONTROL Make a Request] van [!DNL Workfront Fusion] aan uw scenario toe.
1. Opstelling de module volgens de API van de Webdienst documentatie en het runnen van het scenario, zoals die in de sectie [ wordt verklaard Opstelling de [!UICONTROL HTTP] module ](#set-up-the-http-module) in dit artikel.

>[!NOTE]
>
>De [!DNL Pushover] -meldingsservice wordt in dit artikel als voorbeeld gebruikt.

## Een nieuwe toepassing maken en het API-token ophalen

>[!NOTE]
>
>Webservices maken en distribueren API-sleutels of API-tokens op verschillende manieren. Ga naar de website van de service en zoek naar &quot;API-sleutel&quot; of &quot;API-token&quot; voor instructies voor het verkrijgen van een API-sleutel en -token voor de gewenste webservice.
>
>We nemen alleen instructies voor het verkrijgen van een Pushover API-sleutel op als voorbeeld van wat u zou kunnen vinden.

1. Meld u aan bij uw [!DNL Pushover] -account.
1. Klik op **[!UICONTROL Create an Application/API Token]** onder aan de pagina.
1. Vul de toepassingsgegevens in en klik op **[!UICONTROL Create an Application]** .
1. Sla de opgegeven API-token op een veilige plaats op. U zult het voor de [!DNL Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Make a Request] module nodig hebben om met de gewenste Webdienst ([!DNL Pushover], in dit geval) te verbinden.

## De module [!UICONTROL HTTP] instellen

Om een Webdienst met uw [!DNL Workfront Fusion] scenario te verbinden, moet u de [!UICONTROL HTTP] > [!UICONTROL Make a request] module in het scenario gebruiken en opstelling de module volgens de API van de Webdienst documentatie.

1. Voeg de module [!UICONTROL HTTP] > [!UICONTROL Make a Request] aan uw scenario toe.
1. Als u een bericht wilt verzenden met [!DNL Workfront Fusion] , stelt u de HTTP-module als volgt in.

   >[!NOTE]
   >
   >Deze moduleinstellingen komen overeen met de documentatie van de [!DNL Pushover] webservice-API. De instellingen voor andere webservices kunnen afwijken. Het API-token kan bijvoorbeeld worden ingevoegd in het veld [!UICONTROL Header] en niet in het veld [!UICONTROL Body] .

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>Het veld URL bevat het eindpunt dat u kunt vinden in de API-documentatie van de webservice.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Method]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>De gebruikte methode hangt van het overeenkomstige eindpunt af. Het eindpunt van Pushover voor het duwen van berichten gebruikt de methode van de POST.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
      <td> <p>Sommige webservices kunnen headers gebruiken om de API-tokenverificatie of andere parameters op te geven. Dit is niet het geval in ons voorbeeld als eindpunt van de Pushover voor het drukken van berichten gebruikt het Lichaam (zie hieronder) voor alle verzoektypes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Query String]</p> </td> 
      <td> <p>Sommige webservices kunnen een queryreeks gebruiken om andere parameters op te geven. Dit is niet het geval in ons voorbeeld, aangezien de [!DNL Pushover] webservice [!UICONTROL Body] gebruikt (zie hieronder) voor alle aanvraagtypen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Body Type]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>Met deze instelling kunt u het JSON-inhoudstype selecteren in het onderstaande veld [!UICONTROL Content Type] .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON is het vereiste inhoudstype voor de app [!UICONTROL Pushover] . Dit kan verschillen van andere webservices.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Request Content]</p> </td> 
      <td> <p>Voer de [!UICONTROL Body] -aanvraaginhoud in de JSON-indeling in. U kunt [!UICONTROL JSON] gebruiken &gt; [!UICONTROL Create JSON] module zoals die in <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref"> wordt verklaard het Lichaam van JSON die [!UICONTROL JSON] &gt; [!UICONTROL Create JSON] module </a> in dit artikel in kaart wordt gebracht. Of u kunt de inhoud JSON manueel ingaan, zoals die in <a href="#json-body-entered-manually" class="MCXref xref"> wordt verklaard JSON Body manueel </a> in dit artikel werd ingegaan.</p> <p>Zie de API-documentatie van de webservice voor de vereiste parameters voor die webservice.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## JSON Body handmatig ingevoerd

Geef parameters en waarden op in de JSON-indeling.

>[!INFO]
>
>**Voorbeeld:**
>
>```
>{"user":"12345c2ecu1hq42ypqzhswbyam34",
>"token":"123459evz8aepwtxydndydgyumbfx",
>"message":"Hello World!",
>"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL user]</p> </td> 
   <td> <p>UW USER_KEY. Dit vindt u op het dashboard van [!DNL Pushover] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL token] </td> 
   <td> <p>Uw API-token/API-sleutel die is gegenereerd, hebt u uw [!DNL Pushover] -app gemaakt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL message] </td> 
   <td> <p>De tekstinhoud van de pushmelding die naar het apparaat of de apparaten wordt verzonden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL title] </td> 
   <td> <p>(Optioneel) De titel van je bericht. Als er geen waarde wordt ingevoerd, wordt de naam van uw app gebruikt. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Hoofdtekst van JSON toegewezen via de module [!UICONTROL JSON] > [!UICONTROL Create JSON]

De module [!UICONTROL Create JSON] maakt het opgeven van JSON eenvoudiger. U kunt hiermee ook dynamisch waarden definiëren.

Voor meer informatie over de modules JSON, zie [ modules JSON ](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Voer de waarden in waarvan u JSON wilt maken of wijs deze toe.

   ![](assets/json-values-350x288.png)

1. Sluit de module [!UICONTROL JSON] > [!UICONTROL Create JSON] aan op HTTP > Een aanvraag maken.
1. Wijs de JSON-tekenreeks van de module [!UICONTROL Create JSON] toe aan het veld [!UICONTROL Request content] in de module [!UICONTROL HTTP] > [!UICONTROL Make a Request] .

   Wanneer u het scenario nu uitvoert, wordt het pushbericht verzonden naar het apparaat dat is geregistreerd in uw [!DNL Pushover] -account.
