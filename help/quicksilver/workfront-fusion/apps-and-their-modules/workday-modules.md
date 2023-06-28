---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Workday-modules
description: In een Adobe Workfront Fusion-scenario kunt u workflows automatiseren die [!DNL Workday]en deze verbinding maken met meerdere toepassingen en services van derden.
author: Becky
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# [!DNL Workday] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL Workday]en deze verbinding maken met meerdere toepassingen en services van derden.

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

Als u de opdracht [!DNL Workday] modules, moet u:

* hebben een [!DNL Workday] account.

* Een OAuth-toepassing maken in [!DNL Workday]. Zie voor instructies de [!DNL Workday] documentatie.

## Verbinden [!DNL Workday] tot [!DNL Workfront Fusion]

1. In alle [!DNL Workfront Fusion] module, klikt u op [!UICONTROL Add] naast de [!UICONTROL Connection] field

2. Vul de volgende velden in:

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Connection name]</p>
                </td>
                <td>Geef een naam op voor de verbinding</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Workday host]</td>
                <td>Voer het adres in van uw [!DNL Workday] host zonder <code>https://</code>. Bijvoorbeeld: <code>mycompany.workday.com</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Services URL]</td>
                <td>Voer het adres in van uw [!DNL Workday] webservices zonder <code>https://</code>. Bijvoorbeeld: <code>mycompany-services.workday.com</code>.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Tenant name]</td>
                <td>Voer hier de huurder voor in [!DNL Workday] account. Uw huurder is de id van uw organisatie en kan worden weergegeven in de URL die u gebruikt om u aan te melden bij Workday. Voorbeeld: in het adres <code>https://www.myworkday.com/mycompany</code>, de huurder <code>mycompany</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Client ID]</td>
                <td>Voer de client-id in voor de [!DNL Workday] die door deze verbinding wordt gebruikt. Dit wordt verkregen wanneer u de toepassing maakt in [!DNL Workday].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Client Secret]</td>
                <td>Voer het clientgeheim in voor de [!DNL Workday] die door deze verbinding wordt gebruikt. Dit wordt verkregen wanneer u de toepassing maakt in [!DNL Workday].</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Session timeout (min)]</td>
                <td >Voer het aantal minuten in waarna het verificatietoken verloopt.</td>
            </tr>
        </tbody>
    </table>


3. Klikken [!UICONTROL Continue] om de verbinding te bewaren en aan de module terug te keren

## [!DNL Workday] modules en hun velden

Wanneer u [!DNL Workday] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Workday] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Handeling](#action)

* [Zoeken](#search)


### Handeling

* [[!UICONTROL Create a record]](#create-a-record)

* [[!UICONTROL Delete a record]](#delete-a-record)

* [[!UICONTROL Make a custom API call]](#make-a-custom-api-call)

* [[!UICONTROL Update a record]](#update-a-record)


#### [!UICONTROL Create a record]

Deze actiemodule maakt één record in [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Voor instructies over het aansluiten van uw [!DNL Workday] account aan Workfront Fusion, zie <a href="#Connect" class="MCXref xre[!DNL ]f" >Verbinden [!DNL Workday] tot [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Record Type]</td>
            <td>Selecteer het type record dat u wilt maken.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>Voer de id in van de record die u wilt maken of wijs deze toe.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Subresource ID]</td>
            <td >Ga of kaart identiteitskaart van submiddel in u wilt tot stand brengen.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL Delete a record]

In deze actiemodule wordt één record verwijderd uit [!DNL Workday].

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Voor instructies over het aansluiten van uw [!DNL Workday] account aan [!DNL Workfront Fusion], zie <a href="#Connect" class="MCXref xre[!DNL ]f" >Verbinden [!DNL Workday] tot [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Record type]</td>
            <td>Selecteer het type record dat u wilt verwijderen.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Specific record type]</td>
            <td>Selecteer het specifieke type record dat u wilt verwijderen. Deze zijn gebaseerd op het recordtype dat u hebt gekozen.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Subresource ID]</td>
            <td>Ga of kaart identiteitskaart van subresource in u wilt schrappen.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Voer de id in van de record die u wilt verwijderen of wijs deze toe.</td>
        </tr>
    </tbody>
</table>


### [!UICONTROL Make a custom API call]

Deze actiemodule laat u een douane voor authentiek verklaarde vraag aan het maken [!DNL Workday] API. Op deze manier kunt u een automatisering van de gegevensstroom maken die niet door de ander kan worden uitgevoerd [!DNL Workday] modules.

Als u deze module configureert, worden de volgende velden weergegeven.

De module keert een statuscode, samen met de kopballen en het lichaam van de API vraag terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>Voor instructies over het aansluiten van uw [!DNL Workday] account aan [!DNL Workfront Fusion], zie <a href="#Connect" class="MCXref xre[!DNL ]f" >Verbinden [!DNL Workday] tot [!DNL Workfront Fusion]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Een pad invoeren ten opzichte van <code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] Hiermee voegt u de machtigingsheaders voor u toe.</p> </td> 
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

#### [!UICONTROL Update a record]

Deze actiemodule werkt één record bij in [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Voor instructies over het aansluiten van uw [!DNL Workday] account aan Workfront Fusion, zie <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] naar Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">Recordtype</td>
            <td>Selecteer het type record t[!UICONTROL ]Wat u wilt bijwerken.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>Voer de id in van de record die u wilt bijwerken of wijs deze toe.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Subresource ID]</td>
            <td >Ga of kaart identiteitskaart van submiddel in u wilt bijwerken.</td>
        </tr>
    </tbody>
</table>

### Zoeken

* [[!UICONTROL Read a record]](#read-a-record)

* [[!UICONTROL List records]](#list-records)


#### [!UICONTROL Read a record]

Deze actiemodule leest één record.

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Voor instructies over het aansluiten van uw [!DNL Workday] account aan Workfront Fusion, zie <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] naar Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Record type]</td>
            <td>Selecteer het type record dat u wilt verwijderen.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Specific record type]</td>
            <td>Selecteer het specifieke type record dat u wilt lezen. Deze zijn gebaseerd op het recordtype dat u hebt gekozen.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Voer de id in van de record die u wilt verwijderen of wijs deze toe.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL List records]

Deze zoekmodule haalt een lijst met records van het opgegeven type op.

<table style="table-layout:auto"> 
      <col/>
      <col/>
      <tbody>
          <tr>
              <td role="rowheader">[!UICONTROL Connection]</td>
              <td>Voor instructies over het aansluiten van uw [!DNL Workday] account aan [!DNL Workfront Fusion], zie <a href="#Connect" class="MCXref xref" >Verbinden [!DNL Workday] tot [!DNL Workfront Fusion]</a></td>
          </tr>
          <tr>
              <td  role="rowheader">[!UICONTROL Record Type]</td>
              <td>Selecteer het type record dat u wilt ophalen.</td>
          </tr>
          <tr>
              <td role="rowheader">[!UICONTROL Limit]</td>
              <td >
                  <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugwinnen.</p>
              </td>
          </tr>
      </tbody>
  </table>
