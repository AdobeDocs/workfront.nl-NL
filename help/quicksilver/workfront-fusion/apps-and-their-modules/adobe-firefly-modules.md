---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Firefly
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die gebruiken [!DNL Adobe Firefly]en deze verbinding maken met meerdere toepassingen en services van derden.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 1e131c27-571d-4099-9243-69572bdb3f5a
source-git-commit: 7013302a6ba903b410ed1fa8948a195083004eb9
workflow-type: tm+mt
source-wordcount: '1181'
ht-degree: 0%

---

# [!DNL Adobe Firefly] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL Adobe Firefly]en deze verbinding maken met meerdere toepassingen en services van derden.

Als u instructies bij het creëren van een scenario nodig hebt, zie [Een scenario maken](../../workfront-fusion/scenarios/create-a-scenario.md).

Voor informatie over modules, zie [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> <p>Nieuw: [!UICONTROL Standard]</p><p>of</p><p>Huidige: [!UICONTROL Work] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidig: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Verouderd: alle </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Nieuw:</p> <ul><li>[!UICONTROL Select] of [!UICONTROL Prime] [!DNL Workfront] Abonnement: uw organisatie moet aankopen [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] is opgenomen.</li></ul>
   <p>of</p>
   <p>Huidig: Uw organisatie moet het volgende aanschaffen [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

Voordat u de [!DNL Adobe Firefly] -aansluiting, moet u ervoor zorgen dat aan de volgende voorwaarden wordt voldaan:

* U moet een actieve [!DNL Adobe Firefly] account.

## Verbinding maken met [!DNL Adobe Firefly]

Als u een verbinding wilt maken voor uw [!DNL Adobe Firefly] modules:

1. Klikken **[!UICONTROL Add]** naast het vak Verbinding.

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
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>Selecteer of u verbinding maakt met een productie- of niet-productieomgeving.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Selecteer of u verbinding maakt met een serviceaccount of een persoonlijke account.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Voer uw [!UICONTROL Adobe] [!UICONTROL Client ID]. Dit vindt u in het gedeelte [!UICONTROL Credentials] sectie details van de [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Voer uw [!DNL Adobe] [!UICONTROL Client Secret]. Dit vindt u in het gedeelte [!UICONTROL Credentials] sectie details van de [!DNL Adobe Developer Console]</td>
        </tr>
      </tbody>
    </table>

1. Klikken **[!UICONTROL Continue]** om de verbinding op te slaan en terug te keren naar de module.

## [!DNL Adobe Firefly] modules en hun velden

Wanneer u [!DNL Adobe Firefly] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Adobe Firefly] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Een aangepaste API-aanroep maken

Deze actiemodule doet een douanevraag aan de Firefly API.

Zie voor specifieke beschikbare API&#39;s [Adobe Firefly-API](https://developer.adobe.com/firefly-services/docs/firefly-api/) in de documentatie van Adobe Developer.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Firefly], zie <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Verbinding maken met [!DNL Adobe Firefly]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Een pad invoeren ten opzichte van <code>https://firefly-api-enterprise-stage.adobe.io/</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p>
        <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] voegt automatisch machtigingsheaders toe.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:  <p>Bij het gebruik van voorwaardelijke instructies zoals <code>if</code> in uw JSON, plaats de aanhalingstekens buiten de voorwaardelijke verklaring.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### Een afbeelding uitbreiden

Deze actiemodule breidt een afbeelding uit, optioneel met inhoud van een vraag die u opgeeft.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign], zie <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Verbinding maken met [!DNL Adobe Firefly]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt]</td> 
   <td>Voer een vraag in of wijs een vraag toe aan de inhoud waarmee u de afbeelding wilt uitvouwen. Als er geen vraag wordt weergegeven, wordt de afbeelding uitgebreid met inhoud die overeenkomt met de oorspronkelijke afbeelding.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number of variations]</td> 
   <td>Voer een getal in tussen 1 en 4. De module genereert dit aantal uitgebreide afbeeldingsvariaties.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expanded image format]</td> 
   <td>Selecteer de bestandsindeling waarin de uitgevouwen afbeelding wordt opgeslagen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>  <p>Selecteer een bronbestand uit een vorige module of wijs de naam en het afbeeldingsbestand (gegevens) van het bronbestand toe.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Size]</td> 
   <td>Selecteer de grootte van de uitgevouwen afbeelding.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seed]</td> 
   <td>Voer een geheel getal in of wijs een geheel getal toe. U kunt dit zelfde zaad in een andere gebruiken breid een beeldmodule uit om een gelijkaardige beeld met verschillende stijlen te produceren. </td> 
  </tr> 
 </tbody> 
</table>

## Een afbeelding vullen

Deze actiemodule vult het gemaskeerde gebied van een afbeelding, optioneel met inhoud van een vraag die u opgeeft.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign], zie <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Verbinding maken met [!DNL Adobe Firefly]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt]</td> 
   <td>Voer een vraag in of wijs een vraag toe aan de inhoud waarmee u de afbeelding wilt vullen. Als er geen vraag wordt weergegeven, wordt de afbeelding gevuld met inhoud die overeenkomt met de oorspronkelijke afbeelding.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number of variations]</td> 
   <td>Voer een getal in tussen 1 en 4. De module genereert dit aantal gevulde afbeeldingsvariaties.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filled image format]</td> 
   <td>Selecteer de bestandsindeling waarin de gevulde afbeelding wordt opgeslagen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Image]</td> 
   <td>  <p> Klikken <b>Een afbeelding toevoegen</b>. Selecteer een bronbestand uit een vorige module of wijs de bestandsnaam en de afbeeldingsgegevens van het bronbestand toe.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mask]</td> 
   <td>  <p> Klikken <b>Een masker toevoegen</b>. Selecteer een bronbestand uit een vorige module of wijs de naam en het masker van het bronbestand toe. Het maskerbestand vertegenwoordigt het aangepaste masker dat wordt gevuld met gegenereerde inhoud.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Size]</td> 
   <td>Selecteer de grootte van de gevulde afbeelding.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seeds]</td> 
   <td>Klik voor elke afbeelding die de module genereert op <b>Item toevoegen<b> en voert u een geheel getal in of wijst u dit toe. U kunt dit zelfde zaad in een andere gebruiken breid een beeldmodule uit om een gelijkaardige beeld met verschillende stijlen te produceren. Het aantal zaden dat u toevoegt, moet gelijk zijn aan het veld Aantal variaties.</td> 
  </tr> 
 </tbody> 
</table>

## Een afbeelding genereren

Deze actiemodule genereert een afbeelding op basis van een vraag die u opgeeft. U kunt ook een optionele referentieafbeelding opgeven en de gegenereerde afbeelding komt overeen met de stijl van de referentieafbeelding.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign], zie <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Verbinding maken met [!DNL Adobe Firefly]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt]</td> 
   <td>Voer een vraag in of wijs een vraag toe aan de afbeelding die u wilt maken. Als u meer details opgeeft in de vraag, hebt u meer controle over wat er in de afbeelding wordt weergegeven.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number of variations]</td> 
   <td>Voer een getal in tussen 1 en 4. De module genereert dit aantal afbeeldingsvariaties.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Generated image format]</td> 
   <td>Selecteer de bestandsindeling waarin de uitgevouwen afbeelding wordt opgeslagen. Als u de standaardinstelling selecteert, wordt de bestandsindeling JPEG als er geen referentieafbeelding is opgegeven. Als een referentieafbeelding wordt opgegeven, is de bestandsindeling van de gegenereerde afbeelding dezelfde als die van de referentieafbeelding.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>  <p>Selecteer een bronbestand uit een vorige module of wijs de naam van het referentiebestand en het referentieafbeeldingsbestand (gegevens) van het bronbestand toe. De gegenereerde afbeelding wordt zo gemaakt dat deze overeenkomt met de stijl van de referentieafbeelding.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Presets]</td> 
   <td>Als u een vooraf ingestelde stijl wilt gebruiken, voegt de klik punt toe en gaat of kaart de stijl in die u wilt gebruiken.<p>Zie voor een lijst met vooraf ingestelde stijlen <a href="https://developer.adobe.com/firefly-services/docs/firefly-api/guides/concepts/styles/" >Stijlen afbeeldingsmodel</a> in de Adobe Developer documentation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Negative prompt]</td> 
   <td>Typ of wijs de woorden toe die u in de gegenereerde inhoud wilt vermijden. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content class]</td> 
   <td>Selecteer of u de gegenereerde afbeelding meer als een foto wilt weergeven, of meer als een gemaakte illustratie. <ul><li><b>Foto</b><p>Voer waarden in voor de lensopening, de sluitersnelheid (in seconden) en het gezichtsveld (in millimeters).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seed]</td> 
   <td>Voer een geheel getal in of wijs een geheel getal toe. U kunt dit zelfde zaad in een andere gebruiken breid een beeldmodule uit om een gelijkaardige beeld met verschillende stijlen te produceren. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Size]</td> 
   <td>Selecteer de grootte van de gegenereerde afbeelding.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Strength]</td> 
   <td>Voer een geheel getal in of wijs een geheel getal toe dat de intensiteit aangeeft waarmee de gegenereerde afbeelding overeenkomt met de stijl van de vooraf ingestelde stijl of de referentieafbeelding. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visual intensity]</td> 
   <td>Voer een geheel getal in of wijs een geheel getal toe dat de algemene intensiteit van de bestaande visuele kenmerken van de foto vertegenwoordigt. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Locale]</td> 
   <td>Als een landinstelling wordt opgegeven, genereert de module inhoud die relevanter is voor de opgegeven landinstelling. <p>De landinstelling moet worden vermeld in ISO 639-1 taalcode en ISO 3166-1 regio.</p><p> Voorbeeld: <code>en-US</code></p></td> 
  </tr> 
 </tbody> 
</table>
