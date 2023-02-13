---
navigation-topic: search
title: Zoeken [!DNL Adobe Workfront]
description: U kunt items gemakkelijk vinden in [!DNL Adobe Workfront] door naar ze te zoeken wanneer je de exacte locatie niet kunt onthouden.
feature: Get Started with Workfront
author: Lisa
exl-id: 7c856349-c79f-40d8-9c96-b32bfb6d5417
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '1574'
ht-degree: 0%

---

# Zoeken [!DNL Adobe Workfront]

U kunt items gemakkelijk vinden in [!DNL Adobe Workfront] door naar ze te zoeken wanneer je de exacte locatie niet kunt onthouden.

U kunt de [!UICONTROL Search] in de rechterbovenhoek van een pagina binnen [!DNL Workfront].

![](assets/search-globalnavigationbar-350x62.png)

U moet over machtigingen beschikken om een object weer te geven voordat u het in een zoekopdracht kunt vinden. Om deze reden, variëren de onderzoeksresultaten van gebruiker aan gebruiker.

## Toegangsvereisten

+++ Vouw deze sectie uit om de toegang te bekijken die nodig is om de stappen in dit artikel uit te voeren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>Aanvraag of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>[!UICONTROL View] toegang tot het type object </p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>U moet over machtigingen beschikken om een object weer te geven voordat u het in een zoekopdracht kunt vinden.</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

+++

## Zoeken begrijpen

* [[!UICONTROL Objects available for search]](#objects-available-for-search)
* [[!UICONTROL Fields available for search]](#fields-available-for-search)

### Objecten beschikbaar voor zoeken

U kunt in Workfront naar de volgende objecten zoeken:

* Projecten
* Taken
* Problemen
* Rapporten
* Gebruikers
* Sjablonen
* Documenten
* Portfolio
* Programma&#39;s
* Dashboards
* Bedrijven
* Notities

### Beschikbare velden voor zoeken

De velden die u kunt zoeken, zijn gebaseerd op het type zoekopdracht: Basis of [!UICONTROL Advanced Search].

* **Standaardzoekopdracht**: Bij het zoeken naar objecten in een standaardzoekopdracht [!DNL Workfront] zoekt naar tekst die uw trefwoorden in de volgende velden kan bevatten:

   * Objectnamen
   * Beschrijvingen
   * Aangepaste gegevensvelden
   * Updates
   * Documentnamen (in zoekopdrachten in specifieke documenten en in een basiszoekopdracht)

   Voor meer informatie over elementair zoeken in [!DNL Workfront], zie [Standaardzoekopdracht](#basic-search) in dit artikel.

* **[!UICONTROL Advanced Search]**: In een [!UICONTROL Advanced Search], kunt u filters instellen om te zoeken naar velden die niet beschikbaar zijn in de standaardzoekopdracht. Daarom [!UICONTROL Advanced Search] kunt u elk veld in het object doorzoeken.

   Meer informatie over [!UICONTROL Advanced Search], zie [Geavanceerd zoeken](#advanced-search) in dit artikel.

>[!NOTE]
>
>Om een [!UICONTROL Advanced Search], moet u de optie [!UICONTROL Advanced Search] als u begint met zoeken. U kunt een basiszoekopdracht niet verfijnen tot een [!UICONTROL Advanced Search].

## Beperkingen van [!DNL Workfront] zoekopdrachten

Houd rekening met de volgende beperkingen bij het gebruik [!UICONTROL Search] in [!DNL Workfront]:

* Zoekopdrachten zijn niet hoofdlettergevoelig
* [!DNL Workfront] verbetert of begrijpt typos niet
* Zoeken in [!DNL Workfront] ondersteunt geen jokertekens
* Zoeken in [!DNL Workfront] ondersteunt gedeeltelijke woordzoekopdrachten, maar ondersteunt geen zoekopdrachten in subtekenreeksen.\
   Het zoektrefwoord &#39;stand&#39; geeft bijvoorbeeld resultaten met het woord &#39;standard&#39;, maar geeft geen resultaten met het woord &#39;understanding&#39;.

## Meerdere woorden zoeken

Wanneer u meerdere woorden opneemt in een zoekopdracht en u alleen objecten wilt zoeken die overeenkomen met alle woorden in het vak Zoeken, kunt u de woorden in willekeurige volgorde typen.

Als u bijvoorbeeld zoekt naar &quot;Marketingdemo&quot; (zonder aanhalingstekens), worden objecten met de volgende namen gevonden:

* Marketingdemo
* Demo Marketing
* Demo marktanalyse januari

Het vindt ook voorwerpen die &quot;Marketing&quot;in de naam en &quot;Demo&quot;in de beschrijving zouden kunnen hebben.

U kunt echter het volgende doen in het dialoogvenster [!UICONTROL Search] om de weergegeven zoekresultaten aan te passen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Aanhalingstekens opnemen</td> 
   <td> <p>Door woorden in de juiste volgorde binnen dubbele aanhalingstekens in te voeren, kunt u alleen objecten zoeken die exact overeenkomen.<br>Als u bijvoorbeeld zoekt naar "Marketing Demo" (met aanhalingstekens), worden objecten met de volgende namen gevonden:</p> 
    <ul> 
     <li> Marketingdemo</li> 
     <li> Januari Marketing Demo</li> 
     <li>Demoplan voor marketing</li> 
    </ul> <p>In deze zoekopdracht wordt echter geen object gevonden met de naam "Demo Marketing".</p> </td> 
  </tr> 
  <tr> 
   <td>Inclusief OF</td> 
   <td> <p>Door woorden te verbinden met "OR" (zonder aanhalingstekens) kunt u alleen objecten zoeken die overeenkomen met ten minste een van de woorden in het dialoogvenster [!UICONTROL Search] doos. Deze woorden kunnen in willekeurige volgorde worden ingevoerd.<br>Als u bijvoorbeeld zoekt naar "Marketing OR Demo" (zonder aanhalingstekens), worden objecten met de volgende namen gevonden:</p> 
    <ul> 
     <li> Marktanalysedemo</li> 
     <li>Demo marktanalyse januari</li> 
     <li>Demo</li> 
     <li>Marktanalyse</li> 
    </ul> <p>Opmerking: "OR" moet zich in alle uiteinden bevinden. Anders wordt het geïnterpreteerd als een ander woord in de woordgroep waarnaar u zoekt.</p> </td> 
  </tr> 
  <tr> 
   <td>Inclusief EN</td> 
   <td> <p>Door woorden met "AND" (zonder aanhalingstekens) te verbinden, kunt u alleen objecten zoeken die overeenkomen met alle woorden in het dialoogvenster [!UICONTROL Search] doos. Deze woorden kunnen in willekeurige volgorde worden ingevoerd.<br>Als u bijvoorbeeld zoekt naar "Marketing AND Demo" (zonder aanhalingstekens), worden objecten met de volgende namen gevonden:</p> 
    <ul> 
     <li>Marketingdemo</li> 
     <li>Demo Marketing</li> 
     <li>Demo marktanalyse januari</li> 
    </ul> <p>Opmerking: "AND" moet in alle hoofdletters staan. Anders wordt het geïnterpreteerd als een ander woord in de woordgroep waarnaar u zoekt. Op dezelfde manier zoekt "&amp;" (zonder aanhalingstekens) alleen naar objecten die het en-teken bevatten.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Zoeken in gebruiken [!DNL Workfront]

[!DNL Workfront] bevat twee soorten zoekopdrachten: Standaard en geavanceerd. Gebruik de standaardzoekopdracht als u trefwoorden wilt zoeken in veelvoorkomende objectvelden, zoals naam of beschrijving. Gebruiken [!UICONTROL Advanced Search] als u filters wilt gebruiken om te zoeken in andere objectvelden.

* [Standaardzoekopdracht](#basic-search)
* [Geavanceerd zoeken](#advanced-search)

### Standaardzoekopdracht

Met een standaardzoekopdracht kunt u trefwoorden zoeken voor alle objecten in het systeem of voor slechts één object tegelijk (zoals projecten). [!DNL Workfront] zoekt u deze trefwoorden vervolgens in een paar specifieke velden. Vervolgens kunt u de zoekresultaten verfijnen op basis van andere objectspecifieke velden die zijn geselecteerd door [!DNL Workfront].

Voor een lijst met de specifieke velden die worden doorzocht in de standaardzoekopdracht raadpleegt u [Beschikbare velden voor zoeken](#fields-available-for-search) in dit artikel.

>[!NOTE]
>
>Om een [!UICONTROL Advanced Search], moet u de optie [!UICONTROL Advanced Search] als u begint met zoeken. U kunt een basiszoekopdracht niet verfijnen tot een [!UICONTROL Advanced Search].

* [Een basiszoekopdracht uitvoeren](#perform-a-basic-search)
* [Een basiszoekopdracht verfijnen](#refine-a-basic-search)

#### Een basiszoekopdracht uitvoeren

U kunt een basiszoekopdracht op een van de volgende manieren uitvoeren:

* Alle objecten in het systeem (algemene zoekopdracht).
* Op slechts één object tegelijk (objectspecifieke zoekopdracht).

Een basiszoekopdracht uitvoeren:

1. Klik op het vergrootglas ![](assets/search-icon.png) in de rechterbovenhoek van de pagina. U kunt ook typen **[!UICONTROL ALT + /]** of **[!UICONTROL Option + /]** om de [!UICONTROL Search] -menu.

1. (Optioneel) Als u naar een specifiek object wilt zoeken, klikt u op de knop **[!UICONTROL All]** en selecteert u het object dat u wilt zoeken.

   ![](assets/search-objecttype.png)

1. In de **[!UICONTROL Search]** typt u de gegevens waarnaar u zoekt.\
   Voor informatie over welke velden worden doorzocht [!DNL Workfront], zie [Zoeken begrijpen](#understand-search).\
   ![](assets/qs-search-drop-down-highlighted-350x234.png)\
   Terwijl u begint te typen in de zoekbalk, [!DNL Workfront] doet aanbevelingen op basis van uw weergavegeschiedenis en markeert het gewenste trefwoord in blauw.

1. Als het gewenste item wordt weergegeven in het dialoogvenster [!UICONTROL typeahead] klikt u erop.

   of

   Druk **[!UICONTROL Enter]** om een uitgebreide zoekopdracht uit te voeren. Deze zoekopdracht zoekt naar de gehele database in plaats van naar de laatst bekeken items.

   De [!UICONTROL Search Results] De pagina&#39;s worden vanaf links geopend en bedekken het grootste deel van de vorige pagina.

   Als u een algemene zoekopdracht hebt uitgevoerd, [!DNL Workfront] retourneert resultaten voor elk object dat overeenkomt met de zoekterm in een van de doorzochte velden, zoals beschreven in [Zoeken begrijpen](#understand-search). De objecten die overeenkomen met uw zoekopdracht worden weergegeven in een lijst.

   >[!NOTE]
   >
   >Soms worden variaties van een woord weergegeven in de lijst met gevonden items.\
   >Als u bijvoorbeeld zoekt naar &#39;marketing&#39;, worden objecten weergegeven die &#39;marketing&#39; of &#39;markt&#39; in de naam bevatten.

1. (Optioneel) Als uw zoekopdracht te veel resultaten heeft opgeleverd, kunt u de zoekopdracht verfijnen zoals beschreven in [Een basiszoekopdracht verfijnen](#refine-a-basic-search).
1. (Optioneel) Klik op **[!UICONTROL Close]** in de rechterbovenhoek.

>[!NOTE]
>
>De [!UICONTROL Search Results] De pagina blijft alleen geopend wanneer deze de focus heeft. Wanneer u buiten de pagina klikt of een andere pagina opent, wordt het dialoogvenster [!UICONTROL Search Results] pagina.

#### Een basiszoekopdracht verfijnen

Na het uitvoeren van een basisonderzoek-zoals die in wordt beschreven [[!UICONTROL Perform a basic search]](#perform-a-basic-search)—u kunt de zoekopdracht verfijnen.

Gebruik de werkbalk links van de zoekresultaten om de informatie die u zoekt te beperken.

Een zoekopdracht verfijnen:

1. (Voorwaardelijk) Als u een algemene zoekopdracht hebt uitgevoerd, selecteert u het object dat u zoekt in de lijst met objecten linksboven in de resultaten.
1. Zoek de velden die beschikbaar zijn voor de objecten die worden weergegeven in de zoekopdracht op de werkbalk links van de resultaten.\
   De waarden van elke veldweergave, gesorteerd op aantal, tot 10 waarden voor elk veld.
1. Klik in een van de velden die beschikbaar zijn om de lijst met resultaten te verkorten.\
   De selecties die u maakt, worden in blauw gemarkeerd en de veldwaarden die u niet selecteert, worden verborgen.\
   Nadat u elke nieuwe waarde hebt geselecteerd, worden de resultaten aan de rechterkant dynamisch bijgewerkt.\
   ![](assets/qs-refine-search-350x175.png)

1. (Optioneel) Klik op de geselecteerde waarden om deze te deselecteren en alle waarden voor elk veld opnieuw weer te geven.

### [!UICONTROL Advanced Search]

[!UICONTROL Advanced Search] kunt u zoeken met velden en filters die niet beschikbaar zijn voor de standaardzoekopdracht. U kunt bijvoorbeeld zoeken naar projecten met een specifieke prioriteit of de naam van de eigenaar van het document.

>[!NOTE]
>
>Om een [!UICONTROL Advanced Search], moet u de optie [!UICONTROL Advanced Search] als u begint met zoeken. U kunt een basiszoekopdracht niet verfijnen tot een [!UICONTROL Advanced Search].

* [Gebruiken [!UICONTROL Advanced Search]](#use-advanced-search)

#### Gebruiken [!UICONTROL Advanced Search]

U kunt [!UICONTROL Advanced Search] om uw zoekopdracht te filteren op basis van specifieke criteria.\
Dit type zoekopdracht is handig wanneer u een trefwoord dat aan een object is gekoppeld, niet kunt onthouden, maar wel bepaalde specifieke gegevens over dat object kent (bijvoorbeeld: Projectprioriteit, naam eigenaar van document, enz.).

Een geavanceerde zoekopdracht uitvoeren:

1. In de rechterbovenhoek van een pagina in [!DNL Workfront]klikt u op de knop **[!UICONTROL Search]** pictogram ![](assets/search-icon.png). De [!DNL Search] weergegeven.

1. Onder aan het dialoogvenster [!UICONTROL Search] menu, klikt u op **[!UICONTROL Advanced Search]**.\
   ![](assets/qs-advanced-search-350x224.png)\
   De [!UICONTROL Advanced Search] De pagina&#39;s worden vanaf rechts geopend en bedekken het grootste deel van de vorige pagina.

1. Selecteer het type object waarnaar u zoekt.\
   **[!UICONTROL Projects]** is standaard geselecteerd.

   ![](assets/advanced-search-objects-qs-remove-after-prod-release.png)

1. (Optioneel) Typ een trefwoord in het veld boven aan de lijst.
1. (Optioneel) Klik op **[!UICONTROL Filter your results]** Als u de zoekresultaten wilt filteren op basis van specifieke veldtypen, selecteert u een veld in de lijst. Selecteer zo nodig ook een waarde voor het veld.\
   of\
   Voeg een nieuw filter toe.

1. Klik op **[!UICONTROL Search]**.\
   Een lijst met items die overeenkomen met uw zoekopdracht wordt rechts van het dialoogvenster [!UICONTROL Advanced Search] werkbalk.

1. (Optioneel) Klik op **[!UICONTROL Close]** in de rechterbovenhoek.

>[!NOTE]
>
>De [!UICONTROL Search Results] De pagina blijft alleen geopend wanneer deze de focus heeft. Wanneer u buiten de pagina klikt of een andere pagina opent, wordt het dialoogvenster [!UICONTROL Search Results] pagina.
