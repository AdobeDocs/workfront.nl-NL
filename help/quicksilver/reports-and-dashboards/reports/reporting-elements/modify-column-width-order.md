---
product-area: reporting
navigation-topic: reporting-elements
title: Kolombreedte en -volgorde wijzigen
description: Lees dit artikel voor meer informatie over de richtlijnen voor kolombreedte en over het wijzigen van de kolombreedte en -volgorde in Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 0%

---

# Kolombreedte en -volgorde wijzigen

Hieronder volgen enkele richtlijnen voor de werking van kolombreedten in Adobe Workfront:

* Workfront definieert standaard de breedte van kolommen in lijsten en rapporten.
* Workfront past automatisch de breedte van de kolommen aan volgens de `valueformat`informatie in alle lijsten en rapporten, tenzij anders gespecificeerd in de tekstwijze van de kolom.

   >[!NOTE]
   >
   >Workfront past de breedte van de kolommen niet aan volgens de `valueformat` informatie in de lijsten beschikbaar in de Opstelling en de gebieden van Rapporten.

   De `valueformat` value definieert welk type informatie in de kolom wordt weergegeven. Kolommen met een getal zijn bijvoorbeeld smaller dan kolommen waarin het veld Beschrijving wordt weergegeven.

* U kunt de breedte van de kolommen in uw Workfront-lijsten en -rapporten aan uw wensen aanpassen, afhankelijk van het type informatie dat u in kolommen wilt weergeven.

   U kunt de breedte van kolommen tijdelijk wijzigen tijdens het weergeven van een lijst of rapport, of permanent, door de breedte van de kolom aan te passen in de weergavebuilder. Voor informatie over het tijdelijk wijzigen van de breedte van kolommen, zie [Overwegingen bij het tijdelijk wijzigen van de breedte en volgorde van kolommen](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) in dit artikel.

* Kolommen die in ingebouwde weergaven worden weergegeven, hebben breedten die eerder door Workfront zijn gedefinieerd en die een harde code hebben. Als u deze breedten wilt wijzigen, moet u de breedte van deze kolommen handmatig bijwerken met de tekstmodus in de weergavebuilder.

   Zie voor meer informatie over het wijzigen van de kolom in de tekstmodus [Weergave: De breedte van een kolom permanent bewerken](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-abonnement*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken om de weergave in een rapport te bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Rechten beheren voor een rapport om een weergave in een rapport te bewerken</p> <p>Machtigingen beheren voor een weergave om deze te bewerken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Kolombreedte en -volgorde wijzigen

U kunt de breedte en de volgorde van de kolommen in uw rapporten op de volgende manieren wijzigen:

* [De breedte en volgorde van kolommen tijdelijk wijzigen](#modify-width-and-order-of-columns-temporarily)
* [Breedte en volgorde van kolommen permanent wijzigen](#modify-width-and-order-of-columns-permanently)

### De breedte en volgorde van kolommen tijdelijk wijzigen {#modify-width-and-order-of-columns-temporarily}

U kunt kolomranden slepen om de grootte van kolommen te wijzigen en kolommen te slepen en neer te zetten om deze in de meeste lijsten tijdelijk opnieuw te rangschikken op de Workfront-site. Dit zijn rapporten, weergaven, rapporten op dashboards en de Gantt-weergave.

Raadpleeg het artikel voor meer informatie over Workfront-lijsten [Aan de slag met lijsten in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* [Overwegingen bij het tijdelijk wijzigen van de breedte en volgorde van kolommen](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [Kolommen tijdelijk vergroten/verkleinen](#resize-columns-temporarily)
* [Kolommen tijdelijk opnieuw ordenen](#reorder-columns-temporarily)

#### Overwegingen bij het tijdelijk wijzigen van de breedte en volgorde van kolommen {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

U kunt de breedte en volgorde van kolommen in een lijst tijdelijk wijzigen zonder de weergave te bewerken.

Houd rekening met het volgende wanneer u tijdelijk kolommen groter/kleiner maakt en ordent:

* Wanneer het resizing van kolommen, worden de nieuwe kolomgrootte opgeslagen in de lokale opslag van uw browser, en door gebrek bewaard. Als u een andere browser gebruikt of de cache wist of gegevens bladert, wordt de standaardkolomgrootte hersteld. Als u de pagina vernieuwt, blijven de wijzigingen behouden die u aanbrengt in de breedte van de kolommen.
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

Raadpleeg het artikel voor meer informatie over het exporteren van gegevens uit lijsten en rapporten [Gegevens exporteren](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

#### Kolommen tijdelijk vergroten/verkleinen {#resize-columns-temporarily}

1. Ga naar de lijst die u wilt wijzigen.
1. Sleep de rand van een kolom tot de kolom de gewenste grootte heeft bereikt.\
   ![](assets/column-resize-350x124.png)

#### Kolommen tijdelijk opnieuw ordenen {#reorder-columns-temporarily}

1. Ga naar de lijst die u wilt wijzigen.
1. Klik op een kolom die u naar een andere locatie wilt verplaatsen om de kolom te kiezen.
1. Sleep de kolom naar de juiste locatie.
1. Zet de kolom neer in de plaats, om het te bewegen.

   ![](assets/column-reorder-350x118.png)

>[!TIP]
>
>Dit is vooral handig wanneer u het Gantt-diagram en de lijstweergave tegelijk bekijkt. Bij weergave van het Gantt-diagram kunnen kolommen verborgen worden. Als u een kolom wilt weergeven terwijl het Gantt-diagram wordt weergegeven, sleept u gewoon de kolom die u wilt weergeven, zodat deze links op de pagina wordt weergegeven.

### Breedte en volgorde van kolommen permanent wijzigen {#modify-width-and-order-of-columns-permanently}

Zie de sectie voor het permanent opnieuw ordenen van kolommen [Een standaardweergave maken of aanpassen](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view) in het artikel [Overzicht van weergaven in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

U kunt de breedte van een kolom alleen permanent wijzigen in de tekstmodus.

Zie het artikel voor meer informatie over het gebruik van de tekstmodus en het permanent wijzigen van de breedte van een kolom [Overzicht van veelvoorkomende toepassingen voor de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
