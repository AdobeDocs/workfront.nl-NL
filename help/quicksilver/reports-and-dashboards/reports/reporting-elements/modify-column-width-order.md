---
product-area: reporting
navigation-topic: reporting-elements
title: Kolombreedte en -volgorde wijzigen
description: Lees dit artikel voor meer informatie over de richtlijnen voor kolombreedte en over het wijzigen van de kolombreedte en -volgorde in Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1004'
ht-degree: 0%

---

# Kolombreedte en -volgorde wijzigen

<!-- Audited: 11/2024 -->

Hieronder volgen enkele richtlijnen voor de werking van kolombreedten in Adobe Workfront:

* Workfront definieert standaard de breedte van kolommen in lijsten en rapporten.
* Workfront past automatisch de breedte van de kolommen volgens de `valueformat` informatie in alle lijsten en rapporten aan, tenzij anders gespecificeerd in de tekstwijze van de kolom.

  >[!NOTE]
  >
  >Workfront past de breedte van de kolommen niet aan volgens de `valueformat` -informatie in de lijsten die beschikbaar zijn in de gebieden Setup en Reports.

  De waarde `valueformat` definieert welk type informatie in de kolom wordt weergegeven. Kolommen met een getal zijn bijvoorbeeld smaller dan kolommen waarin het veld Beschrijving wordt weergegeven.

* U kunt de breedte van de kolommen in uw Workfront-lijsten en -rapporten aan uw wensen aanpassen, afhankelijk van het type informatie dat u in kolommen wilt weergeven.

  U kunt de breedte van kolommen tijdelijk wijzigen tijdens het weergeven van een lijst of rapport, of permanent, door de breedte van de kolom aan te passen in de weergavebuilder. Voor informatie over het tijdelijk wijzigen van de breedte van kolommen, zie de [&#x200B; Overwegingen wanneer tijdelijk het wijzigen van de breedte en de orde van kolommen &#x200B;](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) sectie in dit artikel.

* Kolommen die in ingebouwde weergaven worden weergegeven, hebben breedten die eerder door Workfront zijn gedefinieerd en die een harde code hebben. Als u deze breedten wilt wijzigen, moet u de breedte van deze kolommen handmatig bijwerken met de tekstmodus in de weergavebuilder.

  Voor informatie over het wijzigen van de kolom op tekstwijze, zie [&#x200B; Mening: geef permanent de breedte van een kolom &#x200B;](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md) uit.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</strong></td> 
   <td> 
    <p>Medewerker of hoger</p>
    <p>Aanvraag of hoger</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een weergave in een rapport te bewerken</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
    <td> <p>Rechten beheren voor een rapport om een weergave in een rapport te bewerken</p> <p>Machtigingen beheren voor een weergave om deze te bewerken</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Kolombreedte en -volgorde wijzigen

U kunt de breedte en de volgorde van de kolommen in uw rapporten op de volgende manieren wijzigen:

* [&#x200B; wijzigt tijdelijk breedte en orde van kolommen &#x200B;](#modify-width-and-order-of-columns-temporarily)
* [Breedte en volgorde van kolommen permanent wijzigen](#modify-width-and-order-of-columns-permanently)

### De breedte en volgorde van kolommen tijdelijk wijzigen {#modify-width-and-order-of-columns-temporarily}

U kunt kolomranden slepen om de grootte van kolommen te wijzigen en kolommen te slepen en neer te zetten om deze in de meeste lijsten tijdelijk opnieuw te rangschikken op de Workfront-site. Dit zijn rapporten, weergaven, rapporten op dashboards en de Gantt-weergave.

Voor meer informatie over de lijsten van Workfront, zie het artikel [&#x200B; begonnen worden met lijsten in Adobe Workfront &#x200B;](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* [&#x200B; Overwegingen wanneer tijdelijk het wijzigen van de breedte en de orde van kolommen &#x200B;](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [&#x200B; vergroot tijdelijk kolommen &#x200B;](#resize-columns-temporarily)
* [Kolommen tijdelijk opnieuw ordenen](#reorder-columns-temporarily)

#### Overwegingen bij het tijdelijk wijzigen van de breedte en volgorde van kolommen {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

U kunt de breedte en volgorde van kolommen in een lijst tijdelijk wijzigen zonder de weergave te bewerken.

Houd rekening met het volgende wanneer u tijdelijk kolommen groter/kleiner maakt en ordent:

* Wanneer het resizing van kolommen, worden de nieuwe kolomgrootte opgeslagen in de lokale opslag van uw browser, en door gebrek bewaard. Als u een andere browser gebruikt of de cache wist of gegevens bladert, wordt de standaardkolomgrootte hersteld. Als u de pagina vernieuwt, blijven de wijzigingen behouden die u aanbrengt in de breedte van de kolommen.

>[!NOTE]
> 
>Kolombreedten worden beperkt door het formaat van het browservenster. Als de pagina wordt vernieuwd, worden de kolommen breder totdat alle kolommen in het venster passen zonder horizontaal te schuiven. Om een kolom te dwingen breder te blijven dan browser zal passen, moet u de breedte van de kolom op tekstwijze plaatsen zoals die in [&#x200B; wordt beschreven wijzigt breedte en orde van kolommen permanent &#x200B;](#modify-width-and-order-of-columns-permanently) en vermijdt manueel om het even welke kolombreedten aan te passen door hun grenzen te slepen.
>

* Wanneer u de kolommen opnieuw rangschikt, blijft de gekozen volgorde alleen behouden totdat u van de lijst af navigeert of de browserpagina vernieuwt. Na het navigeren weg van de lijst of het verfrissen van de browser pagina, keren de kolommen aan hun standaardorde terug.
* Voor optimale prestaties mogen de kolommen die u opnieuw ordent, niet meer dan 100 items in de lijst bevatten.
* Wanneer u de grootte van kolommen wijzigt, worden de wijzigingen alleen toegepast op de weergave die u momenteel gebruikt. De wijzigingen zijn alleen voor u zichtbaar. Als u een weergave deelt met een andere gebruiker, worden de gedefinieerde kolomgrootten niet gedeeld.
* Nadat u het formaat van een kolom hebt gewijzigd door de rand naar rechts te slepen, blijft de breedte van de aangrenzende kolom behouden, behalve in het volgende:

   * Het gedeelte Instellen
   * Het gebied Rapporten
   * Documentlijsten en -rapporten

  >[!NOTE]
  >
  >U kunt de linkerrand van een kolom niet voorbij de linkerrand van de aangrenzende kolom in een lijst verplaatsen.

* Als u een lijst naar een bestand exporteert, wordt de tijdelijke volgorde van de kolommen niet overgedragen naar het geëxporteerde bestand. In het geëxporteerde bestand wordt de volgorde van de kolommen in de oorspronkelijke lijst weergegeven voordat de volgorde van de kolommen is gewijzigd.

Voor meer informatie over het uitvoeren van gegevens van lijsten en rapporten, zie de gegevens van de artikel [&#x200B; Uitvoer &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

#### Kolommen tijdelijk vergroten/verkleinen {#resize-columns-temporarily}

1. Ga naar de lijst die u wilt wijzigen.
1. Sleep de rand van een kolomkop tot de kolom de gewenste grootte heeft bereikt.\
   ![&#x200B; Resize kolom &#x200B;](assets/column-resize-350x124.png)

#### Kolommen tijdelijk opnieuw ordenen {#reorder-columns-temporarily}

1. Ga naar de lijst die u wilt wijzigen.
1. Klik en sleep de kolomkop die u naar de gewenste locatie wilt verplaatsen.

>[!TIP]
>
>Dit is vooral handig wanneer u het Gantt-diagram en de lijstweergave tegelijk bekijkt. Bij weergave van het Gantt-diagram kunnen kolommen verborgen worden. Als u een kolom wilt weergeven terwijl het Gantt-diagram wordt weergegeven, sleept u gewoon de kolom die u wilt weergeven, zodat deze links op de pagina wordt weergegeven.

### Breedte en volgorde van kolommen permanent wijzigen {#modify-width-and-order-of-columns-permanently}

Om kolommen permanent opnieuw in orde te brengen, zie de sectie [&#x200B; een standaardmening &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view) in het artikel [&#x200B; overzicht van Meningen in Adobe Workfront &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md) creëren of aanpassen.

U kunt de breedte van een kolom alleen permanent wijzigen in de tekstmodus.

Voor meer informatie over het gebruiken van tekstwijze en permanent het wijzigen van de breedte van een kolom, zie het artikel [&#x200B; Overzicht van gemeenschappelijk gebruik voor de Wijze van de Tekst &#x200B;](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
