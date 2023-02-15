---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Verbinden [!DNL Adobe Workfront Fusion] naar een webservice die API-tokenautorisatie gebruikt
description: Sommige diensten staan integratieoplossingen zoals niet toe [!DNL Adobe Workfront Fusion] om een app te maken die u gemakkelijk kunt gebruiken in uw scenario.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 0%

---

# Verbinden [!DNL Adobe Workfront Fusion] naar een webservice die API-tokenautorisatie gebruikt

Sommige diensten staan integratieoplossingen zoals niet toe [!DNL Adobe Workfront Fusion] om een app te maken die u gemakkelijk kunt gebruiken in uw scenario.

Er is een oplossing voor deze situatie. U kunt verbinding maken met de gewenste service (app) [!DNL Workfront Fusion] gebruiken [!DNL Workfront Fusion]s [!UICONTROL HTTP] module.

In dit artikel wordt uitgelegd hoe u bijna elke webservice kunt verbinden met [!DNL Workfront Fusion] API-sleutel/API-token gebruiken.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Verbinding maken met een webservice die een API-token gebruikt

De procedure voor het verbinden van de service via een API-token is vergelijkbaar voor de meeste webservices.

1. Een toepassing maken op de website van de webservice, zoals wordt uitgelegd in de sectie [Een nieuwe toepassing maken en het API-token ophalen](#create-a-new-application-and-obtain-the-api-token) in dit artikel.
1. Haal de API-sleutel of API-token op.
1. Toevoegen [!DNL Workfront Fusion]s [!UICONTROL HTTP] > [!UICONTROL Make a Request] aan uw scenario.
1. Stel de module in volgens de API-documentatie van de webservice en voer het scenario uit, zoals uitgelegd in de sectie [Stel de [!UICONTROL HTTP] module](#set-up-the-http-module) in dit artikel.

>[!NOTE]
>
>We gebruiken de [!DNL Pushover] meldingsservice als voorbeeld in dit artikel.

## Een nieuwe toepassing maken en het API-token ophalen

>[!NOTE]
>
>Webservices maken en distribueren API-sleutels of API-tokens op verschillende manieren. Ga naar de website van de service en zoek naar &quot;API-sleutel&quot; of &quot;API-token&quot; voor instructies voor het verkrijgen van een API-sleutel en -token voor de gewenste webservice.
>
>We nemen alleen instructies voor het verkrijgen van een Pushover API-sleutel op als voorbeeld van wat u zou kunnen vinden.

1. Meld u aan bij uw [!DNL Pushover] account.
1. Klikken **[!UICONTROL Create an Application/API Token]** onder aan de pagina.
1. Vul de toepassingsgegevens in en klik op **[!UICONTROL Create an Application]**.
1. Sla de opgegeven API-token op een veilige plaats op. U hebt het nodig voor de [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL Make a Request] om verbinding te maken met de gewenste webservice ([!DNL Pushover], in dit geval).

## Stel de [!UICONTROL HTTP] module

Een webservice verbinden met uw [!DNL Workfront Fusion] scenario, moet u gebruiken [!UICONTROL HTTP] >[!UICONTROL Make a request] in het scenario en stel de module in volgens de API-documentatie van de webservice.

1. Voeg de [!UICONTROL HTTP] >[!UICONTROL Make a Request] aan uw scenario.
1. Als u een bericht wilt duwen met [!DNL Workfront Fusion]stelt u de HTTP-module als volgt in.

   >[!NOTE]
   >
   >Deze modulemontages beantwoorden aan [!DNL Pushover] API-documentatie voor webservices. De instellingen voor andere webservices kunnen afwijken. Het API-token kan bijvoorbeeld worden ingevoegd in de [!UICONTROL Header] en niet aan de [!UICONTROL Body] veld.

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
      <td> <p>Sommige webservices kunnen een queryreeks gebruiken om andere parameters op te geven. Dit is in ons voorbeeld niet het geval [!DNL Pushover] webservicegebruik [!UICONTROL Body] (zie hieronder) voor alle aanvraagtypen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Body Type]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>Met deze instelling kunt u het JSON-inhoudstype selecteren in het dialoogvenster [!UICONTROL Content Type] veld hieronder.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON is het vereiste inhoudstype voor de [!UICONTROL Pushover] app. Dit kan verschillen van andere webservices.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Request Content]</p> </td> 
      <td> <p>Voer de [!UICONTROL Body] inhoud aanvragen in de JSON-indeling. U kunt de [!UICONTROL JSON] &gt; [!UICONTROL Create JSON] module zoals beschreven in <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">JSON-body toegewezen met de opdracht [!UICONTROL JSON] &gt; [!UICONTROL Create JSON] module</a> in dit artikel. U kunt de JSON-inhoud ook handmatig invoeren, zoals wordt uitgelegd in <a href="#json-body-entered-manually" class="MCXref xref">JSON Body handmatig ingevoerd</a> in dit artikel.</p> <p>Zie de API-documentatie van de webservice voor de vereiste parameters voor die webservice.</p> </td> 
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
>
>"token":"123459evz8aepwtxydndydgyumbfx",
>
>"message":"Hello World!",
>
>"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL user]</p> </td> 
   <td> <p>UW USER_KEY. Dit is te vinden in uw [!DNL Pushover] dashboard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL token] </td> 
   <td> <p>Uw API-token/API-sleutel die u hebt gegenereerd, heeft uw [!DNL Pushover] app.</p> </td> 
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

## JSON-body toegewezen met de opdracht [!UICONTROL JSON] >[!UICONTROL Create JSON] module

De [!UICONTROL Create JSON] maakt het opgeven van JSON eenvoudiger. U kunt hiermee ook dynamisch waarden definiëren.

Voor meer informatie over de JSON-modules raadpleegt u [JSON-modules](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Voer de waarden in waarvan u JSON wilt maken of wijs deze toe.

   ![](assets/json-values-350x288.png)

1. Verbind de [!UICONTROL JSON] > [!UICONTROL Create JSON] naar HTTP > Een aanvraagmodule maken.
1. Wijs de JSON-tekenreeks toe vanuit de [!UICONTROL Create JSON] aan de [!UICONTROL Request content] in het [!UICONTROL HTTP] >[!UICONTROL Make a Request] module.

   Wanneer u het scenario uitvoert, wordt het pushbericht verzonden naar het apparaat dat is geregistreerd in uw [!DNL Pushover] account.
