---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: weergaveobjecten die niet zijn opgenomen in de standaardinterface'
description: U kunt objecten weergeven die niet in de standaardmodusinterface zijn opgenomen. U kunt dit alleen doen door ernaar te verwijzen via de tekstmodus.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Weergave: weergaveobjecten die niet zijn opgenomen in de standaardinterface

U kunt objecten weergeven die niet in de standaardmodusinterface zijn opgenomen. U kunt dit alleen doen door ernaar te verwijzen via de tekstmodus.\
U kunt op de volgende manieren bepalen welke velden in een weergave kunnen worden opgenomen:

* Gebruik [ API Ontdekkingsreiziger ](../../../wf-api/general/api-explorer.md) om andere voorwerpen te ontdekken die via tekstwijze kunnen worden van verwijzingen voorzien.\
  Niet alle velden die in de API Explorer worden beschreven, zijn geldige velden voor de tekstmodus. Sommige velden worden alleen gemeld via de API.

* Zoek het veld Id van het object in een kolom. De meeste objecten met een veld-id hebben ook een corresponderende kolom- of veldnaam die niet toegankelijk is via de standaardmodus.

  U kunt de tekstmodus gebruiken om de kolom- of veldnaam op te nemen in een weergave in plaats van de id door de `fieldnameID` te vervangen door de `fieldname:name` .

  Bijvoorbeeld, op de standaardwijzeinterface, is het **gebied van identiteitskaart van de Eigenaar van 0} Portfolio beschikbaar voor een projectweergave, maar het** gebied van de Naam van de Eigenaar van de Portfolio **is niet.** U kunt tekstwijze gebruiken om de **Naam van de Eigenaar van het Portfolio** in de kolom van een mening te tonen.

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

## Voorbeeld: voeg de kolom Naam eigenaar Portfolio toe aan een projectweergave

1. Ga naar een lijst met projecten.
1. Van het **drop-down menu van de Mening**, klik **Nieuwe Mening**.

1. Klik **toevoegen Kolom** dan begin &quot;identiteitskaart van de Eigenaar van het Portfolio&quot;in **tonen in dit kolom** gebied, dan selecteren het wanneer het in de lijst toont.

1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. Beweeg over het gebied van de tekstwijze, en klik **Klik om tekst** uit te geven.
1. Vervang de regel `valuefield` (`valuefield=portfolio:ownerID`) door de volgende regel:

   ```
   valuefield=portfolio:owner:name
   ```

   of

   Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   In dit specifieke voorbeeld wordt het rapport gesorteerd op de Portfolio Eigenaar-id, zoals aangegeven door de regel `querysort` .

   >[!TIP]
   >
   >Als u een veld `ID` met de tekstmodus `name` wilt vervangen, vervangt u `ID` altijd door `:name` in de `valuefield` -regel.

1. Klik **sparen**, dan **sparen Mening**.
