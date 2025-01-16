---
filename: microsoft-word-templates-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft Word-sjabloonmodules
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 889b417c-04a9-4dbf-9a34-0dab65f11f03
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1332'
ht-degree: 0%

---

# [!DNL Microsoft Word Template] modules

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ de modules van het Malplaatje van Microsoft Word ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/microsoft-word-templates-modules.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

In een [!DNL Adobe Workfront Fusion] -scenario kunt u workflows automatiseren die [!DNL Microsoft Word Templates] gebruiken en deze koppelen aan meerdere toepassingen en services van derden.

Als u instructies bij het creëren van een scenario nodig hebt, zie [ een scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) creëren.

Voor informatie over modules, zie [ Modules in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> 
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
 </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

Als u [!DNL Miscrosoft Word Templates] met [!DNL Adobe Workfront Fusion] wilt gebruiken, hebt u een [!DNL Office 365] -account nodig. U kunt er een maken op www.office.com.



## De service [!DNL Office] verbinden met [!DNL Workfront Fusion]

Voor instructies over het aansluiten van uw [!DNL Office] rekening aan [!UICONTROL Workfront Fusion], zie [ een verbinding tot stand brengen [!UICONTROL Adobe Workfront Fusion] - Basisinstructies ](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Sommige Microsoft-toepassingen gebruiken dezelfde verbinding, die is gekoppeld aan individuele gebruikersmachtigingen. Daarom bij het creëren van een verbinding, toont het scherm van de toestemmingstoestemming om het even welke toestemmingen die eerder aan de verbinding van deze gebruiker werden verleend, naast om het even welke nieuwe toestemmingen nodig voor de huidige toepassing.
>
>Bijvoorbeeld, als een gebruiker &quot;Gelezen lijst&quot;toestemmingen heeft die via de schakelaar van Excel worden verleend en dan een verbinding in de schakelaar van Vooruitzichten creeert om e-mails te lezen, zal het scherm van de toestemmingstoestemming zowel de reeds verleende &quot;Gelezen lijst&quot;toestemming en de onlangs vereiste &quot;Schrijf e-mail&quot;toestemming tonen.

## [!DNL Microsoft Word Templates] modules gebruiken

Met een module [!DNL Microsoft Word Template] kunt u gegevens van meerdere webservices samenvoegen in een [!DNL Microsoft Word] -document.

U kunt bijvoorbeeld deze [!DNL Microsoft Word] -sjabloon gebruiken:

![](assets/word-template-before-filled-350x62.png)

Dit document maken:

![](assets/word-template-exampled-filled-350x85.png)

## Waardetags

Een [!DNL Microsoft Word] -sjabloon is een regulier [!DNL Microsoft Word] -document (.docx-bestand) met speciale codes in de tekst die bepalen waar en hoe gegevens moeten worden samengevoegd of ingevuld. Er zijn drie typen tags:

* [ Eenvoudige waardetag ](#simple-value-tag)
* [ markering van de Voorwaarde ](#condition-tag)
* [Tag herhalen](#loop-tag)

### Tag voor eenvoudige waarde {#simple-value-tag}

Een eenvoudige waardetag wordt eenvoudig vervangen door een overeenkomstige waarde. De naam van de tag komt overeen met de waarde van het veld [!UICONTROL Key] , die binnen dubbele accolades wordt geplaatst, bijvoorbeeld `{{name}}` .

**Voorbeeld:** om een document tot stand te brengen dat &quot;Hi, Petr!&quot;zegt, kon u een [!DNL Microsoft Word Template] module gebruiken om het volgende malplaatje tot stand te brengen:

```
> Hi {{name}}!
```

Hiervoor stelt u de module als volgt in:

![](assets/word-template-simple-value-350x286.png)

### Voorwaardetag {#condition-tag}

U kunt een voorwaardelabel gebruiken om tekst te laten omlopen die alleen moet worden gerenderd als aan bepaalde voorwaarden is voldaan. Als u de tekst wilt laten omlopen, plaatst u deze tussen openingstag en afsluitingstag, bijvoorbeeld &quot;hasPhone&quot; als de voorwaarde is of de gegevens al dan niet een telefoonnummer bevatten. De naam van een openingstag wordt voorafgegaan door een hash-teken #. De naam van een afsluitende tag wordt voorafgegaan door een slash /, zoals in het onderstaande voorbeeld wordt getoond.

**Voorbeeld:** om een document te veroorzaken dat het telefoonaantal van een klant omvat als de inputgegevens een telefoonaantal, maar geen e-mailadres omvatten, kon u een [!DNL Microsoft Word Template] module gebruiken en het volgende malplaatje creëren:

```
> {{#hasPhone}}Phone: {{phone}} {{/hasPhone}}
> {{#hasEmail}}Email: {{email}} {{/hasEmail}}
```

Hiervoor stelt u de module als volgt in:

![](assets/word-template-conditional-350x501.png)

In het document ziet het telefoonnummer er als volgt uit:

```
> Phone: 4445551234
```

### Tag herhalen {#loop-tag}

U kunt een sectie met tekst herhalen met een lustag, ook wel sectietag genoemd. Plaats de tekst tussen de openings- en sluitingslustags. De naam van een openingstag wordt voorafgegaan door een hash-teken #. De naam van een afsluitende tag wordt voorafgegaan door een slash /.

* [ markering van de Lijn met Vul een documentmodule ](#loop-tag-with-fill-out-a-document-module)
  <!-- [Loop tag with Fill a document with a batch of data module](#loop-tag-with-fill-a-document-with-a-batch-of-data-module)-->

#### Tag herhalen met een documentmodule invullen {#loop-tag-with-fill-out-a-document-module}

**Voorbeeld:** om een document te veroorzaken dat van de naam en het telefoonaantal van elk contact in een klantenlijst een lijst maakt, kon u a [!DNL Microsoft Word Template] module gebruiken en het volgende malplaatje creëren:

```
> {{#contact}}
>     {{name}}, {{phone}}
> {{/contact}}
```

Hiervoor stelt u de module als volgt in:


![](assets/word-template-fill-out-a-document-350x732.png)

In de module wordt het volgende document gemaakt:

```
> Jan Toman, 4445551234
> Eduard Salo, 4445552345
```

<!--

#### Loop tag with Fill a document with a batch of data module {#loop-tag-with-fill-a-document-with-a-batch-of-data-module}

**Example:** You can export Google contacts into a table that you create using loop tags.

The first module loads the template. The next module retrieves all contacts from the group you specify in [!DNL Google Contacts]. The aggregator module aggregates all values retrieved from Google Contacts and merges them into the template. And the last module saves the filled template to the desired location.

![](assets/word-template-batch-scenario-350x124.png)

You could use this scenario with the following template:

![](assets/word-template-batch-template-350x26.png)

To do this, you would set up the module as follows:

![](assets/word-template-batch-module-setup-350x323.png)

The module would create the following document:

![](assets/word-template-batch-document-350x46.png)
-->

## [!DNL Microsoft Word Template] modules

Deze modules vereisen geen verbinding.

* [ Vul een document ](#fill-out-a-document)
* [Een document vullen met een batch gegevens](#fill-a-document-with-a-batch-of-data)

### [!UICONTROL Fill out a document] {#fill-out-a-document}

Met deze transformatormodule kunt u een document vullen met gegevens die u opgeeft. Deze kan worden gebruikt met eenvoudige waardetags, voorwaardelijke tags of lustags.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start delimiter of the text being replaced]</td> 
   <td> <p>Voer de tekens in die u wilt markeren aan het begin van de tekst die wordt vervangen. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b> Voorbeeld: </b></span></span> ga binnen <code>[[</code> als u een tekst gelijkend op dit wilt vervangen: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL End delimiter of the text being replaced]</p> </td> 
   <td> <p>Voer de tekens in die u wilt markeren aan het einde van de tekst die wordt vervangen. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b> Voorbeeld: </b></span></span> ga binnen <code>]]</code> als u een tekst gelijkend op dit wilt vervangen: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p> Wijs het bestand toe dat u vanuit de vorige module wilt uploaden (bijvoorbeeld HTTP &gt; Een bestand of Dropbox ophalen &gt; Een bestandsmodule ophalen). U kunt het gegevensbestand ook handmatig invoeren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name of filled out file]</td> 
   <td>Voer een bestandsnaam (inclusief extensie) in voor het doeluitvoerbestand.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data source]</td> 
   <td> <p>Selecteer een optie om aan te geven of de gegevens die u gebruikt afkomstig zijn uit een formulier of uit een Raw-gegevensverzameling (onverwerkte computergegevens).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td> <p>Dit moet een array van verzamelingen zijn, waarbij:</p> 
    <ul> 
     <li>Elke verzameling komt overeen met één gegevensitem en bevat één item <code>entry</code></li> 
     <li>Het punt <code>entry </code> bevat een inzameling van <code>key </code> en <code>value</code></li> 
     <li>Het punt <code>key </code> bevat de naam van de markering</li> 
     <li>het punt <code>value </code> bevat de waarde van de markering</li> 
    </ul> 
    <p>Een item toevoegen:</p>
    <ol> 
     <li> Klik op <b>[!UICONTROL Add Item]</b>. </li> 
     <li>Selecteer het waardetype van de ingang.</li> 
     <li>Voeg de naam en waarde toe. Zie het voorbeeld voor het gekozen waardetype in dit artikel voor meer informatie. 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">Tag voor eenvoudige waarde</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">Voorwaardetag</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">Tag herhalen</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Fill a document with a batch of data] {#fill-a-document-with-a-batch-of-data}

Deze aggregatormodule is handig als de gegevensinvoer uit afzonderlijke bundels bestaat. Met deze module, kunt u opstelling gemakkelijk de structuur die voor het gebied van de Waarde wordt vereist en het punten aan elk waardepunt in kaart brengen. In tegenstelling tot de module Een document invullen staat het veld Waarden in het veld Een document vullen met een batch gegevensmodule slechts één item met variabelen toe.

U kunt deze module ook gebruiken als uw gegevensingangen als serie komen, door de *module van de Teller te gebruiken 0} {om de inhoud van de serie in een reeks bundels om te zetten.*

De werkelijke waarden worden gemaakt en ingevuld voor elke binnenkomende bundel. De sjabloon wordt gemaakt nadat alle invoerbundels zijn verwerkt.

Deze aggregatormodule is vooral handig voor het maken van lijsten of rapporten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td>Selecteer de module die de bron van de tekst is.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start delimiter of the text being replaced]</td> 
   <td> <p>Voer de tekens in die u wilt markeren aan het begin van de tekst die wordt vervangen. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b> Voorbeeld: </b></span></span> ga binnen <code>[[</code> als u een tekst gelijkend op dit wilt vervangen: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL End delimiter of the text being replaced]</p> </td> 
   <td> <p>Voer de tekens in die u wilt markeren aan het einde van de tekst die wordt vervangen. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b> Voorbeeld: </b></span></span> ga binnen <code>]]</code> als u een tekst gelijkend op dit wilt vervangen: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by]</td> 
   <td> Definieer een expressie die een of meer in kaart gebrachte items bevat. De samengevoegde gegevens worden gescheiden onder Groepen met de waarde van dezelfde expressie. Elke groep voert als afzonderlijke bundel uit die een Sleutel met de geëvalueerde uitdrukking en de samengevoegde tekst bevat. Door dit te doen, kunt u Sleutel als filter in verdere modules gebruiken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>Schakel deze optie in om de verwerking te stoppen wanneer een aggregatie geen bundels bevat.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p> Wijs het bestand toe dat u vanuit de vorige module wilt uploaden (bijvoorbeeld HTTP &gt; Een bestand of Dropbox ophalen &gt; Een bestandsmodule ophalen). U kunt het gegevensbestand ook handmatig invoeren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name of filled out file]</td> 
   <td>Voer een bestandsnaam (inclusief extensie) in voor het doeluitvoerbestand.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data source]</td> 
   <td> <p>Selecteer een optie om aan te geven of de gegevens die u gebruikt afkomstig zijn uit een formulier of uit een Raw-gegevensverzameling (onverwerkte computergegevens).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td> <p>Dit moet een array van verzamelingen zijn, waarbij:</p> 
    <ul> 
     <li>Elke verzameling komt overeen met één gegevensitem en bevat één item <code>entry</code></li> 
     <li>Het punt <code>entry </code> bevat een inzameling van <code>key </code> en <code>value</code></li> 
     <li>Het punt <code>key </code> bevat de naam van de markering</li> 
     <li>het punt <code>value </code> bevat de waarde van de markering</li> 
    </ul> 
    <p>Een item toevoegen:</p>
    <ol> 
     <li> Klik op <b>[!UICONTROL Add Item]</b>. </li> 
     <li>Selecteer het waardetype van de ingang.</li> 
     <li>Voeg de naam en waarde toe. Zie het voorbeeld voor het gekozen waardetype in dit artikel voor meer informatie. 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">Tag voor eenvoudige waarde</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">Voorwaardetag</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">Tag herhalen</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>
