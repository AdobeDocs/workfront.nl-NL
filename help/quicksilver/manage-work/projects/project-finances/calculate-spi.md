---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Prestatie-index (SPI) voor planning berekenen
description: De index van de Prestaties van het Programma (SPI) beschrijft het verband tussen het geplande programma en werkelijk programma.
author: Alina
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Prestatie-index (SPI) voor planning berekenen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

De index van de Prestaties van het Programma (SPI) beschrijft het verband tussen het geplande programma en werkelijk programma. Adobe Workfront berekent de SPI op het project en de taakniveaus. De managers van het project herzien dit metrisch om te identificeren of de taken of de projecten momenteel voor of achter programma volgen.

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
   <td> <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten en financiële gegevens weergeven</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De mening of hogere toestemmingen aan het project met toestemmingen aan de Financiën van de Mening</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Overzicht van de prestatie-index (SPI) voor schema

* [ wat de waarde SPI ](#what-the-spi-value-shows) toont
* [Hoe Workfront SPI berekent](#how-workfront-calculates-spi)

### Wat de SPI waarde toont {#what-the-spi-value-shows}

Projectmanagers begrijpen dat een SPI-waarde van 1 betekent dat het project op schema of op schema ligt.  Waarden groter dan 1 geven aan dat een project voor de planning ligt en waarden kleiner dan 1 betekenen dat een project achter schema ligt.  Hoe verder van 1, hoe verder van het plan wordt afgeweken.

| **SPI Waarde** | **Verwijzing van &quot;op Programma&quot;** |
|---|---|
| 1 | Op abonnement of op schema |
| > 1 (groter dan 1) | Vooraf gepland |
| &lt; 1 (kleiner dan 1) | Achter schema |

{style="table-layout:auto"}

### Hoe Workfront SPI berekent  {#how-workfront-calculates-spi}

Workfront berekent de SPI met de volgende formule:

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;als Geplande die uren aan Datum = 0, SPI = 1* worden gepland.

Het geplande programma van uren aan Datum wordt berekend op de minuut wanneer u de berekeningen uitvoert. Het toont het aantal Geplande Uren die aan de huidige datum worden gepland. Het kan automatisch worden herberekend wanneer u uw financiële gegevens om correct verandert te zijn. Er is geen veld in Workfront dat deze waarde aangeeft.

Bijvoorbeeld, als u een project met 1 taak hebt en de taak 10 geplande uren en een Duur van 10 dagen heeft, is het Geplande Programma van Uren aan Datum op de 5de dag 5. 

## SPI zoeken in een project of taak

1. Ga naar het project of de taak waar u SPI wilt bekijken.
1. Afhankelijk van of u SPI op een project of een taak wilt bekijken, doe één van het volgende:

   1. Klik **Details van het Project** in het linkerpaneel, dan bekijk het **Financiën** gebied.

   1. Klik **Details van de Taak** in het linkerpaneel, dan bekijk het **Financiën** gebied.

      ![](assets/spi-on-project-nwe.png)

1. Vind het **CPI/SPI/CSI** gebied.
