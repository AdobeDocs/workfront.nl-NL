---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filter: meerdere filterregels maken die verwijzen naar hetzelfde veld ('AND'-instructies)"
description: In de standaardwijzeinterface, wanneer het proberen om veelvoudige filters tot stand te brengen die het zelfde gebied (gebruiken EN bepalend) van verwijzingen voorzien, wordt één van de filters geschrapt wanneer u sparen het rapport en de rapportaannemer weggaat.
author: Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Filter: meerdere filterregels maken die naar hetzelfde veld verwijzen (&quot;AND&quot;-instructies)

<!--Audited: 10/2024-->

In de standaardwijzeinterface, wanneer het proberen om veelvoudige filters tot stand te brengen die het zelfde gebied (gebruiken EN bepalend) van verwijzingen voorzien, wordt één van de filters geschrapt wanneer u sparen het rapport en de rapportaannemer weggaat.

**Voorbeeld:** u zou slechts taken kunnen willen bekijken die het woord &quot;groen&quot;bevatten maar niet het woord &quot;rood&quot;in de naam bevatten. Adobe Workfront staat u niet toe om de volgende filterregels te bewaren gebruikend de standaardwijzeinterface omdat het verwijst naar het zelfde gebied (de Naam van de Taak) maar verschillende bepalingen gebruikt en naar verschillende waarden verwijst:

* Taaknaam > Bevat > Groen
* Taaknaam > Bevat niet > Rood

U kunt dit filter echter maken in de tekstmodus.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> 
    <p>Nieuw:</p>
   <ul><li><p>Medewerker om een filter te wijzigen </p></li>
   <li><p>Standaard voor het wijzigen van een rapport</p></li> </ul>

<p>Huidige:</p>
   <ul><li><p>Verzoek om een filter te wijzigen </p></li>
   <li><p>Plan om een rapport te wijzigen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Meerdere filterregels maken die naar hetzelfde veld verwijzen

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Filter**, uitgezochte **Nieuwe Filter**.
1. Klik **Wijze van de Tekst**.
1. Voeg de volgende code toe in het weergegeven vak:

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

1. Klik **toepassen**, dan **sparen als nieuw**.
