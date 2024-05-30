---
title: Overzicht van formuliervelden
description: In de Planning van Adobe Workfront, kunt u formulengebieden tot stand brengen die functies en bestaande gebieden gebruiken om een nieuwe douanewaarde te berekenen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: 1369269bcb64bd32f26603608782dc996b079cb9
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Overzicht van formuliervelden

<!--update the metadata with real information when making this available in TOC and in the left nav - below-->

<!---
title: Formula fields overview
description: In Adobe Maestro, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

{{planning-important-intro}}

U kunt douanegebieden in de Planning van Adobe Workfront tot stand brengen door naar bestaande gebieden te verwijzen en hen te verbinden op een Formule-type gebied.

Formulervelden genereren een nieuwe waarde met behulp van bestaande waarden uit andere velden in een recordtype en een functie die aangeeft hoe de bestaande waarden moeten worden berekend.

Zie de sectie Formule in het artikel voor meer informatie [Velden maken](../fields/create-fields.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-overeenkomst</p></td>
   <td>
<p>Uw organisatie moet zijn ingeschreven in de vroege toegangsfase voor Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-plan</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td>
   <td>
   <p>Alle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsbesturingselementen voor het inplanten van werktuigen</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Machtigingen beheren in een werkruimte</a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->


## Overwegingen bij formuleringsvelden

* Formulervelden verwijzen naar velden die tot hetzelfde recordtype behoren. U kunt niet naar velden van andere recordtypen verwijzen wanneer u een formuleringsveld maakt. <!--is this still accurate??-->
* U kunt het veldtype van een veld Formule niet wijzigen nadat u het hebt opgeslagen.
* U kunt de berekening van een formuleringsgebied bijwerken nadat u het bewaart, en de resultaten van de berekeningsupdate automatisch voor alle verslagen van het zelfde type.
* U moet de gebieden toevoegen u in formules van verwijzingen voorziet aangezien zij in de interface van de Planning van Workfront tonen.

## Ondersteunde formules

In velden van de Adobe Workfront-planningsformule worden alle expressies van de berekende Workfront-velden ondersteund. Zie voor meer informatie [Overzicht van berekende gegevensexpressies](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Daarnaast ondersteunen we de volgende expressies voor velden van de Workfront-planningsformule:

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
   <td><strong>ARRAYJOIN</strong> </td> 
   <td> <p>Retourneert een samengevoegde tekenreeks met scheidingsteken.</p> <p>De expressie wordt als volgt opgemaakt:

<code>ARRAYJOIN(delimiter,array)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>Retourneert een array met unieke waarden.</p> <p>De expressie wordt als volgt opgemaakt:

<code>ARRAYUNIQUE(array)</code>
</p>
   </td></tr>
     <tr> 
   <td><strong>ID</strong> </td> 
   <td> <p>Retourneert de id van een record. Elke record heeft een unieke id.</p> <p>De expressie wordt als volgt opgemaakt:

<code>{ID}</code>
</p>
   </td></tr>

<tr> 
   <td><strong>SETTIMEZON</strong> </td> 
   <td> <p>Stelt de tijdzone van een datum en tijd in op een specifieke tijdzone.</p> <p>De expressie wordt als volgt opgemaakt:

<code>SETTIMEZONE(date,&#39;America/Los_Angeles&#39;)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>WEEKOFYYEAR</strong> </td> 
   <td> <p>Retourneert het weekgetal in een jaar. U kunt ook aangeven op welke dag de week begint (gebruik 1 voor zondag of 2 voor maandag). Indien weggelaten, beginnen weken standaard op zondag.</p> <p>De expressie wordt als volgt opgemaakt:

<code>WEEKOFYEAR(datum,2)</code>
of
<code>WEEKOFYEAR(datum)</code>
</p>
   </td></tr>

</table>
