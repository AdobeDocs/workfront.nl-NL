---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Filter: uw huidige projecten tonen in afwachting van goedkeuring"'
description: De volgende projectfilter toont projecten in Huidig - in afwachting van de status van de Goedkeuring, waar de het programma geopende gebruiker of Sponsor van het Project of de Manager van de Portfolio is.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Filter: de huidige projecten tonen in afwachting van goedkeuring

De volgende projectfilter toont projecten in Huidig - in afwachting van de status van de Goedkeuring, waar de het programma geopende gebruiker of Sponsor van het Project of de Manager van de Portfolio is.

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

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Huidige projecten filteren in afwachting van goedkeuring

Dit filter toepassen:

1. Ga naar een lijst met projecten.
1. Van de **Filter** vervolgkeuzelijst, selecteert u **Nieuw filter**.

1. Klikken **Overschakelen naar tekstmodus**.
1. In de **Filterregels instellen voor uw rapport** gebied, kopieert en plakt de volgende code:
   <pre>status=CUR:A<br>sponsorID=$$USER.ID<br>OF:a:status=CUR:A<br>OF:a:portfolio:ownerID=$$USER.ID</pre>

1. Klikken **Filter opslaan**.
