---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Frame.io-modules
description: De [!DNL Adobe Workfront Fusion Frame].io modules enable you to monitor, create, update, retrieve, or delete assets and comments in your [!DNL Frame.io] account.
author: Becky
feature: Workfront Fusion
exl-id: 373a86f6-fbba-4914-b08d-a3a035ac0ae4
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1885'
ht-degree: 0%

---

# [!DNL Frame.io] modules

De [!DNL Adobe Workfront Fusion] [!DNL Frame.io] kunt u elementen en opmerkingen in uw [!DNL Frame.io] account.

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

Te gebruiken [!DNL Frame.io] modules, moet u een [!DNL Frame.io] account

## Verbinden [!DNL Frame.io] tot [!UICONTROL Adobe Workfront Fusion]

U kunt verbinding maken met [!DNL Frame.io] het gebruiken van een API teken, of door OAuth 2.0 te gebruiken.

[Verbinden met [!DNL Frame.io] API-token gebruiken](#connect-to-frameio-using-an-api-token)

[Verbinden met [!DNL Frame.io] met OAuth 2.0 PKCE](#connect-to-frameio-using-oauth-20-pkce)

### Verbinden met [!DNL Frame.io] API-token gebruiken

Als u verbinding wilt maken met uw [!DNL Frame.io] account aan [!DNL Workfront Fusion] met behulp van een API-token moet u de API-token in uw [!DNL Frame.io] en voeg deze in bij de [!DNL Workfront Fusion] [!DNL Frame.io] [!UICONTROL Create a connection] .

1. Meld u aan bij uw [!DNL Frame.io] account.
1. Ga naar de **[!UICONTROL Tokens]** pagina in de [!DNL Frame.io] Ontwikkelaar.
1. Klik op **[!UICONTROL New]**.
1. Voer de naam van het token in, selecteer het bereik dat u wilt gebruiken en klik op **[!UICONTROL Create]**.
1. Kopieer de opgegeven token.
1. Ga naar [!DNL Workfront Fusion] en opent u de [!DNL Frame.io] module **[!UICONTROL Create a connection]** .
1. In de **[!UICONTROL Connection type]** veld, selecteren **[!DNL Frame.io]**.
1. Voer de token die u in stap 5 hebt gekopieerd, in naar de **[!UICONTROL Your [!DNL Frame.io] API Key]** veld en klik op **[!UICONTROL Continue]** om de verbinding tot stand te brengen.

De verbinding is tot stand gebracht. U kunt doorgaan met het instellen van de module.

### Verbinden met [!DNL Frame.io] met OAuth 2.0 PKCE

U kunt een verbinding maken met [!DNL Frame.io] gebruik van OAuth 2.0 PKCE met een optionele client-id. Als u een client-id wilt opnemen in uw verbinding, moet u een OAuth 2.0-app maken in uw [!DNL Frame.io] account.

* [Verbinden met [!DNL Frame.io] het gebruiken van OAuth 2.0 PKCE (zonder identiteitskaart van de Cliënt)](#connect-to-frameio-using-using-oauth-20-pkce-without-client-id)
* [Verbinden met [!DNL Frame.io] gebruiken van OAuth 2.0 PKCE (met identiteitskaart van de Cliënt)](#connect-to-frameio-using-using-oauth-20-pkce-with-client-id)

#### Verbinden met [!DNL Frame.io] het gebruiken van OAuth 2.0 PKCE (zonder identiteitskaart van de Cliënt)

1. Ga naar [!DNL Workfront Fusion] en opent u de [!DNL Frame.io] module **[!UICONTROL Create a connection]** .
1. In de **[!UICONTROL Connection type]** veld, selecteren **[!UICONTROL [!DNL Frame.io] OAuth 2.0 PKCE]**.
1. Voer een naam in voor de nieuwe verbinding in het dialoogvenster **[!UICONTROL Connection name]** veld.
1. Klikken **[!UICONTROL Continue]** om de verbinding tot stand te brengen.

De verbinding is tot stand gebracht. U kunt doorgaan met het instellen van de module.

#### Verbinden met [!DNL Frame.io] gebruiken van OAuth 2.0 PKCE (met identiteitskaart van de Cliënt)

1. Een OAuth 2.0-app maken in [!DNL Frame.io]. Zie voor instructies de [!DNL Frame.io] documentatie over [!UICONTROL OAuth 2.0 Code Authorization Flow].

   >[!IMPORTANT]
   >
   >Wanneer u de OAuth 2.0-app maakt in [!DNL Frame.io]:
   >
   >* Voer het volgende in als de omleidings-URI:
   >   
   >  Amerika/APAC `https://app.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >  EMEA `https://app-eu.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >* Schakel de optie PCKE in.



1. Kopieer de opgegeven `client_id`.
1. Ga naar [!DNL Workfront Fusion] en opent u de [!DNL Frame.io] module **[!UICONTROL Create a connection]** .
1. In de **[!UICONTROL Connection type]** veld, selecteren **[!UICONTROL [!DNL Frame.io] OAuth 2.0 PKCE]**.
1. Voer een naam in voor de nieuwe verbinding in het dialoogvenster **[!UICONTROL Connection name]** veld.
1. Klik op **[!UICONTROL Show advanced settings]**.
1. Voer de `client_id` u hebt in stap 2 naar de **[!UICONTROL Client ID]** veld.
1. Klikken **[!UICONTROL Continue]** om de verbinding tot stand te brengen.

De verbinding is tot stand gebracht. U kunt doorgaan met het instellen van de module.

## [!DNL Frame.io] modules en hun velden

Wanneer u [!DNL Frame.io] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Frame.io] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Activa](#assets)
* [Opmerkingen](#comments)
* [Projecten](#projects)
* [Overige](#other)

### Activa

* [[!UICONTROL Create an Asset]](#create-an-asset)
* [[!UICONTROL Delete an Asset]](#delete-an-asset)
* [[!UICONTROL Get an Asset]](#get-an-asset)
* [[!UICONTROL List Assets]](#list-assets)
* [[!UICONTROL Update an Asset]](#update-an-asset)
* [[!UICONTROL Watch Asset Deleted]](#watch-asset-deleted)
* [[!UICONTROL Watch Asset Label Updated]](#watch-asset-label-updated)
* [[!UICONTROL Watch New Asset]](#watch-new-asset)

#### [!UICONTROL Create an Asset]

Deze actiemodule maakt een nieuw element.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Frame.io], zie <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selecteer of wijs het team in kaart dat het project bezit dat u activa voor wilt creëren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>Selecteer het project of wijs identiteitskaart van het project toe dat u activa voor wilt tot stand brengen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>Selecteer de map of wijs de id toe van de map waarin u middelen wilt maken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type] </td> 
   <td> <p>Selecteer of u een map of bestand wilt maken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Voer de naam van het nieuwe bestand of de nieuwe map in.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Type </td> 
    <td> <p>Select the type of file you want to upload.</p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Size </td> 
    <td> <p>The file size in bytes.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source URL] </td> 
   <td> <p>Voer de URL in van het bestand dat u wilt uploaden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description] </td> 
   <td> <p>Voer een korte beschrijving van het element in.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete an Asset]

Met deze actiemodule verwijdert u een opgegeven element.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Frame.io], zie <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selecteer of wijs het team toe dat het project bezit dat de activa bevat u wilt schrappen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> Selecteer het project of het element dat u wilt verwijderen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>Selecteer de map met het element dat u wilt verwijderen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Selecteer of wijs het element toe dat u wilt verwijderen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get an Asset]

Deze actiemodule haalt elementdetails op.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Frame.io], zie <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selecteer of wijs het team in kaart dat het project bezit dat de activa bevat u details over wilt terugwinnen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> Selecteer het project dat het element bevat waarover u details wilt ophalen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>Selecteer de map met het element waarover u meer informatie wilt ophalen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Selecteer het element of wijs de id van het element toe waarover u details wilt ophalen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Assets]

Deze zoekmodule haalt alle elementen in de opgegeven projectmap op.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Frame.io], zie <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selecteer of wijs het team toe dat het project bezit dat de omslag bevat u activa van wilt terugwinnen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> Selecteer het project dat de map bevat waarvan u elementen wilt ophalen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>Selecteer de map waarvan u elementen wilt weergeven.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Het maximumaantal elementen instellen [!DNL Workfront Fusion] wordt tijdens één uitvoeringscyclus geretourneerd.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### `[!UICONTROL Update an Asset]`

Met deze actiemodule kunt u de naam, beschrijving of aangepaste velden van een bestaand element bijwerken.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Frame.io], zie <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selecteer of wijs het team in kaart dat het project bezit dat u activa voor wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>Selecteer het project of wijs identiteitskaart van het project toe dat u activa voor wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>Selecteer de map of wijs de id toe van de map waarin u middelen wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Voer de naam van het bijgewerkte bestand in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description] </td> 
   <td> <p>Voer een korte beschrijving in van het bijgewerkte element.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch Asset Deleted]

Deze triggermodule start een scenario wanneer een element wordt verwijderd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> Voer de naam van de webhaak in, bijvoorbeeld het verwijderde element.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Frame.io], zie <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selecteer het team waarvoor deze webhaak is gemaakt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch Asset Label Updated]

Deze triggermodule start een scenario wanneer de status van een element wordt ingesteld, gewijzigd of verwijderd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> Voer de naam van de webhaak in, bijvoorbeeld de status van het element bijgewerkt.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Frame.io], zie <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selecteer het team waarvoor deze webhaak is gemaakt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch New Asset]

Deze triggermodule start een scenario wanneer een nieuw element wordt gemaakt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> Voer de naam van de webhaak in, bijvoorbeeld het gemaakte element.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Frame.io], zie <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selecteer het team waarvoor deze webhaak is gemaakt.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Opmerkingen

* [[!UICONTROL Create a Comment]](#create-a-comment)
* [[!UICONTROL Delete a Comment]](#delete-a-comment)
* [[!UICONTROL Get a Comment]](#get-a-comment)
* [[!UICONTROL List Comments]](#list-comments)
* [[!UICONTROL Update a Comment]](#update-a-comment)
* [[!UICONTROL Watch Comment Updated]](#watch-comment-updated)
* [[!UICONTROL Watch New Comment]](#watch-new-comment)

#### [!UICONTROL Create a Comment]

Deze actiemodule voegt een nieuwe opmerking of reactie toe aan het element.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Frame.io], zie <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type] </td> 
   <td> <p>Selecteer of u een opmerking wilt maken of op een opmerking wilt reageren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selecteer of wijs het team in kaart dat het project bezit dat de activa bevat u een commentaar aan wilt toevoegen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>Selecteer het project of wijs identiteitskaart van het project toe dat de activa bevat u een commentaar aan wilt toevoegen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>Selecteer de map of wijs de id toe van de map met het element waaraan u een opmerking wilt toevoegen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Selecteer of wijs het element toe waaraan u een opmerking wilt toevoegen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment ID] </td> 
   <td> <p>Selecteer of wijs de commentaar toe u een antwoord aan wilt toevoegen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p> Voer de tekstinhoud van de opmerking of het antwoord in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timestamp] </td> 
   <td> <p>Voer het framenummer in de video in waarnaar de opmerking moet worden gekoppeld.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a Comment]

In deze actiemodule wordt een bestaande opmerking verwijderd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Frame.io], zie <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID]</td> 
   <td> <p> Selecteer of wijs het team toe dat het project bezit dat de activa bevat u een commentaar van wilt schrappen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> Selecteer het project of wijs identiteitskaart van het project toe dat de activa bevat u een commentaar van wilt schrappen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td> <p> Selecteer de map met het element waaruit u een opmerking wilt verwijderen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Selecteer het element dat de opmerking bevat die u wilt verwijderen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment ID] </td> 
   <td> <p>Selecteer de opmerking die u wilt verwijderen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a Comment]

Deze actiemodule wint details van de gespecificeerde commentaar terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Frame.io], zie <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selecteer of wijs het team toe dat het project bezit dat de omslag bevat u activa van wilt terugwinnen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>Selecteer het project dat de map bevat waarvan u elementen wilt ophalen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>Selecteer de map waarvan u elementen wilt weergeven.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Selecteer het element dat de opmerking bevat die u wilt ophalen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment ID] </td> 
   <td> <p>Selecteer de opmerking waarover u details wilt ophalen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Comments]

Deze zoekmodule haalt alle opmerkingen van het opgegeven element op.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Frame.io], zie <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selecteer of wijs het team toe dat het project bezit dat de omslag bevat u commentaren van wilt terugwinnen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>Selecteer het project dat de map bevat waarvan u de opmerkingen wilt ophalen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>Selecteer de map met het element waaruit u de opmerkingen wilt weergeven.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Selecteer het element waarvoor u opmerkingen wilt weergeven.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Het maximum aantal opmerkingen instellen [!DNL Workfront Fusion] wordt tijdens één uitvoeringscyclus geretourneerd.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a Comment]

In deze actiemodule wordt een bestaande opmerking bewerkt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Frame.io], zie <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selecteer of wijs het team toe dat het project bezit dat de activa bevat u een commentaar op wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>Selecteer het project \ dat de activa bevat u een commentaar op wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>Selecteer de map met het element waarop u een opmerking wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Selecteer het element waarop u een opmerking wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment ID] </td> 
   <td> <p>Selecteer de opmerking die u wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p> Voer de tekstinhoud van de opmerking in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timestamp] </td> 
   <td> <p>Voer het framenummer in de video in waarnaar de opmerking is gekoppeld.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch Comment Updated]

Deze triggermodule start een scenario wanneer een opmerking wordt bewerkt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name] </td> 
   <td> <p>Voer de naam van de webhaak in, bijvoorbeeld Opmerking bewerkt.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Frame.io], zie <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selecteer het team waarvoor deze webhaak is gemaakt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch New Comment]

Deze triggermodule start een scenario wanneer een nieuwe opmerking of een nieuw antwoord wordt gemaakt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name] </td> 
   <td> <p>Voer de naam van de webhaak in, bijvoorbeeld Nieuwe opmerking.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Frame.io], zie <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selecteer het team waarvoor deze webhaak is gemaakt.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Projecten

#### [!UICONTROL List Projects]

Deze onderzoeksmodule wint alle projecten voor het gespecificeerde team terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Frame.io], zie <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Selecteer of kaart het team u projecten voor wilt terugwinnen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Het maximumaantal projecten instellen [!DNL Workfront Fusion] wordt tijdens één uitvoeringscyclus geretourneerd.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Overige

#### [!UICONTROL Make an API Call]

In deze module kunt u een aangepaste API-aanroep uitvoeren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Frame.io], zie <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Een pad invoeren ten opzichte van <code>https://api.frame.io</code>. Voorbeeld: <code> /v2/teams</code></p> <p>Opmerking: Voor de lijst met beschikbare eindpunten raadpleegt u de [!DNL Frame.io] API-referentie.</p> </td> 
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
   <td> <p>Voer de queryreeks voor de aanvraag in. Voor elke parameter die u in het vraagkoord wilt omvatten, klik <b>[!UICONTROL Add item]</b> en voert u de naam en de gewenste waarde van het veld in.</p> </td> 
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

**Voorbeeld:** De volgende API-aanroep retourneert alle teams en de bijbehorende details in uw [!DNL Frame.io] account:

URL: `/v2/teams`

Methode: `GET`

![](assets/api-call-example.png)

Het resultaat is te vinden in de Output van de module onder Bundel > Lichaam.

In ons voorbeeld zijn de gegevens van 1 team geretourneerd:

![](assets/api-call-output.png)
