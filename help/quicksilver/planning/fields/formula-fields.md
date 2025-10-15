---
title: Overzicht van formuliervelden
description: In de Planning van Adobe Workfront, kunt u formulengebieden tot stand brengen die functies en bestaande gebieden gebruiken om een nieuwe douanewaarde te berekenen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: b102960e088f072f10baadcbeca4f7f579daa287
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# Overzicht van formuliervelden

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

U kunt douanegebieden in de Planning van Adobe Workfront tot stand brengen door naar bestaande gebieden te verwijzen en hen te verbinden op een Formule-type gebied.

Formulervelden genereren een nieuwe waarde met behulp van bestaande waarden uit andere velden in een recordtype en een functie die aangeeft hoe de bestaande waarden moeten worden berekend.

Voor informatie, zie de &quot;sectie van de Formule&quot;in artikel [ gebieden ](/help/quicksilver/planning/fields/create-fields.md) creëren.

## Toegangsvereisten

+++ Breid uit om de toegangsvereisten voor de functionaliteit in dit artikel te bekijken. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<ul> 
<li><p>Alle Workfront en alle planningspakketten</p></li>
of
<li><p>Alle workflows en planningspakketten</li></ul>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Machtigingen beheren in een werkruimte</p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr>  
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
 
</tbody> 
</table> -->

## Overwegingen bij formuleringsvelden

* Formulervelden verwijzen naar velden die tot hetzelfde recordtype behoren.
* U kunt alleen verwijzen naar velden van andere recordtypen wanneer u een ander recordtype koppelt aan het recordtype waarvoor u een formuleveld maakt.
* Verwijzen van verbonden verslagtypes of hun raadplegingsgebieden in een formule hangt van uw toestemmingen aan de verbonden verslagtypes af. Als u geen machtigingen hebt om het recordtype weer te geven, kunt u niet verwijzen naar de velden in een formule.
* U kunt het veldtype van een veld Formule niet wijzigen nadat u het hebt opgeslagen.
* U kunt de berekening van een formuleringsgebied bijwerken nadat u het bewaart, en de resultaten van de berekeningsupdate automatisch voor alle verslagen van het zelfde type.
* U moet de gebieden toevoegen u in formules van verwijzingen voorziet aangezien zij in de interface van de Planning van Workfront tonen.
* U kunt alleen verwijzen naar velden die worden weergegeven in de tabelweergave van een recordtype of op de pagina met recorddetails.
* U kunt de notatie voor de waarde van een formule-berekening definiëren door een van de volgende indelingsopties te kiezen:

   * Tekst
   * Getal
   * Percentage
   * Valuta
   * Tags
   * Datum

  Voor meer informatie, zie de &quot;sectie van de Formule&quot;in artikel [ gebieden ](/help/quicksilver/planning/fields/create-fields.md) creëren.
* U kunt in nieuwe formules verwijzen naar formuleringsvelden. Zodra de waarde wordt bijgewerkt in een veld waarnaar wordt verwezen in een formuleveld, worden alle volgende velden die verwijzen naar dat veld of naar formulevelden die dat veld bevatten, automatisch bijgewerkt.

<div class="preview">

* Wanneer u een formuleringsgebied of een gebied bijwerkt dat het kon beïnvloeden, brengt een alarm u op de hoogte van de invloed van uw verandering. De waarschuwing wordt in de volgende gevallen weergegeven:

   * Wanneer u een formuleringsgebied (exclusief naam en beschrijvingsveranderingen) bijwerkt wanneer dat gebied afhankelijke formule of raadplegingsgebieden heeft. In de waarschuwing worden die afhankelijke velden vermeld en wordt u gevraagd of u wilt doorgaan.

   * Wanneer u een veld verwijdert dat wordt gebruikt in een formule-expressie of als opzoekveld. De waarschuwing maakt een lijst van de afhankelijke formule en raadplegingsgebieden en vraagt u of u met de schrapping wilt verdergaan.

</div>



<div class="preview">

## Beperkingen van formuliervelden

* U kunt maximaal 20 formulervelden toevoegen voor één recordtype.

  Opzoekvelden van formule die zijn toegevoegd van gekoppelde recordtypen tellen niet mee voor deze limiet.

* De formule-expressie mag niet langer zijn dan 50.000 tekens.

* In de volgende gevallen kunnen formuliervelden worden weergegeven als `#ERROR!` :
   * Wanneer een veld in een formule wordt verwijderd.
   * Wanneer een veld dat in een samengevoegd opzoekveld wordt gebruikt, wordt weergegeven als `#ERROR!` .

     Als u bijvoorbeeld een opzoekveld weergeeft dat geaggregeerde opzoekformulevelden bevat en een van de formuliervelden waarnaar wordt verwezen, wordt weergegeven als `#ERROR!` .
   * Wanneer een formulewaarde niet in het geselecteerde formaat kan worden getoond.

     Als ik bijvoorbeeld Getal kies voor de indeling van een formuleveld en de velden in de formule tekstvelden zijn die alleen niet-numerieke tekstwaarden weergeven, wordt het resultaat van de formule weergegeven als `#ERROR!` omdat de tekst niet in een getal kan worden geparseerd.

</div>

## Ondersteunde formules

De de formules van de Planning van Adobe Workfront gebieden steunen de meeste uitdrukkingen van Workfront berekende gebieden.

>[!NOTE]
>
>De volgende Workfront-expressies worden niet ondersteund voor velden in de Workfront-planningsformule:
>
><!--* SORTASCARRAY-->
><!--* SORTDESCARRAY-->
>* ADDHOUR
>* SCHAKELEN
>* INDELING

<!--remove the ones commented out when we go live to Preview and Prod, if they truly are added to Planning-->

Voor een volledige lijst van de uitdrukkingen van Workfront, zie [ Overzicht van berekende gegevensuitdrukkingen ](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Daarnaast ondersteunen we de volgende expressies voor velden in de formule Workfront Planning. De volgende expressies worden niet ondersteund voor Workfront-expressies:

<!--take these three out when they also come to WF and Lisa has added them to the WF expression article linked above-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Uitdrukking</th> 
   <th>Uitleg en voorbeeld</th> 
  </tr> 
 </thead> 
 <tbody>

<tr> 
   <td><strong> ARRAYJOIN </strong> </td> 
   <td> <p>Retourneert een samengevoegde tekenreeks met scheidingsteken.</p> <p>De expressie wordt als volgt opgemaakt:

<code> ARRAYJOIN (delimiter, serie)</code>
</p>
   </td></tr>
    <tr> 
   <td><strong> ARRAYUNIQUE </strong> </td> 
   <td> <p>Retourneert een array met unieke waarden.</p> <p>De expressie wordt als volgt opgemaakt:

<code> ARRAYUNIQUE (serie)</code>
</p>
   </td></tr>
     <tr> 
   <td><strong> identiteitskaart </strong> </td> 
   <td> <p>Retourneert de id van een record. Elke record heeft een unieke id.</p> <p>De expressie wordt als volgt opgemaakt:

<code>{ID}</code>
</p>
   </td></tr>
  <tr> 
   <td><strong> JSONELEMENT </strong> </td> 
   <td> <p>Retourneert de gegevens van JSON door de opgegeven JSONPath. Als JSONPath niet in JSON bestaat, zal een leeg resultaat zijn teruggekeerd. </p> <p>De expressie wordt als volgt opgemaakt:
      <code>JSONELEMENT(JSONString, JSONPathString) </code>
   </p>
   </td></tr>
  <tr> 
   <td><strong> SETTIMEZONE </strong> </td> 
   <td> <p>Stelt de tijdzone van een datum en tijd in op een specifieke tijdzone.</p> <p>De expressie wordt als volgt opgemaakt:

<code> SETTIMEZONE(date,&#39;America/Los_Angeles&#39;)</code>
</p>
   </td></tr>

<tr> 
   <td><strong> WEEKOFYEAR </strong> </td> 
   <td> <p>Retourneert het weekgetal in een jaar. U kunt ook aangeven op welke dag de week begint (gebruik 1 voor zondag of 2 voor maandag). Indien weggelaten, beginnen weken standaard op zondag.</p> <p>De expressie wordt als volgt opgemaakt:

<code> WEEKOFYEAR (date,2)</code>
of
<code> WEEKOFYEAR (datum)</code>
</p>
   </td></tr>

</table>
