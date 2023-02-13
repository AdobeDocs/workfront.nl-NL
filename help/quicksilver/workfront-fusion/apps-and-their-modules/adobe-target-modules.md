---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Target-modules
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die gebruiken [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] met modules kunt u records maken, lezen, bijwerken of verwijderen, alle records van een bepaald type weergeven, zoekrecords weergeven op basis van criteria die u opgeeft, of een aangepaste API-aanroep naar de [!DNL Adobe Target] API.
author: Becky
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2158'
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
      <td >
        <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Product</td>
      <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td>
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
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Voer uw [!DNL Adobe] Client-id. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Voer uw [!DNL Adobe] Clientgeheim. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Organization ID]</td>
        <td>Voer uw [!DNL Adobe] Organisatie-id. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Technical account ID]</td>
        <td>Voer uw [!DNL Adobe] Technische account-id. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].
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
              <p>Selecteer het type bestand dat u uitpakt.</p>
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
    <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Target], zie <a href="#Create" class="MCXref xref" >Verbinding maken met [!DNL Adobe Target]</a> in dit artikel.</td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Record type]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Selecteer het type record dat u wilt maken.</p>
      <ul>
        <li>
          <p>[!UICONTROL AB Activity]</p>
          <p>Doorgaan naar <a href="#AB%C2%A0Activ" class="MCXref xref" >AB-activiteitsvelden</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL XT Activity]</p>
          <p>Doorgaan naar <a href="#XT" class="MCXref xref" >XT-activiteitvelden</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Offer]</p>
          <p>Doorgaan naar <a href="#Offer" class="MCXref xref" >Velden aanbieden</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Audience]</p>
          <p>Doorgaan naar <a href="#Audience" class="MCXref xref" >Poortvelden</a>.</p>
        </li>
      </ul>
    </td>
  </tr>
</tbody>
</table>

##### AB-activiteitsvelden

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
      <td>Voer de datum en de tijd in om de activiteit in de indeling te starten of wijs de datum en tijd toe <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
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
      <td>Voer de werkruimte in of wijs de werkruimte toe die aan de activiteit is gekoppeld</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Property IDs] </td>
      <td>Voor elke eigenschap die u aan de activiteit wilt toevoegen, klikt u op <b>[!UICONTROL Add item]</b> en selecteer of wijs identiteitskaart van het bezit in kaart.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Reporting audiences]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
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
      <td>Voer de datum en de tijd in om de activiteit in de indeling te starten of wijs de datum en tijd toe <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
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
      <td>Voer de werkruimte in of wijs de werkruimte toe die aan de activiteit is gekoppeld</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Property IDs] </td>
      <td>Voor elke eigenschap die u aan de activiteit wilt toevoegen, klikt u op <b>[!UICONTROL Add item]</b> en selecteer of wijs identiteitskaart van het bezit in kaart.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Reporting audiences]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
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
  </tbody>
</table>

##### Poortvelden

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Voer een naam in of wijs een naam toe aan dit publiek. De naam mag uit maximaal 250 tekens bestaan.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content]</td>
      <td>
        <p>Voer een beschrijving van dit publiek in of wijs deze toe.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Target Rule]</td>
      <td>
        <p>Laat de knevel toe om regels te maken EN, dat wil zeggen, alle regels moeten worden toegepast.</p>
        <p>Voor elke regel die u op het publiek wilt toepassen, klikt u op <b>[!UICONTROL Add item]</b> en voert u de JSON in van de regel die u wilt toepassen. </p>
        <div class="example"><span class="autonumber"><span><b>Voorbeeld: </b></span></span>
          <p>Voorbeelden:</p>
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
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Workspace]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Voer de id van de werkruimte die aan het publiek is gekoppeld in of wijs deze toe. Als deze optie leeg blijft, wordt de aanbieding gekoppeld aan de standaardwerkruimte van de account. Deze functionaliteit is alleen van toepassing op [!DNL Target Premium] rekeningen.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Make a custom API call]

Deze module maakt een aangepaste API-aanroep naar de [!DNL Adobe Target] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Target], zie <a href="#Create" class="MCXref xref" >Verbinding maken met [!DNL Adobe Target]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL [!DNL Target] Basis-URL]</td>
      <td>Voer uw [!DNL Target] basis-URL.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Voer een pad in dat is gebaseerd op {baseURL}/</p>
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
    <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Target], zie <a href="#Create" class="MCXref xref" >Verbinding maken met [!DNL Adobe Target]</a> in dit artikel.</td>
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
    <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Target], zie <a href="#Create" class="MCXref xref" >Verbinding maken met [!DNL Adobe Target]</a> in dit artikel.</td>
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

Deze actiemodule werkt een Activiteit, Aanbieding, of Publiek bij.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Target], zie <a href="#Create" class="MCXref xref" >Verbinding maken met [!DNL Adobe Target]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record type]</td>
      <td>
        <p>Selecteer het type record dat u wilt bijwerken.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL AB Activity]</b>
            </p>
            <p>Zie veldbeschrijvingen in <a href="#AB%C2%A0Activ" class="MCXref xref" >AB-activiteitsvelden</a> krachtens <a href="#Create2" class="MCXref xref" >Een record maken</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL XT Activity]</b>
            </p>
            <p>Zie veldbeschrijvingen in <a href="#XT" class="MCXref xref" >XT-activiteitvelden</a> krachtens <a href="#Create2" class="MCXref xref" >Een record maken</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Other Activity]</b>
            </p>
            <p>Selecteer het veld waarvoor u een waarde wilt bijwerken en voer vervolgens de nieuwe waarde voor het veld in.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer]</b>
            </p>
            <p>Zie veldbeschrijvingen in <a href="#Offer" class="MCXref xref" >Velden aanbieden</a> krachtens <a href="#Create2" class="MCXref xref" >Een record maken</a>.</p>
          </li>
          <li>
            <p><b>[!DNL Audience]</b>
            </p>
            <p>Zie veldbeschrijvingen in <a href="#Audience" class="MCXref xref" >Poortvelden</a> krachtens <a href="#Create2" class="MCXref xref" >Een record maken</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record ID]</td>
      <td>Voer de id in van de record die u wilt bijwerken of wijs deze toe.</td>
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
      <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Target], zie <a href="#Create" class="MCXref xref" >Verbinding maken met [!DNL Adobe Target]</a> in dit artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record type]</td>
      <td>Selecteer het type record dat u wilt bijwerken.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sort by]</td>
      <td>Voor elk veld waarop u wilt sorteren, klikt u op <b>[!UICONTROL Add item]</b> en selecteert u het veld en of de geretourneerde resultaten oplopend of aflopend moeten zijn.</td>
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
    <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Target], zie <a href="#Create" class="MCXref xref" >Verbinding maken met [!DNL Adobe Target]</a> in dit artikel.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record type]</td>
    <td>Selecteer het type record dat u wilt bijwerken.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Sort by]</td>
    <td>Voor elk veld waarop u wilt sorteren, klikt u op <b>[!UICONTROL Add item]</b> en selecteert u het veld en of de geretourneerde resultaten oplopend of aflopend moeten zijn.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Search criteria]</td>
    <td>Voor elke regel die u wilt instellen, selecteert u het veld, de operator en de waarde. Klikken <b>[!UICONTROL Add AND rule]</b> om aanvullende regels op te stellen.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Offset]</td>
    <td>
      <p>Voer het nummer in van de eerste reactie die de module moet retourneren. De eerste geretourneerde reactie heeft een verschuiving van <code>0</code>. Gebruik dit veld in combinatie met het [!UICONTROL Maximum number of returned results] om de reacties te pagineren.</p>
      <p>Als u bijvoorbeeld de derde pagina met reacties wilt weergeven, stelt u [!UICONTROL Offset] tot en met 20 en [!UICONTROL Maximum number of returned] resulteert in 10.</p>
    </td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Maximum number of returned results]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren. Gebruik dit veld in combinatie met het [!UICONTROL Offset] om de reacties te pagineren.</p>
      <p>Als u bijvoorbeeld de derde pagina met reacties wilt weergeven, stelt u [!UICONTROL Offset] tot en met 20 en [!UICONTROL Maximum number of returned] resulteert in 10.</p>
    </td>
  </tr>
</tbody>
</table>
