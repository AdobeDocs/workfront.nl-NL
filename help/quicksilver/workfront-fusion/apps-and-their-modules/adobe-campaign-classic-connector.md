---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Campaign v7/v8-modules
description: Met de [!DNL Adobe Campaign] modules, kunt u beginnen [!DNL Adobe Workfront Fusion] scenario gebaseerd op gebeurtenissen in uw [!DNL Adobe Campaign] overeenkomsten en andere records voor account, maken, lezen of bijwerken, zoeken naar records aan de hand van criteria die u instelt en documenten uploaden.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 7decc5cbf4bb2c3d4d1802dec1f369ca061f6b48
workflow-type: tm+mt
source-wordcount: '1181'
ht-degree: 0%

---

# [!DNL Adobe Campaign] modules

Met de [!DNL Adobe Campaign] modules, kunt u beginnen [!DNL Adobe Workfront Fusion] scenario gebaseerd op gebeurtenissen in uw [!DNL Adobe Campaign v7/v8] records een account maken, lezen of bijwerken, records zoeken aan de hand van criteria die u instelt, en aangepaste API-aanroepen uitvoeren.

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

U moet de Fusion IP-adressen toevoegen aan [!DNL Adobe Campaign].

* Voor instructies bij het toevoegen van IP adressen aan uw lijst van gewenste personen van de Campagne, zie [IP adressen toevoegen aan de lijst van gewenste personen](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/ip-range-allow-listing#adding-ip-addresses-allow-list) in de documentatie van Adobe Campaign.
* Voor een lijst van IP adressen om aan de lijst van gewenste personen toe te voegen, zie [IP Adressen om tot de Fusie van Adobe Workfront toegang te hebben](/help/quicksilver/workfront-fusion/get-started/ip-addresses-for-fusion.md).

## Verbinden [!DNL Adobe Campaign] tot [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>We raden u ten zeerste aan een server-naar-server verbinding te maken. Adobe Campaign heeft hun API bijgewerkt zodat alleen server-naar-server verbindingen worden geaccepteerd. Als u verbinding maakt met Campagne versie 8 of hoger, kunt u **moet** Maak een server-naar-server verbinding.
>
>Voor meer informatie over de nieuwe verbindingsvereisten van de Campagne, zie [Migratie van technische operatoren van campagnes naar Adobe Developer Console](https://experienceleague.adobe.com/docs/campaign/technotes-ac/tn-new/ims-migration.html) in de Campagne documentatie.

1. In alle [!DNL Adobe Campaign] module, klikt u op **[!UICONTROL Add]** naast de [!UICONTROL Connection] veld.
1. Vul de volgende velden in:
   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Connection type]</td>
          <td>
            <p>Selecteer of u een basisverbinding of een server-aan-server verbinding creeert.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Connection name]</td>
          <td>
            <p>Voer een naam in voor deze verbinding.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Base URL]</td>
          <td>Voer de basis-URL in waarmee u verbinding maakt met uw [!DNL Adobe Campaign] -instantie.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Username]</td>
          <td>Voer uw Adobe Campaign-gebruikersnaam in als u een basisverbinding maakt.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Password]</td>
          <td>Als u een basisverbinding maakt, voert u uw Adobe Campaign-wachtwoord in.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client ID]</td>
          <td>Als u een server-aan-server verbinding creeert, ga uw [!DNL Adobe] [!UICONTROL Client ID]. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]</td>
          <td>Als u een server-aan-server verbinding creeert, ga uw [!DNL Adobe] [!UICONTROL Client Secret]. Dit vindt u in het gedeelte [!UICONTROL Credentials details] van de [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Environment]</td>
          <td>Selecteer of u verbinding maakt met een productie- of niet-productieomgeving.
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Type]</td>
          <td>Selecteer of u verbinding maakt met een serviceaccount of een persoonlijke account.
        </tr>
   </tbody>
    </table>
1. Klikken **[!UICONTROL Continue]** om de verbinding tot stand te brengen en terug naar de module te gaan.

## [!DNL Adobe Campaign] modules en hun velden

Wanneer u [!DNL Adobe Campaign] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Adobe Campaign] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

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
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign], zie <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Verbinding maken met [!DNL Adobe Campaign]</a> in dit artikel.</td> 
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

Deze actiemodule maakt een nieuwe record in [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign], zie <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Verbinding maken met [!DNL Adobe Campaign]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Selecteer het type van [!DNL Adobe Campaign] record die u wilt maken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>Selecteer de velden waarvoor u waarden wilt instellen wanneer de record wordt gemaakt en vul vervolgens de waarden voor die velden in. Velden variëren op basis van het type record dat u selecteert.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields]</td> 
   <td> Voor elk aangepast veld dat u aan de nieuwe record wilt toevoegen, klikt u op <b>[!UICONTROL Add item]</b> en voert u de naam en de waarde van het veld in of wijst u deze toe. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Make a custom API call]

Deze module maakt een aangepaste API-aanroep naar de [!DNL Adobe Campaign] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign], zie <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Verbinding maken met [!DNL Adobe Campaign]</a> in dit artikel.</td> 
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

Met deze actiemodule verwijdert u één record uit [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign], zie <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Verbinding maken met [!DNL Adobe Campaign]</a> in dit artikel.</td> 
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

Deze actiemodule voert een geselecteerde handeling uit op een object in het dialoogvenster [!DNL Adobe Campaign] API.

Zie voor informatie over specifieke acties en velden [[!DNL Adobe Campaign] - API-documentatie](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign], zie <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Verbinding maken met [!DNL Adobe Campaign]</a> in dit artikel.</td> 
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

Deze actiemodule leest een record uit [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign], zie <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Verbinding maken met [!DNL Adobe Campaign]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Selecteer het type van [!DNL Adobe Campaign] record die u wilt lezen.</td> 
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
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign], zie <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Verbinding maken met [!DNL Adobe Campaign]</a> in dit artikel.</td> 
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
   <td>Voer het e-mailadres in of wijs het e-mailadres toe van de gebruiker die u wilt abonneren op de informatieservice of het abonnement opzeggen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update record]

Deze actiemodule werkt één record bij in [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign], zie <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Verbinding maken met [!DNL Adobe Campaign]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Selecteer het type van [!DNL Adobe Campaign] record die u wilt maken.</td> 
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
   <td> Klik voor elk aangepast veld dat u wilt bijwerken op <b>[!UICONTROL Add item]</b> en voert u de naam en de waarde van het veld in of wijst u deze toe. </td> 
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
   <td>Voor instructies over het maken van een verbinding met [!DNL Adobe Campaign], zie <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Verbinding maken met [!DNL Adobe Campaign]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Selecteer het type van [!DNL Adobe Campaign] record die u wilt maken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</td> 
  </tr> 
 </tbody> 
</table>
