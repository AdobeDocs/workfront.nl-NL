---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Target-modules
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die gebruiken [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] met modules kunt u records maken, lezen, bijwerken of verwijderen, alle records van een bepaald type weergeven, zoekrecords weergeven op basis van criteria die u opgeeft, of een aangepaste API-aanroep naar de [!DNL Adobe Target] API.
author: Becky
feature: Workfront Fusion
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: b20f08a3c039ac2f1ece9fc4cef7ad5f58421482
workflow-type: tm+mt
source-wordcount: '1786'
ht-degree: 0%

---

# [!DNL Adobe Target] Modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL Adobe Target]en deze verbinding maken met meerdere toepassingen en services van derden. [!DNL Adobe Target] met modules kunt u records maken, lezen, bijwerken of verwijderen, alle records van een bepaald type weergeven, zoekrecords weergeven op basis van criteria die u opgeeft, of een aangepaste API-aanroep naar de [!DNL Adobe Target] API.


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
    </tr>
  </tbody>
</table>


Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

Voordat u de [!DNL Adobe Target] -aansluiting, moet u ervoor zorgen dat aan de volgende voorwaarden wordt voldaan:

* U moet een actieve [!DNL Adobe Target] account.

## Verbinding maken met [!DNL Adobe Target]

Als u een verbinding wilt maken voor uw [!DNL Adobe Target] modules:

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
        <td>Selecteer of u verbinding maakt met een productie- of niet-productieomgeving.
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Selecteer of u verbinding maakt met een serviceaccount of een persoonlijke account.
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
        <td role="rowheader">[!UICONTROL Technical account ID]</td>
        <td>Voer uw [!DNL Adobe] Technische account-id. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Organization ID]</td>
        <td>Voer uw [!DNL Adobe] Organisatie-id. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Tenant]</td>
        <td>
          <p> Meld u aan bij de [!DNL Adobe Experience Cloud], open [!DNL Target]en klik op de knop [!DNL Target] kaart. Gebruik de waarde van de huurder-id zoals vermeld in het URL-subdomein.</p>
          <p>Bijvoorbeeld als uw URL wanneer het programma openen aan [!DNL Adobe Target] is <code>&lt;https://mycompany.experiencecloud.adobe.com/...></code> Dan is je Tenant ID "mijnbedrijf".</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta Scopes]</td>
        <td>Enter <code>ent_marketing_sdk</code>       </td>
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

## [!DNL Adobe Target] modules en hun velden

Wanneer u [!DNL Adobe Target] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Adobe Target] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Handelingen](#actions)

* [Zoekopdrachten](#searches)


### Handelingen

* [[!UICONTROL Create a record]](#create-a-record)

* [[!UICONTROL Make a custom API call]](#make-a-custom-api-call)

* [[!UICONTROL Delete a record]](#delete-a-record)

* [[!UICONTROL Read a record]](#read-a-record)

* [[!UICONTROL Update a record]](#update-a-record)


#### [!UICONTROL Create a record]

Deze actiemodule leidt tot een activiteit AB of XT, een aanbieding, of een publiek.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Target], zie <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Verbinding maken met [!DNL Adobe Target]</a> in dit artikel.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record type]</td>
    <td>
      <p>Selecteer het type record dat u wilt maken.</p>
      <ul>
        <li>
        <b>Eigenschap</b><p>Zie voor meer informatie over velden <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Properties/operation/createProperty">Een eigenschap maken</a> in de Adobe Target API-documentatie.</p>
        </li>
        <li>
        <b>Aanbiedingsaanbeveling</b><p>Zie voor meer informatie over velden <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Offers/operation/createOffer">Nieuwe recs-aanbieding maken</a> in de Adobe Target API-documentatie.</p>
        </li>
        <li>
          <b>[!UICONTROL Offer JSON]</b>
          <p>Doorgaan naar <a href="#offer-fields" class="MCXref xref" >Velden aanbieden</a>.</p>
        </li>
        <li>
          <b>[!UICONTROL Offer Content]</b>
          <p>Doorgaan naar <a href="#offer-fields" class="MCXref xref" >Velden aanbieden</a>.</p>
        </li>
        <li>
        <b>Omgeving</b><p>Zie voor meer informatie over velden <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Environments/operation/createEnvironment">Omgeving maken</a> in de Adobe Target API-documentatie.</p>
        </li>
        <li>
          <b>[!UICONTROL Audience]</b>
          <p>Zie voor meer informatie over velden <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Audiences/operation/createAudience_1_1">publiek maken</a> in de Adobe Target API-documentatie.</p>
        </li>
        <li>
          <b>[!UICONTROL AB Activity]</b>
          <p>Zie voor meer informatie over velden <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Activities/operation/createActivity_4_1">AB-activiteit maken</a> in de Adobe Target API-documentatie.</p>
        </li>
        <li>
          <b>[!UICONTROL XT Activity]</b>
          <p>Doorgaan naar <a href="#xt-activity-fields" class="MCXref xref" >XT-activiteitvelden</a>.</p>
        </li>
        <li>
          <b>[!UICONTROL AP Activity]</b>
          <p>Zie voor meer informatie over velden <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Activities/operation/createActivity_2">AP-activiteit maken</a> in de Adobe Target API-documentatie.</p>
        </li>
        <li>
          <b>[!UICONTROL Response Token]</b>
          <p>Zie voor meer informatie over velden <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Response-tokens/operation/createResponseToken">Responstoken maken</a> in de Adobe Target API-documentatie.</p>
        </li>
      </ul>
    </td>
  </tr>
</tbody>
</table>

<!--

##### AB Activity fields

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Enter or map a name for this activity. The name can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Options]</td>
      <td>
        <p>For each option that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Option local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the option across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map a name for the option. The name must be no more than 250 characters.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer ID]</b>
            </p>
          </li>
          <li>
            <p>Select or map the Offer associated with the option.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Mboxes]</td>
      <td>
        <p>For each Mbox that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p>[!UICONTROL Audience IDs]</p>
            <p>For each audience that you want to add to the Mbox, click <b>[!UICONTROL Add item]</b> and select the Audience ID.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the location across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map a name for the Location. The name must be no more than 250 characters.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selectors]</td>
      <td>
        <p>For each selector that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p>[!UICONTROL Audience IDs]</p>
            <p>For each audience that you want to add to the Mbox, click <b>[!UICONTROL Add item]</b> and select the Audience ID.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the location across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Selector]</b>
            </p>
            <p>Enter or map a string to be used to track the location across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map a name for the Location. The name must be no more than 250 characters.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Experiences]</td>
      <td>
        <p>A list of locations on the page where the content offer is served. A location contains the following:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience local ID]</b>
            </p>
            <p>Enter or map the ID of the experience</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map the name of the experience
</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>For each audience that you want to see the experience, click <b>[!UICONTROL Add item]</b> and enter the Audience ID.
</p>
          </li>
          <li>
            <p><b>[!UICONTROL Visitor Percentage]</b>
            </p>
            <p>Enter or map the percentage of visitors that is allocated to the experience</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Metrics]</td>
      <td><p>For details on metrics, see <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Activities/operation/createActivity_4_1">Create AB activity</a> in the Adobe Target API documentation.</p> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Third Party ID]</td>
      <td>Enter or map an ID to identify this activity. You can choose this ID. This ID must not be the same as another activity, and can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Starts at]</td>
      <td>Enter or map the date and time to start the activity in the format <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ends at]</td>
      <td>Enter or map the date and time to end the activity in the format <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>Enter or map the state of the activity.</p>
        <ul>
          <li>
            <p>[!UICONTROL Approved]</p>
          </li>
          <li>
            <p>[!UICONTROL Deactivated]</p>
          </li>
          <li>
            <p>[!UICONTROL Paused]</p>
          </li>
          <li>
            <p>[!UICONTROL Saved] </p>
          </li>
          <li>
            <p>[!UICONTROL Deleted]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Enter a number that defines the priority of the activity. Higher numbers have higher priority. This value must be between 0 and 999. The default value is 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Auto-allocate traffic]</td>
      <td>
        <p>Enable this option to auto-allocate traffic. Auto-allocating sends more traffic to the more successful experience.</p>
        <p>Select or map the evaluation criteria by which to judge which experience is more successful.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Enter or map the workspace that the activity is associated with</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Property IDs] </td>
      <td>For each property that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and select or map the property's ID.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Reporting audiences]</td>
      <td>
        <p>For each reporting audience that you want to add to the activity, click [!UICONTROL Add item] and enter the following information:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the Reporting Audience across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>Enter or map the Segment to be used in reporting</p>
          </li>
          <li>
            <p><b>[!UICONTROL Metric local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the metric across API requests.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

##### XT-activiteitvelden

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Voer een naam voor deze activiteit in of wijs een naam toe. De naam mag uit maximaal 250 tekens bestaan.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Options]</td>
      <td>
        <p>Voor elke optie die u aan de activiteit wilt toevoegen, klik <b>[!UICONTROL Add item]</b> en vul de volgende velden in:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Option local ID]</b>
            </p>
            <p>Voer een tekenreeks in of wijs een tekenreeks toe die moet worden gebruikt om de optie bij te houden voor verschillende API-aanvragen.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Voer een naam voor de optie in of wijs een naam toe. De naam mag niet meer dan 250 tekens bevatten.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer ID]</b>
            </p>
          </li>
          <li>
            <p>Selecteer of wijs het Voorstel toe verbonden aan de optie.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Locations]</td>
      <td>
        <p>Voor elke box die u aan de activiteit wilt toevoegen, klik <b>[!UICONTROL Add item]</b> en vul de volgende velden in:</p>
        <ul>
          <li>
            <p>[!UICONTROL Audience IDs]</p>
            <p>Voor elk publiek dat u aan Mbox wilt toevoegen, klik <b>[!UICONTROL Add item]</b> en selecteer de publiek-id.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
            </p>
            <p>Voer een tekenreeks in of wijs een tekenreeks toe die moet worden gebruikt om de locatie in API-verzoeken bij te houden.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Voer een naam voor de locatie in of wijs een naam toe. De naam mag niet meer dan 250 tekens bevatten.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Experiences]</td>
      <td>
        <p>Een lijst met locaties op de pagina waar het inhoudsaanbod wordt weergegeven. Een locatie bevat het volgende:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience local ID]</b>
            </p>
            <p>Voer de id van de ervaring in of wijs deze toe</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Voer de naam van de ervaring in of wijs deze toe

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>Voor elk publiek dat u de ervaring wilt zien, klikt u op <b>[!UICONTROL Add item]</b> en voer de publiek-id in.

</p>
          </li>
          <li>
            <p><b>[!UICONTROL Visitor Percentage]</b>
            </p>
            <p>Voer het percentage bezoekers dat aan de ervaring is toegewezen in of wijs dit percentage toe</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Metrics]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Third Party ID]</td>
      <td>Voer een id in of wijs deze toe om deze activiteit te identificeren. U kunt deze id kiezen. Deze id mag niet hetzelfde zijn als een andere activiteit en mag uit maximaal 250 tekens bestaan.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Starts at]</td>
      <td>Voer de datum en tijd in of wijs de datum en tijd aan om de activiteit te starten in de notatie <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ends at]</td>
      <td>Voer de datum en de tijd in om de activiteit in de indeling te beëindigen of wijs de datum en tijd toe <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>Voer de status van de activiteit in of wijs deze toe.</p>
        <ul>
          <li>
            <p>[!UICONTROL Approved]</p>
          </li>
          <li>
            <p>[!UICONTROL Deactivated]</p>
          </li>
          <li>
            <p>[!UICONTROL Paused]</p>
          </li>
          <li>
            <p>[!UICONTROL Saved] </p>
          </li>
          <li>
            <p>[!UICONTROL Deleted]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Voer een getal in dat de prioriteit van de activiteit definieert. Hogere getallen hebben een hogere prioriteit. Deze waarde moet liggen tussen 0 en 999. De standaardwaarde is 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Auto-allocate traffic]</td>
      <td>
        <p>Schakel deze optie in om automatisch verkeer toe te wijzen. De auto-toewijst verzendt meer verkeer naar de succesvolere ervaring.</p>
        <p>Selecteer of kaart de evaluatiecriteria aan om te beoordelen welke ervaring succesvoller is.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Voer de werkruimte in die aan de activiteit is gekoppeld of wijs deze toe</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Property IDs] </td>
      <td>Voor elke eigenschap die u aan de activiteit wilt toevoegen, klikt u op <b>[!UICONTROL Add item]</b> en selecteer of wijs identiteitskaart van het bezit in kaart.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Reporting audiences]</td>
      <td>
        <p>Voor elk rapporterend publiek dat u aan de activiteit wilt toevoegen, klik [!UICONTROL Add item] en voert u de volgende gegevens in:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience local ID]</b>
            </p>
            <p>Ga of kaart een koord in dat moet worden gebruikt om het Publiek van de Rapportering over API verzoeken te volgen.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>Typ of wijs het segment toe dat u wilt gebruiken voor de rapportage</p>
          </li>
          <li>
            <p><b>[!UICONTROL Metric local ID]</b>
            </p>
            <p>Voer een tekenreeks in of wijs een tekenreeks toe die moet worden gebruikt om de metrische gegevens in API-verzoeken bij te houden.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Velden aanbieden

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Voer een naam voor deze activiteit in of wijs een naam toe. De naam mag uit maximaal 250 tekens bestaan.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content]</td>
      <td>
        <p>Voer de inhoud van het aanbod in of wijs deze toe aan de gebruiker.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Voer de id van de werkruimte die aan de aanbieding is gekoppeld in of wijs deze toe. Als deze optie leeg blijft, wordt de aanbieding gekoppeld aan de standaardwerkruimte van de account. Deze functionaliteit is alleen van toepassing op [!DNL Target] Premiumaccounts.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Voer de datum en het tijdstip in waarop deze aanbieding is gewijzigd of wijs de datum en tijd toe.</p>
      </td>
    </tr>
  </tbody>
</table>

<!--

##### Audience fields

>[!NOTE]
>
>Audiences created through Workfront Fusion can only be edit in Fusion or through the API. They cannot be edited from within Target.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Enter or map a name for this audience. The name can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Description]</td>
      <td>
        <p>Enter or map a description of this audience.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Origin]</td>
      <td>
        <p>Select whether this audience's origin is from Target or from the cloud.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Target Rule]</td>
      <td>
        <p>Enable the toggle to make rules AND, that is, all rules must be applied.</p>
        <p>For each rule that you want to apply to the audience, click <b>[!UICONTROL Add item]</b> and enter the JSON of the rule you want to apply. </p>
        <div class="example"><span class="autonumber"><span><b>Example: </b></span></span>
          <p>Example 1:</p>
          <p ><code>&lbrace;</code></p>
                    <p ><code>                "page": "url",</code>
                    </p>
                    <p><code>                "equals":&lbrack;</code>
                    </p>
                    <p ><code>                    "http://www.myhomepage.com/"</code>
                    </p>
                    <p><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;,</code>
                    </p>
                    <p>Example 2</p>
                    <p ><code>            &lbrace;</code>
                    </p>
                    <p><code>                "geo": "region",</code>
                    </p>
                    <p><code>                "matches": &lbrack;</code>
                    </p>
                    <p ><code>                    "california"</code>
                    </p>
                    <p ><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;</code>
                    </p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Enter or map the ID of the workspace associated with the audience. If left blank, the offer is associated with the default workspace of the account. This functionality applies only to [!DNL Target Premium] accounts.</p>
      </td>
    </tr>
  </tbody>
</table>

-->

#### [!UICONTROL Make a custom API call]

Deze module maakt een aangepaste API-aanroep naar de [!DNL Adobe Target] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Target], zie <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Verbinding maken met [!DNL Adobe Target]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL [!DNL Target] Basis-URL]</td>
      <td>Voer uw gegevens in of wijs deze toe [!DNL Target] basis-URL.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Een pad invoeren ten opzichte van {baseURL}/</p>
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
        <p>[!DNL Workfront Fusion] Hiermee worden automatisch machtigingsheaders en x-api-sleutelkoppen toegevoegd.</p>
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
  </tbody>
</table>

#### [!UICONTROL Delete a record]

Deze actiemodule schrapt één enkele activiteit van AB, activiteit XT, Aanbieding, of Publiek.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Target], zie <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Verbinding maken met [!DNL Adobe Target]</a> in dit artikel.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record type]</td>
    <td>Selecteer het type record dat u wilt verwijderen.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record ID]</td>
    <td>Voer de id in van de record die u wilt verwijderen of wijs deze toe.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Read a record]

Deze actiemodule wint gegevens voor één enkele Activiteit, Aanbieding, Publiek, Bezit, of Rapport terug.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Target], zie <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Verbinding maken met [!DNL Adobe Target]</a> in dit artikel.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record type]</td>
    <td>Selecteer het type record dat u wilt lezen.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record ID]</td>
    <td>Voer de id in van de record die u wilt lezen of wijs deze toe.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Update a record]

Deze actiemodule werkt een record bij in Doel.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Target], zie <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Verbinding maken met [!DNL Adobe Target]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record type]</td>
      <td>
        <p>Selecteer het type record dat u wilt bijwerken.</p>
       </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Field names]</td>
      <td>Selecteer de velden die u wilt bijwerken. De velden worden hieronder weergegeven.
          <p>Zie voor meer informatie over velden <a href="https://developer.adobe.com/target/administer/admin-api/">de Adobe Target API-documentatie</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

### Zoekopdrachten

* [[!UICONTROL Get records]](#get-records)

* [[!UICONTROL Search]](#search)


#### [!UICONTROL Get records]

Deze zoekmodule haalt een lijst met records van het geselecteerde type op.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Target], zie <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Verbinding maken met [!DNL Adobe Target]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record type]</td>
      <td>Selecteer het type record dat u wilt bijwerken.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sort by]</td>
      <td>Klik voor elk veld waarop u wilt sorteren op <b>[!UICONTROL Add item]</b> en selecteert u het veld en of de geretourneerde resultaten oplopend of aflopend moeten zijn.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Starts At]</td>
      <td>
        <p>Voer de vroegste datum in waarvoor u records wilt ophalen. </p>
        <p>Voor een lijst met ondersteunde datum- en tijdnotaties raadpleegt u <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Afgedwongen typegebruik in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ends At]</td>
      <td>
        <p>Voer de laatste datum in waarvoor u records wilt ophalen. </p>
        <p>Voor een lijst met ondersteunde datum- en tijdnotaties raadpleegt u <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Afgedwongen typegebruik in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Search]

Deze zoekmodule zoekt naar Activiteiten, Aanbiedingen of Soorten publiek op basis van criteria die u opgeeft.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Target], zie <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Verbinding maken met [!DNL Adobe Target]</a> in dit artikel.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record type]</td>
    <td>Selecteer het type record dat u wilt bijwerken.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Sort by]</td>
    <td>Klik voor elk veld waarop u wilt sorteren op <b>[!UICONTROL Add item]</b> en selecteert u het veld en of de geretourneerde resultaten oplopend of aflopend moeten zijn.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Search criteria]</td>
    <td>Selecteer voor elke regel die u wilt instellen het veld, de operator en de waarde. Klikken <b>[!UICONTROL Add AND rule]</b> om aanvullende regels op te stellen.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Offset]</td>
    <td>
      <p>Voer het nummer in van de eerste reactie die de module moet retourneren. De eerste geretourneerde reactie heeft een verschuiving van <code>0</code>. Gebruik dit veld in combinatie met het [!UICONTROL Maximum number of returned results] om de reacties te pagineren.</p>
      <p>Als u bijvoorbeeld de derde pagina met reacties wilt weergeven, stelt u [!UICONTROL Offset] tot en met 20 [!UICONTROL Maximum number of returned] resulteert in 10.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Limit]</td>
    <td>
      <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren. Gebruik dit veld in combinatie met het [!UICONTROL Offset] om de reacties te pagineren.</p>
      <p>Als u bijvoorbeeld de derde pagina met reacties wilt weergeven, stelt u [!UICONTROL Offset] tot en met 20 [!UICONTROL Maximum number of returned] resulteert in 10.</p>
    </td>
  </tr>
</tbody>
</table>
