---
title: Alle rapporten weergeven die een bepaald aangepast veld of een bepaalde widget gebruiken
description: U kunt een aangepaste weergave toevoegen in het gebied Aangepaste Forms, waarin wordt aangegeven welke rapporten een bepaald aangepast veld of een bepaalde widget gebruiken. Dit is handig wanneer u het veld of de widget moet bewerken of verwijderen, omdat deze mogelijk al in een of meer rapporten is geïmplementeerd. Het is belangrijk om te beoordelen of die rapporten aanpassingen zullen nodig hebben om behoorlijk te blijven werken.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 0%

---

# Alle rapporten weergeven die een bepaald aangepast veld of een bepaalde widget gebruiken

U kunt een aangepaste weergave toevoegen in het gebied Aangepaste Forms, waarin wordt aangegeven welke rapporten een bepaald aangepast veld of een bepaalde widget gebruiken. Dit is handig wanneer u het veld of de widget moet bewerken of verwijderen, omdat deze mogelijk al in een of meer rapporten is geïmplementeerd. Het is belangrijk om te beoordelen of die rapporten aanpassingen zullen nodig hebben om behoorlijk te blijven werken.

Voor informatie over douanegebieden en widgets in douanevormen, zie [ Ontwerp een vorm met de vormontwerper ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-plan</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
   <p>Nieuw: Standaard</p>
   <p>of</p>
   <p>Huidig: Plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Een lijst weergeven van de rapporten die een bepaald aangepast veld of een bepaalde aangepaste widget gebruiken

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Aangepaste Forms**.
1. Klik **Gebieden** om een rapport te tonen dat van alle douanegebieden en widgets in uw instantie van Workfront een lijst maakt.

1. Klik het **menu van de Mening**, dan controle voor om het even welke douanemeningen in de lijst die de **kolom van Rapporten** omvatten (die geen standaardkolom op dit lusje is).

   In de kolom Rapporten kunt u zien welke rapporten elk aangepast veld en elke aangepaste widget gebruiken die aan een aangepast formulier in uw systeem is toegevoegd. Het is mogelijk dat iemand reeds een mening heeft gecreeerd die de **kolom van Rapporten** omvat.

1. Als u geen mening ziet die de **kolom van Rapporten** omvat, creeer een nieuwe mening die het omvat:

   1. Klik het **menu van de Mening**, dan klik **Nieuwe Mening**.

   1. Op de **Nieuwe pagina van de Mening** die, in de doos dichtbij de upper-left hoek verschijnt, vervang **Nieuwe Mening van de Parameter** met een beschrijvende naam voor de mening, zoals *Gebieden en widgets*.

   1. Klik **toevoegen Kolom** dichtbij de laag-juiste hoek.
   1. In **toon in deze kolom** doos die dichtbij de upper-left hoek toont, begin *rapport* te typen, dan uitgezochte **Rapporten** wanneer het in de lijst onder de doos verschijnt.

   1. (Voorwaardelijk) als u de **kolom wilt bewegen van Rapporten** u enkel aan een verschillende horizontale positie toevoegde, versleep zijn kopbal in het **gebied van de Voorproef van de Kolom** bij de bodem van de pagina.

   1. Klik **Gedaan**, dan klik **sparen Mening**.

1. Klik het **drop-down menu van de Mening**, dan selecteer de naam van de douanemening u enkel creeerde.
1. In de **kolom van de Naam**, vind het douanegebied of widget u van plan bent uit te geven of te schrappen, dan bekijk de **kolom van Rapporten** op die rij om te zien welke rapporten het gebruiken, als om het even welk.

   Workfront zoekt naar de aangepaste velden en widgets in alle rapportfilters, weergaven en groepen om de informatie voor deze kolom te zoeken.

   Als u een plusteken ziet, kunt u op die tekstregel klikken om een vak weer te geven met alle extra rapporten die het veld of de widget gebruiken.

   >[!NOTE]
   >
   >De eerste laadtijd voor dit gereedschap kan van 10 seconden tot 2,5 minuten duren, afhankelijk van de hoeveelheid gegevens in uw systeem.

   >[!TIP]
   >
   >Als u geen tijd hebt om de rapporten te onderzoeken die het douanegebied of widget gebruiken, kunt u de Uitvoer klikken om een dossier tot stand te brengen dat hen een lijst maakt. U zou dit dossier met iedereen kunnen delen die een rapport bezit dat het gebied of widget gebruikt en de verandering bespreken die moet gebeuren, de invloed het op het rapport zou kunnen hebben, en wat moet worden gedaan om ervoor te zorgen dat het rapport correct blijft werken.
   >
   >Deze mening is ook beschikbaar in een rapport van de Parameter:
   >      
   > 1. In het Belangrijkste Menu, klik **Rapporten**.
   > 1. Bij de upper-left hoek, klik **Nieuw Rapport**, dan klik **Parameter** in de lijst die toont.
   > 1. Klik **toevoegen Kolom** dichtbij de laag-juiste hoek.
   > 1. In **toon in deze kolom** doos die dichtbij de upper-left hoek toont, begin *rapport* te typen, dan uitgezochte **Rapporten** wanneer het in de lijst onder de doos verschijnt.
   > 1. (Voorwaardelijk) als u de **kolom wilt bewegen van Rapporten** u enkel aan een verschillende horizontale positie toevoegde, versleep zijn kopbal in het **gebied van de Voorproef van de Kolom** bij de bodem van de pagina.
   > 1. Klik **Gedaan**, dan klik **sparen+Sluiten**.
   > 1. Typ een beschrijvende naam voor het rapport, zoals *Gebieden en widgets*.
