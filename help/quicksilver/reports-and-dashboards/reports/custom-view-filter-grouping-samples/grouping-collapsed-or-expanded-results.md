---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groeperen: aangeven of de resultaten van een groepering moeten worden samengevouwen of uitgevouwen in de tekstmodus.'
description: 'Groeperen: aangeven of de resultaten van een groepering moeten worden samengevouwen of uitgevouwen in de tekstmodus.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Groeperen: aangeven of de resultaten van een groepering moeten worden samengevouwen of uitgevouwen in de tekstmodus

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

U kunt erop wijzen of de resultaten in een groepering zouden moeten doen ineenstorten of in een lijst of rapport door de standaard rapportbouwer te gebruiken worden uitgebreid. De resultaten in een gegroepeerde weergave worden standaard uitgevouwen. Voor informatie over het maken van een groep raadpleegt u [Groepen maken in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

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

## Geef aan of de resultaten van een groepering moeten worden samengevouwen of uitgevouwen in de tekstmodus

1. Ga naar een lijst met objecten.
1. Van de **Groepering** vervolgkeuzelijst, selecteert u **Nieuwe groepering**.

1. Een groep toevoegen en klikken **Overschakelen naar tekstmodus**.

   of

   Als de groepering reeds op tekstwijze is, voeg de volgende code aan het groeperingsniveau toe dat u samengevouwen wilt tonen:

   ```
   group.0.iscollapsed=true
   ```

1. (Optioneel) Als u wilt dat de groep wordt uitgevouwen, voegt u de volgende code toe aan het juiste groeperingsniveau:

   ```
   group.0.iscollapsed=false
   ```

1. Klikken **Gereed** vervolgens **Groepering opslaan**.
