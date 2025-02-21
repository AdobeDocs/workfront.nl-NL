---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: Koppeling naar een object in een kolom verwijderen'
description: Sommige objecten die u in een weergave weergeeft, zijn standaard gekoppeld aan de pagina Details van het object. Bijvoorbeeld, is de kolom die de Naam van een project toont een verbinding aan het project; de kolom die de Naam van een gebruiker toont is een verbinding aan de de profielpagina van de gebruiker.
author: Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# Weergave: koppeling naar een object in een kolom verwijderen

<!--Audited: 11/2024-->

Sommige objecten die u in een weergave weergeeft, zijn standaard gekoppeld aan de pagina Details van het object. Bijvoorbeeld, is de kolom die de Naam van een project toont een verbinding aan het project; de kolom die de Naam van een gebruiker toont is een verbinding aan de de profielpagina van de gebruiker.

U kunt deze koppeling verwijderen met de tekstmodus in kolommen die in alle weergaven worden weergegeven.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

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
   <td> <p> Huidige: 
   <ul>
   <li>Verzoek om een weergave te wijzigen</li> 
   <li>Plan om een rapport te wijzigen</li>
   </ul>
     </p>
     <p> Nieuw: 
   <ul>
   <li>Medewerker om een weergave te wijzigen</li> 
   <li>Standaard voor het wijzigen van een rapport</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Voorbeeld: verwijder de verbinding aan een taak uit de kolom van de Naam van de Taak in een taakmening:

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Mening**, klik **Nieuwe Mening** om een nieuwe mening tot stand te brengen.

   of

   Klik het **uitgeven pictogram** ![ uitgeven pictogram ](assets/edit-icon.png)

   als u een bestaande weergave wilt bewerken, selecteert u de weergave.

1. Klik **toevoegen Kolom** om een nieuwe kolom toe te voegen.

   of

   Klik op een bestaande kolom met een koppeling naar een object.

1. Klik **Schakelaar aan de Wijze van de Tekst** > **uitgeven de Wijze van de Tekst**.
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
   >* Vervang de regel `valuefield` van de code door `valueexpression` en zorg dat dezelfde naam tussen accolades na het gelijkteken staat.
   >* Verwijder alle regels die beginnen met `link.` uit de oorspronkelijke tekst van de kolom. Verwijder bijvoorbeeld alle volgende regels:
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

