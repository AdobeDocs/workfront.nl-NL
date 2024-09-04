---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Azure DevOps-modules
description: In een  [!DNL Adobe Workfront Fusion]  scenario, kunt u werkschema's automatiseren die  [!DNL Azure DevOps] gebruiken, evenals het met veelvoudige derdetoepassingen en de diensten verbinden.
author: Becky
feature: Workfront Fusion
exl-id: ecaa93c9-47bb-4fe1-87b4-d2e117cc68ae
source-git-commit: ed7ea1d3409c39caea5fe8b107b7b2907dc87d76
workflow-type: tm+mt
source-wordcount: '1541'
ht-degree: 0%

---

# [!DNL Azure DevOps] modules

In een [!DNL Adobe Workfront Fusion] -scenario kunt u workflows automatiseren die [!DNL Azure DevOps] gebruiken en deze koppelen aan meerdere toepassingen en services van derden.

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

Als u [!DNL Azure DevOps] -modules wilt gebruiken, hebt u een [!DNL Azure] DevOps-account nodig.

## Verbinden [!DNL Azure DevOps] met [!DNL Workfront Fusion] {#connect-azure-devops-to-workfront-fusion}

1. Voeg een module [!DNL Azure DevOps] toe aan uw scenario.
1. Klik op **[!UICONTROL Add]** naast het veld [!UICONTROL Connection] .
1. Selecteer **[!DNL Azure DevOps]** in het veld [!UICONTROL Connection Type] .

   >[!IMPORTANT]
   >
   >Het verbindingstype [!UICONTROL [!DNL Azure DevOps] (Request All Scopes)] wordt in de nabije toekomst vervangen. Daarom raden wij u niet aan het te gebruiken.

1. Vul de volgende velden in:

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL Connection name]</td>
            <td>Voer een naam in voor de verbinding die u maakt.</td>
        </tr>
      <tr>
            <td>[!UICONTROL Organization]</td>
            <td>Voer de naam in van de organisatie waaronder u de [!DNL Azure DevOps] -toepassing hebt gemaakt.</td>
        </tr>
    </table>

1. Klik op **[!UICONTROL Continue]** om het instellen van de verbinding te voltooien en door te gaan met het maken van uw scenario.

## [!UICONTROL Azure DevOps] modules en hun velden

Wanneer u [!DNL Azure DevOps] modules configureert, geeft [!DNL Workfront Fusion] de onderstaande velden weer. Daarnaast kunnen aanvullende [!DNL Azure DevOps] -velden worden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Voor meer informatie, zie [ informatie van de Kaart van één module aan een andere in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Handelingen](#actions)
* [Zoekopdrachten](#searches)

### Triggers

#### [!UICONTROL Watch for work items]

Deze instant trigger-module voert een scenario uit wanneer een record wordt toegevoegd, bijgewerkt of verwijderd in [!UICONTROL Azure DevOps] .

De module retourneert alle standaardvelden die aan de record zijn gekoppeld, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Selecteer of voeg een webhaak voor de module toe.</p> <p>Voor meer informatie over websites in trekkermodules, zie <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref"> Onmiddellijke trekkers (webhooks) in [!DNL Adobe Workfront Fusion]</a>.</p> <p>Voor informatie over hoe te om een webhaak tot stand te brengen, zie <a href="../../workfront-fusion/apps-and-their-modules/webhooks-updated.md" class="MCXref xref"> Webhooks </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Handelingen

* [Een record maken](#create-a-record)
* [Aangepaste API-aanroep](#custom-api-call)
* [Een bijlage downloaden](#download-an-attachment)
* [Werkitems koppelen](#link-work-items)
* [Record lezen](#read-record)
* [Een tijdelijk item bijwerken](#update-a-work-item)
* [[!UICONTROL Upload an attachment]](#upload-an-attachment)

#### [!UICONTROL Custom API Call]

Met deze actiemodule kunt u een aangepaste, geverifieerde aanroep van de [!DNL Azure DevOps] API maken. Op deze manier kunt u een automatisering van de gegevensstroom maken die niet door de andere [!DNL Azure DevOps] -modules kan worden uitgevoerd.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Azure DevOps] met [!UICONTROL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Azure DevOps] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Base URL]</td> 
   <td> <p>Selecteer of wijs de basis-URL toe die u gebruikt om verbinding te maken met uw [!DNL Azure DevOps] -account</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Relative URL]</td> 
   <td> <p>Voer de relatieve URL in waarmee u verbinding wilt maken voor deze API-aanroep.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b> Voorbeeld: </b></span></span><code>{organization}/_apis[/{area}]/{resource}</code> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>Selecteer of wijs de versie van [!DNL Azure DevOps] API toe die u voor deze API vraag wilt verbinden. Als er geen versie is geselecteerd, maakt [!DNL Workfront Fusion] verbinding met [!DNL Azure DevOps] API versie 5.1.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override=""> HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a> voor meer informatie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p> </td> 
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
 </tbody> 
</table>

#### [!UICONTROL Create a record]

Deze actiemodule leidt tot een nieuw project of het werkpunt.

De module geeft de object-id weer voor het nieuwe werkitem of de URL en statuscode van een nieuw gemaakt project.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Azure DevOps] met [!UICONTROL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Azure DevOps] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Selecteer of u een het werkpunt of een project wilt tot stand brengen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Project]</strong> </p> <p>Vul de volgende velden in:</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Name]</strong>:Ga of kaart een naam voor het nieuwe project in.</p> </li> 
       <li> <p><strong>[!UICONTROL Description]</strong>:Ga of kaart een beschrijving voor het nieuwe project in. </p> </li> 
       <li> <p><strong>[!UICONTROL Visibility]</strong>: Selecteer of u wilt dat uw project openbaar of privé is. De gebruikers moeten in uw organisatie worden ondertekend en moeten toegang tot het project hebben verleend om met een privé project in wisselwerking te staan. De openbare projecten zijn zichtbaar aan gebruikers die niet binnen aan uw organisatie worden ondertekend.</p> </li> 
       <li> <p><strong>[!UICONTROL Version control]</strong>: Selecteer of u het project [!DNL Git] of [!UICONTROL Team Foundation Version Control (TFCV)] wilt gebruiken voor versiebeheer.</p> </li> 
       <li> <p><strong>[!UICONTROL Work item process]</strong>: Selecteer het werkproces dat u voor het project wilt gebruiken. De opties zijn [!UICONTROL Basic] , [!UICONTROL Scrum] , [!UICONTROL Capability Maturity Model Integration (CMMI)] en [!UICONTROL Agile] .</p> <p>Voor meer informatie over [!DNL Azure DevOps] processen, zie <a href="https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&amp;tabs=basic-process"> een Proces </a> in de [!DNL Azure DevOps] Documentatie kiezen.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Work item]</strong> </p> <p>Vul de volgende velden in:</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Project]</strong>: Selecteer het project waar u het het werkpunt wilt tot stand brengen.</p> </li> 
       <li> <p><strong>[!UICONTROL Work item type]</strong>: Selecteer het type werkitem dat u wilt maken.</p> </li> 
       <li> <p><strong>[!UICONTROL Other fields]</strong>:Op deze gebieden, ga de waarde in die u het het werkpunt voor een bepaalde bezit wilt hebben. Beschikbare velden zijn afhankelijk van het type werkitem.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download an attachment]

Deze actiemodule downloadt een bijlage.

De module retourneert de bestandsinhoud van de bijlage.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Azure DevOps] met [!UICONTROL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Azure DevOps] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Attachment URL]</td> 
   <td> <p>Voer de URL in van de bijlage die u wilt downloaden of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Link work items]

Deze actiemodule verbindt twee het werkpunten en bepaalt het verband tussen hen.

De module retourneert de id van het hoofdwerkitem en alle bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Azure DevOps] met [!UICONTROL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Azure DevOps] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item ID]</td> 
   <td>Voer de id in van het hoofdwerkitem waarnaar u een ander werkitem wilt koppelen of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Linked work item ID]</td> 
   <td>Voer de id in van het werkitem dat u wilt koppelen aan het hoofdwerkitem of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Link Type]</td> 
   <td> <p>Bepaal de verhouding tussen de het werkpunten die u wilt verbinden.</p> <p>Voor meer informatie, zie <a href="https://docs.microsoft.com/en-us/azure/devops/boards/queries/link-type-reference?view=azure-devops"> Verwijzing van het Type van Verbinding </a> in de [!UICONTROL Azure DevOps] Documentatie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment]</td> 
   <td>Voer de tekst van een opmerking in of wijs deze toe. Dit is nuttig om de redenering of de intentie van het verband uit te leggen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Read record]

Deze actiemodule leest gegevens uit één record in [!DNL Azure DevOps] .

U geeft de id van de record op.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Azure DevOps] met [!UICONTROL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Azure DevOps] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Selecteer of u een project of een het werkpunt wilt lezen</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Project]</strong>: Selecteer het project dat u wilt lezen.</p> </li> 
     <li> <p><strong>[!UICONTROL Work item]</strong>: Selecteer het project dat het het werkpunt bevat u wilt lezen, dan het type van het het werkpunt selecteren.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Selecteer de informatie die u in de uitvoerbundel voor deze module wilt opnemen. Beschikbare velden zijn afhankelijk van het type werkitem.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Voer de id in van de record die u wilt lezen of wijs deze toe.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a work item]

Deze actiemodule werkt een bestaand werkitem bij met behulp van de bijbehorende id.

De module keert identiteitskaart van het bijgewerkte het werkpunt terug.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Azure DevOps] met [!UICONTROL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Azure DevOps] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td>Selecteer het project dat het het werkpunt bevat u wilt bijwerken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work Item Type]</td> 
   <td> <p>Selecteer het type werkitem dat u wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Other Fields]</td> 
   <td>Op elk van deze gebieden, ga de waarde in die u het het werkpunt voor een bepaalde bezit wilt hebben. Beschikbare velden zijn afhankelijk van het type werkitem.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item ID]</td> 
   <td>Voer de id in van het werkitem dat u wilt bijwerken of wijs deze toe.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Upload an attachment]

Deze actiemodule uploadt een bestand en koppelt dit aan een tijdelijk item.

De module retourneert de bijlage-id en een download-URL voor de bijlage.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Azure DevOps] met [!UICONTROL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Azure DevOps] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project] </td> 
   <td> <p>Selecteer het project waar u een gehechtheid wilt uploaden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item ID]</td> 
   <td> <p>Ga of kaart identiteitskaart van het het werkpunt in waar u een gehechtheid wilt uploaden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment]</td> 
   <td>Voer de tekst in van een opmerking die u aan de geüploade bijlage wilt toevoegen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file] </td> 
   <td>Selecteer een bronbestand uit een vorige module of voer de naam en inhoud van het bronbestand in of wijs deze toe.</td> 
  </tr> 
 </tbody> 
</table>

### Zoekopdrachten

#### [!UICONTROL List work items]

Deze actiemodule wint alle het werkpunten van een specifiek type in een [!DNL Azure DevOps] project terug.

De module retourneert de id van het hoofdwerkitem en alle bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Azure DevOps] met [!UICONTROL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Azure DevOps] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td>Selecteer het project waarvan u de het werkpunten wilt terugwinnen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item type]</td> 
   <td> <p>Selecteer het type werkitem dat u wilt ophalen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Selecteer de eigenschappen die u in de uitvoer van de module wilt weergeven. De beschikbare velden zijn afhankelijk van het type werkitem dat u wilt ophalen. U moet ten minste één eigenschap selecteren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Voer het maximale aantal werkitems in dat [!DNL Workfront Fusion] tijdens één uitvoeringscyclus retourneert of wijs dit toe.</td> 
  </tr> 
 </tbody> 
</table>
