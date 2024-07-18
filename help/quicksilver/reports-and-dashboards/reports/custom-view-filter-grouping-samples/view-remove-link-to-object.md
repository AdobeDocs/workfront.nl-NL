---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: koppeling naar een object in een kolom verwijderen'
description: Sommige objecten die u in een weergave weergeeft, zijn standaard gekoppeld aan de pagina Details van het object. Bijvoorbeeld, is de kolom die de Naam van een project toont een verbinding aan het project; de kolom die de Naam van een gebruiker toont is een verbinding aan de de profielpagina van de gebruiker.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 5480d6b5e97c4c2e21080bb92ffe255f60ed6f60
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# Weergave: koppeling naar een object in een kolom verwijderen

Sommige objecten die u in een weergave weergeeft, zijn standaard gekoppeld aan de pagina Details van het object. Bijvoorbeeld, is de kolom die de Naam van een project toont een verbinding aan het project; de kolom die de Naam van een gebruiker toont is een verbinding aan de de profielpagina van de gebruiker.

U kunt deze koppeling verwijderen met de tekstmodus in kolommen die in alle weergaven worden weergegeven.

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
   <td> <p>Verzoek om een weergave te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Voorbeeld: verwijder de verbinding aan een taak uit de kolom van de Naam van de Taak in een taakmening:

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Mening**, klik **Nieuwe Mening** om een nieuwe mening tot stand te brengen.

   of

   Klik het **uitgeven pictogram** ![](assets/edit-icon.png)

   als u een bestaande weergave wilt bewerken, selecteert u de weergave.

1. Klik **toevoegen Kolom** om een nieuwe kolom toe te voegen.

   of

   Klik op een bestaande kolom met een koppeling naar een object.

1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. Beweeg over het gebied van de tekstwijze, en klik **Klik om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:
   <pre>displayname=Task Naam <br> linkedname=direct <br> namekey=name <br> querysort=name <br> textmode=true <br><strong> valueexpression= {name} </strong><br> valueformat=Compound</pre>

   >[!TIP]
   >
   >U kunt vergelijkbare code voor andere objecten gebruiken door het volgende aan te passen:
   >
   >* Vervang de **lijn van het waardegebied 0} {van de code met** waardeuitdrukking **en houd de zelfde naam inbegrepen in krullende steunen na het gelijke teken.**
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

1. Klik **sparen**, dan **sparen Mening**.
