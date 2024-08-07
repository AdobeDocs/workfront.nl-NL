---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filter: meerdere filterregels maken die naar hetzelfde veld verwijzen ('AND'-instructies)"
description: In de standaardwijzeinterface, wanneer het proberen om veelvoudige filters tot stand te brengen die het zelfde gebied (gebruiken EN bepalend) van verwijzingen voorzien, wordt één van de filters geschrapt wanneer u sparen het rapport en de rapportaannemer weggaat.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# Filter: meerdere filterregels maken die naar hetzelfde veld verwijzen (&quot;AND&quot;-instructies)

In de standaardwijzeinterface, wanneer het proberen om veelvoudige filters tot stand te brengen die het zelfde gebied (gebruiken EN bepalend) van verwijzingen voorzien, wordt één van de filters geschrapt wanneer u sparen het rapport en de rapportaannemer weggaat.

**Voorbeeld:** u zou slechts taken kunnen willen bekijken die het woord &quot;groen&quot;bevatten maar niet het woord &quot;rood&quot;in de naam bevatten. Adobe Workfront staat u niet toe om de volgende filterregels te bewaren gebruikend de standaardwijzeinterface omdat het verwijst naar het zelfde gebied (de Naam van de Taak) maar verschillende bepalingen gebruikt en naar verschillende waarden verwijst:

* Taaknaam > Bevat > Groen
* Taaknaam > Bevat niet > Rood

U kunt dit filter echter maken in de tekstmodus.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Verzoek om een filter te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Meerdere filterregels maken die naar hetzelfde veld verwijzen

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Filter**, uitgezochte **Nieuwe Filter**.
1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. Beweeg over het gebied van de tekstwijze, en klik **Klik om tekst** uit te geven.
1. Voeg de volgende code toe in het gedeelte Filterregels instellen voor het rapportgebied:

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >Als u vergelijkbare filters wilt maken, moet u eerst de eerste instructie maken. Bijvoorbeeld:
   >
   >```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >Kopieer en plak de instructie zo vaak als nodig is. Vervolgens kunt u zoveel instructies toevoegen als u nodig hebt om naar hetzelfde veld te verwijzen (in ons geval &#39;name&#39;) en de volgende wijzigingen in de aanvullende instructies aanbrengen:
   >
   >1. Ga de twee gekopieerde lijnen met &quot;EN :1:&quot;, &quot;EN :2:&quot;, &quot;EN :3:&quot;, enz. voor elk nieuw gebied mogelijke waarde vooraf.
   >1. Vervang de veldregel door de nieuwe veldwaarde (na het &quot;=&quot;-teken).
   >1. Vervang de bepalingslijn (_Mod) met de nieuwe bepaling.
   >   
   >Deze instructies zijn hoofdlettergevoelig.

1. Klik **Gedaan**, dan **sparen Filter**.
