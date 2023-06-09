---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Campaign Classic-modules
description: Met de [!DNL Adobe Campaign Classic] modules, kunt u beginnen [!DNL Adobe Workfront Fusion] scenario gebaseerd op gebeurtenissen in uw [!DNL Adobe Campaign Classic] overeenkomsten en andere records voor account, maken, lezen of bijwerken, zoeken naar records aan de hand van criteria die u instelt en documenten uploaden.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 482725764ede6b2700985fa67dc2cb9f92d3bb12
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 0%

---

# [!DNL Adobe Campaign Classic] modules

Met de [!DNL Adobe Campaign Classic] modules, kunt u beginnen [!DNL Adobe Workfront Fusion] scenario gebaseerd op gebeurtenissen in uw [!DNL Adobe Campaign Classic] records een account maken, lezen of bijwerken, records zoeken aan de hand van criteria die u instelt, en aangepaste API-aanroepen uitvoeren.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Verbinden [!DNL Adobe Campaign Classic] tot [!DNL Adobe Workfront Fusion]

1. In alle [!DNL Adobe Campaign Classic] module, klikt u op **[!UICONTROL Add]** naast de [!UICONTROL Connection] veld.
1. Voer de basis-URL in die u gebruikt om verbinding te maken met uw [!DNL Adobe Campaign Classic] -instantie.
1. Voer uw gebruikersnaam en wachtwoord in.
1. Klikken **[!UICONTROL Continue]** om de verbinding tot stand te brengen en terug naar de module te gaan.

## [!DNL Adobe Campaign Classic] modules en hun velden

Wanneer u [!DNL Adobe Campaign Classic] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Adobe Campaign Classic] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Handelingen](#actions)
* [Zoekopdrachten](#searches)

### Triggers

#### [!UICONTROL Watch records]

Deze geplande trekkermodule begint een scenario wanneer een verslag verandert.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign Classic], zie <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Verbinding maken met [!DNL Adobe Campaign Classic]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Selecteer of u naar nieuwe verslagen, bijgewerkte verslagen, of allebei wilt letten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Selecteer de bron die u wilt controleren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields to include in output]</td> 
   <td>Selecteer de velden die u in de uitvoer van de module wilt opnemen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields to include in output]</td> 
   <td>Voor elk aangepast veld dat u in de uitvoer wilt opnemen, klikt u op <b>[!UICONTROL Add]</b> en voert u de naam van het aangepaste veld in.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned results]</td> 
   <td>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</td> 
  </tr> 
 </tbody> 
</table>


### Handelingen

* [[!UICONTROL Create a record]](#create-a-record)
* [[!UICONTROL Make a custom API call]](#make-a-custom-api-call)
* [[!UICONTROL Delete a record]](#delete-record)
* [[!UICONTROL Perform an action]](#perform-an-action)
* [[!UICONTROL Read a record]](#-read-a-record)
* [[!UICONTROL Subscribe or unsubscribe]](#subscribe-or-unsubscribe)
* [[!UICONTROL Update a record]](#update-record)

#### [!UICONTROL Create a record]

Deze actiemodule maakt een nieuwe record in [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign Classic], zie <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Verbinding maken met [!DNL Adobe Campaign Classic]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Selecteer het type van [!DNL Adobe Campaign Classic] record die u wilt maken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>Selecteer de velden waarvoor u waarden wilt instellen wanneer de record wordt gemaakt en vul vervolgens de waarden voor die velden in. Velden variëren op basis van het type record dat u selecteert.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields]</td> 
   <td> Voor elk aangepast veld dat u aan de nieuwe record wilt toevoegen, klikt u op <b>[!UICONTROL Add item]</b> en voert u de naam en waarde van het veld in of wijst u deze toe. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Make a custom API call]

Deze module maakt een aangepaste API-aanroep naar de [!DNL Adobe Campaign Classic] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign Classic], zie <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Verbinding maken met [!DNL Adobe Campaign Classic]</a> in dit artikel.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Action]</td>
      <td><p>Selecteer de handeling die de API-aanroep moet uitvoeren.</p>
      <p>[!UICONTROL Execute query]</p>
      <p>[!UICONTROL Write]</p>
      <p>[!UICONTROL Get entity if more recent]</p>
      <p>[!UICONTROL Select all]</p>
      <p>[!UICONTROL Push event]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p>
        <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] voegt de [!UICONTROL x-security] automatisch een tokenkoptekst.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL XML Body]</td>
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in XML, zonder het sessieelement. </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Delete Record]

Met deze actiemodule verwijdert u één record uit [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign Classic], zie <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Verbinding maken met [!DNL Adobe Campaign Classic]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Selecteer het type bron dat u wilt verwijderen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Voer de id in van de bron die u wilt verwijderen of wijs deze toe.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Perform an action]

Deze actiemodule voert een geselecteerde handeling uit op een object in het dialoogvenster [!DNL Adobe Campaign Classic] API.

Voor informatie over specifieke acties en velden raadpleegt u [[!DNL Adobe Campaign] - API-documentatie](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign Classic], zie <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Verbinding maken met [!DNL Adobe Campaign Classic]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td><p>Selecteer de handeling die op het object moet worden uitgevoerd.</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> Zie voor beschikbare velden <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> in dit artikel. </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> Zie voor beschikbare velden <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> in dit artikel. </p></li> 
   <li><p><b>[!UICONTROL Create]</b></p><p> Zie voor beschikbare velden <a href="#create-a-record" class="MCXref xref" >[!UICONTROL Create a record]</a> in dit artikel. </p></li>
   <li><p><b>[!UICONTROL Update]</b></p><p> Zie voor beschikbare velden <a href="#update-record" class="MCXref xref" >[!UICONTROL Update a record]</a> in dit artikel. </p></li>
   <li><p><b>[!UICONTROL Delete]</b></p><p> Zie voor beschikbare velden <a href="#delete-record" class="MCXref xref" >[!UICONTROL Delete a record]</a> in dit artikel. </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL Read a record]

Deze actiemodule leest een record uit [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign Classic], zie <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Verbinding maken met [!DNL Adobe Campaign Classic]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Selecteer het type van [!DNL Adobe Campaign Classic] record die u wilt lezen.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Voer een kaart in met de id van de record die u wilt lezen.</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL Fields to include in output] </td> 
   <td>Selecteer de velden die u in de uitvoer van de module wilt opnemen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields to include in output]</td> 
   <td>Voor elk aangepast veld dat u in de uitvoer wilt opnemen, klikt u op <b>[!UICONTROL Add]</b> en voert u de naam van het aangepaste veld in.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Subscribe or unsubscribe]

Deze actiemodule abonneert een gebruiker aan of unsubscribes een gebruiker van een informatiedienst.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign Classic], zie <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Verbinding maken met [!DNL Adobe Campaign Classic]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscribe or unsubscribe]</td> 
   <td>Geef op of u zich wilt abonneren op de informatieservice of het abonnement wilt opzeggen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Service name]</td> 
   <td>Selecteer de service waarvan u een abonnement wilt nemen of waarvan u een abonnement wilt opzeggen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recipient email address] </td> 
   <td>Voer het e-mailadres in of wijs het e-mailadres toe van de gebruiker die u wilt abonneren op of zich niet meer wilt abonneren op de informatieservice.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update record]

Deze actiemodule werkt één record bij in [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign Classic], zie <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Verbinding maken met [!DNL Adobe Campaign Classic]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Selecteer het type van [!DNL Adobe Campaign Classic] record die u wilt maken.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Voer de toewijzing in van de id van de record die u wilt bijwerken.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>Selecteer de velden waarvoor u de waarden wilt bijwerken en vul vervolgens de waarden voor die velden in. Velden variëren op basis van het type record dat u selecteert.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields]</td> 
   <td> Voor elk aangepast veld dat u wilt bijwerken, klikt u op <b>[!UICONTROL Add item]</b> en voert u de naam en waarde van het veld in of wijst u deze toe. </td> 
  </tr> 
 </tbody> 
</table>

### Zoekopdrachten

#### [!UICONTROL Search]

Deze zoekmodule retourneert records die op de opgegeven criteria zijn gebaseerd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign Classic], zie <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Verbinding maken met [!DNL Adobe Campaign Classic]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Selecteer het type van [!DNL Adobe Campaign Classic] record die u wilt maken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</td> 
  </tr> 
 </tbody> 
</table>
