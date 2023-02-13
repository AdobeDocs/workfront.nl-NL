---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Datadog-modules
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die Datadog gebruiken, evenals het met veelvoudige derdetoepassingen en de diensten verbinden.
author: Becky
feature: Workfront Fusion
exl-id: a0b4352d-a1ce-4459-a58e-71de860b8a90
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '721'
ht-degree: 0%

---

# [!DNL Datadog] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL Datadog]en deze verbinding maken met meerdere toepassingen en services van derden.

Als u instructies bij het creëren van een scenario nodig hebt, zie [Een scenario maken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Voor informatie over modules, zie [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Vereisten

Te gebruiken [!DNL Datadog] modules, moet u een [!DNL Datadog] account.

## Verbinden [!DNL Datadog] tot [!DNL Workfront Fusion] {#connect-datadog-to-workfront-fusion}

### API-sleutel en toepassingssleutel ophalen {#retrieve-your-api-key-and-application-key}

Als u verbinding wilt maken met uw [!DNL Datadog] account aan [!DNL Workfront Fusion] u moet een API-sleutel en een toepassingssleutel ophalen vanuit uw [!DNL Datadog] account.

1. Meld u aan bij uw [!DNL Datadog] account.
1. Klik in het navigatievenster aan de linkerkant op **[!UICONTROL Integrations]** en klik vervolgens op **[!UICONTROL APIs]**.
1. Klik in het hoofdscherm op **[!UICONTROL API Keys]**.
1. Houd de muisaanwijzer boven de paarse balk om de API-sleutel weer te geven.
1. Kopieer de API-sleutel naar een beveiligde locatie.
1. Klik in het hoofdscherm op **[!UICONTROL Application Keys]**.
1. Houd de muisaanwijzer boven de paarse balk om de toepassingstoets weer te geven.
1. Kopieer de toepassingssleutel naar een veilige locatie.

### Verbinding maken met [!DNL Datadog] in [!DNL Workfront Fusion]

U kunt een verbinding maken met uw [!DNL Datadog] rechtstreeks vanuit een [!UICONTROL Datadog] module.

1. In alle [!UICONTROL Datadog] module, klikt u op **[!UICONTROL Add]** naast de [!UICONTROL Connection] veld.
1. Vul de velden van de module als volgt in:

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection Type]</td> 
      <td> <p> Selecteer [!UICONTROL [!DNL Datadog] Optie van toepassing] om volledige toegang te krijgen tot [!DNL Datadog] API.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection Name]</td> 
      <td> <p> Voer een naam in voor de verbinding.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Domain] </td> 
      <td> <p>Selecteer het domein waarmee u verbinding wilt maken (VS of EU).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API Key]</td> 
      <td> <p> Voer uw [!DNL Datadog] API-sleutel. </p> <p>Voor instructies over het ophalen van de API-sleutel raadpleegt u <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">API-sleutel en toepassingssleutel ophalen</a> in dit artikel.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Application Key]</td> 
      <td> <p> Voer uw [!DNL Datadog] toepassingssleutel. </p> <p>Voor instructies over het ophalen van de toepassingssleutel raadpleegt u <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">API-sleutel en toepassingssleutel ophalen</a> in dit artikel.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **[!UICONTROL Continue]** om de verbinding tot stand te brengen en terug naar de module te gaan.

## [!DNL Datadog] modules en hun velden

Wanneer u [!DNL Datadog] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Datadog] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Handelingen

* [[!UICONTROL Post Timeseries Points]](#post-timeseries-points)
* [[!UICONTROL Make an API Call]](#make-an-api-call)

#### [!UICONTROL Post Timeseries Points]

In de module kunt u gegevens uit de tijdreeks na de tijdreeks plaatsen waarop u een afbeelding kunt maken [!DNL Datadog]&#39;s dashboards.

De limiet voor gecomprimeerde ladingen is 3,2 megabyte (3200000) en 62 megabyte (62914560) voor gedecomprimeerde ladingen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Datadog] account aan [!DNL Workfront Fusion], zie <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Datadog] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Series]</td> 
   <td> <p>Tijdreeks toevoegen waarnaar u wilt verzenden [!DNL Datadog].</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Metric]</strong> </p> <p>Voer de naam van de tijdreeksen in.</p> </li> 
     <li> <p><strong>[!UICONTROL Type]</strong> </p> <p>Selecteer het type metrisch.</p> </li> 
     <li> <p><strong>[!UICONTROL Interval]</strong> </p> <p> Als het type van metrisch tarief of telling is, bepaal het overeenkomstige interval.</p> </li> 
     <li> <p><strong>[!UICONTROL Points]</strong> </p> <p>Voeg punten met betrekking tot metrisch toe.</p> <p>Dit is een JSON-array van punten. Elk punt heeft het formaat: <code>[[POSIX_timestamp, numeric_value], ...] </code></p> <p>Opmerking:  <p>De tijdstempel moet in seconden staan.</p> <p>De tijdstempel moet actueel zijn. De stroom wordt gedefinieerd als niet meer dan 10 minuten in de toekomst of meer dan 1 uur in het verleden.</p> <p> De numerieke notatie moet een zwevende waarde zijn.</p> </p> <p>Dit veld moet ten minste 1 item bevatten.</p> </li> 
     <li> <p><strong>[!UICONTROL Host]</strong> </p> <p>Ga de naam van de gastheer in die metrisch produceerde.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Make an API Call]

Met deze actiemodule kunt u een aangepaste API-aanroep uitvoeren.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Datadog] account aan [!DNL Workfront Fusion], zie <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Datadog] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Een pad invoeren ten opzichte van <code>https://api.datadoghq.com/api/</code>. Voorbeeld:<code> /v1/org</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion voegt de machtigingsheaders voor u toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Voeg de query voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:  <p>Bij het gebruik van voorwaardelijke instructies zoals <code>if</code> in uw JSON, plaats de aanhalingstekens buiten de voorwaardelijke verklaring.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Voorbeeld:** De volgende API-aanroep retourneert alle dashboards in uw [!DNL Datadog] account:

URL: `/v1/dashboard`

Methode: `GET`

![](assets/datadog-api-example.png)

Het resultaat is te vinden in de Output van de module onder Bundel > Tekst > dashboards.

In ons voorbeeld werden 3 dashboards geretourneerd:

![](assets/datadog-api-response-example.png)
