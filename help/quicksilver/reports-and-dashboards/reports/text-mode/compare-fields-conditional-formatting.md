---
product-area: reporting
navigation-topic: text-mode-reporting
title: Velden in voorwaardelijke opmaak vergelijken
description: Met voorwaardelijke opmaak kunt u twee verschillende velden in een weergave vergelijken en markeren als aan bepaalde criteria is voldaan tussen de velden.
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Velden in voorwaardelijke opmaak vergelijken

<!-- Audited: 1/2025 -->

Met voorwaardelijke opmaak kunt u twee verschillende velden in een weergave vergelijken en markeren als aan bepaalde criteria is voldaan tussen de velden.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
      <p>Nieuw:</p>
         <ul>
         <li><p>Standaard</p></li>
         </ul>
      <p>Huidige:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken om de weergave in een rapport te bewerken</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten beheren voor een rapport om de weergave in een rapport te bewerken</p> <p>Rechten beheren voor een weergave</p></td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voorbeeld: werkelijke begindatum en geplande begindatum vergelijken

Als de werkelijke begindatum van een taak bijvoorbeeld na de geplande begindatum ligt, kunt u de kolom Geplande begindatum markeren met voorwaardelijke opmaak.

U kunt als volgt de geplande begindatum en de werkelijke begindatum vergelijken met voorwaardelijke opmaak:

1. Ga naar een taakmening of een rapport.
1. (Voorwaardelijk) als u met een rapport werkt, van het **lusje van Kolommen (Mening)** in de rapportredacteur, klik de kopbal van de kolom u voorwaardelijk wilt formatteren om het te selecteren.\
   Bijvoorbeeld, selecteer de **Ware kolom van de Datum van het Begin** als u het voorwaardelijke formatteren aan het wilt toevoegen door de Geplande Datum van het Begin en de Ware gebieden van de Datum van het Begin te vergelijken.

1. Klik **Geavanceerde Opties**, dan klik toevoegen a **Regel voor deze Kolom**.

1. Voer de vergelijkingscriteria in op basis van bestaande waarden in de builder en geef de voorwaardelijke opmaak op.\
   We willen bijvoorbeeld taken markeren waarbij de werkelijke begindatum later is dan (of hoger is dan) de geplande begindatum. Selecteer de optie Groter dan en selecteer een werkelijke datum in het datumveld.

   ![](assets/cond-format-1-350x84.png)

1. (Optioneel) Selecteer **Toepassen op volledige rij** als u de opmaak op de volledige rij wilt toepassen.
1. Klik **sparen**.

1. Selecteer de **Ware kolom van de Datum van het Begin**, dan klik **Schakelaar aan de Wijze van de Tekst**.

1. Klik **uitgeven de Wijze van de Tekst**, dan voeg de volgende lijn van tekst toe:

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   In ons voorbeeld:

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >Als u een eigen Workfront-veld vergelijkt, gebruikt u de syntaxis van camelhoofdletters voor de naam van het veld. Als u een douanegebied vergelijkt, gebruik **DE:Ware Naam van het Gebied** voor het naamgebied u met het eerste gebied vergelijkt.\
   >Bijvoorbeeld, als u de **Ware Datum van het Begin** met een douanegebied etiketteerde **Datum van de Levering** vergelijkt, voeg de volgende verklaring op uw code van de tekstwijze toe:
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. Zorg ervoor dat de coderegel `righttext` overeenkomt met de instructie in de coderegel `rightmethod` .

   ![](assets/cond-format-2-350x171.png)

1. Klik **sparen**.
1. Klik **sparen + Sluiten**.

   In de kolom worden de velden gemarkeerd die aan uw criteria voldoen.
