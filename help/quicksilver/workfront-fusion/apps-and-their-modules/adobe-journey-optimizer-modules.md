---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Journey Optimizer-modules
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die gebruiken [!DNL Adobe Journey Optimizer]en deze verbinding maken met meerdere toepassingen en services van derden.
author: Becky
feature: Workfront Fusion
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '1222'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] Modules

<!--
Becky: pull from main, add to TOCs, then push to merge.
-->

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL Adobe Journey Optimizer]en deze verbinding maken met meerdere toepassingen en services van derden. [!DNL Adobe Journey Optimizer] kunt u records maken, lezen, bijwerken of verwijderen, of een aangepaste API-aanroep naar de [!DNL Adobe Journey Optimizer] API.


Als u instructies bij het creëren van een scenario nodig hebt, zie [Een scenario maken](../../workfront-fusion/scenarios/create-a-scenario.md).

Voor informatie over modules, zie [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table>
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

Voordat u de [!DNL Adobe Journey Optimizer] -aansluiting, moet u ervoor zorgen dat aan de volgende voorwaarden wordt voldaan:

* U moet een actieve [!DNL Adobe Journey Optimizer] account.

## Verbinding maken met [!DNL Adobe Journey Optimizer]

Als u een verbinding wilt maken voor uw [!DNL Adobe Journey Optimizer] modules:

1. In alle [!DNL Adobe Journey Optimizer] module, klikt u op **[!UICONTROL Add]** naast het vak Verbinding.

1. Vul de volgende velden in:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Connection name]</td>
          <td>
            <p>Voer een naam in voor deze verbinding.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client ID]</td>
          <td>Voer uw [!DNL Adobe] [!UICONTROL Client ID]. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]</td>
          <td>Voer uw [!DNL Adobe] [!UICONTROL Client Secret]. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Technical account ID]</td>
          <td>Voer uw [!DNL Adobe] [!UICONTROL Technical account ID]. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Organization ID]</td>
          <td>Voer uw [!DNL Adobe] [!UICONTROL Organization ID]. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Meta scopes]</td>
          <td>
            Voer het metabereik in dat nodig is voor de verbinding.
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Private key]</td>
          <td>
            <p>Voer de persoonlijke sleutel in die is gegenereerd toen uw referenties werden gemaakt in het dialoogvenster [!DNL Adobe Developer Console]. </p>
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
      </tbody>
    </table>
1. Klikken **[!UICONTROL Continue]** om de verbinding op te slaan en terug te keren naar de module.

## [!DNL Adobe Journey Optimizer] modules en hun velden

Wanneer u [!DNL Adobe Journey Optimizer] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Adobe Journey Optimizer] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Handelingen](#actions)
* [Zoekopdrachten](#searches)

### Handelingen

* [[!UICONTROL Create a record]](#create-a-record)
* [[!UICONTROL Make a custom API call]](#make-a-custom-api-call)
* [[!UICONTROL Delete a record]](#delete-a-record)
* [[!UICONTROL Update a record]](#update-a-record)

#### [!UICONTROL Create a record]

Deze actiemodule leidt tot een plaatsing, besluitvormingsregel, markering, gepersonaliseerde aanbieding, inzameling, of reserveaanbieding.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer], zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record type]
      </td>
      <td>
        Selecteer het type record dat u wilt maken
        <ul>
        <li><b>[!UICONTROL Placement]</b>: Doorgaan naar <a href="#placement-fields" >[!UICONTROL Placement] velden</a>.</li>
        <li><b>[!UICONTROL Decision rule]</b>: Doorgaan naar <a href="#decision-rule-fields" >[!UICONTROL Decision rule] velden</a>.</li>
        <li><b>[!UICONTROL Decision]</b>: Doorgaan naar <a href="#decision-fields" >[!UICONTROL Decision] velden</a>.</li>
        <li><b>[!UICONTROL Tag]</b>: Doorgaan naar <a href="#tag-fields" >[!UICONTROL Tag] velden</a>.</li>
        <li><b>[!UICONTROL Collection]</b>: Doorgaan naar <a href="#collection-fields" >[!UICONTROL Collection] velden</a>.</li>
        <li><b>[!UICONTROL Fallback offer]</b>: Doorgaan naar <a href="#fallback-offer-fields" >[!UICONTROL Fallback offer] velden</a>.</li>
        <li><b>[!UICONTROL Personalized offer]</b>: Doorgaan naar <a href="#personalized-offer-fields" >[!UICONTROL Personalized offer] velden</a>.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Placement] velden

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Voer een naam voor de plaatsing in of wijs een naam toe.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Description]
      </td>
      <td>Voer een beschrijving voor de plaatsing in of wijs een beschrijving toe.
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL Decision rule] velden

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Voer een naam voor de beschrijvingsregel in of wijs deze toe.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Description]
      </td>
      <td>Voer een beschrijving voor de beslissingsregel in of wijs deze toe.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Condition]
      </td>
      <td>Ga of kaart de voorwaarde in de beslissingsregel.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Decision] velden

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Voer een naam voor de beschrijvingsregel in of wijs deze toe.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status]</td>
      <td>Selecteer de status voor de beslissing.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Start date]</td>
      <td><p>Voer de begindatum voor de beslissing in of wijs deze toe.</p><p>Voor een lijst met ondersteunde datumnotaties raadpleegt u <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Afgedwongen typegebruik in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL End date]</td>
      <td><p>Voer de einddatum voor de beslissing in of wijs deze toe.</p><p>Voor een lijst met ondersteunde datumnotaties raadpleegt u <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Afgedwongen typegebruik in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Placements]</td>
      <td>Selecteer de plaatsen om aan dit besluit toe te voegen
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Collection]</td>
      <td>Selecteer de aanbiedingsinzameling die de aanbiedingen bevat die dit besluit zal overwegen.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Fallback offer]</td>
      <td>Selecteer de reserveaanbieding die aan klanten zal worden voorgesteld die niet de regels voor dit besluit aanpassen.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Tag] velden

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Voer een naam voor de tag in of wijs een naam toe.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Collection] velden

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Voer een naam voor de verzameling in of wijs een naam toe.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Filter Type]
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Elements]
      </td>
      <td>Selecteer de tags die u in de verzameling wilt opnemen.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Fallback offer] velden

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Voer een naam in of wijs een naam toe aan de fallback-aanbieding.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Status]
      </td>
      <td> Selecteer de status van de fallback-aanbieding.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Placement]
      </td>
      <td>Voer de plaatsing voor de fallback-aanbieding in of wijs deze toe.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Personalized offer] velden

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Voer een naam voor de beschrijvingsregel in of wijs deze toe.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status]</td>
      <td>Selecteer de status voor de beslissing.
      </td>
    </tr>
    <tr>
      <td role="rowheader">Plaatsing</td>
      <td>Selecteer de plaatsing voor de gepersonaliseerde aanbieding.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Start date]</td>
      <td><p>Voer de begindatum voor de gepersonaliseerde aanbieding in of wijs deze toe.</p><p>Voor een lijst met ondersteunde datumnotaties raadpleegt u <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Afgedwongen typegebruik in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL End date]</td>
      <td><p>Voer de einddatum voor de gepersonaliseerde aanbieding in of wijs deze toe.</p><p>Voor een lijst met ondersteunde datumnotaties raadpleegt u <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Afgedwongen typegebruik in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Decision rules]</td>
      <td>Selecteer de besluitvormingsregels om aan dit gepersonaliseerde voorstel toe te voegen.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Selecteer de prioriteit van deze aanbieding. Prioriteit bepaalt of dit aanbod wordt gepresenteerd in plaats van een ander aanbod.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Capping constraint]</td>
      <td>Voer het aantal keren in dat dit voorstel wordt gepresenteerd of geef het door aan.
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Delete a record]

In deze actiemodule wordt één record verwijderd uit [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer], zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record type]
      </td>
      <td>
        Selecteer het type record dat u wilt verwijderen
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision rule]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Fallback offer]</li>
        <li>[!UICONTROL Personalized offer]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        Selecteer de record die u wilt verwijderen.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Make a custom API call]

Deze module maakt een aangepaste API-aanroep naar de [!DNL Adobe Journey Optimizer] API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer], zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Een pad invoeren ten opzichte van {baseURL} beginnen met<code>/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
      <td>
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p>
        <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion voegt automatisch machtigingsheaders en x-api-sleutelkopballen toe.</p>
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

#### [!UICONTROL Delete a Record]

In deze actiemodule wordt één record verwijderd uit [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer], zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record Type]
      </td>
      <td>
        Selecteer het type record dat u wilt verwijderen
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision rule]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Fallback offer]</li>
        <li>[!UICONTROL Personalized offer]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        Selecteer de record die u wilt verwijderen.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Update a record]

Deze actiemodule leidt tot een plaatsing, besluit, besluitvormingsregel, markering, gepersonaliseerde aanbieding, inzameling, of reserveaanbieding.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer], zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record type]
      </td>
      <td>
        Selecteer het type record dat u wilt bijwerken
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision rule]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Fallback offer]</li>
        <li>[!UICONTROL Personalized offer]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        Selecteer de record die u wilt bijwerken.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Fields]
      </td>
      <td>Voor elk veld dat u wilt bijwerken:
      <ol>
      <li>Klik op <b>[!UICONTROL Add]</b>.</li>
      <li>Selecteer of u waarden wilt toevoegen, vervangen of verwijderen.</li>
      <li>Voer het veld in dat u wilt bijwerken.</li>
      <li>Voer de nieuwe waarde voor het veld in.</li>
      </td>
    </tr>

</tbody>
</table>


### Zoekopdrachten

#### [!UICONTROL List records]

Deze zoekmodule bevat records van het geselecteerde type, met resultaten die zijn gebaseerd op criteria die u opgeeft.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer], zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record type]</p>
      </td>
      <td>
        <p>Selecteer het type record dat u wilt weergeven.</p>
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision rule]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Fallback offer]</li>
        <li>[!UICONTROL Personalized offer]</li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Query operator]</p>
      </td>
      <td>
        <p>Selecteer een operator om toe te passen op parameters in de query</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fields]</td>
      <td><p>Als u de zoekopdracht wilt beperken tot specifieke velden, voert u de velden in. Voor elk veld tot waar u de zoekopdracht wilt beperken, klikt u op [!UICONTROL Add item] en voert u de naam van het veld in.</p><p>Padexpressies hebben de vorm van door punten gescheiden paden, zoals <code>_instance.xdm:name</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order by] </td>
      <td>Voer de eigenschap in of wijs de eigenschap toe waarmee u de resultaten wilt bestellen.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order direction]</td>
   <td>Selecteer of u resultaten in oplopende of aflopende richting wilt bestellen.
    </td>
     </tr>
  </tbody>
</table>
