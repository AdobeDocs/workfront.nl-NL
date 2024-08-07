---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Journey Optimizer-modules
description: In een  [!DNL Adobe Workfront Fusion]  scenario, kunt u werkschema's automatiseren die  [!DNL Adobe Journey Optimizer] gebruiken, evenals het met veelvoudige derdetoepassingen en de diensten verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: a2b9722f3964fccab6e30f2cd79e5ac63f736ba4
workflow-type: tm+mt
source-wordcount: '3247'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] modules

In een [!DNL Adobe Workfront Fusion] -scenario kunt u workflows automatiseren die [!DNL Adobe Journey Optimizer] gebruiken en deze koppelen aan meerdere toepassingen en services van derden. Met [!DNL Adobe Journey Optimizer] -modules kunt u records maken, lezen, bijwerken of verwijderen, of een aangepaste API-aanroep naar de [!DNL Adobe Journey Optimizer] API uitvoeren.


Als u instructies bij het creëren van een scenario nodig hebt, zie [ een scenario ](../../workfront-fusion/scenarios/create-a-scenario.md) creëren.

Voor informatie over modules, zie [ Modules in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table>
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

+++

## Vereisten

Voordat u de [!DNL Adobe Journey Optimizer] -connector kunt gebruiken, moet u controleren of aan de volgende voorwaarden is voldaan:

* U moet een actieve [!DNL Adobe Journey Optimizer] account hebben.

## Verbinding maken met Adobe Journey Optimizer

U kunt een verbinding maken in elke Adobe Journey Optimizer-module.

1. Klik op **[!UICONTROL Add]** naast het vak Verbinding.

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
        <td>Selecteer of u verbinding maakt met een productie- of niet-productieomgeving.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Selecteer of u verbinding maakt met een serviceaccount of een persoonlijke account.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Voer uw [!UICONTROL Adobe] [!UICONTROL Client ID] in. Dit vindt u in het gedeelte [!UICONTROL Credentials] Details van het dialoogvenster [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Voer uw [!DNL Adobe] [!UICONTROL Client Secret] in. Dit vindt u in het gedeelte [!UICONTROL Credentials] Details van het dialoogvenster [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Organization ID]</td>
        <td>Voer uw [!DNL Adobe] [!UICONTROL Organization ID] in. Dit vindt u in het gedeelte [!UICONTROL Credentials] Details van het dialoogvenster [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Sandbox Name]</td>
        <td>Voer de naam in van de sandbox die door deze verbinding wordt gebruikt.</td>
        </tr>
      </tbody>
    </table>


## [!DNL Adobe Journey Optimizer] modules en hun velden

Wanneer u [!DNL Adobe Journey Optimizer] modules configureert, geeft [!DNL Workfront Fusion] de onderstaande velden weer. Daarnaast kunnen aanvullende [!DNL Adobe Journey Optimizer] -velden worden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Voor meer informatie, zie [ informatie van de Kaart van één module aan een andere in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Configuratiebeheer](#configuration-management)
* [Pakketbeheer](#package-management)
* [Recordbeheer](#record-management)
* [Berichtenbeheer](#message-management)
* [Status](#status-checks)
* [Zoekopdrachten](#searches)
* [Overige](#other)




### Configuratiebeheer

* [Een configuratie maken](#create-a-configuration)
* [Een configuratie implementeren](#deploy-a-configuration)
* [Een configuratie bijwerken](#update-a-configuration)
* [Implementatie van een configuratie ongedaan maken](#undeploy-a-configuration)
* [Controleren of configuratie kan worden geïmplementeerd](#check-if-configuration-can-be-deployed)
* [Een configuratie verwijderen](#delete-a-configuration)
* [Een configuratie ophalen](#get-a-configuration)

#### Een configuratie maken

Deze actiemodule leidt tot een het in kaart brengen eindpunt of throttling configuratie.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select configuration type]</td> 
   <td>Selecteer of u een het maximum configuratie of een throttling configuratie creeert.<ul><li><p><b>Afbeelding</b></p>Ga aan <a href="#capping-fields" class="MCXref xref" > Afschilderende gebieden </a> verder.</li><li><p><b>Throttling</b></p>Ga aan <a href="#throttling-fields" class="MCXref xref" > Throtting gebieden </a> verder.</li></ul></td> 
  </tr> 
   </tbody> 
</table>

##### Velden uitlijnen

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Ga of kaart URL van het eindpunt in u wilt vormen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IMS Org ID]</td> 
   <td>Voer de Adobe IMS-id van de organisatie in of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methods]</td> 
   <td>Selecteer de methoden die u in deze configuratie wilt gebruiken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Service]</td> 
   <td>Selecteer of u een actie of een gegevensbron voor deze configuratie gebruikt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum HTTP connections]</td> 
   <td>Ga of kaart het maximumaantal gelijktijdige verbindingen aan dit eindpunt in.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum calls]</td> 
   <td>Ga of kaart het maximumaantal vraag in dat op de periode wordt uitgevoerd die op het gebied van de Periode wordt gespecificeerd.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Time period (milliseconds)]</td> 
   <td>Ga of kaart het aantal milliseconden in dat op het Maximum vraaggebied betrekking heeft.</td> 
  </tr> 
 </tbody> 
</table>

##### Verschuivende velden

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Ga of kaart een naam voor deze configuratie in.</td> 
<tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Ga of kaart een beschrijving voor deze configuratie in.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL URL pattern]</td> 
   <td>Ga of kaart URL voor het eindpunt in u wilt vertragen.</td> 
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methods]</td> 
   <td>Selecteer de methoden die u in deze configuratie wilt gebruiken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max throughput]</td> 
   <td>Selecteer of u een actie of een gegevensbron voor deze configuratie gebruikt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum HTTP connections]</td> 
   <td>Ga of kaart het maximumaantal gelijktijdige verbindingen aan dit eindpunt in.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum calls]</td> 
   <td>Ga of kaart de maximumproductie in die u voor dit eindpunt wilt. Deze waarde moet liggen tussen 200 en 5000.</td> 
  </tr> 
 </tbody> 
</table>

#### Een configuratie implementeren

Deze actiemodule stelt de gespecificeerde het in kaart brengen of het vertragen configuratie op.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select configuration type]</td> 
   <td>Selecteer of u een het begrenzen configuratie of een throttling configuratie opstelt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Configuration ID]</td> 
   <td>Ga of kaart identiteitskaart van de configuratie in u wilt opstellen.</td> 
  </tr> 
 </tbody> 
</table>

#### Een configuratie bijwerken

Deze actiemodule werkt de opgegeven configuratie voor het aftappen of vertragen bij.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select configuration type]</td> 
   <td>Selecteer of u een het maximum configuratie of een throttling configuratie bijwerkt.<ul><li><p><b>Afbeelding</b></p>Voor gebieden, zie <a href="#capping-fields" class="MCXref xref" > Afdekkende gebieden </a> in Create een configuratiesectie van dit artikel.</li><li><p><b>Throttling</b></p>Voor gebieden, zie <a href="#throttling-fields" class="MCXref xref" > Throtting gebieden </a> in Create een configuratiesectie van dit artikel.</li></ul></td> 
  </tr> 
  </tbody> 
</table>

#### Implementatie van een configuratie ongedaan maken

Deze actiemodule maakt de implementatie van een configuratie voor plafonneren of vertragen ongedaan. De configuratiestaat wordt veranderd terug naar de staat vóór de plaatsing (`created` of `updated`).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select configuration type]</td> 
   <td>Selecteer of u een het begrenzen configuratie of een throttling configuratie verwijdert.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Configuration ID]</td> 
   <td>Ga of kaart identiteitskaart van de configuratie in u wilt onbruikbaar maken.</td> 
  </tr> 
 </tbody> 
</table>

#### Controleren of configuratie kan worden geïmplementeerd

Deze actiemodule verifieert of een maximum of throttling configuratie kan worden opgesteld.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select configuration type]</td> 
   <td>Selecteer of u een het maximum configuratie of een throttling configuratie controleert.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Configuration ID]</td> 
   <td>Ga of kaart identiteitskaart van de configuratie in u wilt controleren.</td> 
  </tr> 
 </tbody> 
</table>

#### Een configuratie verwijderen

Deze actiemodule schrapt een het in kaart brengen eindpunt of throttling configuratie.

Als de configuratie is opgesteld, moet het worden gedesgroepeerd alvorens het kan worden geschrapt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select configuration type]</td> 
   <td>Selecteer of u een het begrenzen configuratie of een throttling configuratie schrapt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Configuration ID]</td> 
   <td>Ga of kaart identiteitskaart van de configuratie in u wilt schrappen.</td> 
  </tr> 
 </tbody> 
</table>

#### Een configuratie ophalen

Deze actiemodule keert de het begrenzen of vertragen configuratie terug die door gespecificeerde identiteitskaart wordt geïdentificeerd. De meest recente definitie wordt geretourneerd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select configuration type]</td> 
   <td>Selecteer of u een het begrenzen configuratie of een throttling configuratie terugwint.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Configuration ID]</td> 
   <td>Ga of kaart identiteitskaart van de configuratie in u wilt terugwinnen.</td> 
  </tr> 
 </tbody> 
</table>




### Pakketbeheer

* [Een pakket maken](#create-a-package)
* [Een pakket bijwerken](#update-a-package)
* [Een pakket verwijderen](#delete-a-package)
* [Een pakket opzoeken](#look-up-a-package)
* [Een pakket importeren](#import-a-package)
* [Publish een pakket](#publish-a-package)
* [Importeren verzenden](#submit-an-import)



#### Een pakket maken

Deze actiemodule maakt een pakket met meerdere artefacten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Voer een naam voor het pakket in of wijs een naam toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Voer een beschrijving van het pakket in of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expiration date]</td> 
   <td>Voer de tijdstempel in of wijs deze toe die de vervaldatum voor het pakket definieert. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Package type]</td> 
   <td>Selecteer het type pakket dat u wilt maken.<ul><li><p><b>Volledig</b></p>Het pakket bevat alle artefacten</p></li><li><p><b>Gedeeltelijk</b></p><p>Het pakket bevat alleen artefacten die u toevoegt. </p></li><ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Artifacts]</td> 
   <td>Als u een gedeeltelijk pakket creeert, voor elk artefact wilt u toevoegen, <b> klikken voegt artefact </b> toe en specificeert identiteitskaart, type, en titel van het artefact. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Sandbox]</td> 
   <td>Voer de naam en de IMS-organisatie-id in of wijs deze toe van de sandbox met de items die het pakket moet bevatten.</td> 
  </tr> 
 </tbody> 
</table>

#### Een pakket bijwerken

Met deze actiemodule kunt u artefacten uit een pakket toevoegen of verwijderen of pakketmetagegevens bijwerken.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select action]</td> 
   <td>Selecteer de actie die u wilt uitvoeren.<ul><li><p><b>Artefact toevoegen</b></p><p>Voor elk artefact wilt u toevoegen, <b> klikken vervorming </b> toevoegen en identiteitskaart van het artefact, type, en titel specificeren, dan ingaan of de vervaldatum voor het pakket in kaart brengen. </p></li><li><p><b>Artefact verwijderen</b></p><p>Voor elk artefact wilt u schrappen, <b> klikken voegt artefact </b> toe en specificeert identiteitskaart, type, en titel van het artefact. </p></li><li><p><b>Metagegevens bijwerken</b></p><p>Voer nieuwe waarden in voor de naam, beschrijving of naam van de bronsandbox of de IMS-organisatie-id.</p></li></ul></td> 
  </tr> 
 </tbody> 
</table>

#### Een pakket verwijderen

In deze actiemodule wordt een pakket met meerdere artefacten verwijderd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Package ID]</td> 
   <td>Voer de id in van het pakket dat u wilt verwijderen of wijs deze toe.</td> 
  </tr> 
 </tbody> 
</table>

#### Een pakket opzoeken

Deze actiemodule wint details van het gespecificeerde pakket terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Package ID]</td> 
   <td>Voer de id in van het pakket waarvoor u details wilt retourneren of wijs deze toe.</td> 
  </tr> 
 </tbody> 
</table>

#### Een pakket importeren

Deze actiemodule haalt de conflicterende objecten op in de opgegeven doelsandbox. Conflicterende objecten vertegenwoordigen vergelijkbare objecten die al aanwezig zijn in de doelsandbox.

U moet een pakket publiceren voordat u het kunt importeren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Package ID]</td> 
   <td>Voer de id in van het pakket dat u wilt importeren of wijs deze toe.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Target sandbox]</td> 
   <td>Typ of wijs de naam van de sandbox toe waar u het pakket wilt importeren.</td> 
  </tr> 
 </tbody> 
</table>

#### Publish een pakket

U moet een pakket publiceren voordat u het kunt importeren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Package ID]</td> 
   <td>Voer de id in van het pakket dat u wilt publiceren of wijs deze toe.</td> 
  </tr> 
 </tbody> 
</table>

#### Importeren verzenden

Deze actiemodule verzendt een import voor een pakket nadat u conflicten hebt bekeken en vervangende gegevens hebt opgegeven. Het resultaat wordt opgegeven als een payload, die de importtaak start voor de doelsandbox zoals opgegeven in de payload.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Package ID]</td> 
   <td>Voer de id in van het pakket dat u wilt publiceren of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Voer een naam in of wijs een naam toe aan de importtaak.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Een beschrijving van de importtaak invoeren of toewijzen</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL (Destination sandbox) Name]</td> 
   <td>Voer de naam in van de sandbox waarnaar u de importbewerking verzendt of wijs de naam hiervan toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL (Destination sandbox) IMS Org ID]</td> 
   <td>Voer de Adobe IMS-organisatie-id in of wijs deze toe voor de sandbox waarnaar u de import verzendt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL (Source sandbox) ID]</td> 
   <td>Voer de id in van de sandbox die het pakket bevat dat u wilt publiceren of wijs deze id toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL (Source sandbox) Type]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL (Source sandbox) Link]</td> 
   <td>Voer de koppeling in of wijs de koppeling toe voor het pakket dat u wilt publiceren.</td> 
  </tr> 
 </tbody> 
</table>


<!--

### Artifact management

* [Copy artifacts synchronously](#copy-artifacts-synchronously)
* [Export artifacts asynchronously](#export-artifacts-asynchronously)
* [Import artifacts asynchronously](#import-artifacts-asynchronously)

#### Copy artifacts synchronously

This action module copies artifacts from a source sandbox into a destination sandbox.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Enter or map a name for the new file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Enter or map a description for the new file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination sandbox]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Artifacts]</td> 
   <td>For each artifact you want to copy, click <b>Add artifact</b> and continue to <a href="#artifact-fields" class="MCXref xref" >Artifact fields</a>.</td> 
  </tr> 
 </tbody> 
</table>

##### Artifact fields

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the ID of the artifact.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Enter or map the artifact type, such as <code>REGISTRY_SCHEMA<code> or <code>JOURNEY</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Version]</td> 
   <td>Enter or map the visibility of the artifact. This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td>Enter or map the visibility (tenant or global). This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Found]</td> 
   <td>Select <b>Yes</b> if this item was found using a GET operation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tasks]</td> 
   <td>For each task you want to add, click <b>Add task</b> and fill in the following:
   <ul>
   <li><p><b>Method</b></p></li>
   <li><p><b>Action</b></p></li>
   <li><p><b>Using</b></p></li>
   <li><p><b>With</b></p></li>
   </ul>
   </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Messages]</td> 
   <td>For each task you want to add, click <b>Add message</b> and fill in the following:
   <ul>
   <li><p><b>Status</b></p><p>Enter or map the status that this message represents, such as <code>ERROR</code>.</li>
   <li><p><b>Attempt</b></p><p>Enter or map the attempt number related to this message. This may be useful if different attempts produce different messages.</p></li>
   <li><p><b>Message</b></p><p>Enter or map the text of the message.</li>
   <li><p><b>Object</b></p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

#### Export Artifacts asynchronously

This action module exports artifacts from the specified sandbox.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Enter or map a name for the export file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Enter or map a description for the export file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Artifacts]</td> 
   <td>For each artifact you want to export, click <b>Add artifact</b> and continue to <a href="#artifact-fields" class="MCXref xref" >Artifact fields</a>.</td> 
  </tr> 
 </tbody> 
</table>

##### Artifact fields

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the ID of the artifact.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Enter or map the artifact type, such as <code>REGISTRY_SCHEMA<code> or <code>JOURNEY</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Version]</td> 
   <td>Enter or map the visibility of the artifact. This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td>Enter or map the visibility (tenant or global). This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Found]</td> 
   <td>Select <b>Yes</b> if this item was found using a GET operation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tasks]</td> 
   <td>For each task you want to add, click <b>Add task</b> and fill in the following:
   <ul>
   <li><p><b>Method</b></p></li>
   <li><p><b>Action</b></p></li>
   <li><p><b>Using</b></p></li>
   <li><p><b>With</b></p></li>
   </ul>
   </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Messages]</td> 
   <td>For each task you want to add, click <b>Add message</b> and fill in the following:
   <ul>
   <li><p><b>Status</b></p><p>Enter or map the status that this message represents, such as <code>ERROR</code>.</li>
   <li><p><b>Attempt</b></p><p>Enter or map the attempt number related to this message. This may be useful if different attempts produce different messages.</p></li>
   <li><p><b>Message</b></p><p>Enter or map the text of the message.</li>
   <li><p><b>Object</b></p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>



#### Import Artifacts asynchronously

This action module imports a snapshot containing artifacts.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Snapshot ID]</td> 
   <td>Enter or map the ID of the snapshot you want to import.</td> 
  </tr> 
 </tbody> 
</table>

-->

### Recordbeheer

* [Een record maken](#create-a-record)
* [Een record bijwerken](#update-a-record)
* [Een record verwijderen](#delete-a-record)
* [Een record repareren](#patch-a-record)
* [Een record ophalen](#get-a-record)

#### Een record maken

In deze actiemodule wordt een nieuwe inhoudssjabloon of een nieuw inhoudsfragment gemaakt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select content type]</td> 
   <td>Selecteer of u een inhoudssjabloon of een inhoudsfragment maakt.<ul><li><p><b>Inhoudssjabloon</b></p>Ga aan <a href="#template-fields" class="MCXref xref" > gebieden van het Malplaatje </a> verder.</li><li><p><b>Inhoudsfragment</b></p>Ga aan <a href="#fragment-fields" class="MCXref xref" > gebieden van het Fragment </a> verder.</li></ul></td> 
  </tr> 
  </tbody> 
</table>

##### Sjabloonvelden

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Voer een naam voor deze inhoudssjabloon in of wijs deze toe.</td> 
<tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Voer een beschrijving voor deze inhoudssjabloon in of wijs deze toe.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Selecteer het type sjabloon dat u wilt maken.</td> 
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channels]</td> 
   <td>Selecteer de kanalen die in deze sjabloon zijn opgenomen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content template origin]</td> 
   <td>Selecteer de bron voor deze sjabloon.</td>  
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>Als u aangepaste eigenschappen in de nieuwe sjabloon wilt opnemen, selecteert u "Metagegevens toevoegen" en voert u de sleutel en waarde van de metagegevens in of wijst u deze toe. Herhaal dit voor elk aangepast veld dat u wilt opnemen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email HTML]</td> 
   <td>Voer de HTML in van het e-mailbericht dat in deze sjabloon is opgenomen of wijs dit toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Editor context]</td> 
   <td>Als u aangepaste eigenschappen in de e-mail wilt opnemen, selecteert u "Editor-context toevoegen" en voert u de sleutel en waarde van de context in of wijst u deze toe. Herhaal dit voor elk aangepast veld dat u wilt opnemen.</td> 
  </tr> 
 </tbody> 
</table>

##### Fragmentvelden

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Voer een naam in of wijs een naam toe aan dit inhoudsfragment.</td> 
<tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Voer een beschrijving voor dit inhoudsfragment in of wijs deze toe.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Selecteer het type sjabloon dat u wilt maken.</td> 
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channels]</td> 
   <td>Selecteer de kanalen die in deze sjabloon zijn opgenomen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content fragment origin]</td> 
   <td>Selecteer de bron voor dit fragment.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>Als u aangepaste eigenschappen in de nieuwe sjabloon wilt opnemen, selecteert u "Metagegevens toevoegen" en voert u de sleutel en waarde van de metagegevens in of wijst u deze toe. Herhaal dit voor elk aangepast veld dat u wilt opnemen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content]</td> 
   <td>Voer de inhoud van het fragment in of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Editor context]</td> 
   <td>Als u aangepaste eigenschappen in de e-mail wilt opnemen, selecteert u "Editor-context toevoegen" en voert u de sleutel en waarde van de context in of wijst u deze toe. Herhaal dit voor elk aangepast veld dat u wilt opnemen.</td> 
  </tr> 
 </tbody> 
</table>

#### Een record bijwerken

Deze actiemodule werkt een inhoudssjabloon of fragment bij.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select content type]</td> 
   <td>Selecteer of u een het maximum configuratie of een throttling configuratie bijwerkt.<ul><li><p><b>Sjabloon</b></p>Voor gebieden, zie {de gebieden van het 0} Malplaatje </a> in Create een verslagsectie van dit artikel.<a href="#template-fields" class="MCXref xref" ></li><li><p><b>Fragment</b></p>Voor gebieden, zie {de gebieden van het 0} Fragment </a> in Create een verslagsectie van dit artikel.<a href="#fragment-fields" class="MCXref xref" ></li></ul></td> 
  </tr> 
  </tbody> 
  </table>

#### Een record verwijderen

Met deze actiemodule verwijdert u een inhoudssjabloon of inhoudsfragment.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select content type]</td> 
   <td>Selecteer of u een inhoudssjabloon of inhoudsfragment verwijdert.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Template/Fragment ID]</td> 
   <td>Voer de id in van de sjabloon of het fragment dat u wilt verwijderen of wijs deze toe.</td> 
  </tr> 
 </tbody> 
</table>

#### Een record repareren

Deze actiemodule werkt een record bij met behulp van PATCH met JSON-aanwijzerindeling

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select content type]</td> 
   <td>Selecteer of u een inhoudssjabloon of inhoudsfragment patcheert.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Template/Fragment ID]</td> 
   <td>Voer de id in van de sjabloon of het fragment dat u wilt repareren of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Payload data]</td> 
   <td>Een record toevoegen aan de lading van deze patch: <ol><li>Klik <b> toevoegen een verslag </b>.</li><li>Selecteer de bewerking: Toevoegen, Verwijderen of Vervangen.</li><li>Selecteer in het veld Pad of u de naam of de beschrijving wilt repareren.</li><li> Voer in het veld Van een tekenreeks in of wijs een tekenreeks toe die een JSON-aanwijzerwaarde bevat.</li><li>Voer in het veld Waarde de waarde in die u in de bewerking wilt gebruiken.</li></ol></td> 
  </tr> 
 </tbody> 
</table>

#### Een record ophalen

Deze actiemodule retourneert de inhoudssjabloon of het inhoudsfragment dat door de opgegeven id wordt geïdentificeerd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select content type]</td> 
   <td>Selecteer of u een inhoudssjabloon of inhoudsfragment ophaalt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Template/Fragment ID]</td> 
   <td>Voer de id in of wijs deze toe aan de sjabloon of het fragment dat u wilt ophalen.</td> 
  </tr> 
 </tbody> 
</table>


### Berichtenbeheer

* [Eenvoudige berichtuitvoering activeren](#trigger-a-unitary-message-execution)
* [Een op het publiek gebaseerd bericht activeren](#trigger-an-audience-based-message)
* [Controleer de status van een bericht dat is gebaseerd op een publiek](#check-the-status-for-audience-based-message)



#### Eenvoudige berichtuitvoering activeren

Deze actiemodule activeert een eenheidbericht aan de ontvangers u specificeert.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Request ID]</td> 
   <td>Ga of kaart identiteitskaart van het verzoek verbonden aan dit bericht in.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campaign ID]</td> 
   <td>Voer de id van de campagne die aan dit bericht is gekoppeld in of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recipients]</td> 
   <td>Voor elke ontvanger wilt u dit bericht ontvangen, <b> toevoegen ontvanger </b> en ga het volgende in:
   <ul>
   <li><p><b>Type</b></p>Selecteer <code>aep</code> .</li>
   <li><p><b>Gebruikersnaam</b></p>Voer de Adobe Experience Platform Profile identifier van de ontvanger in of wijs deze toe.</li>
   <li><p><b>Naamruimte</b></p>Voer de Adobe Experience Platform Profile-naamruimte van de ontvanger in of wijs deze toe.</li>
   <li><p><b>E-mailadres</b></p></li>
   <li><p><b>Mobiel telefoonnummer</b></p></li>
   <li><p><b>Voornaam</b></p></li>
   <li><p><b>Achternaam</b></p></li>
   <li><p><b>Product</b></p>Ga of kaart het product verbonden aan dit bericht in. Dit wordt gebruikt voor dynamische veranderlijke vervanging in de berichtinhoud.</li>
   </ul></td> 
  </tr> 
 </tbody> 
</table>

#### Een op het publiek gebaseerd bericht activeren

Deze actiemodule brengt de uitvoering van een op publiek-gebaseerd bericht teweeg, dat op het verzoek en de campagne wordt gebaseerd u specificeert.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Request ID]</td> 
   <td>Ga of kaart identiteitskaart van het verzoek verbonden aan dit bericht in.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campaign ID]</td> 
   <td>Voer de id van de campagne die aan dit bericht is gekoppeld in of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Product]</td> 
   <td>Ga of kaart het product verbonden aan dit bericht in. Dit wordt gebruikt voor dynamische veranderlijke vervanging in de berichtinhoud.</td> 
  </tr> 
 </tbody> 
</table>

#### De status controleren voor een bericht op basis van een publiek

Deze actiemodule controleert de status van een publiek-gebaseerd partijbericht.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message execution ID]</td> 
   <td>Voer de id in van het bericht dat u wilt controleren of wijs deze toe.</td> 
  </tr> 
 </tbody> 
</table>

### Status

<!--* [Check service health](#check-service-health)-->
* [De importafhankelijkheden controleren](#check-the-import-dependencies)
* [De status van een importtaak controleren](#check-the-status-of-an-import-job)

<!--

#### Check service health

This action module checks that the service represented by the connection is running.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
 </tbody> 
</table>

-->

#### De importafhankelijkheden controleren

Deze actiemodule controleert de gebiedsdelen voor pakketartefacten. Op deze manier kunt u controleren of u machtigingen hebt om pakketartefacten te importeren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Package ID]</td> 
   <td>Voer de id in van het pakket waarvoor u machtigingen wilt controleren of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Target sandbox]</td> 
   <td>Typ of wijs de naam van de sandbox toe waarin u het pakket wilt importeren.</td> 
  </tr> 
 </tbody> 
</table>

#### De status van een importtaak controleren

Deze actiemodule controleert of een importtaak is gelukt of mislukt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Job ID]</td> 
   <td>Voer de id in van de taak waarvoor u gegevens wilt ophalen of wijs deze toe.</td> 
  </tr> 
 </tbody> 
</table>

### Zoekopdrachten

* [Alle afhankelijke objecten weergeven](#list-all-dependent-objects)
* [Lijstconfiguraties](#list-configurations)
* [Exporteer en importeer taken](#list-export-and-import-jobs)
* [Lijstpakketten](#list-packages)
* [Lijstrecords](#list-records)

#### Alle afhankelijke objecten weergeven

In deze zoekmodule worden alle afhankelijke objecten voor objecten in het opgegeven pakket weergegeven

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Package objects]</td> 
   <td>Voor elk voorwerp in het pakket dat u afhankelijk voorwerp voor wilt terugkeren, <b> voegt voorwerp </b> toe en gaat de naam en het type van objecten in.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Package ID]</td> 
   <td>Voer de id in van het pakket waarvoor u afhankelijke objecten wilt weergeven of wijs deze toe.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Target sandbox]</td> 
   <td>Typ of wijs de naam toe van de sandbox die het pakket bevat waarvoor u afhankelijke objecten wilt weergeven.</td> 
  </tr> 
 </tbody> 
</table>

#### Lijstconfiguraties

Deze actiemodule maakt een lijst van alle maximum of vertragende configuraties.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select configuration type]</td> 
   <td>Selecteer of u de configuraties van de plafondconfiguratie of een vertragende configuratie wilt vermelden.</td> 
  </tr> 
 </tbody> 
</table>

#### Exporteer en importeer taken

In deze zoekmodule wordt de huidige export- en importtaak vermeld. U kunt queryparameters gebruiken om de lijst te filteren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned results]</td> 
      <td>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
      <td>Selecteer of u resultaten wilt sorteren op gemaakte datum of op gewijzigde datum.</td>
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Query parameter]</td> 
   <td>Voor elke vraagparameter die u wilt filtreren door, <b> klikken voegt vraagparameter </b> toe, dan selecteert het gebied en de exploitant, en gaat de gebiedswaarde voor de filter in.</td> 
  </tr> 
 </tbody> 
</table>



#### Lijstpakketten

In deze zoekmodule worden alle pakketten in uw organisatie weergegeven. U kunt queryparameters gebruiken om de lijst te filteren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned results]</td> 
      <td>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
      <td>Selecteer of u resultaten wilt sorteren op gemaakte datum of op gewijzigde datum.</td>
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Query parameter]</td> 
   <td>Voor elke vraagparameter die u wilt filtreren door, <b> klikken voegt vraagparameter </b> toe, dan selecteert het gebied en de exploitant, en gaat de gebiedswaarde voor de filter in.</td> 
  </tr> 
 </tbody> 
</table>

#### Lijstrecords

Deze zoekmodule bevat een lijst met alle configuraties die kunnen worden bijgesneden of vertraagd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select content type]</td> 
   <td>Selecteer of u een inhoudssjabloon of inhoudsfragment ophaalt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td>Voer de parameternaam in of wijs deze toe waarop u deze lijst wilt sorteren. Voeg <code>-</code> of <code>+</code> toe om aflopend of oplopend te sorteren. Als er geen teken is opgegeven, wordt de lijst aflopend gesorteerd.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start]</td> 
   <td>Dit veld wordt gebruikt voor paginering. Voer de criteria voor de volgende pagina in of wijs deze toe met betrekking tot de eigenschap die in het veld Volgorde per veld is opgegeven.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td>Voer de parameternaam in of wijs deze toe waarop u deze lijst wilt sorteren. Voeg <code>-</code> of <code>+</code> toe om aflopend of oplopend te sorteren. Als er geen teken is opgegeven, wordt de lijst aflopend gesorteerd.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter by property]</td> 
   <td>Voor elke bezitsfilter wilt u toevoegen, <b> toevoegen punt </b> klikken en de sleutel en de waarde van het bezit ingaan. Records die de opgegeven waarde voor de eigenschap bevatten, worden in de lijst opgenomen.</td> 
  </tr> 
 </tbody> 
</table>


### Overige


#### Een aangepaste API-aanroep maken

Deze actiemodule maakt een aangepaste API-aanroep naar de Adobe Journey Optimizer API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Zie <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" > Verbinding maken met [!DNL Adobe Journey Optimizer]</a> in dit artikel voor instructies over het maken van een verbinding met [!DNL Adobe Journey Optimizer] .</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Voer een pad in ten opzichte van de basis-URL.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override=""> HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a> voor meer informatie.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p>
        <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] voegt automatisch machtigings-, <code>x-api-key</code> en <code>x-gw-ims-org-id</code> kopteksten toe.</p>
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
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:  <p>Wanneer u voorwaardelijke instructies gebruikt, zoals <code>if</code> in uw JSON, plaatst u de aanhalingstekens buiten de voorwaardelijke instructie.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>







<!--

* [Check if configuration can be deployed](#check-if-configuration-can-be-deployed)
* [Check service health](#check-service-health)
* [Check the import dependencies](#check-the-import-dependencies)
* [Check the status for audience-based message](#status-for-audience-based-message)
* [Copy artifacts synchronously](#copy-artifacts-synchronously)
* [Create a configuration](#create-a-configuration)
* [Create a package](#create-a-package)
* [Create a record](#create-a-record)
* [Delete a configuration](#delete-a-configuration)
* [Delete a package](#delete-a-package)
* [Delete a record](#delete-a-record)
* [Deploy a configuration](#deploy-a-configuration)
* [Export artifacts asynchronously](#export-artifacts-asynchronously)
* [Get a configuration](#get-a-configuration)
* [Get a record](#get-a-record)
* [Import a package](#import-a-package)
* [Import artifacts asynchronously](#import-artifacts-asynchronously)
* [List all dependent objects](#list-all-dependent-objects)
* [List export and import jobs](#list-import-and-export-jobs)
* [Look up a package](#look-up-a-package)
* [Make a custom API call](#make-a-custom-api-call)
* [Patch a record](#patch-a-record)
* [Publish a package](#publish-a-package)
* [Submit an import](#submit-an-import)
* [Trigger a unitary message execution](#trigger-a-unitary-message-execution)
* [Trigger an audience-based message](#trigger-an-audience-based-message)
* [Undeploy a configuration](#undeploy-a-configuration)
* [Update a configuration](#update-a-configuration)
* [Update a package](#update-a-package)
* [Update a record](#update-a-record)
* [List configurations](#list-configurations)
* [List packages](#list-packages)
* [List records](#list-records)

-->
