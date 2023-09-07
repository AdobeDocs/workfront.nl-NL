---
title: HubSpot CRM-modules
description: De [!DNL Adobe Workfront Fusion] De modules van CRM van HubSpot laten u toe om gebeurtenissen, verslagen, contacten, overeenkomsten, dossier en vormbijdragen te controleren, of, verslagen, contacten, overeenkomsten, gebeurtenissen, of dossiers in te creëren, terug te winnen bij te werken en te schrappen in uw [!DNL HubSpot CRM] account.
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: 5bb394c2fffb4426d66a8b144802db8f7c97afe1
workflow-type: tm+mt
source-wordcount: '2140'
ht-degree: 0%

---

# [!DNL HubSpot CRM] modules

De [!DNL Adobe Workfront Fusion] [!DNL HubSpot CRM] -modules kunt u gebeurtenissen, records, contactpersonen, services, bestanden en formulierverzendingen controleren, of records, contactpersonen, services, gebeurtenissen of bestanden in uw [!DNL HubSpot CRM] account.

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

Te gebruiken [!DNL HubSpot CRM] modules, moet u een [!DNL HubSpot CRM] account.

## Verbinden [!DNL Adobe Workfront Fusion] tot [!DNL HubSpot CRM]

Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie [Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL HubSpot CRM] modules en hun velden

Wanneer u [!DNL Hubspot CRM] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Hubspot CRM] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [CRM-objecten](#crm-objects)
* [Records (Deals, Contacten, en Bedrijven)](#records-deals-contacts-and-companies)
* [Contactpersonen](#contacts)
* [Overeenkomsten](#deals)
* [Bedrijven](#companies)
* [Bestanden](#files)
* [Tickets](#tickets)
* [Maak een API Vraag](#make-an-api-call)

### CRM-objecten

#### [!UICONTROL Search for CRM Objects]

Deze zoekmodule zoekt naar CRM-objecten op aangepaste eigenschappen of op query. Als u naar producten of lijnitems wilt zoeken, gebruikt u een speciale verbinding met een vereist aangepast bereik.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Ga of kaart het maximumaantal punten in dat de module in één uitvoeringscyclus zal terugkeren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Type to Search]</td> 
   <td>Selecteer het type van voorwerp van Hubspot CRM dat u naar wilt zoeken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>Selecteer de eigenschappen die u in de uitvoer van de module wilt weergeven. De beschikbare velden zijn afhankelijk van het object dat u hebt geselecteerd.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter by] </td> 
   <td> <p>Selecteer hoe u de zoekopdracht wilt filteren</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>De query invoeren of toewijzen</p> </li> 
     <li> <p><strong>[!UICONTROL Properties]</strong> </p> <p>Voer de groepen of filters voor uw zoekopdracht in.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort by]</td> 
   <td> <p>Klik als u de resultaten wilt sorteren. Als u de resultaten wilt sorteren, worden de volgende velden weergegeven. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Property name]</strong> </p> <p>Selecteer de eigenschap waarmee u de resultaten wilt sorteren</p> </li> 
     <li> <p><strong>[!UICONTROL Direction]</strong> </p> <p>Kies of u de resultaten in oplopende of aflopende richting wilt sorteren.</p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Start Offset</td> 
    <td>Enter or map the ID of the first item you want to retrieve details for. This module only returns up to 5000 results at a time. Setting a start offset allows you to retrieve items other than the first 5000. If the start offset is 5000, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

### Records (Deals, Contacten, en Bedrijven)

* [[!UICONTROL Create a Record (Legacy)]](#create-a-record-legacy)
* [[!UICONTROL Get a Record]](#get-a-record)
* [[!UICONTROL Update a Record]](#update-a-record)
* [[!UICONTROL Delete a Record]](#delete-a-record)
* [[!UICONTROL Get a Record Property]](#get-a-record-property)
* [[!UICONTROL Watch Records]](#watch-records)

#### [!UICONTROL Create a Record (Legacy)]

Deze actiemodule leidt tot contact, een bedrijf, of een overeenkomst.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het type record dat u wilt maken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>Vul de eigenschappen in die u voor de record wilt instellen. De beschikbare velden zijn afhankelijk van het type record dat u wilt maken.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a Record]

Deze actiemodule krijgt details van een contact, een bedrijf, of een overeenkomst.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Selecteer het recordtype.</p> 
    <ul> 
     <li>[!UICONTROL Contact]</li> 
     <li>[!UICONTROL Company] </li> 
     <li>[!UICONTROL Deal]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search Type]</td> 
   <td>Als u contact krijgt, selecteer of u het door identiteitskaart of door E-mailadres wilt identificeren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Ga identiteitskaart van het contact, het bedrijf of de overeenkomst in die u wilt terugwinnen. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Voer het e-mailadres in van de contactpersoon waarvan u de gegevens wilt ophalen. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a Record]

Deze actiemodule werkt een contact, een bedrijf, of een overeenkomst bij.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Selecteer het type record dat u wilt bijwerken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search Type]</td> 
   <td> <p>Als u een contact krijgt, selecteer hoe u het verslag wilt identificeren:</p> 
    <ul> 
     <li> <p>[!UICONTROL ID]</p> </li> 
     <li> <p>[!UICONTROL Email]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Voer de id in van de contactpersoon, het bedrijf of de deal die u wilt bijwerken. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Voer het e-mailadres in van de contactpersoon waarvan u de gegevens wilt bijwerken. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>Vul de eigenschappen in die u voor de record wilt instellen. De beschikbare velden zijn afhankelijk van het type record dat u wilt maken.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a Record]

Deze actiemodule schrapt een contact, een bedrijf, of een overeenkomst.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Selecteer het type record dat u wilt verwijderen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Ga identiteitskaart van het contact, het bedrijf, of de overeenkomst in u wilt schrappen. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a Record Property]

Deze actiemodule krijgt meta-gegevens voor een specifiek verslagbezit door zijn (interne) naam.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Selecteer het type record met de eigenschap waarvoor u metagegevens wilt ophalen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Property Name]</td> 
   <td>Selecteer de eigenschap waarvoor u metagegevens wilt ophalen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Option ID]</td> 
   <td> <p> Sommige eigenschappen hebben een set beschikbare opties die een gebruiker als eigenschapswaarde kan selecteren. Voer de id in van de optie die de eigenschapwaarde vertegenwoordigt die u wilt ophalen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch Records]

Deze trekkermodule begint een scenario wanneer een contact, bedrijf, of overeenkomst binnen de laatste 30 dagen is gewijzigd of gecreeerd. De uitvoer is beperkt tot 10.000 records.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Selecteer het type record met de eigenschap die u wilt controleren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Selecteer of u onlangs gewijzigde of onlangs tot stand gebrachte verslagen wilt letten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Selecteer de eigenschappen die u in de uitvoer van de module wilt opnemen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Contactpersonen

* [[!UICONTROL Create/Update a Contact (Legacy)]](#createupdate-a-contact-legacy)
* [[!UICONTROL Create/Update a Group of Contacts]](#createupdate-a-group-of-contacts)
* [[!UICONTROL Add Contacts to a List]](#add-contacts-to-a-list)
* [[!UICONTROL Remove a Contact from a List]](#remove-a-contact-from-a-list)
* [[!UICONTROL Merge contacts]](#merge-contacts)
* [[!UICONTROL Search for Contacts]](#search-for-contacts)
* [[!UICONTROL List Contacts]](#list-contacts)
* [[!UICONTROL List Contacts of a Company]](#list-contacts-of-a-company)

#### [!UICONTROL Create/Update a Contact (Legacy)]

Creeert een contact als het niet in een portaal reeds bestaat, of werkt het met de recentste bezitswaarden bij als het in een portaal bestaat.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>Vul om het even welke eigenschappen in die u voor het contact wilt plaatsen of bijwerken. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create/Update a Group of Contacts]

Creeert een groep contacten of werkt hen bij als zij reeds bestaan. De prestaties zijn het best wanneer de partijgrootte tot 100 contacten of minder wordt beperkt. De veranderingen die door dit eindpunt worden aangebracht worden verwerkt asynchroon, zodat kan het verscheidene notulen voor veranderingen nemen die op contactverslagen moeten worden toegepast.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Batch of Contacts to Create/Update] </td> 
   <td> <p>Voeg de partij contacten toe.</p> <p>Klikken <strong>[!UICONTROL Add item]</strong> om een nieuwe contactpersoon toe te voegen. Voer in het venster dat wordt weergegeven de volgende gegevens in of wijs deze toe:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Search Type]</strong> </p> <p>Selecteer hoe u de contactpersoon wilt identificeren:</p> 
      <ul> 
       <li> <p>[!UICONTROL ID]</p> <p>Voer de id in van de contactpersoon die u wilt maken of bijwerken. </p> </li> 
       <li> <p>[!UICONTROL Email]</p> <p>Voer het e-mailadres in van de contactpersoon die u wilt maken of bijwerken. </p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Properties]</strong> </p> <p>Vul om het even welke eigenschappen in die u voor het contact wilt plaatsen of bijwerken.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add Contacts to a List]

Deze module voegt contactverslagen toe die reeds in het systeem aan een contactlijst zijn gecreeerd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID] </td> 
   <td>Selecteer identiteitskaart van de lijst waaraan u de contact wilt toevoegen. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IDs/Emails] </td> 
   <td> <p>Selecteer hoe u de contacten wilt identificeren u aan de lijst wilt toevoegen:</p> 
    <ul> 
     <li> <p>[!UICONTROL IDs]</p> <p>Voeg identiteitskaarts van de contacten toe die u aan de lijst wilt toevoegen.</p> </li> 
     <li> <p>[!UICONTROL Emails]</p> <p>Voeg de e-mailadressen toe van de contactpersonen die u aan de lijst wilt toevoegen.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remove a Contact from a List]

Hiermee verwijdert u een contactpersoon uit een lijst met contactpersonen.

>[!NOTE]
>
>U kunt contactpersonen niet handmatig uit een dynamische lijst verwijderen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID] </td> 
   <td>Selecteer identiteitskaart van de lijst waarvan u de contact wilt verwijderen. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact ID] </td> 
   <td>Voer de id in van de contactpersoon die u uit de lijst wilt verwijderen. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Merge contacts]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 1] </td> 
   <td>Ga identiteitskaart van één van de contacten in u wilt samenvoegen. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 2] </td> 
   <td>Voer de id in van de andere contactpersoon die u wilt samenvoegen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Search for Contacts]

Haalt een lijst met contactpersonen op met de zoekquery.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td>Voer de zoekquery in.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Ga of kaart het maximumaantal contacten in [!DNL Workfront Fusion] moet tijdens één cyclus van de scenariouitvoering worden geretourneerd. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Contacts]

Keert alle contacten terug die in het portaal zijn gecreeerd. De output is beperkt tot 5000 contacten. Om van vorige of volgende contacten een lijst te maken, kunt u gebruiken [!UICONTROL advanced] om de lijst te verschuiven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Het maximumaantal contacten [!DNL Workfront Fusion] moet tijdens één cyclus van de scenariouitvoering worden geretourneerd. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>Selecteer de eigenschappen die u in de uitvoer van de module wilt weergeven. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL List Contacts of a Company]

Wint een lijst van contacten in het bedrijf terug. De output is beperkt tot 5000 contacten. Om van vorige of volgende contacten een lijst te maken, kunt u gebruiken [!UICONTROL advanced] om de lijst te verschuiven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Ga identiteitskaart van het bedrijf in waarvan contacten u wilt een lijst maken. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Het maximumaantal contacten [!DNL Workfront Fusion] moet tijdens één cyclus van de scenariouitvoering worden geretourneerd. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Watch contacts added to a list]

Deze trekkermodule begint een scenario wanneer een nieuw contact aan een lijst wordt toegevoegd. Dit is alleen beschikbaar voor gebruikers met een betaalde marketingaccount.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Ga of kaart identiteitskaart van de lijst in die de contacten bevat u wilt letten op.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Selecteer de eigenschappen die u in de uitvoer van de module wilt opnemen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Overeenkomsten

* [[!UICONTROL List Deal/Ticket Pipelines]](#list-dealticket-pipelines)
* [[!UICONTROL Get a Deal's CRM Pipeline]](#get-a-deals-crm-pipeline)

#### [!UICONTROL List Deal/Ticket Pipelines]

Retourneert alle deal- en kaartpijpleidingen voor een bepaald portaal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Type] </td> 
   <td>Selecteer of u deals of tickets wilt weergeven.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a Deal's CRM Pipeline]

Keert een specifieke overeenkomstenpijpleiding terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pipeline ID] </td> 
   <td>Ga of kaart identiteitskaart van de pijpleiding in u details voor wilt terugwinnen. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stage ID] </td> 
   <td>Voer de id in van het werkgebied waarvoor u details wilt ophalen of wijs deze toe. </td> 
  </tr> 
 </tbody> 
</table>

### Bedrijven

#### [!UICONTROL Search for Companies by domain]

Haalt een lijst op van bedrijven die op een nauwkeurige gelijke met het domeinbezit worden gebaseerd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Domain] </td> 
   <td>Voer het domein in van de bedrijven waarnaar u wilt zoeken, zoals <code>[!DNL hubspot].com</code>. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Het maximumaantal ondernemingen [!DNL Workfront Fusion] moet tijdens één cyclus van de scenariouitvoering worden geretourneerd. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>Selecteer de eigenschappen die u in de uitvoer van de module wilt weergeven. </td> 
  </tr> 
 </tbody> 
</table>

### Bestanden

* [[!UICONTROL Create a Folder]](#create-a-folder)
* [[!UICONTROL Delete a Folder]](#delete-a-folder)
* [[!UICONTROL Move a File]](#move-a-file)

#### [!UICONTROL Create a Folder]

Deze module maakt een map.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder Name] </td> 
   <td>Voer een naam voor de nieuwe map in of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parent Folder ID] </td> 
   <td>Selecteer de id van de bovenliggende map voor de map die u maakt. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a Folder]

Hiermee markeert u een map als verwijderd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Voer de id in van de map die u wilt verwijderen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Move a File]

Hiermee verplaatst u een bestand naar een andere map.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID] </td> 
   <td>Voer de id in van het bestand dat u wilt verplaatsen of wijs deze toe. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td>Selecteer de id van de map waarin u het bestand wilt verplaatsen. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Voer een naam in voor het verplaatste bestand.</td> 
  </tr> 
 </tbody> 
</table>

### Tickets

#### [!UICONTROL Delete a Ticket]

Verwijdert een bestaand ticket met zijn id.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Voer de id in van het ticket dat u wilt verwijderen. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Make an API Call]

Hiermee kunt u een aangepaste API-aanroep uitvoeren.

>[!NOTE]
>
>De volgende eindpunten werden afgekeurd in HubSpot API op 31 Augustus, 2023, en kunnen niet meer in de modules van de Fusie worden gebruikt.
>
>* Gebeurtenissen voor inhoud weergeven
>* Sociale gebeurtenissen weergeven
>* Taakgebeurtenissen voor agenda weergeven
>* Alle kalendergebeurtenissen weergeven
>* Kalendertaak maken
>* Kalendertaak ophalen op id
>* Kalender bijwerken
>* Een kalendertaak verwijderen

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL HubSpot CRM] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Voer een pad in dat relatief is ten opzichte van https://api.hubapi.com/. Bijvoorbeeld /contacten/v1/lists/all/contacten/all</p> <p>Voor de lijst met beschikbare eindpunten raadpleegt u de <a href="https://legacydocs.hubspot.com/docs/overview">[!DNL HubSpot] API-documentatie</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Selecteer de HTTP-methode die u wilt gebruiken:</p> <p>[!UICONTROL GET]</p> <p>om informatie voor een ingang terug te winnen.</p> <p>[!UICONTROL POST]</p> <p>om een nieuw item te maken.</p> <p>[!UICONTROL PUT]</p> <p>om een bestaand item bij te werken of te vervangen.</p> <p>[!UICONTROL PATCH]</p> <p>om een gedeeltelijke ingsupdate te maken.</p> <p>[!UICONTROL DELETE]</p> <p>om een item te verwijderen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p> Voer de gewenste aanvraagheaders in. Je hoeft geen autorisatieheaders toe te voegen; dat hebben we al voor je gedaan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Voer de queryreeks voor de aanvraag in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.Wanneer u voorwaardelijke instructies gebruikt, zoals <code>if</code> in uw JSON, plaats de aanhalingstekens buiten de voorwaardelijke verklaring.<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Voorbeeld:** De volgende API vraag keert alle contacten in uw terug [!DNL HubSpot] account:
>
>**URL**: `/contacts/v1/lists/all/contacts/all`
>
>**Methode**: `GET`
>
>![](assets/hubspot-api-config.png)
>
>De gelijken van het onderzoek kunnen in de Output van de module onder worden gevonden [!UICONTROL Bundle] > [!UICONTROL Body] > [!UICONTROL contacts].
>
>In ons voorbeeld, zijn 3 contacten teruggekeerd:
>
>![](assets/hubspot-api-output.png)

## Een nieuwe toepassing maken

1. Aanmelden bij uw [!DNL HubSpot] ontwikkelaarsaccount.
1. Selecteer de **[!UICONTROL Create an App]** -optie.
1. Voer de toepassingsnaam in en [!UICONTROL Save] het dialoogvenster.
1. Selecteer het bereik dat u nodig hebt voor uw webhaak.

   Bijvoorbeeld, voeg contactwerkingsgebied voor het teweegbrengen van de module toe wanneer een nieuw contact wordt gecreeerd of geschrapt.

   De [!UICONTROL contacts scope] is alles u contacten, overeenkomsten, en de webhooks van de bedrijfgebeurtenis moet ontvangen.

   >[!IMPORTANT]
   >
   >Vul de [!UICONTROL Redirect URL] veld.
