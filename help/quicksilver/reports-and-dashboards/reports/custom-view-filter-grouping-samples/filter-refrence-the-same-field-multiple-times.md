---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filter: meerdere filterregels maken die naar hetzelfde veld verwijzen ('AND'-instructies)"
description: In de standaardwijzeinterface, wanneer het proberen om veelvoudige filters tot stand te brengen die het zelfde gebied (gebruiken EN bepalend) van verwijzingen voorzien, wordt één van de filters geschrapt wanneer u sparen het rapport en de rapportaannemer weggaat.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 8b6324302a70319f387d1e09d1eb92fbdabf7e32
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Filter: meerdere filterregels maken die naar hetzelfde veld verwijzen (&quot;AND&quot;-instructies)

In de standaardwijzeinterface, wanneer het proberen om veelvoudige filters tot stand te brengen die het zelfde gebied (gebruiken EN bepalend) van verwijzingen voorzien, wordt één van de filters geschrapt wanneer u sparen het rapport en de rapportaannemer weggaat.

**Voorbeeld:** Mogelijk wilt u alleen taken weergeven die het woord &quot;groen&quot; bevatten, maar niet het woord &quot;rood&quot; in de naam. Adobe Workfront staat u niet toe om de volgende filterregels te bewaren gebruikend de standaardwijzeinterface omdat het verwijst naar het zelfde gebied (de Naam van de Taak) maar verschillende bepalingen gebruikt en naar verschillende waarden verwijst:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Meerdere filterregels maken die naar hetzelfde veld verwijzen

1. Ga naar een takenlijst.
1. Van de **Filter** vervolgkeuzelijst, selecteert u **Nieuw filter**.
1. Klikken **Overschakelen naar tekstmodus**.
1. Houd de cursor boven het gebied van de tekstmodus en klik op **Klik om tekst te bewerken**.
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
   >
   ```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >Kopieer en plak de instructie zo vaak als nodig is. Vervolgens kunt u zoveel instructies toevoegen als u nodig hebt om naar hetzelfde veld te verwijzen (in ons geval &#39;name&#39;) en de volgende wijzigingen in de aanvullende instructies aanbrengen:
   >
   >1. Vóór de twee gekopieerde regels &quot;AND&quot;:1:&quot;, &quot;AND:2:&quot;, &quot;AND:3:&quot;, enz. voor elk nieuw veld mogelijke waarde.
   >1. Vervang de veldregel door de nieuwe veldwaarde (na het &quot;=&quot;-teken).
   >1. Vervang de bepalingslijn (_Mod) met de nieuwe bepaling.

   >   
   >Deze instructies zijn hoofdlettergevoelig.

1. Klikken **Gereed** vervolgens **Filter opslaan**.
