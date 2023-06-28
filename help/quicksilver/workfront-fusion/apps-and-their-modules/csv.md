---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: CSV
description: Met de Adobe Workfront Fusion CSV-modules kunt u CSV-bestanden maken en CSV-tekst parseren op basis van een ontvangen tekstwaarde of een bestand.
author: Becky
feature: Workfront Fusion
exl-id: 4e37482a-e84e-4ab2-a48f-7e7bfbecee56
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 0%

---

# CSV

De [!DNL Adobe Workfront Fusion] [!UICONTROL CSV] Met modules kunt u CSV-bestanden maken en CSV-tekst parseren op basis van een ontvangen tekstwaarde of een bestand.

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
   <p>Huidige vergunningsvereiste: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor arbeidsautomatisering en -integratie],  [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
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

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Create CSV]

De [!UICONTROL Create CSV] Met aggregator kunt u een CSV-tekst maken van ontvangen tekstwaarden.

Voor meer informatie over aggregators, zie [Samenvoegmodule in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Selecteer de module die u gebruikt om de velden samen te voegen die u nodig hebt.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Aggregated Fields]</td>
        <td>Selecteer de velden die u wilt samenvoegen in de lijst met beschikbare velden.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Include headers in the first row]</td>
        <td>Selecteer deze optie om de kopteksten in het resultaat op te nemen.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Group by]</td>
        <td>Voer het filter in om de resultaten te groeperen. Voer bijvoorbeeld een datum in.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Stop processing after an empty aggregation]</td>
        <td>Selecteer deze optie om het scenario te stoppen als er geen resultaten zijn.</td>
    </tr>
</table>

## [!UICONTROL Create CSV (advanced)]

De [!UICONTROL Create CSV (advanced)] Met aggregator kunt u een CSV-tekst maken van ontvangen tekstwaarden. Er wordt een gegevensstructuur gebruikt die de CSV-kolommen in het resulterende CSV-bestand definieert. Zodra bepaald, verschijnen de kolommen als gebieden in de CSV moduleopstelling, en kunnen aan recentere module in het scenario worden in kaart gebracht.

Voor meer informatie over aggregators, zie [Samenvoegmodule in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td>Selecteer de toepassingsmodule die u gebruikt om de velden samen te voegen die u nodig hebt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data Structure]</td> 
   <td> <p>Selecteer de gegevensstructuur om de velden op de gewenste manier samen te voegen. Nadat u de gegevensstructuur hebt gedefinieerd, kunt u de items toewijzen aan de corresponderende velden.</p> <p>Zie voor meer informatie <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Gegevensstructuren in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include headers in the first row] </td> 
   <td>Selecteer deze optie om de kopteksten in het resultaat op te nemen. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by] </td> 
   <td>Voer het filter in om de resultaten te groeperen. Voer bijvoorbeeld een datum in. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stop processing after an empty aggregation] </td> 
   <td>Selecteer deze optie om het scenario te stoppen als er geen resultaten zijn. </td> 
  </tr> 
 </tbody> 
</table>


<p>Laten we aannemen dat u uw Google-contactpersonen wilt exporteren naar een CSV-bestand met twee kolommen Volledige naam en E-mail. De uitvoerbundel van de [!UICONTROL Google Contacts] &gt;[!UICONTROL Get contacts from a group] heeft de volgende structuur. De e-mailadressen worden opgeslagen in de <code>[!UICONTROL Emails[]]</code> item, dat een array van verzamelingen is, waarbij elke verzameling twee items bevat: <code>Label</code> en <code>Email</code>.</p>
<p> <img src="assets/transforming-350x546.png" style="width: 350;height: 546;"> </p>
<p>Als u de eenvoudige [!DNL Create CSV] wordt u een lijst aangeboden met selectievakjes die overeenkomen met de items op hoofdniveau van een bundel. Als u probeert te tikken <code>Full name</code> en <code>Emails</code> items, de [!UICONTROL Create CSV] de volgende output veroorzaakt, die waarschijnlijk niet is wat u wilt:</p>
<p>"emails","fullName"</p>
<p>"[object Object]","Winner delen"</p>
<p>"[object Object]","Lizeth Fulmore"</p>
<p>"[object Object]","Hilario Gullatt"</p>
<p>"[Object Object Object]","Abby Eisenbarth"</p>
<p>Sinds het object <code>Full Name</code> is van het eenvoudige typeTekst, wordt het uitgevoerd enkel fijn. Maar het item <code>Emails</code>, een complex type Array van verzamelingen, wordt geëxporteerd als [objectobject]. Op deze manier worden verzamelingen en arrays standaard omgezet in tekst. Zie voor meer informatie <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Gegevenstypen item in Adobe Workfront Fusion</a>.</p>
<p>Inhoud van het dialoogvenster exporteren <code>Email </code>item van de eerste collectie van de <code>Emails[]</code> in plaats daarvan, is het noodzakelijk om [!UICONTROL Create CSV (advanced)] module. De module laat u toe om individuele kolommen van uw Csv- dossier te bepalen en punten aan hen, met inbegrip van genestelde degenen in kaart te brengen.</p>
<ol>
<li value="1">De module invoegen [!UICONTROL Create CSV (advanced)] in een scenario en open zijn configuratie.</li>
<li value="2">Klik op de knop <strong>[!UICONTROL Add]</strong> naast de knop [!UICONTROL Data structure] om een nieuwe gegevensstructuur te maken.</li>
<li value="3"> <p>Schrijf een naam voor de gegevensstructuur en klik op de knop <strong>[!UICONTROL Add item]</strong> om de afzonderlijke kolommen toe te voegen. Als u twee kolommen wilt exporteren: "Volledige naam" en "E-mail" zou de resulterende gegevensstructuur er als volgt uitzien:</p> <p> <img src="assets/google-contacts-350x524.png" style="width: 350;height: 524;"> </p> </li>
<li value="4"> <p>Als u de gegevensstructuur hebt gedefinieerd, worden de velden die overeenkomen met elke kolom weergegeven in de configuratie van het dialoogvenster [!UICONTROL Create CSV (advanced)] zodat u de items kunt toewijzen. Het eerste item uit de <code>[!UICONTROL Emails[]]</code> array en wijs het item toe <code>Email </code>in het veld/de kolom E-mail:</p> <p> <img src="assets/create-csv-advanced-350x308.png" style="width: 350;height: 308;"> </p> </li>
<li value="5"> <p>Voer het scenario uit. Sinds het object <code>Emails[1]: Email</code> toegewezen aan kolom "E-mail" is van het eenvoudige type Tekst, wordt nu correct geëxporteerd:</p> <p>"Volledige naam","E-mail"</p> <p>"Shon Winer","Shon@Winer.com"</p> <p>"Lizeth Fulmore","Lizeth@Fulmore.com"</p> <p>"Hilario Gullatt","Hilario@Gullatt.com"</p> <p>"Abby Eisenbarth","Abby@Eisenbarth.com"</p> </li>
</ol>
</div>

## [!UICONTROL Parse CSV]

De [!UICONTROL Parse CSV] Met de transformator kunt u CSV-tekst parseren van een ontvangen tekstwaarde of een bestand.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number of columns]</td> 
   <td>Geef het aantal kolommen op in het CSV-bestand.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV contains headers]</td> 
   <td> <p>Selecteer deze optie als de eerste rij van de CSV-tekst kopteksten bevat.</p> <p>Opmerking: De module gebruikt deze kopballen niet om de kolommen in de output te etiketteren. In plaats daarvan zorgt dit veld ervoor dat de kopteksten niet worden opgenomen in de uitvoergegevens.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL delimiterType]</td> 
   <td> <p>Selecteer het scheidingsteken voor het CSV-bestand. Het scheidingsteken is het tekstteken dat de grens tussen afzonderlijke waarden of velden aangeeft.</p> 
    <ul> 
     <li>[!UICONTROL Comma]</li> 
     <li>[!UICONTROL Tab]</li> 
     <li> <p>[!UICONTROL Other]</p> <p>Als u [!UICONTROL Other]voert u het scheidingsteken in dat het CSV-bestand gebruikt om waarden van elkaar te scheiden. U moet precies één teken invoeren.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Preserve quotes inside unquoted field]</td> 
   <td>Schakel deze optie in om de aanhalingstekens te behouden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV]</td> 
   <td>Voer het CSV-bestand in of wijs het toe dat u wilt parseren.<p>Opmerking: <p>Als uw gegevens binair zijn (doorgaans uit een bestand), moet u de functie ` toString()` gebruiken om de binaire gegevens om te zetten in [!UICONTROL String]:</p><p><img src="assets/parse-csv-350x123.png" style="width: 350;height: 123;"></p></p></td> 
  </tr> 
 </tbody> 
</table>
