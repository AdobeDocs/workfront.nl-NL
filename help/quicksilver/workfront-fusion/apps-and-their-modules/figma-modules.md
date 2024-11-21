---
filename: figma-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Figuurmodules
description: Met de  [!DNL Adobe Workfront Fusion]  modules van Figma, kunt u lijsten van commentaren, dossiers, dossierversies, of projecten terugwinnen. U kunt ook een opmerking plaatsen of een aanroep van de figma-API maken.
author: Becky
feature: Workfront Fusion
exl-id: d88db592-32d4-4765-952f-9ffb58cf1720
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '2025'
ht-degree: 0%

---

# [!DNL Figma] Modules

Met de modules [!DNL Adobe Workfront Fusion] [!DNL Figma] kunt u lijsten met opmerkingen, bestanden, bestandsversies of projecten ophalen. U kunt ook een opmerking plaatsen of de [!DNL Figma] API aanroepen.

Als u instructies bij het creëren van een scenario nodig hebt, zie [ een scenario ](../../workfront-fusion/scenarios/create-a-scenario.md) creëren.

Voor informatie over modules, zie [ Modules in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Vereisten

Als u [!DNL Figma] -modules wilt gebruiken, moet u een [!DNL Figma] -account hebben.

## Informatie over de figuren-API

De Figma-aansluiting gebruikt het volgende:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td> https://api.figma.com/v1</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-versie</td> 
   <td> v1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-tag</td> 
   <td>v1.8.25</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Figma] modules en hun velden

Wanneer u [!DNL Figma] modules configureert, geeft [!DNL Workfront Fusion] de onderstaande velden weer. Daarnaast kunnen aanvullende [!DNL Figma] -velden worden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Voor meer informatie, zie [ informatie van de Kaart van één module aan een andere in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Opmerkingen](#comments)

* [Projecten en bestanden](#projects-and-files)

* [Componenten en stijlen](#components-and-styles)

* [Overige](#other)


### Opmerkingen

* [Een opmerking verwijderen](#delete-a-comment)

* [Opmerkingen weergeven](#list-comments)

* [Opmerkingen plaatsen](#post-a-comment)


#### [!UICONTROL Delete a comment]

In deze actiemodule wordt één opmerking uit een bestand verwijderd.

<table style="table-layout:auto"> 
  <col/>
  <col />
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Voor instructies over het verbinden van uw [!DNL Figma] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies.</a></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>Voer de bestands-id in of wijs de bestands-id toe van het bestand waaruit u een opmerking wilt verwijderen. </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comment]</td>
      <td>Voer de tekst in van de opmerking die u wilt verwijderen.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List comments]

In deze zoekmodule worden alle opmerkingen weergegeven die aan één bestand in [!DNL Figma] zijn gekoppeld.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Voor instructies over het verbinden van uw [!DNL Figma] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Voer de bestands-id in of wijs deze toe aan het bestand waarvoor u opmerkingen wilt ophalen. </p>
        <ul>
          <li>
            <p>Als u de id niet kent, klikt u op <b>[!UICONTROL Find Files]</b> en voert u de id in of wijst u deze toe aan het project waaraan het bestand is gekoppeld. Selecteer vervolgens het bestand.</p>
          </li>
          <li>
            <p>Als u niet identiteitskaart van het project kent, klik <b>[!UICONTROL Find Projects]</b> en ga of kaart identiteitskaart van het team in dat het project bezit het dossier wordt geassocieerd met, dan selecteer het project, dan het dossier.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Ga of kaart het maximumaantal commentaren in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Post a comment]

In deze actiemodule wordt een opmerking naar een figuurbestand gepost.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Voor instructies over het verbinden van uw [!DNL Figma] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies.</a></p>
    </tr>
    <tr>
      <td  role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Voer de bestands-id in of wijs deze toe aan het bestand waarnaar u een opmerking wilt plaatsen. </p>
        <ul>
          <li>
            <p>Als u de id van het bestand niet kent, klikt u op <b>[!UICONTROL Find Files]</b> en voert u de id in of wijst u deze toe aan het project waaraan het bestand is gekoppeld. Selecteer vervolgens het bestand.</p>
          </li>
          <li>
            <p>Als u probeert om identiteitskaart van het dossier te vinden en niet identiteitskaart van het project kent, klik <b>[!UICONTROL Find Projects]</b> en ga of kaart identiteitskaart van het team in dat het project bezit het dossier wordt geassocieerd met. Selecteer het project en selecteer het bestand.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comment]</td>
      <td>Voer de tekst van de opmerking in.</td>
    </tr>
  </tbody>
</table>


### Projecten en bestanden

* [Een bestand of afbeelding ophalen](#get-a-file-or-image)

* [Versiehistorie van bestand weergeven](#list-file-version-history)

* [Projectbestanden weergeven](#list-project-files)

* [Projecten weergeven](#list-projects)


#### [!UICONTROL Get a file or image]

Met deze actiemodule haalt u één bestand of afbeelding op uit een figuurbibliotheek

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Voor instructies over het verbinden van uw [!DNL Figma] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Object type]</td>
      <td>
        <p>Selecteer het type object dat u wilt ophalen.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL File]</b>
            </p>
            <p>De module retourneert het document waarnaar [!UICONTROL Key] verwijst als een JSON-object. De bestandstoets kan vanuit elke URL van het figuurbestand worden geparseerd.</p>
            <p>Zie <a href="#Get2" class="MCXref xref" >[!UICONTROL Get a file or image: File]</a> voor velden.</p>
          </li>
          <li>
            <p><b>[!UICONTROL File nodes]</b>
            </p>
            <p>Retourneert de knooppunten waarnaar door id's wordt verwezen als een JSON-object. De knooppunten worden opgehaald uit het [!DNL Figma] -bestand waarnaar wordt verwezen door [!UICONTROL Key] .</p>
            <p>Zie <a href="#Get3" class="MCXref xref" >[!UICONTROL Get a file or image: File nodes]</a> voor velden.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Image]</b>
            </p>
            <p>De module rendert afbeeldingen uit een bestand.</p>
            <p>Zie <a href="#Get4" class="MCXref xref" >[!UICONTROL Get a file or image: Image]</a> voor velden.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Image fills]</b>
            </p>
            <p>De module retourneert downloadkoppelingen voor alle afbeeldingen die zich in afbeeldingsvullingen in een document bevinden. Afbeeldingsvullingen vormen de manier waarop [!DNL Figma] door de gebruiker opgegeven afbeeldingen vertegenwoordigt. Wanneer u een afbeelding naar [!DNL Figma] sleept, maakt [!DNL Figma] een rechthoek met één vulling die de afbeelding vertegenwoordigt en kan de gebruiker de rechthoek (en de eigenschappen van de vulling) transformeren.</p>
            <p>Zie <a href="#Get5" class="MCXref xref" >[!UICONTROL Get a file or image: Image fills]</a> voor velden.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL Get a file or image: File]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Selecteer het bestand waaruit u JSON wilt retourneren.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Version ID]</td>
      <td>Ga of kaart de versie van het dossier in u de module wilt terugkeren. Laat dit veld leeg voor de huidige module.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Node IDs]</td>
      <td>
        <p>Als u alleen een subset van het document wilt retourneren, voert u de knooppunten in die de module moet retourneren. De module keert de vermelde knopen, hun kinderen, en om het even wat tussen de wortelknoop en de vermelde knopen terug.</p>
        <p>Voor elk knooppunt dat u wilt retourneren, klikt u op <b>[!UICONTROL Add]</b> en voert u de tekst van het knooppunt in.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Depth]</td>
      <td>
        <p>Voer een geheel getal in of wijs een geheel getal toe dat aangeeft hoe diep in de documentstructuur u de resultaten voor wilt retourneren. </p>
        <div class="example"><span class="autonumber"><span><b> Voorbeeld: </b></span></span>
          <ul>
            <li>
              <p>Voer <code>1</code> in als u alleen pagina's wilt retourneren.</p>
            </li>
            <li>
              <p>Voer <code>2</code> in als u pagina's en objecten op het hoogste niveau wilt retourneren.</p>
            </li>
          </ul>
        </div>
        <p>Laat dit veld leeg als u alle knooppunten wilt retourneren.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometry]</td>
      <td>Voer <code>paths</code> in om vectorgegevens te retourneren.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Plugin data]</td>
      <td>Een komma gescheiden lijst van stop - identiteitskaarts en/of het koord "[!UICONTROL shared]". Alle gegevens die aanwezig zijn in het document dat door deze plug-ins wordt geschreven, worden opgenomen in het resultaat in de eigenschappen <code>pluginData</code> en <code>sharedPluginData</code> .</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Branch data]</td>
      <td>Schakel deze optie in om metagegevens van vertakkingen te retourneren voor het gevraagde bestand. Als het bestand een vertakking is, wordt de sleutel van het hoofdbestand opgenomen in het geretourneerde antwoord. Als het bestand vertakkingen heeft, worden de metagegevens opgenomen in het geretourneerde antwoord. Standaard: <code>false</code>.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Get a file or image: File nodes]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Selecteer het bestand waaruit u JSON wilt retourneren.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Node IDs]</td>
      <td>
        <p>Voer de knooppunten in die u wilt retourneren en converteren</p>
        <p>Voor elk knooppunt dat u wilt retourneren, klikt u op <b>[!UICONTROL Add]</b> en voert u de tekst van het knooppunt in.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Version ID]</td>
      <td>Ga of kaart de versie van het dossier in u de module wilt terugkeren. Laat dit veld leeg voor de huidige module.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Depth]</td>
      <td>
        <p>Voer een geheel getal in of wijs een geheel getal toe dat aangeeft hoe diep in de documentstructuur u de resultaten voor wilt retourneren. </p>
        <div class="example"><span class="autonumber"><span><b> Voorbeeld: </b></span></span>
          <ul>
            <li>
              <p>Voer <code>1</code> in als u alleen pagina's wilt retourneren.</p>
            </li>
            <li>
              <p>Voer <code>2</code> in als u pagina's en objecten op het hoogste niveau wilt retourneren.</p>
            </li>
          </ul>
        </div>
        <p>Laat dit veld leeg als u alle knooppunten wilt retourneren.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometry]</td>
      <td>Voer <code>paths</code> in om vectorgegevens te retourneren.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Plugin data]</td>
      <td>Een door komma's gescheiden lijst met insteekmodules en/of de tekenreeks "shared". Alle gegevens die aanwezig zijn in het document dat door deze plug-ins wordt geschreven, worden opgenomen in het resultaat in de eigenschappen pluginData en sharedPluginData.</td>
    </tr>
  </tbody>
</table>


##### Een bestand of afbeelding ophalen: Afbeelding

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Selecteer het bestand waaruit u JSON wilt retourneren.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Node IDs]</td>
      <td>
        <p>Ga de knopen in die u de module wilt teruggeven.</p>
        <p>Voor elk knooppunt dat u wilt renderen, klikt u op <b>[!UICONTROL Add]</b> en voert u de tekst van het knooppunt in.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Scale]</td>
      <td>Als u de afbeelding wilt schalen, voert u de schaalfactor in of wijst u deze toe. Dit getal moet tussen 0,01 en 4 liggen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Format]</td>
      <td>
        <p>Selecteer de indeling voor de uitgevoerde afbeelding.</p>
        <ul>
          <li>
            <p>JPG</p>
          </li>
          <li>
            <p>PNG</p>
          </li>
          <li>
            <p>SVG</p>
          </li>
          <li>
            <p>PDF</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - Include ID]</td>
      <td>Schakel deze optie in om id-kenmerken op te nemen voor alle SVG-elementen. Standaard: [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - Simplify Stroke]</td>
      <td>Schakel deze optie in om binnenomlijnen en buitenomlijnen te vereenvoudigen en gebruik indien mogelijk het lijnkenmerk in plaats van &lt;mask&gt;. Standaard: [!UICONTROL true].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Use absolute bounds]</td>
      <td>Schakel deze optie in om de volledige afmetingen van het knooppunt te gebruiken, ongeacht of het knooppunt wordt uitgesneden of dat de ruimte rondom het knooppunt leeg is. Gebruik deze optie om tekstknooppunten te exporteren zonder ze uit te snijden. Standaard: [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Version ID]</td>
      <td>Ga of kaart de versie van het dossier in u de module wilt terugkeren. Laat dit veld leeg voor de huidige module.</td>
    </tr>
  </tbody>
</table>

##### Een bestand of afbeelding ophalen: afbeeldingsvullingen

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Selecteer het bestand waaruit u JSON wilt retourneren.</td>
    </tr>
  </tbody>
</table>

### [!UICONTROL List file version history]

Deze zoekmodule retourneert de versiegeschiedenis van één bestand in [!UICONTROL Figma] .
<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Voor instructies over het verbinden van uw [!DNL Figma] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies.</a></p>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Voer de bestands-id in of wijs deze toe aan het bestand waarvoor u versiehistorie wilt ophalen. </p>
        <ul>
          <li>
            <p>Als u de id van het bestand niet kent, klikt u op <b>[!UICONTROL Find Files]</b> en voert u de id in of wijst u deze toe aan het project waaraan het bestand is gekoppeld. Selecteer vervolgens het bestand.</p>
          </li>
          <li>
            <p>Als u probeert om identiteitskaart van het dossier te vinden en niet identiteitskaart van het project kent, klik <b>[!UICONTROL Find Projects]</b> en ga of kaart identiteitskaart van het team in dat het project bezit het dossier wordt geassocieerd met. Selecteer het project en selecteer het bestand.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List project files]

Deze zoekmodule retourneert een lijst met alle bestanden in het opgegeven project.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Voor instructies over het verbinden van uw [!DNL Figma] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Ga of kaart identiteitskaart van het Project in het project dat u dossiers voor wilt terugwinnen. </p>
        <ul>
          <li>
            <p>Als u niet identiteitskaart van de projecten kent, klik <b>[!UICONTROL Find Projects]</b> en ga of kaart identiteitskaart van het team in dat het project met wordt geassocieerd, dan selecteer het project.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List projects]

Deze onderzoeksmodule keert een lijst van alle projecten binnen het gespecificeerde team terug.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Voor instructies over het verbinden van uw [!DNL Figma] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Team ID]</td>
      <td>Ga of kaart identiteitskaart van het Project van het project in dat u dossiers voor wilt terugwinnen. De team-id vindt u in de URL van de pagina van het team in Figma</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</td>
    </tr>
  </tbody>
</table>


### Componenten en stijlen

#### [!UICONTROL Get a style or component]

Deze actiemodule haalt één stijl of component, of een reeks stijlen of componenten op.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Voor instructies over het verbinden van uw [!DNL Figma] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies.</a></p>
    </tr>
    <tr>
      <td role="rowheader">&lt;[!UICONTROL Object> key]</td>
      <td>Voer de sleutel (unieke id) in van het object dat u wilt ophalen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Team ID]</td>
      <td>Ga of kaart identiteitskaart van het team in dat het verslag of de verslagen met worden geassocieerd.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Page Size]</td>
      <td>Voer het aantal of de resultaten die u per pagina wilt retourneren in of wijs dit toe. Standaard: 30.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL After]</td>
      <td>
        <p>Voer het nummer in van het resultaat waarna u de resultaten wilt ophalen of wijs het resultaat toe. Dit kan met het [!UICONTROL Page Size] gebied worden gecombineerd om resultaten te pagineren.</p>
        <p>Deze waarde komt niet overeen met object-id's.</p>
        <p>Dit veld kan niet worden gebruikt in combinatie met het veld [!UICONTROL Before] .</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Before]</td>
      <td>
        <p>Voer het nummer in van het resultaat voordat u het resultaat wilt ophalen of wijs dit toe. Dit kan met het [!UICONTROL Page Size] gebied worden gecombineerd om resultaten te pagineren.</p>
        <p>Deze waarde komt niet overeen met object-id's.</p>
        <p>Dit veld kan niet worden gebruikt in combinatie met het veld [!UICONTROL After] .</p>
      </td>
    </tr>
  </tbody>
</table>


### Overige

* [Een API-aanroep maken](#make-an-api-call)

* [Gebeurtenissen van Let](#watch-events)


#### [!UICONTROL Make an API call]

Deze actiemodule laat u een douane voor authentiek verklaarde vraag aan Figma API maken zonder het moeten door authentificatie denken. Op deze manier kunt u een automatisering van de gegevensstroom maken die niet door de andere modules van Figma kan worden verwezenlijkt.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Voor instructies over het verbinden van uw [!DNL Figma] rekening met [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Voer een pad in dat relatief is ten opzichte van <code>https://api.figma.com/v1/</code> .</p>
        <p>Bijvoorbeeld: <code>[!DNL files/7179110/comments]</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Method]</td>
      <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override=""> HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a> voor meer informatie.</p> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p>
        <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] Hiermee voegt u de machtigingsheaders voor u toe.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]</td>
      <td>
        <p>Voeg de query voor de API-aanroep toe als een standaard JSON-object.</p>
        <p>Bijvoorbeeld: <code>{"name":"something-urgent"}</code></p>
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

#### [!UICONTROL Watch events]

Deze triggermodule start een scenario wanneer een van de volgende gebeurtenissen plaatsvindt voor een specifiek team in de teamruimte van [!DNL Figma]

* Bestandsupdate

* Bestandsversie bijwerken

* Bestand verwijderen

* Bibliotheek publiceren

* Opmerking bestand

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>
        <p>Selecteer de webhaak die in de module wordt gevolgd.</p>
        <p>Een nieuwe webhaak toevoegen:</p>
        <ol>
          <li value="1">
            <p>Klik op <b>[!UICONTROL Add]</b> naast het veld [!UICONTROL Webhook] .</p>
          </li>
          <li value="2">
            <p>Selecteer de verbinding die u voor deze webhaak wilt gebruiken. Voor instructies over het verbinden van uw [!DNL Figma] rekening met [!UICONTROL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!UICONTROL Adobe Workfront Fusion] - Basisinstructies.</a></p>
          </li>
          <li value="3">
            <p>Selecteer het gebeurtenistype dat u de module wilt controleren.</p>
          </li>
          <li value="4">
            <p>Voer de id in van het team waarvan u de gebeurtenissen wilt bekijken die de webhaak moet bekijken.</p>
          </li>
          <li value="5">
            <p>Voer de waarde [!UICONTROL Status] of [!UICONTROL Description] in van gebeurtenissen die de webhaak moet controleren.</p>
          </li>
          <li value="6">
            <p>Klik op <b>[!UICONTROL Save]</b> om de webhaak op te slaan en terug te keren naar de module.</p>
          </li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>
