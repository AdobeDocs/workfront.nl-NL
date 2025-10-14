---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groeperen: geef aan of de resultaten van een groepering moeten worden samengevouwen of uitgevouwen met de tekstmodus'
description: 'Groeperen: geeft aan of de resultaten van een groepering moeten worden samengevouwen of uitgevouwen met de tekstmodus'
author: Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# Groeperen: geeft aan of de resultaten van een groepering moeten worden samengevouwen of uitgevouwen met de tekstmodus

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

U kunt erop wijzen of de resultaten in een groepering zouden moeten doen ineenstorten of in een lijst of rapport door de standaard rapportbouwer te gebruiken worden uitgebreid. De resultaten in een gegroepeerde weergave worden standaard uitgevouwen. Voor informatie over het creëren van een groepering, zie [&#x200B; groepen in Adobe Workfront &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md) creëren.

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

*For informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Geef aan of de resultaten van een groepering moeten worden samengevouwen of uitgevouwen in de tekstmodus

1. Ga naar een lijst met objecten.
1. Van **het Groeperen** drop-down menu, uitgezochte **Nieuwe Groepering**.

1. Voeg een groepering toe, dan klik **Schakelaar aan de Wijze van de Tekst**.

   of

   Als de groepering reeds op tekstwijze is, voeg de volgende code aan het groeperingsniveau toe dat u samengevouwen wilt tonen:

   `group.0.iscollapsed=true`

1. (Optioneel) Als u wilt dat de groep wordt uitgevouwen, voegt u de volgende code toe aan het juiste groeperingsniveau:

   `group.0.iscollapsed=false`

1. Klik **Gedaan**, dan **sparen Groepering**.
1. (facultatief) werk de naam van de groepering bij, dan klik **sparen Groepering**.
