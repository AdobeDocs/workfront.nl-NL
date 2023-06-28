---
filename: powerbi-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Power BI
description: Adobe Workfront Fusion vereist naast een Adobe Workfront-licentie een Adobe Workfront Fusion-licentie.
author: Becky
exl-id: 01405f5f-6821-4c38-b34c-373922f63004
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1986'
ht-degree: 0%

---

# [!DNL Power BI] Modules

[!DNL Power BI] is een toepassing waarmee u gegevens kunt visualiseren en presenteren aan uw belanghebbenden. Het kan gegevens uit een verscheidenheid van bronnen nemen.

>[!NOTE]
>
>[!DNL Workfront Fusion] is geen gegevensbron. while [!DNL Workfront Fusion] kan gegevensbronnen maken en gebruiken, worden uw gegevens niet opgeslagen.


## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] of hoger</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!DNL Plan], [!DNL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige vergunningsvereiste: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereisten: Als u de [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Oudere productvereisten: Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

&#42;&#42;Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!DNL Power BI] modules en hun velden

Wanneer u [!DNL Power BI], [!DNL Workfront Fusion] geeft de onderstaande velden weer. Afhankelijk van factoren zoals uw toegangsniveau in de app of service, kunnen er naast deze velden mogelijk extra velden worden weergegeven. Een vette titel in een module geeft een vereist veld aan.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [Informatie van de ene module toewijzen aan de andere in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Dashboards

#### [!UICONTROL List Dashboards]

Deze zoekmodule haalt een lijst met dashboards op.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>
        <p>Selecteer of wijs identiteitskaart van de Groep toe die de dashboards bezit u wilt een lijst maken.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List Dashboard Tiles]

Deze zoekmodule haalt een lijst met dashboardtegels op.

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Enter a Dashboard ID]</td>
    <td>
      <p>Selecteer of wijs de optie toe om het dashboard te kiezen waarvan de tegels u wilt vermelden.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Dashboard ID]</td>
    <td>
      <p>Voer de id van het dashboard in of wijs deze toe met de tegels die u wilt weergeven.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Group ID]  </td>
    <td>Selecteer of wijs identiteitskaart van de Groep toe die de dashboards bezit die de tegels bevat u wilt een lijst maken.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Limit]  </td>
    <td>
      <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p>
    </td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Get a Dashboard]

Deze actiemodule wint meta-gegevens van een gespecificeerd dashboard terug.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Dashboard ID]</td>
      <td>
        <p>Selecteer of wijs de optie toe om het dashboard te kiezen waarvoor u meta-gegevens wilt terugwinnen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dashboard ID]</td>
      <td>
        <p>Voer de id van het dashboard in of wijs deze toe waarvoor u metagegevens wilt ophalen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Selecteer of wijs identiteitskaart van de Groep toe die het dashboard bezit dat u meta-gegevens voor wilt terugwinnen.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get a Dashboard Tile]

Deze actiemodule wint meta-gegevens van een gespecificeerde dashboardtegel terug.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Dashboard ID]</td>
      <td>
        <p>Selecteer of wijs de optie toe om de dashboarddetails te kiezen u wilt terugwinnen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dashboard ID]</td>
      <td>
        <p>Voer de id van het dashboard in of wijs deze toe waarvoor u details wilt ophalen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tile ID]</td>
      <td>Voer de id van de [!DNL Power BI] De tegel waarvoor u details wilt terugwinnen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Selecteer of wijs identiteitskaart van de Groep toe die de tegel bezit u wilt terugwinnen.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Create a Dashboard]

Deze actiemodule maakt een nieuw dashboard.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Voer een naam voor het dashboard in of wijs deze toe.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Selecteer of wijs identiteitskaart van de Groep toe die het nieuwe dashboard zal bezitten.</td>
    </tr>
  </tbody>
</table>

### Rapporten

#### [!UICONTROL List Reports]

Deze zoekmodule haalt een lijst met rapporten op.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>
        <p>Selecteer of wijs identiteitskaart van de Groep toe die de rapporten bezit u wilt een lijst maken.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get a Report]

Deze actiemodule wint meta-gegevens van een gespecificeerd rapport terug.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Selecteer of wijs de optie in kaart om het rapport te kiezen waarvoor u meta-gegevens wilt terugwinnen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Ga of kaart identiteitskaart van het rapport in dat u meta-gegevens voor wilt terugwinnen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Selecteer of wijs identiteitskaart van de Groep toe die het rapport bezit dat u meta-gegevens voor wilt terugwinnen.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Copy a Report]

Deze actiemodule kopieert een bestaand rapport.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Selecteer of wijs de optie in kaart om het rapport te kiezen dat u wilt kopiëren.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Ga of kaart identiteitskaart van het rapport in dat u wilt kopiëren.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Selecteer of wijs identiteitskaart van de Groep toe die het rapport bezit dat u wilt kopiëren.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL New Copied Report Name]</td>
      <td>Ga of kaart een naam voor het nieuwe rapport in.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Delete a Report]

Deze actiemodule verwijdert een rapport.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Selecteer of wijs de optie in kaart om het rapport te kiezen dat u wilt schrappen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Ga of kaart identiteitskaart van het rapport in dat u wilt schrappen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Selecteer of wijs identiteitskaart van de Groep toe die het rapport bezit dat u wilt schrappen.</td>
    </tr>
  </tbody>
</table>

### Gegevensset

#### [!UICONTROL List Datasets]

Deze onderzoeksmodule wint een lijst van datasets terug.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Selecteer of wijs identiteitskaart van de Groep toe die het rapport bezit dat u meta-gegevens voor wilt terugwinnen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>
        <p>Ga of kaart het maximumaantal verslagen in u de module aan [actie] tijdens elke cyclus van de scenariouitvoering wilt.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get a Dataset]

Deze actiemodule wint meta-gegevens van een gespecificeerde dataset terug.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Selecteer of wijs de optie in kaart om het rapport te kiezen waarvoor u meta-gegevens wilt terugwinnen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Ga of kaart identiteitskaart van de dataset in die u meta-gegevens voor wilt terugwinnen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Selecteer of wijs identiteitskaart van de Groep toe die de dataset bezit die u meta-gegevens voor wilt terugwinnen.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Create a Dataset]

Deze actiemodule leidt tot een nieuwe dataset.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Ga of kaart een naam voor de dataset in.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Selecteer of kaart identiteitskaart van de Groep die de nieuwe dataset zal bezitten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Default Mode]</td>
      <td>
        <p>Selecteer of wijs de standaardwijze voor de dataset toe:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL As Azure]</b>: Een dataset met een levende verbinding met [!DNL Azure Analysis Service]</p>
          </li>
          <li>
            <p><b>[!UICONTROL As on Prem]</b>: Een dataset met een levende verbinding met [!DNL On-premise Analysis] Service</p>
          </li>
          <li>
            <p><b>[!DNL Push]</b>: Een dataset die programmatic toegang voor het duwen van gegevens in toestaat [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Push Streaming]</b>: Een dataset die gegevens het stromen steunt en programmatische toegang toestaat voor het duwen van gegevens in [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Streaming]</b>: Een dataset die gegevens het stromen steunt</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tables]</td>
      <td>Voeg lijsten aan de dataset toe. Zie voor velden <a href="#Table" class="MCXref_0">Tabelvelden</a></td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Data sources]</td>
      <td>Voeg de gegevensbronnen toe. Zie voor velden <a href="#Data" class="MCXref_0">Gegevensbronvelden</a>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Default Retention Policy]  </td>
      <td>
        <p>Selecteer of wijs het opzettelijke beleid voor de dataset toe:</p>
        <ul>
          <li>
            <p>[!UICONTROL None]</p>
          </li>
          <li>
            <p>[!UICONTROL Basic FIFO]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Tabelvelden

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>
        <p>  Voer een naam voor de tabel in of wijs deze toe.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Columns]</td>
      <td>
        <p>Voeg de kolommen toe:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Voer (kaart) een kolomnaam in.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Data Type]</b>
            </p>
            <p>Selecteer of wijs het gegevenstype toe:</p>
            <ul>
              <li>
                <p>[!UICONTROL String]</p>
              </li>
              <li>
                <p>[!UICONTROL Integer]</p>
              </li>
              <li>
                <p>[!UICONTROL Boolean]</p>
              </li>
              <li>
                <p>[!UICONTROL Date Time]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>[!UICONTROL Format String]</b>
            </p>
            <p>Voer de indelingstekenreeks in (kaart).</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rows]</td>
      <td>Voer rijdetails in of wijs deze toe.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Measures]</td>
      <td>Voeg de maatregel voor de lijsten toe.</td>
    </tr>
  </tbody>
</table>

##### Gegevensbronvelden

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Database]  </td>
      <td>
        <p>Voer de database die u wilt gebruiken in of wijs deze toe.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Server]  </td>
      <td>
        <p>Voer de naam in of wijs de naam toe van de server die u wilt gebruiken.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]  </td>
      <td>
        <p>Voer de gewenste URL in of wijs deze toe.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data source ID]</td>
      <td>
        <p>  Voer de id van de gegevensbron in of wijs deze toe.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data source Type]  </td>
      <td>
        <p>Selecteer of wijs het gegevenstype van de gegevensbron in kaart. Voorbeeld: SQL.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gateway ID]  </td>
      <td>Ga of kaart identiteitskaart van de gateway in u wilt gebruiken.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Add or Delete Rows in a Dataset Table]

Deze actiemodule voegt rijen van een gespecificeerde lijst van duwdataset toe of schrapt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a table]</td>
      <td>Selecteer of wijs de optie toe om de dataset te selecteren die de lijst bevat u wilt aanpassen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dataset ID]</td>
      <td>Ga of kaart identiteitskaart van de dataset in die de rijen bevat u wilt toevoegen of schrappen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Table Name]  </td>
      <td>
        <p>Typ of wijs de naam toe van de tabel die de rijen bevat die u wilt toevoegen of verwijderen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Ga of kaart identiteitskaart van de groep in die de dataset bezit.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Select the Action]</td>
      <td>
        <p>Selecteer of wijs de actie toe die u wilt uitvoeren.</p>
        <ul>
          <li>
            <p>[!UICONTROL Add rows]</p>
          </li>
          <li>
            <p>[!UICONTROL Delete All Rows]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rows]</td>
      <td>
        <p>Voeg de rijvelden toe.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Key]</b>
            </p>
            <p>Voer de sleutelnaam in of wijs deze toe.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Field Type]</b>
            </p>
            <p>Selecteer of wijs het veldtype toe:</p>
            <ul>
              <li>
                <p>Boolean</p>
              </li>
              <li>
                <p>Datum</p>
              </li>
              <li>
                <p>Tekst</p>
              </li>
              <li>
                <p>Getal</p>
              </li>
            </ul>
          </li>
          <li>
            <p>[!UICONTROL Value]</p>
            <p>Voer de sleutelwaarde in of wijs deze toe.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Refresh a Dataset]

Deze actiemodule vernieuwt een gespecificeerde dataset.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a dataset]</td>
      <td>Selecteer of wijs de optie in kaart om de dataset te selecteren die u wilt verfrissen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dataset ID]</td>
      <td>Ga of kaart identiteitskaart van de dataset in die u wilt verfrissen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Table Name]  </td>
      <td>
        <p>Typ of wijs de naam toe van de tabel die de rijen bevat die u wilt toevoegen of verwijderen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Ga of kaart identiteitskaart van de groep in die de dataset bezit.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Notify Option]  </td>
      <td>
        <p>Selecteer of wijs de optie toe om op de hoogte te brengen:</p>
        <ul>
          <li>
            <p>[!UICONTROL Mail on Completion]</p>
          </li>
          <li>
            <p>[!UICONTROL Mail on Failure]</p>
          </li>
          <li>
            <p>[!UICONTROL No Notification]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Delete a Dataset]

Deze actiemodule schrapt een dataset.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Selecteer of wijs de optie in kaart om de dataset te kiezen die u wilt schrappen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Ga of kaart identiteitskaart van de dataset in die u wilt schrappen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Selecteer of wijs identiteitskaart van de Groep toe die de dataset bezit die u wilt schrappen.</td>
    </tr>
  </tbody>
</table>

### Apps

#### [!UICONTROL Watch Apps]

Deze triggermodule start een scenario wanneer een app wordt bijgewerkt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List Apps]

Deze zoekmodule haalt een lijst op met alle geïnstalleerde apps.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List App's Reports]

Deze zoekmodule haalt een lijst op met alle rapporten in de opgegeven app.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]</td>
      <td>Selecteer of wijs de id van de app toe waaruit u rapporten wilt weergeven.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List App's Dashboards]

Deze zoekmodule haalt een lijst met dashboards op uit een opgegeven app.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]</td>
      <td>Selecteer of wijs de id van de app toe waaruit u de dashboards wilt weergeven.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get an App]

Deze actiemodule haalt metagegevens van een opgegeven toepassing op.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Selecteer of wijs de id toe van de app die u wilt ophalen.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get an App's Report]

Deze actiemodule haalt metagegevens op van het rapport van een opgegeven app.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Selecteer of wijs identiteitskaart van app toe die het rapport bevat u wilt terugwinnen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>  Selecteer of wijs identiteitskaart van het rapport toe u wilt terugkeren.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get an App's Dashboard]

Deze actiemodule haalt metagegevens op van het dashboard van een opgegeven app.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Selecteer of wijs de id van de app toe die het dashboard bevat dat u wilt ophalen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>  Selecteer of wijs identiteitskaart van het dashboard toe u wilt terugkeren.</p>
      </td>
    </tr>
  </tbody>
</table>

### Overige

#### [!UICONTROL Make an API Call]

Deze actiemodule voert een API-aanroep uit naar de [!DNL Power BI] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Power BI] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Een pad invoeren ten opzichte van <code>https://api.powerbi.com</code>. Voorbeeld: <code>/v1.0/myorg/datasets</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
      <td>
        <p>Selecteer [!UICONTROL HTTP] request method you need to configure the API call. Zie voor meer informatie [!UICONTROL HTTP] aanvraagmethoden.</p>
      </td>
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
