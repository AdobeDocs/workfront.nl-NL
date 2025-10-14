---
title: Bouw een formules gebied in het Rapporteren van Canvas
description: Bouw een formules gebied in het Rapporteren van Canvas
hidefromtoc: true
hide: true
exl-id: 22a2c3d7-39db-4f5d-94f3-222ca3ee0615
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---

# Bouw een formules gebied in het Rapporteren van Canvas

De gebiedsbouwer in het Melden van Canvas staat u toe om gebieden tot stand te brengen die douaneberekeningen uitvoeren.

## Vereisten

Alvorens u begint, moet u in de bèta van het Canvas van de Rapportering inschrijven. Voor meer informatie, zie [&#x200B; Rapporterend de bèta van het Canvas: overzicht &#x200B;](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Een veld met een formule maken

1. Creeer of navigeer aan een lijstblok, zoals die in [&#x200B; wordt beschreven voeg of geef een lijstblok in het Melden van Canvas &#x200B;](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md) toe uit.
1. Voor de lijstkopbal in het rapport, klik **uitgeven** pictogram ![&#x200B; pictogram geeft pictogram &#x200B;](assets/edit-icon.png) uit.

   ![&#x200B; geef pictogram in lijstkopbal uit &#x200B;](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Als u de tabel hebt gemaakt en nog geen velden hebt toegevoegd, klikt u in plaats daarvan op de knop Bewerken in het midden van de tabel.

1. Klik **Nieuw +** bij de bovenkant van de **lijst van Gebieden** op het juiste paneel.
1. In de nieuwe pagina die opent, **uitgeeft** pictogram ![&#x200B; geeft pictogram &#x200B;](assets/edit-icon.png) naast de gebiedsnaam in de top-left hoek uit om de naam van het formuleringsgebied te veranderen.
1. Sleep **Functies** of **Gebieden** van het linkerpaneel op de gebiedsbouwer in het centrum om hen aan uw formuleringsgebied toe te voegen.


   >[!TIP]
   >
   >Aangezien u uw formuleringsgebied bouwt, **de voorproef van het Gebied** op het recht toont voorbeelden van het resulterende gebied.

   Elke functie bevat een aantal lege gestippelde rechthoeken die als argumenten voor het berekenen van een resultaat zullen worden gebruikt. Deze kunnen worden gevuld door statische tekst of getallen in te voeren, een veld vanuit het linkerdeelvenster te slepen (met de waarde van het veld in de berekening) of door een andere functie te slepen en neer te zetten (een geneste functie maken). Mogelijke functies zijn:

   | Functie | Beschrijving | Uitvoer |
   |---|---|---|
   | IF | Vergelijk twee argumenten die op een geselecteerde bepaling worden gebaseerd, dan voer een gespecificeerde actie uit die op de resulterende Waar (Is Waar:) of Vals (Is Vals:) waarde wordt gebaseerd. Opmerking: momenteel kan het tweede argument geen statische waarde Waar of Onwaar zijn. In plaats daarvan, kunt u een genestelde functie zoals ISBLANK (de Naam van het Project) gebruiken die altijd Vals als een oplossing terugkeert. | True/False, Date, Number of String |
   | CONCREET | Voeg twee of meer tekenreeksen van begin tot eind samen om een nieuwe tekenreeks te maken. | String |
   | BEVATTEN | Evalueer of een veld voor een tekenreeksargument (Tekst zoeken) zich in een ander veld voor een tekenreeksargument bevindt (Binnen tekst). | Waar/Onwaar |
   | IN | Evalueren of de waarde van een argumentveld (Zoeken) overeenkomt met de waarde van ten minste een ander argumentveld (Binnen) | Waar/Onwaar |
   | ISBLANK | Evalueren of een argumentveld leeg is. | Waar/Onwaar |
   | LEN | Meet de lengte (in aantal tekens) van een argumentveld. | Getal |
   | ROND | Retourneert een afgerond getal op basis van de geselecteerde precisie. | Getal |
   | FLOOR | Retourneert het dichtstbijzijnde gehele getal, naar beneden afgerond. | Getal |
   | NUMMER | Geeft de grootste interger minder dan de waarde van een numeriek argument (identiek aan een functie Floor). | Getal |
   | TEKENREEKS | Zet de inhoud van een argumentveld om in een tekenreeks | String |
   | SUBSTR | Maak een nieuwe tekenreeks van een grotere tekenreeks, die de tekens bevat tussen het ene indexnummer (Start) en het andere (End). | String |
   | LINKS | Maak een nieuwe tekenreeks van een grotere tekenreeks, die tekens bevat die beginnen met het meest linkse teken en een aantal tekens rechts tellen (Lengte). | String |
   | RECHTS | Maak een nieuwe tekenreeks van een grotere tekenreeks, die tekens bevat die beginnen met de meest rechtse en die een aantal tekens links tellen (Lengte). | String |
   | SUM | Voeg de waarden van twee of meer argumentvelden samen toe. | Getal |
   | SUB | Trek de waarden van twee of meer argumentvelden af (in volgorde van links naar rechts). | Getal |
   | PROD | Vermenigvuldig de waarden van twee of meer argumentvelden samen. | Getal |
   | DIV | Verdeel de waarde van twee of meer argumentvelden (in volgorde van links naar rechts). | Getal |
   | MAAND | Retourneert een getal dat gelijk is aan de maandwaarde voor een datum. | Getal |
   | JAAR | Retourneert een getal dat gelijk is aan de jaarwaarde voor een datum. | Getal |
   | DATEDIFF | Berekent het totale aantal dagen tussen twee datums, afgerond op één decimaal. | Getal |
   | WEEKDAYDIFF | Berekent het aantal weekdagen tussen twee datums, afgerond op één decimaal. | Getal |

   {style="table-layout:auto"}

1. Klik **gaan terug** pijl in de upper-left hoek van het scherm om aan uw lijst terug te keren.
