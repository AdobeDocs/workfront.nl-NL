---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Anaplan-modules
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die Anaplan gebruiken, evenals het met veelvoudige derdetoepassingen en de diensten verbinden.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: 03bcd0a4-c8ec-4f44-b1e1-b57e79595309
source-git-commit: 43b64d1371438909063d2ac81cccb90b97179dfc
workflow-type: tm+mt
source-wordcount: '1555'
ht-degree: 0%

---

# [!DNL Anaplan] Modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL Anaplan]en deze verbinding maken met meerdere toepassingen en services van derden.

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

Voordat u de [!DNL Anaplan] -aansluiting, moet u ervoor zorgen dat aan de volgende voorwaarden wordt voldaan:

* U moet een actieve [!UICONTROL Anaplan] account.
* U moet Werkruimten, Modellen, en andere vormen [!DNL Anaplan] objecten in uw [!UICONTROL Anaplan] account voor [!DNL Workfront Fusion] kan met hen communiceren.

## Verbinden [!DNL Anaplan] tot [!DNL Workfront Fusion] {#connect-anaplan-to-workfront-fusion}

Als u een verbinding wilt maken voor uw [!DNL Anaplan] modules:

1. Klikken **[!UICONTROL Add]** naast de [!UICONTROL Connection] doos.
1. Selecteer het verbindingstype.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL Basic]</td> 
      <td> <p>An [!DNL Anaplan] [!UICONTROL Basic] Voor het maken van de verbinding is alleen een e-mailadres en wachtwoord vereist. </p> <p>Voer een naam voor de verbinding in en voer vervolgens uw e-mailadres en het wachtwoord van uw [!DNL Anaplan] account.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL CA Certificate]</td> 
      <td> <p>An [!DNL Anaplan] [!UICONTROL CA Certificate] verbinding vereist een [!UICONTROL Certificate Key], [!UICONTROL Encoded Data], en [!UICONTROL Encoded Signed Data]. U kunt deze genereren in uw [!DNL Anaplan] account. Zie voor instructies de [!DNL Anaplan] documentatie.</p> <p>Voer een naam in voor de verbinding en voer vervolgens de [!UICONTROL Certificate Key], [!UICONTROL Encoded Data], en [!UICONTROL Encoded Signed Data] die u in uw [!DNL Anaplan] account.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **[!UICONTROL Continue]** om de verbinding op te slaan en terug te keren naar de module.

## [!DNL Anaplan] modules en hun velden

Wanneer u [!DNL Anaplan] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Anaplan] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Handelingen](#actions)
* [Zoekopdrachten](#searches)

### Triggers

#### [!DNL Watch records]

Deze triggermodule start een scenario wanneer een record van het gekozen type wordt gemaakt of bijgewerkt.

>[!NOTE]
>
>Deze module keert de gegevens van nieuwe verslagen terug. De gegevens van gewijzigde bestaande records worden niet geretourneerd.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Anaplan], zie <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] tot [!DNL Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Type object dat moet worden gecontroleerd</td> 
   <td>Selecteer het type item dat u wilt controleren. Het scenario begint wanneer dit type record wordt gemaakt of bijgewerkt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">&lt;object&gt; ID</td> 
   <td>Voer de id in van het object in Anaplan, zoals een model of module, dat is gekoppeld aan de objecten die u wilt controleren</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limiet</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module aan [actie] tijdens elke cyclus van de scenariouitvoering wilt.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Handelingen

* [[!UICONTROL Create a list item]](#create-a-list-item)
* [[!UICONTROL Make a custom API Call]](#make-a-custom-api-call)
* [[!UICONTROL Read a record]](#read-a-record)
* [[!UICONTROL Run an action]](#run-an-action)
* [[!UICONTROL Update a record]](#update-a-record)
* [[!UICONTROL Upload a file]](#upload-a-file)

#### [!UICONTROL Create a list item]

Deze actiemodule voegt een nieuw punt aan een lijst in Anaplan toe.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Connection]</td>
        <td>Voor instructies over het maken van een verbinding met [!DNL Anaplan], zie <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] tot [!DNL Workfront Fusion]</a> in dit artikel.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Workspace ID]</td>
        <td>Selecteer of wijs identiteitskaart van de Werkruimte Anaplan toe die de lijst bevat waar u een punt wilt toevoegen.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Model ID]</td>
        <td>Selecteer of wijs identiteitskaart van het Model toe dat de lijst bevat waar u een punt wilt toevoegen.</td>
    </tr>
    <tr>
        <td>[!UICONTROL List ID]</td>
        <td>Selecteer of wijs identiteitskaart van de Lijst toe waar u een punt wilt tot stand brengen.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Name]</td>
        <td>Voer een naam in voor het nieuwe item.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Code]</td>
        <td>Voer de code voor het nieuwe item in. Codes zijn door de gebruiker gegenereerde codes waarmee u onderscheid kunt maken tussen regelitems met dezelfde naam.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Parent]</td>
        <td>Voer de naam in van het bovenliggende item waarop u het nieuwe item wilt maken.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Properties]</td>
        <td>Als de lijst waaraan u een item wilt toevoegen aangepaste eigenschappen heeft, selecteert u de eigenschappen waarvoor u waarden wilt toevoegen en voegt u vervolgens de waarden toe.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Subsets]</td>
        <td>Als de lijst waaraan u items wilt toevoegen aangepaste subsets bevat, selecteert u de subsets waaraan u het item wilt toevoegen en selecteert u vervolgens <b>[!UICONTROL Yes]</b> om het nieuwe item aan die subset toe te voegen.</td>
    </tr>
</table>

#### [!UICONTROL Make a custom API Call]

Met deze module kunt u een aangepaste API-aanroep naar de [!DNL Anaplan] API.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Anaplan], zie <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] tot [!DNL Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Een pad invoeren ten opzichte van <code>https://api.anaplan.com/2/0/</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] voegt automatisch machtigingsheaders toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String] </td> 
   <td> <p>Voer de queryreeks voor de aanvraag in.</p> </td> 
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

#### [!UICONTROL Delete a record]

Met deze actiemodule verwijdert u een bestaande record.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Anaplan], zie <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] tot [!DNL Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Selecteer of wijs identiteitskaart van de Werkruimte Anaplan toe die het voorwerp bevat u wilt schrappen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model ID]</td> 
   <td>Voer de id in van het model dat het object bevat dat u wilt verwijderen of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Verwijderen</td> 
   <td> <p>Selecteer het type object dat u wilt verwijderen.</p> 
    <ul> 
     <li> <p><b>Handeling</b> </p> <p>Selecteer of wijs de actie toe om te schrappen.</p> </li> 
     <li> <p><b>Lijstitem</b> </p> <p>Selecteer de lijst waarvan u een item wilt verwijderen en voer de id of de code in van het item dat u wilt verwijderen.</p>  </li> 
     <li> <p><b>[!UICONTROL File]</b> </p> <p>Selecteer of wijs het bestand toe dat u wilt verwijderen.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Read a record]

Deze actiemodule leest één record.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Anaplan], zie <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] tot [!DNL Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Selecteer het type record dat u wilt lezen.</p> 
    <ul> 
     <li> <p><b>Model</b> </p> <p>Selecteer of wijs identiteitskaart van het Model toe u wilt lezen</p> </li> 
     <li> <p><b>Modellijst</b> </p> <p>Selecteer of wijs identiteitskaarts van de Werkruimte en het Model toe die de Lijst bevatten u wilt lezen, dan de Lijst selecteren. In de [!UICONTROL Data type] in het veld selecteert u of u gegevens of metagegevens wilt lezen.</p> </li> 
     <li> <p><b>Modelversie</b> </p> <p>Selecteer of wijs identiteitskaart van het Model toe u wilt lezen.</p> </li> 
     <li> <p><b>Gebruiker</b> </p> <p>Selecteer of u gegevens wilt retourneren over de eigenaar van de account die wordt gebruikt, of een andere gebruiker. Als u een andere gebruiker selecteert, selecteert u de naam van de gebruiker.</p> </li> 
     <li> <p><b>Werkruimte</b> </p> <p>Selecteer of wijs identiteitskaart van de Werkruimte toe u wilt lezen.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Run an action]

Met deze actiemodule kunt u een handeling importeren, exporteren, verwijderen of verwerken.

<table style="table-layout:auto"> 
     <col/>
     <col/>
     <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Connection]</td>
        <td>Voor instructies over het maken van een verbinding met [!DNL Anaplan], zie <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect Anaplan to Workfront Fusion]</a> in dit artikel.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Workspace ID]</td>
        <td>Selecteer of wijs identiteitskaart van toe [!DNL Anaplan] Werkruimte waar u de handeling wilt uitvoeren</td>
      </tr>
      <tr >
        <td role="rowheader">[!UICONTROL Model ID]</td>
        <td>Selecteer of wijs identiteitskaart van het Model toe waar u de actie wilt uitvoeren.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Action type]</td>
        <td>
          <p>Selecteer de handeling die u wilt uitvoeren</p>
            <ul>
              <li>
                <p><b>[!UICONTROL Delete]</b>
                </p>
                <p>Voer de id in van de handeling die u wilt verwijderen of wijs deze toe.</p>
              </li>
              <li>
                <p><b>[!UICONTROL Export]</b>
                </p>
                <p>Voer de id in van de exportdefinitie die u wilt gebruiken of wijs deze toe. U kunt exporteren naar de volgende bestandsindelingen:</p>
                  <ul>
                    <li>
                      <p>XLS</p>
                    </li>
                    <li>
                      <p>XLSX</p>
                    </li>
                    <li>
                      <p>CSV</p>
                    </li>
                  </ul>
                </li>
                <li>
                  <p><b>[!UICONTROL Import] </b>
                  </p>
                  <p style="font-weight: normal;">Voer de id in van de importdefinitie die u wilt gebruiken of wijs deze toe.</p>
                </li>
                <li>
                 <p><b>[!UICONTROL Process]</b>
                 </p>
                  <p>Voer de id in van het proces dat u wilt gebruiken of wijs deze toe. </p>
                </li>
              </ul>
            </td>
          </tr>
        </tbody>
      </table>


#### [!UICONTROL Update a record]

Deze actiemodule werkt één record bij in [!UICONTROL Anaplan].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Anaplan], zie <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] tot [!DNL Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Selecteer het type record dat u wilt bijwerken.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL List item]</b> </p> <p>Zie voor velden <a href="#create-a-list-item" class="MCXref xref">Een lijstitem maken</a> in dit artikel.</p> </li> 
     <li> <p><b>[!UICONTROL Module cell data]</b> </p> <p>Wanneer u celgegevens bijwerkt, worden ook alle downstreamberekeningen bijgewerkt die die gegevens gebruiken.</p> <p>Vul de volgende velden in:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Model ID]</b> </p> <p>Selecteer of wijs het Model toe dat de cel bevat u wilt bijwerken.</p> </li> 
       <li> <p><b>[!UICONTROL Module ID]</b> </p> <p>Selecteer of wijs de Module toe die de cel bevat u wilt bijwerken</p> </li> 
       <li> <p><b>[!UICONTROL Line item name]</b> </p> <p>Selecteer of wijs het lijnpunt van de cel toe u wilt bijwerken</p> </li> 
       <li> <p style="font-weight: bold;">[!UICONTROL Dimension ID]</p> <p>Selecteer of wijs de afmeting toe die op het lijnpunt is.</p> 
       <p><b>Opmerking: </b> 
       <ul>
       <li> Dimension key (value) moet ofwel <code>dimensionName</code> (volgende) of <code>dimensionId</code> (ID).</li>
       <li>Itemsleutel (waarde) moet zijn <code>itemName</code> (tekst), <code>itemCode</code> (tekst), of <code>itemId</code> (ID).</li>
       <li>Dimension- en itemtoetsen moeten van hetzelfde type zijn (tekst of id).
       </ul>
        </p> 
        <p>Voor meer informatie over de afmetingen zoekt u naar Dimension in het dialoogvenster [!DNL Anaplan Anapedia].</p> </li> 
       <li> <p><b>[!UICONTROL Value]</b> </p> <p>Voer de nieuwe waarde voor de cel in of wijs deze toe.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Model current fiscal year]</b> </p> <p>Voer de werkruimte-id en de model-id in van het model waarvoor u het belastingjaar wilt bijwerken en voer vervolgens het nieuwe jaar voor het model in of wijs dit toe.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Upload a file]

Deze actiemodule uploadt een bestand naar Anaplan. Het bestand moet al zijn geüpload naar Anaplan. U kunt deze module gebruiken om het aan extra plaatsen binnen Anaplan te uploaden.
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL Connection]</td>
<td>Voor instructies over het maken van een verbinding met [!DNL Anaplan], zie <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] tot [!DNL Workfront Fusion]</a> in dit artikel.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL Workspace ID]</td>
<td>Selecteer of wijs identiteitskaart van toe [!DNL Anaplan] Werkruimte waarin u een bestand wilt uploaden.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL Model ID]</td>
<td>Selecteer of wijs identiteitskaart van het Model toe waar u een dossier wilt uploaden.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL File ID]</td>
<td>Selecteer of wijs identiteitskaart van het dossier toe u wilt uploaden.</td>
</tr>
</tbody>
</table>
</div>

### Zoekopdrachten

#### [!UICONTROL Get record]

Deze zoekmodule retourneert alle toegankelijke records van het geselecteerde type.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Anaplan], zie <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] tot [!DNL Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record types]</td> 
   <td> <p>Selecteer het type record dat u wilt ophalen.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Workspaces]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Models]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Line items]</b> </p> <p>Selecteer of wijs identiteitskaart van het Model toe dat identiteitskaart bevat [!DNL line] objecten die u wilt ophalen.</p> </li> 
       <li> <p><b>[!UICONTROL Model lists]</b> </p> <p>Selecteer of wijs identiteitskaart van de Werkruimte en Model identiteitskaart toe die de Modellijsten bevatten u wilt terugwinnen.</p> </li> 
       <li> <p><b>[!UICONTROL Model calendar]</b> </p> <p>Selecteer of wijs identiteitskaart van de Werkruimte toe die de Model kalender bevat u wilt terugwinnen.</p> </li> 
       <li> <p><b>Modelversies</b> </p> </li> 
       <li> <p>Selecteren of toewijzen [!UICONTROL ]De id van het model dat de modelversies bevat die u wilt ophalen.</p> </li> 
       <li> <p><b>[!UICONTROL Users]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Views]</b> </p> <p>Selecteer of u de mening door Module of door Model wilt kiezen, dan selecteer of kaart identiteitskaart van de Module of het Model dat de mening bevat u wilt terugwinnen.</p> </li> 
      </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Return workspace size]</td> 
   <td>Schakel deze optie in om een schatting van de huidige grootte van de werkruimte te retourneren. Deze schatting is gebaseerd op de grootte van alle modules in de werkruimte.</td> 
  </tr> 
 </tbody> 
</table>
