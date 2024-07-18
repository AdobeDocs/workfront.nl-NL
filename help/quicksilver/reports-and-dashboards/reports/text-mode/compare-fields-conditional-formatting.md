---
product-area: reporting
navigation-topic: text-mode-reporting
title: Velden in voorwaardelijke opmaak vergelijken
description: Met voorwaardelijke opmaak kunt u twee verschillende velden in een weergave vergelijken en markeren als aan bepaalde criteria is voldaan tussen de velden.
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Velden in voorwaardelijke opmaak vergelijken

Met voorwaardelijke opmaak kunt u twee verschillende velden in een weergave vergelijken en markeren als aan bepaalde criteria is voldaan tussen de velden.

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
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken om de weergave in een rapport te bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten beheren voor een rapport om de weergave in een rapport te bewerken</p> <p>Rechten beheren voor een weergave</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Voorbeeld: werkelijke begindatum en geplande begindatum vergelijken

Als de werkelijke begindatum van een taak bijvoorbeeld na de geplande begindatum ligt, kunt u de kolom Geplande begindatum markeren met voorwaardelijke opmaak.

U kunt als volgt de geplande begindatum en de werkelijke begindatum vergelijken met voorwaardelijke opmaak:

1. Ga naar een taakmening of een rapport.
1. (Voorwaardelijk) als u met een rapport werkt, van de **Kolommen (Mening)** tabel, klik de kopbal van de kolom u voorwaardelijk wilt formatteren om het te selecteren.\
   Bijvoorbeeld, selecteer de **Ware kolom van de Datum van het Begin** als u het voorwaardelijke formatteren aan het wilt toevoegen door de Geplande Datum van het Begin en de Ware gebieden van de Datum van het Begin te vergelijken.

1. Klik **Geavanceerde Opties**, dan klik toevoegen a **Regel voor deze Kolom**.

1. Voer de vergelijkingscriteria in op basis van bestaande waarden in de builder en geef de voorwaardelijke opmaak op.\
   We willen bijvoorbeeld taken markeren waarbij de werkelijke begindatum later is dan (of hoger is dan) de geplande begindatum. Selecteer de optie Groter dan en selecteer een werkelijke datum in het datumveld.\
     ![](assets/cond-format-1-350x84.png)

1. (Optioneel) Selecteer **Toepassen op volledige rij** als u de opmaak op de volledige rij wilt toepassen.
1. Klik **toevoegen Regel**, dan **Gedaan**.

1. Selecteer de **Ware kolom van de Datum van het Begin**, dan klik **Schakelaar aan de Wijze van de Tekst**.

1. **klik om tekst** wijze uit te geven dan de volgende lijn van tekst toe te voegen:

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
