---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Google Docs-modules
description: De Adobe Workfront Fusion [!DNL Google Docs] met modules kunt u documenten in uw [!DNL Google Docs] en [!DNL Google Docs] (voor [!DNL G Suite]-gebruikers).
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: fbe7d628-d833-43ce-83b8-8e4e6a812fd1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '3326'
ht-degree: 0%

---

# [!DNL Google Docs] modules

De [!DNL Adobe Workfront Fusion] [!DNL Google Docs] met modules kunt u documenten in uw [!DNL Google Docs] en [!DNL Google Docs] (for [!DNL G Suite] gebruikers).

Voor gebruik [!DNL Google Docs] with [!DNL Adobe Workfront Fusion], is het noodzakelijk [!DNL Google] account. Als u geen [!DNL Google] -account nog kunt u er een maken op de [!DNL Google] Help-pagina voor account.

Als u instructies bij het creëren van een scenario nodig hebt, zie [Een scenario maken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Voor informatie over modules, zie [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

Te gebruiken [!DNL Google Docs] hebt u een Google-account nodig.

## [!DNL Google Docs] modules en hun velden

Wanneer u [!DNL Google Docs] modules, [!UICONTROL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Google Docs] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Document

* [[!UICONTROL Watch Documents]](#watch-documents)
* [[!UICONTROL List Documents]](#list-documents)
* [[!UICONTROL Get Content of a Document]](#get-content-of-a-document)
* [[!UICONTROL Create a Document]](#create-a-document)
* [[!UICONTROL Create a Document From a Template]](#create-a-document-from-a-template)
* [[!UICONTROL Insert a Paragraph to a Document]](#insert-a-paragraph-to-a-document)
* [[!UICONTROL Insert an Image to a Document]](#insert-an-image-to-a-document)
* [[!UICONTROL Replace an Image with a New Image]](#replace-an-image-with-a-new-image)
* [[!UICONTROL Replace Text in a Document]](#replace-text-in-a-document)
* [[!UICONTROL Download a Document]](#download-a-document)
* [[!UICONTROL Delete a Document]](#delete-a-document)

#### [!UICONTROL Watch Documents]

Deze triggermodule retourneert documentdetails wanneer een nieuw document wordt gemaakt of gewijzigd in de geselecteerde map.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch Documents]</td> 
   <td> <p style="color: #000000;">Selecteer of u de aanmaak wilt controleren ([!UICONTROL By Created Date]) of gewijzigd ([!UICONTROL By Modified Date]).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Selecteer het type station dat u wilt controleren.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selecteer de map die u wilt controleren voor gemaakte of gewijzigde documenten.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Selecteer de map die u wilt controleren voor gemaakte of gewijzigde documenten.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Gedeeld station]</strong> (beschikbaar voor [!DNL G Suite] alleen gebruikers)</p> <p>Selecteer of u wilt [!UICONTROL Use Domain Admin Access]. Selecteren [!UICONTROL Yes] geeft het verzoek uit als domeinbeheerder, en alle gedeelde aandrijving waarin de aanvrager een beheerder is teruggekeerd.</p> <p>Selecteer het gedeelde station dat u wilt controleren.</p> <p>Opmerking: Als u de optie [!DNL Google Shared Drive] in dit veld en u bent geen [!DNL G Suite] gebruiker, de fout <code>[400] Invalid Value</code> wordt geretourneerd.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Stel het maximumaantal documenten in dat Workfront Fusion in één uitvoeringscyclus retourneert.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Documents]

Deze actiemodule wint een lijst van documenten van de geselecteerde omslag terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Selecteer het type station waaruit u documenten wilt weergeven.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selecteer de map waaruit u documenten wilt weergeven.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Selecteer de map waaruit u documenten wilt weergeven.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Gedeeld station]</strong> (beschikbaar voor [!DNL G Suite] alleen gebruikers)</p> <p>Selecteer of u wilt [!UICONTROL Use Domain Admin Access]. Selecteren [!UICONTROL Yes] geeft het verzoek uit als domeinbeheerder, en alle gedeelde aandrijving waarin de aanvrager een beheerder is teruggekeerd.</p> <p>Selecteer het gedeelde station waarvan u documenten wilt weergeven.</p> <p>Opmerking: Als u de optie [!DNL Google Docs] in dit veld en u bent geen [!DNL G Suite] gebruiker, de fout <code>[400] Invalid Value</code> wordt geretourneerd.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Het maximum aantal documenten instellen [!DNL Workfront Fusion] retourneert in één uitvoeringscyclus.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Content of a Document]

Met deze actiemodule wordt een opgegeven document opgehaald.

Mogelijk moet u uw machtigingen uitbreiden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get Content of a Document]</td> 
   <td> <p>Selecteer of u de document-id van het document wilt toewijzen of het document handmatig in het keuzemenu wilt selecteren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Selecteer het type station dat het document bevat dat u wilt ophalen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selecteer de map met het document dat u wilt ophalen.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Selecteer de map met het document dat u wilt ophalen.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Gedeeld station]</strong> (beschikbaar voor [!DNL G Suite] alleen gebruikers)</p> <p>Selecteer of u wilt [!UICONTROL Use Domain Admin Access]. Selecteren [!UICONTROL Yes] geeft het verzoek uit als domeinbeheerder, en alle gedeelde aandrijving waarin de aanvrager een beheerder is teruggekeerd.</p> <p>Selecteer het gedeelde station dat het document bevat dat u wilt ophalen.</p> <p>Opmerking: Als u de optie [!DNL Google Docs] in dit veld en u bent geen [!DNL G Suite] gebruiker, de fout <code>[400] Invalid Value</code> wordt geretourneerd.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Selecteer het object dat u wilt retourneren in de uitvoer van de module.</p> 
    <ul> 
     <li>[!UICONTROL Image] (standaard)</li> 
     <li>[!UICONTROL Drawing]</li> 
     <li>[!UICONTROL Chart]</li> 
    </ul> <p>Opmerking:  <p>Gebruik voor het verder toewijzen van deze objecten de [!UICONTROL Inline Objects Array] waarde in de uitvoer van deze module (in plaats van [!UICONTROL inlineObjects]).</p> <p>De [!UICONTROL Inline Objects Array] objecten worden in dezelfde volgorde gesorteerd als in het document. Het maakt verdere verwerking gemakkelijker.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a Document]

In deze actiemodule kunt u een nieuw document maken in de geselecteerde map.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Voer de naam van het document in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content]</td> 
   <td> <p>Voer de inhoud van het document in. HTML wordt ondersteund.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Selecteer het type station waarop u een document wilt maken.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selecteer de map waarin u een document wilt maken.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Selecteer de map waarin u een document wilt maken.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Gedeeld station]</strong> (beschikbaar voor [!DNL G Suite] alleen gebruikers)</p> <p>Selecteer of u wilt [!UICONTROL Use Domain Admin Access]. Selecteren [!UICONTROL Yes] geeft het verzoek uit als domeinbeheerder, en alle gedeelde aandrijving waarin de aanvrager een beheerder is teruggekeerd.</p> <p>Selecteer het gedeelde station waar u een document wilt maken.</p> <p>Opmerking: Als u de optie [!DNL Google Docs] in dit veld en u bent geen [!DNL G Suite] gebruiker, de fout <code>[400] Invalid Value</code> wordt geretourneerd.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Insert a Header]</td> 
   <td> <p> Schakel deze optie in om de koptekst in te voegen in het document en voer vervolgens de tekst van de koptekst in of wijs deze toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Insert a Footer] </td> 
   <td> <p>Schakel deze optie in om de voettekst in te voegen in het document en voer vervolgens de tekst van de koptekst in of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a Document From a Template]

In deze actiemodule wordt een kopie van een bestaand sjabloondocument gemaakt en worden alle tags vervangen. In deze module kunnen gebruikers ook afbeeldingen vervangen door nieuwe afbeeldingen door URL&#39;s.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Create a Document from a Template]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Selecteer deze optie om de documentsjabloon toe te wijzen.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br>Selecteer deze optie om de documentsjabloon in het keuzemenu te kiezen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Selecteer het type station waarop de sjabloon zich bevindt. Deze optie is beschikbaar als u [!UICONTROL By Dropdown] in het vorige veld.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selecteer de map waarin de sjabloon zich bevindt.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Selecteer de map waarin de sjabloon zich bevindt.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Gedeeld station]</strong> (beschikbaar voor [!DNL G Suite] alleen gebruikers)</p> <p>Selecteer of u wilt [!UICONTROL Use Domain Admin Access]. Selecteren [!UICONTROL Yes] geeft het verzoek uit als domeinbeheerder, en alle gedeelde aandrijving waarin de aanvrager een beheerder is teruggekeerd.</p> <p>Selecteer de gedeelde schijf waarop uw sjabloon zich bevindt.</p> <p>Opmerking: Als u de optie [!DNL Google Docs] in dit veld en u bent geen [!DNL G Suite] gebruiker, de fout <code>[400] Invalid Value</code> wordt geretourneerd.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Values]</p> </td> 
   <td> <p>Voer de waarden in die u wilt invoeren in plaats van de variabelen voor het nieuwe document.</p> 
    <ul> 
     <li><strong>[!UICONTROL Tags]</strong> <br>Voer de tags in die zich in de documentsjabloon bevinden. Niet gebruiken <code>&#123;&#123;&#125;&#125;</code>. Voorbeeld: gebruiken <code>name</code> in plaats van <code>&#123;&#123;name&#125;&#125;</code>.</li> 
     <li><strong>[!UICONTROL Replaced Value]</strong><br>Voer de waarde van de tag in.</li> 
    </ul> <p>Bijvoorbeeld de<code> &#123;&#123;name&#125;&#125;</code> variabele in het brondocument wordt hier weergegeven als het naamveld, waar de waarde kan worden ingevoegd, zoals <code>John</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Images Replacement]</p> </td> 
   <td> <p>Voer de koppeling naar de [!UICONTROL Image Object ID] en [!UICONTROL Image URL] Hiermee vervangt u de huidige afbeelding.</p> <p>Opmerking: U kunt de afbeeldings-id's ophalen met [!UICONTROL Get a Document] -module, waarbij de id's zich in de array bevinden [!UICONTROL Inline Object Array].</p> <p>We raden u aan ALT-tekst toe te voegen aan afbeeldingen in uw [!DNL Google] document. </p> <p>Een ALT-tekst toevoegen aan de [!DNL Google Docs] afbeelding:</p> 
    <ol> 
     <li value="1">Klik met de rechtermuisknop op de afbeelding.</li> 
     <li value="2">Selecteer [!UICONTROL ALT text] optie.</li> 
     <li value="3">Voer de [!UICONTROL ALT text] in de [!UICONTROL Title] veld en klik op [!UICONTROL OK].</li> 
    </ol> <p>Nadat de ALT-tekst aan de afbeelding is toegevoegd, wordt de ALT-tekst tussen haakjes weergegeven in de veldnaam.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title] </td> 
   <td> <p>Voer de naam voor het nieuwe document in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Selecteer het type station waarop de sjabloon zich bevindt. Deze optie is beschikbaar als u [!UICONTROL By Dropdown] in het vorige veld.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selecteer de map waar u het document wilt maken.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Selecteer de map waar u het document wilt maken.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Gedeeld station]</strong> (beschikbaar voor [!DNL G Suite] alleen gebruikers)</p> <p>Selecteer of u wilt [!UICONTROL Use Domain Admin Access]. Selecteren [!UICONTROL Yes] geeft het verzoek uit als domeinbeheerder, en alle gedeelde aandrijving waarin de aanvrager een beheerder is teruggekeerd.</p> <p>Selecteer het gedeelde station waar u het document wilt maken.</p> <p>Opmerking: Als u de optie [!DNL Google Docs] in dit veld en u bent geen [!DNL G Suite] gebruiker, de fout <code>[400] Invalid Value</code> wordt geretourneerd.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Insert a Paragraph to a Document]

Deze actiemodule voegt een nieuwe alinea toe aan of voegt een nieuwe alinea in een bestaand document in.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Select a Document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Selecteer deze optie om het document toe te wijzen.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Selecteer deze optie als u het document in de vervolgkeuzelijst wilt kiezen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Selecteer het type station waaraan het document moet worden toegevoegd. Deze optie is beschikbaar als u [!UICONTROL By Dropdown] in het vorige veld.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selecteer de map waarin het document zich bevindt waaraan u een alinea wilt toevoegen, en selecteer vervolgens het document.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Selecteer de map waarin het document zich bevindt waaraan u een alinea wilt toevoegen, en selecteer vervolgens het document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Gedeeld station]</strong> (beschikbaar voor [!DNL G Suite] alleen gebruikers)</p> <p>Selecteer of u wilt [!UICONTROL Use Domain Admin Access]. Selecteren [!UICONTROL Yes] geeft het verzoek uit als domeinbeheerder, en alle gedeelde aandrijving waarin de aanvrager een beheerder is teruggekeerd.</p> <p>Selecteer het gedeelde station waar het document zich bevindt waaraan u een alinea wilt toevoegen en selecteer vervolgens het document.</p> <p>Opmerking: Als u de optie [!DNL Google Docs] in dit veld en u bent geen [!DNL G Suite] gebruiker, de fout <code>[400] Invalid Value</code> wordt geretourneerd.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Insert a Paragraph]</p> </td> 
   <td> <p>Selecteer hoe u de nieuwe tekst in het document wilt invoegen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL By specification of location]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL By index]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>Voer het indexnummer in waar u de tekst wilt invoegen. U kunt de [!UICONTROL Get a Document] -module indexnummer ophalen.</p> <p>Als u alle tekens (inclusief verborgen) in het document wilt weergeven, kunt u de opdracht [!UICONTROL Show] invoegtoepassing. U kunt de invoegtoepassing onder [!UICONTROL Add-ons] &gt; [!UICONTROL Get add-ons]. Zoeken naar [!UICONTROL Show] en installeer de [!UICONTROL Show] invoegtoepassing.</p> </li> 
         <li> <p><strong>[!UICONTROL Inserted text]</strong> </p> <p>Voer de tekst in die u in het document wilt invoegen.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL By segment ID]</strong> </p> <p>Selecteer de kop- en voettekst waarop u de tekstinhoud wilt invoegen en voer de tekst in die u aan de corresponderende velden wilt invoegen.</p> <p>Als de kop- of voettekst al tekst bevat, wordt de nieuwe tekst vóór de bestaande tekst toegevoegd.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL By appending to the body of the document]</strong> </p> <p>Voegt ingevoerde tekst toe aan het einde van de inhoud van het document.</p> <p>De stijl van de nieuwe alinea wordt gekopieerd uit de alinea bij de huidige invoegindex, inclusief lijsten en opsommingstekens.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL By appending to the end of segment (Header and Footer)]</strong> </p> <p>Selecteer de kop- en voettekst waarop u de tekstinhoud wilt invoegen en voer de tekst in die u aan de corresponderende velden wilt invoegen.</p> <p>Als de kop- of voettekst al tekst bevat, wordt de nieuwe tekst na de bestaande tekst toegevoegd.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Appended Text]</td> 
   <td>Typ of wijs de tekst toe die u aan het document wilt toevoegen</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Insert an Image to a Document]

Deze actiemodule voegt een afbeelding van de URL in het document in.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Select a Document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Selecteer deze optie om de documentsjabloon toe te wijzen.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Selecteer deze optie als u het document in de vervolgkeuzelijst wilt kiezen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Selecteer het type station waaraan het document moet worden toegevoegd. Deze optie is beschikbaar als u [!UICONTROL By Dropdown] in het vorige veld.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selecteer de map waarin het document zich bevindt waaraan u een afbeelding wilt toevoegen en selecteer vervolgens het document.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Selecteer de map waarin het document zich bevindt waaraan u een afbeelding wilt toevoegen en selecteer vervolgens het document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Gedeeld station]</strong> (beschikbaar voor [!DNL G Suite] alleen gebruikers)</p> <p>Selecteer of u wilt [!UICONTROL Use Domain Admin Access]. Selecteren [!UICONTROL Yes] geeft het verzoek uit als domeinbeheerder, en alle gedeelde aandrijving waarin de aanvrager een beheerder is teruggekeerd.</p> <p>Selecteer het gedeelde station waar het document zich bevindt waaraan u een afbeelding wilt toevoegen en selecteer vervolgens het document.</p> <p>Opmerking: Als u de optie [!DNL Google Docs] in dit veld en u bent geen [!DNL G Suite] gebruiker, de fout <code>[400] Invalid Value</code> wordt geretourneerd.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Insert an Image]</p> </td> 
   <td> <p>Selecteer hoe u de nieuwe afbeelding in het document wilt invoegen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL By specification of location]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL By index]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>Voer het indexnummer in waar u de afbeelding wilt invoegen. U kunt de [!UICONTROL Get a Document] module ophalen [!UICONTROL Index number].</p> <p>Als u alle tekens (inclusief verborgen) in het document wilt weergeven, kunt u de opdracht [!UICONTROL Show] invoegtoepassing. U kunt de invoegtoepassing onder [!UICONTROL Add-ons] &gt; [!UICONTROL Get add-ons]. Zoeken naar [!UICONTROL Show] en installeer de [!UICONTROL Show] invoegtoepassing.</p> </li> 
         <li> <p><strong>[!UICONTROL Image URL]</strong> </p> <p>Voer de URL in van de afbeelding die u in het document wilt invoegen.</p> <p>De maximale afbeeldingsgrootte is 50 MB. Mag niet groter zijn dan 25 megapixels. Alleen de indeling PNG, JPEG of GIF wordt ondersteund.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL By segment ID]</strong> </p> <p>Selecteer de kop- en voettekst waarop u de afbeelding wilt invoegen en typ de afbeeldings-URL naar de desbetreffende velden.</p> <p>De maximale afbeeldingsgrootte is 50 MB. De afbeelding mag niet groter zijn dan 25 megapixels. Alleen de indeling PNG, JPEG of GIF wordt ondersteund.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL By appending to the body of the document]</strong> </p> <p>Hiermee voegt u een specifieke afbeelding toe aan het einde van de hoofdinhoud van het document.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL By appending to the end of segment (Header and Footer)]</strong> </p> <p>Selecteer de kop- en voettekst waarop u een afbeelding wilt invoegen en voer de afbeeldings-URL in die u wilt invoegen in de desbetreffende velden.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Height Magnitude in Points/Width Magnitude in Points]</p> </td> 
   <td> <p>Hiermee bepaalt u de grootte van de ingevoegde afbeelding. De hoogte-breedteverhouding blijft behouden.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Replace an Image with a New Image]

Deze actiemodule vervangt een bestaande afbeelding. De hoogte-breedteverhouding van de oorspronkelijke afbeelding blijft behouden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Select a Document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Selecteer deze optie om de documentsjabloon toe te wijzen.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Selecteer deze optie als u het document in de vervolgkeuzelijst wilt kiezen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Selecteer het type station waar het document staat dat u wilt vervangen. Deze optie is beschikbaar als u [!UICONTROL By Dropdown] in het vorige veld.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selecteer de map waarin het document staat dat u een afbeelding wilt vervangen en selecteer het document.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Selecteer de map waarin het document staat dat u een afbeelding wilt vervangen en selecteer het document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Gedeeld station]</strong> (beschikbaar voor [!DNL G Suite] alleen gebruikers)</p> <p>Selecteer of u wilt [!UICONTROL Use Domain Admin Access]. Selecteren [!UICONTROL Yes] geeft het verzoek uit als domeinbeheerder, en alle gedeelde aandrijving waarin de aanvrager een beheerder is teruggekeerd.</p> <p>Selecteer het gedeelde station waar het document zich bevindt dat u wilt vervangen en selecteer vervolgens het document.</p> <p>Opmerking: Als u de optie [!DNL Google Docs] in dit veld en u bent geen [!DNL G Suite] gebruiker, de fout <code>[400] Invalid Value</code> wordt geretourneerd.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Image URL]</p> </td> 
   <td> <p>Geef de URL op of wijs de URL toe van de nieuwe afbeelding die de bestaande afbeelding vervangt.</p> <p>Afbeeldingen worden weergegeven in de volgorde waarin ze in het document worden weergegeven. Bijvoorbeeld: <code>Body: Image No. 1</code> is de eerste afbeelding in het document.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Replace Text in a Document]

Deze actiemodule vervangt tekst in een document.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Select a Document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Selecteer deze optie om de documentsjabloon toe te wijzen.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Selecteer deze optie als u het document in de vervolgkeuzelijst wilt kiezen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Selecteer het type station waaraan het document moet worden toegevoegd. Deze optie is beschikbaar als u [!UICONTROL By Dropdown] in het vorige veld.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selecteer de map waarin het document zich bevindt waaraan u tekst wilt toevoegen en selecteer het document.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Selecteer de map waarin het document zich bevindt waaraan u tekst wilt toevoegen en selecteer het document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Gedeeld station]</strong> (beschikbaar voor [!DNL G Suite] alleen gebruikers)</p> <p>Selecteer of u wilt [!UICONTROL Use Domain Admin Access]. Selecteren [!UICONTROL Yes] geeft het verzoek uit als domeinbeheerder, en alle gedeelde aandrijving waarin de aanvrager een beheerder is teruggekeerd.</p> <p>Selecteer het gedeelde station waar het document zich bevindt waaraan u tekst wilt toevoegen en selecteer vervolgens het document.</p> <p>Opmerking: Als u de optie [!DNL Google Docs] in dit veld en u bent geen [!DNL G Suite] gebruiker, de fout <code>[400] Invalid Value</code> wordt geretourneerd.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Replace a Text]</p> </td> 
   <td> <p>Voeg elke tekst toe die u wilt vervangen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Old text to be replaced]</strong> </p> <p>Voer de tekst in die u wilt vervangen.</p> </li> 
     <li> <p><strong>[!UICONTROL New text to be inserted]</strong> </p> <p>Voer de nieuwe tekst in.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download a Document]

Deze actiemodule converteert en downloadt het geselecteerde document.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Selecteer het type station waarop het document dat u wilt downloaden zich bevindt.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selecteer de map waarin het document dat u wilt downloaden zich bevindt en selecteer het document.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Selecteer de map waarin het document dat u wilt downloaden zich bevindt en selecteer het document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Gedeeld station]</strong> (beschikbaar voor [!DNL G Suite] alleen gebruikers)</p> <p>Selecteer of u wilt [!UICONTROL Use Domain Admin Access]. Selecteren [!UICONTROL Yes] geeft het verzoek uit als domeinbeheerder, en alle gedeelde aandrijving waarin de aanvrager een beheerder is teruggekeerd.</p> <p>Selecteer het gedeelde station waar het document dat u wilt downloaden zich bevindt en selecteer vervolgens het document.</p> <p>Opmerking: Als u de optie [!DNL Google Docs] in dit veld en u bent geen [!DNL G Suite] gebruiker, de fout <code>[400] Invalid Value</code> wordt geretourneerd.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type] </p> </td> 
   <td> <p>Selecteer de doelbestandsindeling van het gedownloade document.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a Document]

Met deze actiemodule verwijdert u een document.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Selecteer het type station waarop het document dat u wilt verwijderen zich bevindt.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selecteer de map waarin het document dat u wilt verwijderen zich bevindt en selecteer het document.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Selecteer de map waarin het document dat u wilt verwijderen zich bevindt en selecteer het document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Gedeeld station]</strong> (beschikbaar voor [!DNL G Suite] alleen gebruikers)</p> <p>Selecteer of u wilt [!UICONTROL Use Domain Admin Access]. Selecteren [!UICONTROL Yes] geeft het verzoek uit als domeinbeheerder, en alle gedeelde aandrijving waarin de aanvrager een beheerder is teruggekeerd.</p> <p>Selecteer het gedeelde station waar het document dat u wilt verwijderen zich bevindt en selecteer vervolgens het document.</p> <p>Opmerking: Als u de optie [!DNL Google Docs] in dit veld en u bent geen [!DNL G Suite] gebruiker, de fout <code>[400] Invalid Value</code> wordt geretourneerd.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Shared Drive]</td> 
   <td> <p>Selecteer het station dat het document bevat dat u wilt downloaden en selecteer vervolgens een document. Deze optie is beschikbaar als u [!DNL Google Docs] in de [!UICONTROL Choose a Drive] veld.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Document ID]</td> 
   <td> <p> Selecteer of wijs het document toe waarin u een of meer afbeeldingen wilt vervangen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Overige

* [[!UICONTROL Make an API Call]](#make-an-api-call)
* [[!UICONTROL Make All Links in a Document Clickable]](#make-all-links-in-a-document-clickable)

#### [!UICONTROL Make an API Call]

Met deze actiemodule kunt u een aangepaste API-aanroep uitvoeren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Een pad invoeren ten opzichte van <code>https://docs.googleapis.com/</code>. Voorbeeld: <code>/v1/documents/{presentationID}</code>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van de aanvraag toe in de vorm van een standaard JSON-object. Bijvoorbeeld: <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] Hiermee voegt u de machtigingsheaders voor u toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Voer de queryreeks voor de aanvraag in.</p> </td> 
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

**Voorbeeld:** Met de volgende API-aanroep worden de gegevens voor het opgegeven document opgehaald in uw Google Docs:

**URL:**

/v1/documents/1ujkf-GDgB0TQSYPrxbCSK4Uso54tHVMqHZEVZZxB6aY

**Methode:**

[!UICONTROL GET]

![](assets/api-call-example.png)

Details van het opgehaalde document vindt u in de Output van de module onder [!UICONTROL Bundle] > [!UICONTROL Body].

![](assets/api-output.png)

#### [!UICONTROL Make All Links in a Document Clickable]

Met deze actiemodule vindt u alle koppelingen in het document en kunt u erop klikken.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Make All Links in a Document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Selecteer deze optie om de documentsjabloon toe te wijzen.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Selecteer deze optie als u het document in de vervolgkeuzelijst wilt kiezen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Selecteer het type station waarin het document staat waarin u koppelingen klikbaar wilt maken. Deze optie is beschikbaar als u [!UICONTROL By Dropdown] in het vorige veld.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Selecteer de map waarin het document staat waarin u wilt dat koppelingen klikbaar zijn. Selecteer vervolgens het document.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Selecteer de map waarin het document staat waarin u wilt dat koppelingen klikbaar zijn. Selecteer vervolgens het document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Gedeeld station]</strong> (beschikbaar voor [!DNL G Suite] alleen gebruikers)</p> <p>Selecteer of u wilt [!UICONTROL Use Domain Admin Access]. Selecteren [!UICONTROL Yes] geeft het verzoek uit als domeinbeheerder, en alle gedeelde aandrijving waarin de aanvrager een beheerder is teruggekeerd.</p> <p>Selecteer het gedeelde station waarin het document zich bevindt waarop u koppelingen klikbaar wilt maken en selecteer vervolgens het document.</p> <p>Opmerking: Als u de optie [!DNL Google Docs] in dit veld en u bent geen [!DNL G Suite] gebruiker, de fout <code>[400] Invalid Value</code> wordt geretourneerd.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Shared Drive]</td> 
   <td> <p>Selecteer het station met het document waarin u de koppelingen wilt bijwerken en selecteer vervolgens een document. Deze optie is beschikbaar als u [!DNL Google Docs] in de [!UICONTROL Choose a Drive field].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Document ID]</td> 
   <td> <p> Selecteer of wijs het document toe u de verbindingen binnen wilt bijwerken.</p> </td> 
  </tr> 
 </tbody> 
</table>
