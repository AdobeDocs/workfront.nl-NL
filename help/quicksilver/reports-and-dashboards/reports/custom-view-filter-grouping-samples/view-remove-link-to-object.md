---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: koppeling naar een object in een kolom verwijderen'
description: Sommige objecten die u in een weergave weergeeft, zijn standaard gekoppeld aan de pagina Details van het object. Bijvoorbeeld, is de kolom die de Naam van een project toont een verbinding aan het project; de kolom die de Naam van een gebruiker toont is een verbinding aan de de profielpagina van de gebruiker.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '411'
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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Voorbeeld: Verwijder de verbinding aan een taak uit de kolom van de Naam van de Taak in een taakmening:

1. Ga naar een takenlijst.
1. Van de **Weergave** vervolgkeuzelijst, klikt u op **Nieuwe weergave** om een nieuwe weergave te maken.

   of

   Klik op de knop **Pictogram Bewerken** ![](assets/edit-icon.png)

   als u een bestaande weergave wilt bewerken, selecteert u de weergave.

1. Klikken **Kolom toevoegen** om een nieuwe kolom toe te voegen.

   of

   Klik op een bestaande kolom met een koppeling naar een object.

1. Klikken **Overschakelen naar tekstmodus**.
1. Houd de cursor boven het gebied van de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:

   <pre>displayname=Task Name<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueformat=Compound</pre>

   >[!TIP]
   >
   >U kunt vergelijkbare code voor andere objecten gebruiken door het volgende aan te passen:
   >
   >   
   >   
   >   * Vervang de **taxiveld** regel van de code met **valueexpression** en zorg dat dezelfde naam tussen accolades na het gelijkteken staat.
   >   
   >   
   >
   >   
   >   
   >   * Alle regels die beginnen met > verwijderen

      >   
      >     ```>   
      >     link.
      >     ```   >   
      >   
      >     
      from the original text of the column. For example, eliminate all the following lines:
      >     <pre>link.linkproperty.0.name=ID</pre><pre>link.linkproperty.0.valuefield=ID</pre><pre>link.linkproperty.0.valueformat=string</pre><pre>link.lookup=link.view</pre><pre>link.value=val(objCode)</pre>
      >   
      >   
      >



1. Klikken **Opslaan** vervolgens **Weergave opslaan**.
