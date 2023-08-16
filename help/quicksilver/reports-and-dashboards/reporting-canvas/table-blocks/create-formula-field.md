---
title: Bouw een formules gebied in het Rapporteren van Canvas
description: Bouw een formules gebied in het Rapporteren van Canvas
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: 22a2c3d7-39db-4f5d-94f3-222ca3ee0615
hidefromtoc: true
hide: true
source-git-commit: a9c36ff874d3272e1d2de70578c420af29b9d44c
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---


# Bouw een formules gebied in het Rapporteren van Canvas

De gebiedsbouwer in het Melden van Canvas staat u toe om gebieden tot stand te brengen die douaneberekeningen uitvoeren.

## Vereisten

Alvorens u begint, moet u in de bèta van het Canvas van de Rapportering inschrijven. Zie voor meer informatie [Bewerken van canvas melden: overzicht](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Een veld met een formule maken

1. Een tabelblok maken of naar een tabelblok navigeren, zoals beschreven in [Een tabelblok toevoegen of bewerken in het rapportcanvas](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md).
1. Voor de lijstkopbal in het rapport, klik **Bewerken** pictogram ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Als u de tabel hebt gemaakt en nog geen velden hebt toegevoegd, klikt u in plaats daarvan op de knop Bewerken in het midden van de tabel.

1. Klikken **Nieuw +** boven aan het dialoogvenster **Velden** in het rechterdeelvenster.
1. Klik op de nieuwe pagina die wordt geopend op de knop **Bewerken** pictogram ![](assets/edit-icon.png) naast de veldnaam in de linkerbovenhoek om de naam van het formuleveld te wijzigen.
1. Slepen **Functies** of **Velden** van het linkerpaneel op de gebiedsbouwer in het centrum om hen aan uw formuleringsgebied toe te voegen.


   >[!TIP]
   >
   >Wanneer u het veld voor de formule maakt, **Voorvertoning veld** rechts in het scherm worden voorbeelden van het resulterende veld weergegeven.

   Elke functie bevat een aantal lege gestippelde rechthoeken die als argumenten voor het berekenen van een resultaat zullen worden gebruikt. Deze kunnen worden gevuld door statische tekst of getallen in te voeren, een veld vanuit het linkerdeelvenster te slepen (met de waarde van het veld in de berekening) of door een andere functie te slepen en neer te zetten (een geneste functie maken). Mogelijke functies zijn:

   | -functie | Beschrijving | Uitvoer |
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

1. Klik op de knop **Terug** om terug te keren naar uw tabel.
