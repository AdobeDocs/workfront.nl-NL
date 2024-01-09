---
title: Overzicht van formuliervelden
description: In Adobe Maestro, kunt u formuleringsgebieden tot stand brengen die functies en bestaande gebieden gebruiken om een nieuwe douanewaarde te berekenen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 4e3449e7c31d29e1a289a7866ba98f873e62922c
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---


# Overzicht van formuliervelden

<!--update the metadata with real information when making this available in TOC and in the left nav - below-->

<!--**********ADD TO miniTOC************>

<!---
title: Formula fields
description: In Adobe Maestro, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

>[!IMPORTANT]
>
>De informatie in dit artikel verwijst naar Adobe Maestro, een nieuw aanbod van Adobe Workfront.
>
>Adobe Maestro maakt momenteel deel uit van een bètaprogramma dat voor een beperkt aantal klanten toegankelijk is. U moet een Workfront-klant zijn om Maestro-mogelijkheden te kunnen gebruiken.
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro-overview.md).

U kunt aangepaste velden maken in Adobe Maestro door naar bestaande velden te verwijzen en deze met een formule te verbinden. U kunt dit doen door een aangepast Formule-type gebied tot stand te brengen.

Formulervelden genereren een nieuwe waarde met behulp van bestaande waarden uit andere velden in een recordtype en een functie die aangeeft hoe de bestaande waarden moeten worden berekend.

Zie voor meer informatie [Velden maken](../fields/create-fields.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-overeenkomst</p></td>
   <td>
<p>Uw organisatie moet zijn ingeschreven voor het afgesloten bètaprogramma van de Adobe Maestro. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
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
   <td role="rowheader">Toegangsniveau</td>
   <td> <p>Alle</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Lay-outsjabloon</td>
   <td> <p>Uw systeembeheerder moet het gebied Maestro in uw lay-outmalplaatje toevoegen. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->

## Overwegingen bij formuleringsvelden

* Formulervelden verwijzen naar velden die tot hetzelfde recordtype behoren. U kunt niet naar velden van andere recordtypen verwijzen wanneer u een formuleringsveld maakt. <!--is this still accurate??-->
* U kunt het veldtype van een veld Formule niet wijzigen nadat u het hebt opgeslagen.
* U kunt de berekening van een formuleringsgebied bijwerken nadat u het bewaart, en de resultaten van de berekeningsupdate automatisch voor alle verslagen van het zelfde type.
* U moet de velden toevoegen waarnaar u verwijst in formules zoals deze worden weergegeven in de Maestro-interface.
* Het gebruik van opzoekvelden van gekoppelde recordtypen in een formule is op een latere datum beschikbaar.

## Ondersteunde formules

In Maestro-formulevelden worden alle expressies van de berekende Workfront-velden ondersteund. Zie voor meer informatie [Overzicht van berekende gegevensexpressies](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Daarnaast ondersteunen we de volgende expressies voor Maestro-formuleringsvelden:


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
   <td> <p>Retourneert de id van een record.</p> <p>De expressie wordt als volgt opgemaakt:

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
   <td> <p>Retourneert het weekgetal in een jaar. U kunt ook aangeven op welke dag de week begint (gebruik 1 voor zondag of 2 voor maandag). Als u dit opgeeft, beginnen weken standaard op zondag.</p> <p>De expressie wordt als volgt opgemaakt:

<code>WEEKOFYEAR(datum,2)</code>
of
<code>WEEKOFYEAR(datum)</code>
</p>
   </td></tr>

</table>





