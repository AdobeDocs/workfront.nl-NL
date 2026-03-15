---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergeven: Koppeling naar een object in een kolom verwijderen'
description: Sommige objecten die u in een weergave weergeeft, zijn standaard gekoppeld aan de pagina Details van het object. De kolom die bijvoorbeeld de naam van een project weergeeft, is een koppeling naar het project. De kolom die de naam van een gebruiker weergeeft, is een koppeling naar de profielpagina van de gebruiker.
author: Courtney
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---

# Weergeven: koppeling naar een object in een kolom verwijderen

<!--Audited: 11/2024-->

Sommige objecten die u in een weergave weergeeft, zijn standaard gekoppeld aan de pagina Details van het object. De kolom die bijvoorbeeld de naam van een project weergeeft, is een koppeling naar het project. De kolom die de naam van een gebruiker weergeeft, is een koppeling naar de profielpagina van de gebruiker.

U kunt deze koppeling verwijderen met de tekstmodus in kolommen die in alle weergaven worden weergegeven.

## Toegangsvereisten

+++ Vouw uit om de toegangsvereisten voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Bijdrager of verzoek om een weergave te wijzigen </p>
   <p>Standaard of Plan om een rapport te wijzigen</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards en kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen voor een rapport beheren</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++


## Voorbeeld: verwijder de koppeling naar een taak uit de kolom Taaknaam in een taakweergave:

1. Ga naar een lijst met taken.
1. Van het **drop-down menu van de Mening**, klik **Nieuwe Mening** om een nieuwe mening tot stand te brengen.

   Of

   Klik het **uitgeven pictogram** ![ pictogram ](assets/edit-icon.png) uitgeven om een bestaande mening uit te geven, dan de mening te selecteren.

1. Klik **voeg Kolom** toe om een nieuwe kolom toe te voegen.

   Of

   Klik op een bestaande kolom met een koppeling naar een object.

1. Klik **Schakelaar aan de Wijze van de Tekst** > **geef de Wijze van de Tekst** uit.
1. Verwijder de tekst u in **vindt geef de Wijze van de Tekst** vakje uit, en vervang het met de volgende code:

   ```
   displayname=Task Name
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression={name}
   valueformat=Compound
   ```

   >[!TIP]
   >
   >U kunt vergelijkbare code voor andere objecten gebruiken door het volgende aan te passen:
   >
   >* Vervang de `valuefield` -regel van de code door `valueexpression` en zorg dat dezelfde naam tussen accolades na het gelijkteken staat.
   >* Verwijder alle regels die met `link.` beginnen uit de oorspronkelijke tekst van de kolom. Verwijder bijvoorbeeld alle volgende regels:
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. Klik **Gedaan**, dan **sparen Mening**.

