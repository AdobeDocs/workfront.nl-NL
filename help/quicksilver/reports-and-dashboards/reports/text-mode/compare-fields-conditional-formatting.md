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
source-wordcount: '510'
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
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken om de weergave in een rapport te bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten beheren voor een rapport om de weergave in een rapport te bewerken</p> <p>Machtigingen beheren voor een weergave</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Voorbeeld: Ware begindatum en geplande begindatum vergelijken

Als de werkelijke begindatum van een taak bijvoorbeeld na de geplande begindatum ligt, kunt u de kolom Geplande begindatum markeren met voorwaardelijke opmaak.

U kunt als volgt de geplande begindatum en de werkelijke begindatum vergelijken met voorwaardelijke opmaak:

1. Ga naar een taakmening of een rapport.
1. (Voorwaardelijk) Als u met een rapport werkt, kunt u **Kolommen (weergave)** klikt u op de kop van de kolom die u voorwaardelijk wilt opmaken om deze te selecteren.\
   Selecteer bijvoorbeeld de **Werkelijke begindatum** als u de voorwaardelijke opmaak eraan wilt toevoegen door de velden Geplande begindatum en Werkelijke begindatum te vergelijken.

1. Klikken **Geavanceerde opties** en klik vervolgens op Een **Regel voor deze kolom**.

1. Voer de vergelijkingscriteria in op basis van bestaande waarden in de builder en geef de voorwaardelijke opmaak op.\
   We willen bijvoorbeeld taken markeren waarbij de werkelijke begindatum later is dan (of hoger is dan) de geplande begindatum. Selecteer de optie Groter dan en selecteer een werkelijke datum in het datumveld.\
     ![](assets/cond-format-1-350x84.png)

1. (Optioneel) Selecteer **Toepassen op hele rij** als u de opmaak op de hele rij wilt toepassen.
1. Klikken **Regel toevoegen** vervolgens **Gereed**.

1. Selecteer **Werkelijke begindatum** kolom, klik vervolgens op **Overschakelen naar tekstmodus**.

1. **Klik om tekst te bewerken** Voeg vervolgens de volgende tekstregel toe:

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   In ons voorbeeld: 

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >Als u een eigen Workfront-veld vergelijkt, gebruikt u de syntaxis van camelhoofdletters voor de naam van het veld. Als u een aangepast veld vergelijkt, kunt u **DE:Werkelijke naam van het veld** voor het naamveld dat u vergelijkt met het eerste veld.\
   >Als u bijvoorbeeld de **Werkelijke begindatum** met een aangepast veld met label **Leveringsdatum** voegt u de volgende instructie toe aan de code van de tekstmodus:
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. Zorg ervoor dat de `righttext` coderegel komt overeen met de instructie in het dialoogvenster `rightmethod` coderegel.

   ![](assets/cond-format-2-350x171.png)

1. Klikken **Opslaan**.
1. Klikken **Opslaan + Sluiten**.

   De kolom markeert de velden die aan uw criteria voldoen.
