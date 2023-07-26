---
filename: creative-cloud-libraries-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Creative Cloud-bibliotheekmodules
description: Met de [!DNL Adobe Workfront Fusion Adobe Creative Cloud] De modules van Bibliotheken, kunt u een scenario beginnen wanneer een element of een bibliotheek worden gecreeerd of wordt bijgewerkt. U kunt ook elementen uploaden, ophalen, archiveren of een lijst maken, of een oproep doen aan de [!DNL Adobe Creative Cloud Libraries] API.
author: Becky
feature: Workfront Fusion
exl-id: 8affa34b-803d-48a5-a986-9fbe0cb8c8f5
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 0%

---

# Adobe Creative Cloud-bibliotheekmodules

Met de [!DNL Adobe Workfront Fusion] [!DNL Adobe Creative Cloud Libraries] modules, kunt u een scenario beginnen wanneer een element of een bibliotheek worden gecreeerd of wordt bijgewerkt. U kunt ook elementen uploaden, ophalen, archiveren of een lijst maken, of een oproep doen aan de [!DNL Adobe Creative Cloud Libraries] API.

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

Te gebruiken [!DNL Adobe Creative Cloud Libraries] modules, moet u een [!UICONTROL Adobe Creative Cloud] account.

## [!UICONTROL Adobe Creative Cloud Libraries] modules en hun velden

Wanneer u [!UICONTROL Adobe Creative Cloud Libraries] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Adobe Creative Cloud Libraries] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


* [Elementen](#elements)

* [Bibliotheken](#libraries)

* [Overige](#other)


### Elementen

* [[!UICONTROL Archive an Element]](#archive-an-element)

* [[!UICONTROL Get an Element]](#get-an-element)

* [[!UICONTROL List Elements]](#list-elements)

* [[!UICONTROL Upload an Element]](#upload-an-element)

* [!UICONTROL [Nieuw element controleren in bibliotheek]](#watch-new-element-in-library)

* [[!UICONTROL Watch Updated Elements]](#watch-updated-elements)


#### [!UICONTROL Archive an Element]

Deze actiemodule archiveert een element uit een bibliotheek.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het aansluiten van uw [!DNL Adobe Creative Cloud] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Selecteer de bibliotheek die het element bevat dat u wilt archiveren.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL Element ID]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Selecteer het element dat u wilt archiveren.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get an Element]

Deze actiemodule retourneert één element uit een bibliotheek.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het aansluiten van uw [!DNL Adobe Creative Cloud] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Selecteer de bibliotheek met het element dat u wilt ophalen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Element ID]</td>
      <td>Ga of kaart identiteitskaart van het element in dat u wilt terugwinnen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selector]</td>
      <td>
        <p>Selecteer het type informatie dat de module terugkeert. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Default]</b>
            </p>
            <p>Basisgegevens</p>
          </li>
          <li>
            <p><b>[!UICONTROL Details]</b>
            </p>
            <p>Alle beschikbare gegevens</p>
          </li>
          <li>
            <p><b>[!UICONTROL Representations]</b>
            </p>
            <p>Een samengevoegde lijst met elementen die zijn gekoppeld aan het bibliotheekelement</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List Elements]

Deze actiemodule wint een lijst van elementen in een bibliotheek terug.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het aansluiten van uw [!DNL Adobe Creative Cloud] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Selecteer de bibliotheek waarvan u elementen wilt weergeven.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order by]</td>
      <td>Selecteer of u de resultaten wilt sorteren op naam of op de laatste datum waarop het element is gewijzigd.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type]</td>
      <td >Voer een MIME-type in om de resultaten te beperken tot elementen die met het opgegeven MIME-type zijn geïdentificeerd. Voorbeeld: <code>string</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selector]</td>
      <td>
        <p>Selecteer het type informatie dat de module terugkeert. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Default]</b>
            </p>
            <p>Basisgegevens</p>
          </li>
          <li>
            <p><b>[!UICONTROL Details]</b>
            </p>
            <p>Alle beschikbare gegevens</p>
          </li>
          <li>
            <p><b>[!UICONTROL Representations]</b>
            </p>
            <p>Een samengevoegde lijst met elementen die zijn gekoppeld aan het bibliotheekelement</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Upload an Element]

Deze actiemodule uploadt een klein bestandsmiddel naar een bestaande bibliotheek. De maximale bestandsgrootte is 1 GB.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het aansluiten van uw [!DNL Adobe Creative Cloud] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Selecteer de bibliotheek waarvan u elementen wilt weergeven.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Invocation Mode]</td>
      <td>
        <p>Selecteer de verwerkingsmodus om dit aanvraagproces aan te roepen.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL sync]</b>
            </p>
            <p>De API-aanroep wordt synchroon verwerkt. De reactie wordt geleverd wanneer de verwerking volledig is (tenzij de vraagtijden uit.)</p>
          </li>
          <li>
            <p><b>[!UICONTROL async]</b>
            </p>
            <p>De asynchrone monitorreactie wordt onmiddellijk teruggekeerd, en de verzoekverwerking komt asynchroon voor. Het roepen is verantwoordelijk voor het opiniepeilen van het eindpunt tot voltooiing.</p>
          </li>
          <li>
            <p><b>[!UICONTROL sync,async]</b> (Standaard)</p>
            <p>Er wordt geprobeerd het verzoek synchroon te verwerken. Wanneer de verwerking langer dan 5000 ms duurt, wordt de asynchrone monitorreactie geretourneerd. De URL van de monitor moet worden opgevraagd totdat het verzoek is voltooid.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type File]</td>
      <td >Voer het MIME-type van het geüploade bestand in of wijs dit toe.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Source File]</td>
      <td>
        <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Watch New Element in Library]

Deze triggermodule start een scenario wanneer een element aan een bibliotheek wordt toegevoegd.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het aansluiten van uw [!DNL Adobe Creative Cloud] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Selecteer de bibliotheek die u wilt controleren voor bijgewerkte elementen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Watch Updated Elements]

Deze triggermodule start een scenario wanneer een element in een bibliotheek wordt bijgewerkt.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het aansluiten van uw [!DNL Adobe Creative Cloud] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Selecteer de bibliotheek die u wilt controleren voor nieuwe elementen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</td>
    </tr>
  </tbody>
</table>

### Bibliotheken

* [[!UICONTROL Watch New Libraries]](#watch-new-libraries)

* [[!UICONTROL Watch Updated Libraries]](#watch-updated-libraries)


#### [!UICONTROL Watch New Libraries]

Deze triggermodule start een scenario wanneer een nieuwe bibliotheek wordt gemaakt.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het aansluiten van uw [!DNL Adobe Creative Cloud] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Watch Updated Libraries]

Deze triggermodule start een scenario wanneer een bestaande bibliotheek wordt bijgewerkt.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het aansluiten van uw [!DNL Adobe Creative Cloud] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</td>
    </tr>
  </tbody>
</table>

### Overige

#### [!UICONTROL Make an API Call]

Deze module maakt een aangepaste API-aanroep naar de [!DNL Adobe Creative Cloud Libraries] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Ga voor instructies over het verbinden van uw Adobe Creative Cloud-account met Workfront Fusion naar <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe Workfront Fusion - Basisinstructies.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Een pad invoeren ten opzichte van <code>https://cc-libraries.adobe.io/api</code>.</p>
    <p>Bijvoorbeeld <code>/v1/libraries</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL API version]</td>
      <td>
        <p>Selecteer de versie van de [!DNL Adobe Analytics] API waarmee u verbinding wilt maken.</p>
      </td>
    </tr>    <tr>
      <td role="rowheader">[!UICONTROL Method]</td>
      <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p>
        <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion voegt de machtigingsheaders voor u toe.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]</td>
      <td>
        <p>Voeg de query voor de API-aanroep toe als een standaard JSON-object.</p>
        <p>Bijvoorbeeld: <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:  <p>Bij het gebruik van voorwaardelijke instructies zoals <code>if</code> in uw JSON, plaats de aanhalingstekens buiten de voorwaardelijke verklaring.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
       <tr>
      <td role="rowheader">[!UICONTROL Upload a transient document]</td>
      <td>
      <p>Als u een tijdelijk document wilt uploaden, voert u het bronbestand in voor het document dat u wilt uploaden.</p>
      <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p>
    </td>
    </tr>

</tbody>
</table>
