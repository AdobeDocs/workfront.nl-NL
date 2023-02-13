---
title: Jira-softwaremodules
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die gebruiken [!DNL Jira] Software, en sluit het aan veelvoudige derdetoepassingen en de diensten aan.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 0%

---

# [!DNL Jira Software] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL Jira Software]en deze verbinding maken met meerdere toepassingen en services van derden.

Als u instructies bij het creëren van een scenario nodig hebt, zie [Een scenario maken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Voor informatie over modules, zie [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

<!-- Bob Fix this compared to original -->

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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Vereisten

Te gebruiken [!DNL Jira] modules u moet hebben [!DNL Jira] account.

## Verbinden [!DNL Jira Software] tot [!DNL Workfront Fusion]

Uw verbindingsmethode is gebaseerd op of u gebruikt [!DNL Jira Cloud] of [!DNL Jira Server].

* [Verbinden [!DNL Jira Cloud] naar Workfront Fusion](#connect-jira-cloud-to-workfront-fusion)
* [Verbinden [!DNL Jira Server] tot [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### Verbinden [!DNL Jira Cloud] tot [!DNL Workfront Fusion]

Verbinden [!DNL Jira Cloud] tot [!DNL Workfront Fusion]

Verbinding maken [!DNL Jira Software] tot [!DNL Workfront Fusion], moet u een API-token maken en deze samen met uw Service URL en gebruikersnaam aan de [!UICONTROL Create a connection] veld in [!DNL Workfront Fusion].

#### Een API-token maken in [!DNL Jira]

1. Ga naar [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) en aanmelden.
1. Klik op **[!UICONTROL Create API token]**.
1. Typ een naam voor het token, zoals *Workfront Fusion*.
1. Kopieer het token met de **[!UICONTROL Copy to clipboard]** knop.

   >[!IMPORTANT]
   >
   >U kunt het token niet meer weergeven nadat u dit dialoogvenster hebt gesloten.
1. Sla het gegenereerde token op een veilige plaats op.
1. Doorgaan met [Configureer de [!DNL Jira] API-token in [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion).

#### Configureer de [!DNL Jira] API-token in [!DNL Workfront Fusion]

1. In [!DNL Workfront Fusion], voegt u een [!DNL Jira] aan een scenario om te openen **[!UICONTROL Create a connection]** doos.
1. Geef de volgende informatie op:

   * **[!UICONTROL Service URL]**
   * **[!UICONTROL Username]**
   * **[!UICONTROL API token]:** Dit is de API-token die u hebt gemaakt in het dialoogvenster [Een API-token maken in [!DNL Jira]](#create-an-api-token-in-jira) van dit artikel.

1. Klikken [!UICONTROL Continue] om de verbinding tot stand te brengen en aan de module terug te keren.

### Verbinden [!DNL Jira Server] tot [!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

Een verbinding autoriseren tussen [!DNL Workfront Fusion] en [!DNL Jira Server], hebt u uw Consumentensleutel, Privé Sleutel, en de Dienst URL nodig. Mogelijk moet u contact opnemen met uw [!DNL Jira] beheerder voor deze informatie.

* [Genereer openbare en persoonlijke sleutels voor uw [!DNL Jira] verbinding](#generate-public-and-private-keys-for-your-jira-connection)
* [De clienttoepassing configureren als een consument in [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [Verbinding maken met [!DNL Jira] Server- of Jira-datacenter in [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Genereer openbare en persoonlijke sleutels voor uw [!DNL Jira] verbinding

Als u een persoonlijke sleutel voor uw [!DNL Workfront Fusion Jira] verbinding, moet u openbare en privé sleutels produceren.

1. In uw terminal, stel het volgende in werking `openssl` opdrachten.

   * `openssl genrsa -out jira_privatekey.pem 1024`

      Met deze opdracht wordt een persoonlijke sleutel van 1024 bits gegenereerd.

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

      Met deze opdracht maakt u een X509-certificaat.

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

      Met deze opdracht wordt de persoonlijke sleutel (PKCS8-indeling) geëxtraheerd naar de `jira_privatekey.pcks8`
bestand.

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

      Met deze opdracht haalt u de openbare sleutel uit het certificaat naar het `jira_publickey.pem` bestand.

      >[!NOTE]
      >
      >Als u Vensters gebruikt, zou u de openbare sleutel aan kunnen moeten bewaren `jira_publickey.pem` bestand handmatig:
      >
      >1. In uw terminal, stel het volgende bevel in werking:
      >   
      >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
      >   
      >1. Kopieer de terminaluitvoer (inclusief `-------BEGIN PUBLIC KEY--------` en `-------END PUBLIC KEY--------`
      >   
      >1. Plak de einduitvoer in een bestand met de naam `jira_publickey.pem`.



1. Doorgaan naar [De clienttoepassing configureren als een consument in [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)

#### De clienttoepassing configureren als een consument in [!DNL Jira]

1. Meld u aan bij uw [!DNL Jira] -instantie.
1. Klik in het navigatievenster aan de linkerkant op **[!UICONTROL [!DNL Jira] Settings]** ![](assets/jira-settings-icon.png) > **[!UICONTROL Applications]**> **[!UICONTROL Application links]**.
1. In de **[!UICONTROL Enter the URL of the application you want to link]** veld, Enter

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. Klik op **[!UICONTROL Create new link]**. Negeer het foutbericht &quot;Er is geen reactie ontvangen van de URL die u hebt ingevoerd&quot;.
1. In de **[!UICONTROL Link applications]** venster, voert u waarden in in de **[!UICONTROL Consumer key]** en **[!UICONTROL Shared secret]** velden.

   U kunt de waarden voor deze velden kiezen.

1. Kopieer de waarden van de **[!UICONTROL Consumer key]** en **[!UICONTROL Shared secret]** velden naar een beveiligde locatie.

   U zult deze waarden later in het configuratieproces vereisen.

1. Vul de URL-velden als volgt in:

   | Veld | Beschrijving |
   |---|---|
   | [!UICONTROL Request Token URL] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL Authorization URL] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL Access Token URL] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. Selecteer **[!UICONTROL Create incoming link]** selectievakje.
1. Klik op **[!UICONTROL Continue]**.
1. In de **[!UICONTROL Link applications]** venster, vult de volgende velden in:

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Consumer Key]</p> </td> 
      <td> Plak in de consumentensleutel die u naar een beveiligde locatie hebt gekopieerd.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Consumer name]</td> 
      <td>Voer een naam van uw keuze in. Deze naam is voor uw eigen referentie.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Public key]</td> 
      <td>Plak de openbare sleutel vanuit uw <code>[!DNL jira_publickey.pem]</code> bestand.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klik op **[!UICONTROL Continue]**.
1. Doorgaan naar [Verbinding maken met [!DNL Jira Server] of [!DNL Jira Data Center] in [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Verbinding maken met [!DNL Jira Server] of [!DNL Jira Data Center] in [!DNL Workfront Fusion]

>[!NOTE]
>
>Gebruik de [!DNL Jira Server] toepassing om verbinding te maken met [!DNL Jira Server] of [!DNL Jira Data Center].
1. In alle [!DNL Jira Server] module in [!DNL Workfront Fusion], klikt u op **[!UICONTROL Add]** naast de [!UICONTROL connection] veld.
1. In de [!UICONTROL Create a connection] vult de volgende velden in:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td> <p>Geef een naam op voor de verbinding</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Consumer Key]</td> 
      <td>Plak in de consumentensleutel die u naar een beveiligde locatie hebt gekopieerd <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">De clienttoepassing configureren als een consument in [!DNL Jira]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>Plakken in de persoonlijke sleutel vanuit de <code>[!DNL jira_privatekey.pcks8]</code> bestand dat u hebt gemaakt in <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">Genereer openbare en persoonlijke sleutels voor uw [!DNL Jira] verbinding</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>Voer uw [!DNL Jira] instantie-URL. </td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **[!UICONTROL Continue]** om de verbinding tot stand te brengen en terug naar de module te gaan.

## [!DNL Jira Software] modules en hun velden

Wanneer u [!DNL Jira Software] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Jira Software] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Handelingen](#actions)
* [Zoekopdrachten](#searches)

### Triggers

#### [!UICONTROL Watch for records]

Deze triggermodule start een scenario wanneer een record wordt toegevoegd, bijgewerkt of verwijderd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Selecteer de webhaak die u wilt gebruiken om te controleren op records. </p> <p>Een nieuwe webhaak toevoegen:</p> 
    <ol> 
     <li value="1">Klikken <strong>[!UICONTROL Add]</strong></li> 
     <li value="2">Voer een naam in voor de webhaak.</li> 
     <li value="3"> <p>Selecteer de verbinding die u voor uw webhaak wilt gebruiken. </p> <p>Voor instructies over het aansluiten van uw [!DNL Jira Software] account aan [!DNL Workfront Fusion], zie <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </li> 
     <li value="4"> <p>Selecteer het recordtype waarop u de software wilt letten:</p> 
      <ul> 
       <li>[!UICONTROL Comment] </li> 
       <li>[!UICONTROL Issue]</li> 
       <li>[!UICONTROL Project] </li> 
       <li>[!UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### Handelingen

* [[!UICONTROL Add issue to sprint]](#add-issue-to-sprint)
* [[!UICONTROL Custom API Call]](#custom-api-call)
* [[!UICONTROL Create a Record]](#create-a-record)
* [[!UICONTROL Delete a record]](#delete-a-record)
* [[!UICONTROL Download an attachment]](#download-an-attachment)
* [[!UICONTROL Read a record]](#read-a-record)
* [[!UICONTROL Update a record]](#update-a-record)

#### [!UICONTROL Add issue to sprint]

Deze actiemodule voegt een of meer uitgaven aan een sprint toe.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Jira Software] account aan [!DNL Workfront Fusion], zie <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sprint ID]</td> 
   <td>Typ of wijs de afdruk-id van de sprint toe waaraan u een uitgave wilt toevoegen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Issue ID or Keys]</td> 
   <td>Voeg een Issue ID of Key toe voor elke uitgave die u aan de sprint wilt toevoegen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a Record]

Deze actiemodule maakt een nieuwe record in Jira.

De module retourneert alle standaardvelden die aan de record zijn gekoppeld, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Jira Software] account aan [!DNL Workfront Fusion], zie <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type record dat de module moet maken. Wanneer u een recordtype selecteert, worden andere velden die specifiek zijn voor dat recordtype, weergegeven in de module.</p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Custom API Call]

Deze actiemodule laat u een douane voor authentiek verklaarde vraag aan het maken [!DNL Jira Software] API. Op deze manier kunt u een automatisering van de gegevensstroom maken die niet door de ander kan worden uitgevoerd [!DNL Jira Software] modules.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Jira Software] account aan [!DNL Workfront Fusion], zie <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Een pad invoeren ten opzichte van<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] Hiermee voegt u de machtigingsheaders voor u toe.</p> </td> 
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

#### [!UICONTROL Delete a record]

Deze actiemodule verwijdert een bepaalde record.

U geeft de id van de record op.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Jira Software] account aan [!DNL Workfront Fusion], zie <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type record dat de module moet verwijderen. </p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID or Key]</td> 
   <td>Voer de id of sleutel in of wijs deze toe aan de record die u wilt verwijderen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download an attachment]

Deze actiemodule downloadt een bepaalde bijlage.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Jira Software] account aan [!DNL Workfront Fusion], zie <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Voer de id in van de bijlage die u wilt downloaden of wijs deze toe.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Read a record]

Deze actiemodule leest gegevens uit één record in [!DNL Jira Software].

U geeft de id van de record op.

De module retourneert alle standaardvelden die aan de record zijn gekoppeld, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Jira Software] account aan [!DNL Workfront Fusion], zie <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type van [!DNL Jira] neem op u de module wilt lezen.</p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL User]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Selecteer de uitvoer die u wilt ontvangen. Uitvoeropties zijn beschikbaar op basis van het type record dat is geselecteerd in het dialoogvenster "[!UICONTROL Record Type]".</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>De unieke sleutel invoeren of toewijzen [!DNL Jira Software] Id van de record die de module moet lezen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a record]

Deze actiemodule werkt een bestaand record bij, zoals een uitgave of project.

U geeft de id van de record op.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Jira Software] account aan [!DNL Workfront Fusion], zie <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type record dat de module moet bijwerken. Wanneer u een recordtype selecteert, worden andere velden die specifiek zijn voor dat recordtype, weergegeven in de module.</p> 
    <ul> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Transition issue]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID or Key]</td> 
   <td>Voer de id of sleutel in of wijs deze toe aan de record die u wilt bijwerken.</td> 
  </tr> 
 </tbody> 
</table>

### Zoekopdrachten

* [[!UICONTROL List records]](#list-records)
* [[!UICONTROL Search for records]](#search-for-records)

#### [!UICONTROL List records]

Deze zoekmodule haalt alle items van een specifiek type op die overeenkomen met uw zoekopdracht

U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Jira Software] account aan [!DNL Workfront Fusion], zie <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type record dat in de module moet worden vermeld. Wanneer u een recordtype selecteert, worden andere velden die specifiek zijn voor dat recordtype, weergegeven in de module.</p> 
    <ul> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint issue]</li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Max Results]</p> </td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugwinnen.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Search for records]

Deze zoekmodule zoekt naar records in een object in [!DNL Jira Software] die overeenkomen met de zoekquery die u opgeeft.

U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Jira Software] account aan [!DNL Workfront Fusion], zie <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type record waarnaar de module moet zoeken. Wanneer u een recordtype selecteert, worden andere velden die specifiek zijn voor dat recordtype, weergegeven in de module.</p> 
    <ul> 
     <li>[!UICONTROL Issues]</li> 
     <li> <p>[!UICONTROL Issues by JQL (Jira Query Lanuguage)] </p> <p>Zie voor meer informatie over JQL <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> op de Atlassiaanse Help-site. </p> </li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Project by issue]</li> 
     <li>[!UICONTROL User]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
