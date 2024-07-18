---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groeperen: aangeven of de resultaten van een groepering moeten worden samengevouwen of uitgevouwen in tekstmodus'
description: 'Groeperen: aangeven of de resultaten van een groepering moeten worden samengevouwen of uitgevouwen in tekstmodus'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# Groeperen: geeft aan of de resultaten van een groepering moeten worden samengevouwen of uitgevouwen met de tekstmodus

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

U kunt erop wijzen of de resultaten in een groepering zouden moeten doen ineenstorten of in een lijst of rapport door de standaard rapportbouwer te gebruiken worden uitgebreid. De resultaten in een gegroepeerde weergave worden standaard uitgevouwen. Voor informatie over het creëren van een groepering, zie [ groepen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md) creëren.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* Wanneer u groepen handmatig aanpast wanneer u een lijst weergeeft, onthoudt Adobe Workfront uw handmatige voorkeur totdat u zich afmeldt. Wanneer u zich weer aanmeldt, wordt de lijst weergegeven volgens deze instelling.
>* De resultaten van een groepering tonen altijd uitgevouwen na de toegang tot hen van een grafiekelement.
>

U kunt ook aangeven of een groep moet worden uitgevouwen of samengevouwen in de tekstmodus.

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
   <td> <p>Verzoek om een groepering te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een groep te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Geef aan of de resultaten van een groepering moeten worden samengevouwen of uitgevouwen in de tekstmodus

1. Ga naar een lijst met objecten.
1. Van **het Groeperen** drop-down menu, uitgezochte **Nieuwe Groepering**.

1. Voeg een groepering toe en klik **Schakelaar aan de Wijze van de Tekst**.

   of

   Als de groepering reeds op tekstwijze is, voeg de volgende code aan het groeperingsniveau toe dat u samengevouwen wilt tonen:

   ```
   group.0.iscollapsed=true
   ```

1. (Optioneel) Als u wilt dat de groep wordt uitgevouwen, voegt u de volgende code toe aan het juiste groeperingsniveau:

   ```
   group.0.iscollapsed=false
   ```

1. Klik **Gedaan**, dan **sparen Groepering**.
