---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Split.io-modules
description: In een  [!DNL Adobe Workfront Fusion]  scenario, kunt u werkschema's automatiseren die  [!DNL Split.io] gebruiken, evenals het met veelvoudige derdetoepassingen en de diensten verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 4576a2e4-b495-430e-a9de-4e1ec7379ab8
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 0%

---

# [!DNL Split.io] modules

In een [!DNL Adobe Workfront Fusion] -scenario kunt u workflows automatiseren die [!DNL Split.io] gebruiken en deze koppelen aan meerdere toepassingen en services van derden.

Als u instructies bij het creëren van een scenario nodig hebt, zie [ een scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) creëren.

Voor informatie over modules, zie [ Modules in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Vereisten

Als u [!DNL Split.io] -modules wilt gebruiken, moet u een [!DNL Split.io] -account hebben.

## Verbinden [!DNL Split.io] met [!DNL Workfront Fusion] {#connect-split-io-to-workfront-fusion}

U kunt rechtstreeks vanuit een [!DNL Split.io] -module verbinding maken met uw [!DNL Split.io] -account.

1. Klik in een willekeurige [!DNL Split.io] -module op **[!UICONTROL Add]** naast het [!UICONTROL Connection] -veld.
1. Voer een naam in voor de verbinding.
1. Voer uw API-sleutel voor [!DNL Split.io] in.

   Voor meer informatie over [!DNL Split.io] API sleutels, zie [ API sleutels ](https://help.split.io/hc/en-us/articles/360019916211-API-keys) in de [!DNL Split.io] documentatie.

1. Klik op **[!UICONTROL Continue]** om de verbinding te maken en terug te gaan naar de module.

## [!DNL Split.io] modules en hun velden

Wanneer u [!DNL split.io] modules configureert, geeft [!DNL Workfront Fusion] de onderstaande velden weer. Daarnaast kunnen aanvullende [!DNL split.io] -velden worden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Voor meer informatie, zie [ informatie van de Kaart van één module aan een andere in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Handelingen](#actions)
* [Zoekopdrachten](#searches)

### Handelingen

* [[!UICONTROL Custom API Call]](#custom-api-call)
* [[!UICONTROL Get Split]](#get-split)
* [[!UICONTROL Get Split Definition in Environment]](#get-split-definition-in-environment)
* [[!UICONTROL Create Split]](#create-split)
* [[!UICONTROL Delete Split]](#delete-split)
* [[!UICONTROL Create Split Definition in Environment]](#create-split-definition-in-environment)
* [[!UICONTROL Remove Split Definition from Environment]](#remove-split-definition-from-environment)
* [[!UICONTROL Partial Update Split Definition in Environment]](#partial-update-split-definition-in-environment)
* [[!UICONTROL Associate Tags]](#associate-tags)

#### [!UICONTROL Custom API Call]

Met deze actiemodule kunt u een aangepaste, geverifieerde aanroep van de [!DNL split.io] API maken. Op deze manier kunt u een automatisering van de gegevensstroom maken die niet door de andere [!DNL split.io] -modules kan worden uitgevoerd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Split.io] met [!UICONTROL Workfront Fusion] </a> in dit artikel voor instructies over het verbinden van uw [!DNL Split.io] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Voer een pad in dat relatief is ten opzichte van <code>https://api.split.io/internal/api/v2/</code> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref"> HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a> voor meer informatie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion voegt de machtigingsheaders voor u toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Voeg de query voor de API-aanroep toe als een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:  <p>Wanneer u voorwaardelijke instructies gebruikt, zoals <code>if</code> in uw JSON, plaatst u de aanhalingstekens buiten de voorwaardelijke instructie.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Ga of kaart het maximumaantal verslagen in u de module wilt werken met tijdens elke cyclus van de scenariouitvoering.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Split]

Deze actiemodule haalt de splitsing op.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Split.io] met [!UICONTROL Workfront Fusion] </a> in dit artikel voor instructies over het verbinden van uw [!DNL Split.io] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecteer of wijs de werkruimte toe die de splitsing bevat u wilt terugwinnen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Voer de naam in van de splitsing die u wilt ophalen of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Split Definition in Environment]

Deze actiemodule wint een specifieke gespleten definitie van het aangewezen milieu terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Split.io] met [!UICONTROL Workfront Fusion] </a> in dit artikel voor instructies over het verbinden van uw [!DNL Split.io] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecteer of wijs de werkruimte toe die de gesplitste definitie bevat u wilt terugwinnen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>Selecteer of wijs het milieu toe dat de gespleten definitie bevat u wilt terugwinnen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Voer de naam in of wijs de naam toe van de splitsing waarvoor u de gesplitste definitie wilt ophalen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create Split]

Deze actiemodule leidt tot een nieuwe spleet in uw organisatie, op basis van een verkeerstype.

>[!NOTE]
>
>De API configureert de splitsing in geen enkele omgeving.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Split.io] met [!UICONTROL Workfront Fusion] </a> in dit artikel voor instructies over het verbinden van uw [!DNL Split.io] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecteer of wijs de werkruimte toe waar u de splitsing wilt maken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Traffic Type ID or Name]</td> 
   <td>Selecteer of wijs het verkeerstype toe dat u wilt gebruiken om de splitsing tot stand te brengen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Voer een naam in of wijs een naam toe voor de splitsing die u wilt maken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Description]</td> 
   <td>Voer een [!UICONTROL split] -beschrijving in of wijs deze toe voor de splitsing die u wilt maken.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete Split]

Deze actiemodule verwijdert een splitsing van uw organisatie. Hierdoor wordt de gesplitste definitie automatisch van alle omgevingen verwijderd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Split.io] met [!UICONTROL Workfront Fusion] </a> in dit artikel voor instructies over het verbinden van uw [!DNL Split.io] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecteer of wijs de werkruimte toe waar u de splitsing wilt verwijderen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Voer de naam in van de splitsing die u wilt verwijderen of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create Split Definition in Environment]

Deze actiemodule vormt een gespleten definitie voor een specifiek milieu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Split.io] met [!UICONTROL Workfront Fusion] </a> in dit artikel voor instructies over het verbinden van uw [!DNL Split.io] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecteer of wijs de werkruimte toe waar u een gespleten definitie wilt tot stand brengen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>Selecteer of wijs de omgeving toe waar u een gesplitste definitie wilt maken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Typ of wijs de naam van de splitsing toe waarvoor u een definitie wilt maken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comments]</td> 
   <td>Voer opmerkingen in of wijs deze toe die u aan de gesplitste definitie wilt toevoegen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rules]</td> 
   <td> <p>Voor elke het richten regel wilt u aan de definitie toevoegen, klik <b>[!UICONTROL Add item]</b>, dan ingaan of de regel in kaart brengen.</p> <p>Voor meer informatie bij het richten van regels, zie <a href="https://docs.split.io/reference#create-split-definition-in-environment"> gespleten definitie in een milieu </a> in de [!DNL Split.io] documentatie creëren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Default rule]</td> 
   <td> <p>Ga of kaart de regel in dat u de spatie voor het verkeer wilt gebruiken dat niet specificaties voor de andere regels ontmoet.</p> <p>Voor meer informatie bij het richten van regels, zie <a href="https://docs.split.io/reference#create-split-definition-in-environment"> gespleten definitie in een milieu </a> in de [!DNL Split.io] documentatie creëren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Default treatment]</td> 
   <td> <p>Ga of kaart de behandeling in die u de splitsing wilt gebruiken als de splitsing wordt gedood of de klant niet inbegrepen in verkeerstoewijzing is.</p> <p>Voor meer informatie over behandelingen, zie <a href="https://docs.split.io/reference#create-split-definition-in-environment"> gespleten definitie in een milieu </a> in de [!DNL Split.io] documentatie creëren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Treatments]</td> 
   <td> <p>Voor elke behandeling die u aan de definitie wilt toevoegen, klikt u op <b>[!UICONTROL Add item]</b> en voert u de behandeling in of wijst u deze toe.</p> <p>Voor meer informatie over behandelingen, zie <a href="https://docs.split.io/reference#create-split-definition-in-environment"> gespleten definitie in een milieu </a> in de [!DNL Split.io] documentatie creëren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remove Split Definition from Environment]

Deze actiemodule maakt de configuratie van een gesplitste definitie voor een specifieke omgeving ongedaan.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Split.io] met [!UICONTROL Workfront Fusion] </a> in dit artikel voor instructies over het verbinden van uw [!DNL Split.io] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecteer of wijs de werkruimte toe waar u een gesplitste definitie wilt verwijderen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>Selecteer of wijs het milieu in kaart waar u een gespleten definitie wilt verwijderen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Typ of wijs de naam van de splitsing toe waarvoor u een definitie wilt verwijderen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comments]</td> 
   <td>Voer opmerkingen in of wijs deze toe die u aan de gesplitste definitie wilt toevoegen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Partial Update Split Definition in Environment]

Deze actiemodule werkt een gesplitste definitie voor een specifieke omgeving bij.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Split.io] met [!UICONTROL Workfront Fusion] </a> in dit artikel voor instructies over het verbinden van uw [!DNL Split.io] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecteer of wijs de werkruimte toe waar u een gesplitste definitie wilt bijwerken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>Selecteer of wijs de omgeving toe waar u een gesplitste definitie wilt bijwerken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Typ of wijs de naam van de splitsing toe waarvoor u een definitie wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Update content]</td> 
   <td> <p>Voor elk kenmerk van de splitsing dat u wilt bijwerken, klikt u op <b>[!UICONTROL Add item]</b> en voert u de gewenste wijzigingen in of wijst u deze toe.</p> <p>Voor meer informatie, zie <a href="https://docs.split.io/reference#partial-update-split-definition-in-environment"> Gedeeltelijke Gesplitste Definitie van de Update in Milieu </a> in de [!DNL Split.io] documentatie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comments]</td> 
   <td>Voer opmerkingen in of wijs deze toe die u aan de gesplitste definitie wilt toevoegen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Associate Tags]

Deze actiemodule voegt labels toe aan het opgegeven object.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Split.io] met [!UICONTROL Workfront Fusion] </a> in dit artikel voor instructies over het verbinden van uw [!DNL Split.io] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecteer of wijs de werkruimte toe waar u een markering wilt toevoegen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Name]</td> 
   <td>Voer de naam in of wijs de naam toe van het object waaraan u tags wilt toevoegen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Type]</td> 
   <td> <p>Typ of wijs het type object toe waaraan u tags wilt toevoegen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td> <p>Voor elke tag die u wilt toevoegen, klikt u op <b>[!UICONTROL Add item]</b> en voert u de tag in of wijst u deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Zoekopdrachten

* [[!UICONTROL Get Workspaces]](#get-workspaces)
* [[!UICONTROL Get Environments]](#get-environments)
* [[!UICONTROL Get Splits]](#get-splits)
* [[!UICONTROL List Split Definitions in an Environment]](#list-split-definitions-in-an-environment)
* [[!UICONTROL Get Traffic Types]](#get-traffic-types)

#### [!UICONTROL Get Workspaces]

Deze onderzoeksmodule wint de werkruimten voor een organisatie terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Split.io] met [!UICONTROL Workfront Fusion] </a> in dit artikel voor instructies over het verbinden van uw [!DNL Split.io] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Ga of kaart het maximumaantal werkruimten in u de module tijdens elke cyclus van de scenariouitvoering wilt terugwinnen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Environments]

Deze zoekmodule haalt een lijst met omgevingen op.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Split.io] met [!UICONTROL Workfront Fusion] </a> in dit artikel voor instructies over het verbinden van uw [!DNL Split.io] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecteer of wijs de werkruimte toe die de milieu's bevat u wilt een lijst maken.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Splits]

Deze zoekmodule haalt een lijst met splitsingen op.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Split.io] met [!UICONTROL Workfront Fusion] </a> in dit artikel voor instructies over het verbinden van uw [!DNL Split.io] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecteer of wijs de werkruimte toe die de splitsingen bevat die u wilt weergeven.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Ga of kaart het maximumaantal splitsingen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugwinnen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Split Definitions in an Environment]

Deze zoekmodule haalt een lijst op met gesplitste definities in een bepaalde omgeving.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Split.io] met [!UICONTROL Workfront Fusion] </a> in dit artikel voor instructies over het verbinden van uw [!DNL Split.io] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecteer of wijs de werkruimte toe die de gesplitste definities bevat u wilt een lijst maken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>Selecteer of wijs de omgeving toe die de gesplitste definities bevat die u wilt weergeven.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Ga of kaart het maximumaantal gespleten definities in u de module tijdens elke cyclus van de scenariouitvoering wilt terugwinnen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Traffic Types]

Deze onderzoeksmodule wint een lijst van verkeerstypes terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Split.io] met [!UICONTROL Workfront Fusion] </a> in dit artikel voor instructies over het verbinden van uw [!DNL Split.io] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecteer of wijs de werkruimte toe die de verkeerstypes bevat u van lijst wilt maken.</td> 
  </tr> 
 </tbody> 
</table>
