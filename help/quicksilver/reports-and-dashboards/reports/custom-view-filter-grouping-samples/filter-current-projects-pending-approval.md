---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: uw huidige projecten weergeven in afwachting van goedkeuring'
description: De volgende projectfilter toont projecten in Huidig - in afwachting van de status van de Goedkeuring, waar de het programma geopende gebruiker of Sponsor van het Project of de Manager van het Portfolio is.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Filter: uw huidige projecten weergeven in afwachting van goedkeuring

De volgende projectfilter toont projecten in Huidig - in afwachting van de status van de Goedkeuring, waar de het programma geopende gebruiker of Sponsor van het Project of de Manager van het Portfolio is.

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

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Huidige projecten filteren in afwachting van goedkeuring

Dit filter toepassen:

1. Ga naar een lijst met projecten.
1. Van het **drop-down menu van de Filter**, uitgezochte **Nieuwe Filter**.

1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. In het **plaats de Regels van de Filter voor uw gebied van het Rapport**, kopieer en kleef de volgende code:
   <pre>status=CUR:A<br> sponsorID=$$USER.ID <br> OF :a: status=CUR:A <br> OF :a: portefeuille:ownerID=$$USER.ID</pre>

1. Klik **sparen Filter**.
