---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Authenticator-module
description: Met de Adobe Authenticator-module kunt u via één enkele verbinding verbinding verbinding maken met elk Adobe product met een API.
author: Becky
feature: Workfront Fusion
source-git-commit: 07443d85e160004c273fc977629dd9f588cc23b2
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 0%

---

# Adobe Authenticator-modules

Met de Adobe Authenticator-module kunt u verbinding maken met elke Adobe-API via één verbinding. Hierdoor kunt u gemakkelijker verbinding maken met Adobe-producten die nog geen speciale Fusion-connector hebben.

Het voordeel ten opzichte van de HTTP-modules is dat u een verbinding kunt maken, zoals in een specifieke app.

Zie X voor een lijst met beschikbare Adobe-API&#39;s. U kunt mogelijk alleen de API&#39;s gebruiken waaraan u bent toegewezen.

## Toegangsvereisten

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan</td>
      <td>
        <p>Nieuw: alle</p><p>of</p><p>Huidige: [!UICONTROL Pro] of hoger</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licentie</td>
      <td>
        <p>Nieuw: Standaard</p><p>of</p><p>Huidige: [!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie</td>
      <td>
   <p>Huidige Fusion-vergunningsvereiste: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere Fusion-licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Product</td>
      <td>
   <p>Nieuw Workfront-abonnement: als je de [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Huidig Workfront-abonnement: Uw organisatie moet het volgende kopen [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td>
    </tr>
  </tbody>
</table>

## Vereisten

* U moet toegang hebben tot het product van de Adobe dat u de module wilt verbinden met.
* U moet toegang hebben tot de Adobe Developer-console.
* U moet een project in de Adobe Developer-console hebben dat de API bevat waarmee u verbinding wilt maken met de module. U kunt:

   * Maak een nieuw project met de API.

     of
   * Voeg API aan een bestaand project toe.

  Voor informatie over het maken of toevoegen van een API aan een project in de Adobe Developer Console raadpleegt u [Een project maken](https://developer.adobe.com/dep/guides/dev-console/create-project/) in de documentatie bij de Adobe.

## Verbinding maken

Een Adobe Authenticator-verbinding maakt verbinding met één project in de Adobe Developer-console. Als u dezelfde verbinding voor meerdere Adobe-API wilt gebruiken, voegt u de API&#39;s toe aan hetzelfde project en maakt u een verbinding met dat project.

U kunt afzonderlijke verbindingen aan afzonderlijke projecten tot stand brengen, maar u kunt geen verbinding gebruiken om tot API toegang te hebben die niet op het project is dat in die verbinding wordt gespecificeerd.

>[!IMPORTANT]
>
>Met de Adobe Authenticator-connector hebt u de keuze tussen het maken van een OAuth Server-to-server verbinding of een Service Account (JWT)-verbinding. Adobe heeft JWT-referenties vervangen, die na 1 januari 2025 niet meer werken. **Daarom adviseren wij hoogst tot stand brengend OAuth verbindingen.**
>
>Voor meer informatie over deze types van verbindingen, zie [Server-naar-server verificatie](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/) in de documentatie van de Adobe

Een verbinding maken:

1. Klik in een willekeurige Adobe Authenticator-module op **Toevoegen** naast het veld Verbinding.
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
          <p>Selecteer of u een Server-aan-Server verbinding OAuth, of een verbinding van de de dienstrekening (JWT) wilt tot stand brengen.</p>
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
        <td>Voer uw [!DNL Adobe] Client-id. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Voer uw [!DNL Adobe] Clientgeheim. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Scopes]</td>
        <td>Als u een OAuth-verbinding hebt geselecteerd, voert u het bereik in dat nodig is voor deze verbinding.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Technical account ID]</td>
        <td>Voer uw [!DNL Adobe] Technische account-id. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Organization ID]</td>
        <td>Als u een JWT-verbinding hebt geselecteerd, voert u uw [!DNL Adobe] Organisatie-id. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta Scopes]</td>
        <td>Als u een JWT-verbinding hebt geselecteerd, voert u het metabereik in dat nodig is voor deze verbinding. </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Private key]</td>
        <td>
          <p>Als u een JWT-verbinding hebt geselecteerd, voert u de persoonlijke sleutel in die is gegenereerd toen uw referenties werden gemaakt in het dialoogvenster [!DNL Adobe Developer Console]. </p>
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
              <p>Klikken <b>[!UICONTROL Save]</b> om het bestand uit te pakken en terug te keren naar de verbindingsinstelling.</p>
            </li>
          </ol>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>Selecteer of u verbinding maakt met een productie- of niet-productieomgeving.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Selecteer of u verbinding maakt met een serviceaccount of een persoonlijke account.</td>
      </tr>
    </tbody>
    </table>

1. Klikken **[!UICONTROL Continue]** om de verbinding op te slaan en terug te keren naar de module.

## Module

### Een aangepaste API-aanroep maken

Met deze actiemodule kunt u elke Adobe-API aanroepen.

>[!TIP]
>
>U moet de volledige URL invoeren voor de API waarmee u verbinding wilt maken. Deze module accepteert geen relatieve URL&#39;s.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Voor instructies over het maken van een verbinding met de Adobe Authenticator-module raadpleegt u <a href="#create-a-connection" class="MCXref xref" >Verbinding maken</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL]</p>
      </td>
      <td>
        <p>Voer de volledige URL in van het API-punt waarmee u verbinding wilt maken.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p>
        <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion voegt automatisch machtigingsheaders toe.</p>
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
     <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Voer het maximale aantal resultaten in dat de module in één uitvoeringscyclus moet retourneren.</p>
      </td>
    </tr>
  </tbody>
</table>

