---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Prestatie-index (SPI) voor planning berekenen
description: De index van de Prestaties van het Programma (SPI) beschrijft het verband tussen het geplande programma en werkelijk programma.
author: Lisa
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Prestatie-index (SPI) voor planning berekenen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

De index van de Prestaties van het Programma (SPI) beschrijft het verband tussen het geplande programma en werkelijk programma. Adobe Workfront berekent de SPI op het project en de taakniveaus. De managers van het project herzien dit metrisch om te identificeren of de taken of de projecten momenteel voor of achter programma volgen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td>
   <p>Licht of hoger</p>
   <p>Controleren of hoger</p></td>  
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>Toegang tot projecten en financiële gegevens weergeven</td> 
  </tr> 
  <tr> 
   <td>Objectmachtigingen</td> 
   <td>De mening of hogere toestemmingen aan het project met toestemmingen aan de Financiën van de Mening</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overzicht van de prestatie-index (SPI) voor schema

* [&#x200B; wat de waarde SPI &#x200B;](#what-the-spi-value-shows) toont
* [Hoe Workfront SPI berekent](#how-workfront-calculates-spi)

### Wat de SPI waarde toont {#what-the-spi-value-shows}

Projectmanagers begrijpen dat een SPI-waarde van 1 betekent dat het project op schema of op schema ligt.  Waarden groter dan 1 geven aan dat een project voor de planning ligt en waarden kleiner dan 1 betekenen dat een project achter schema ligt.  Hoe verder van 1, hoe verder van het plan wordt afgeweken.

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

Het geplande programma van uren aan Datum wordt berekend op de minuut wanneer u de berekeningen uitvoert. Het toont het aantal Geplande Uren die aan de huidige datum worden gepland. Het kan automatisch worden herberekend wanneer u uw financiële gegevens om correct verandert te zijn. Er is geen veld in Workfront dat deze waarde aangeeft.

Bijvoorbeeld, als u een project met 1 taak hebt en de taak 10 geplande uren en een Duur van 10 dagen heeft, is het Geplande Programma van Uren aan Datum op de 5de dag 5.

## SPI zoeken in een project of taak

1. Ga naar het project of de taak waar u SPI wilt bekijken.
1. Afhankelijk van of u SPI op een project of een taak wilt bekijken, doe één van het volgende:

   1. Klik **Details van het Project** in het linkerpaneel, dan bekijk het **Financiën** gebied.

   1. Klik **Details van de Taak** in het linkerpaneel, dan bekijk het **Financiën** gebied.

      ![&#x200B; SPI op project &#x200B;](assets/spi-on-project-nwe.png)

1. Vind het **CPI/SPI/CSI** gebied.
