---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Weergave: weergaveobjecten die niet zijn opgenomen in de standaardinterface"'
description: U kunt objecten weergeven die niet in de standaardmodusinterface zijn opgenomen. U kunt dit alleen doen door ernaar te verwijzen via de tekstmodus. U kunt op de volgende manieren bepalen welke velden in een weergave kunnen worden opgenomen - BEWERK ME.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Weergave: weergaveobjecten die niet zijn opgenomen in de standaardinterface

U kunt objecten weergeven die niet in de standaardmodusinterface zijn opgenomen. U kunt dit alleen doen door ernaar te verwijzen via de tekstmodus.\
U kunt op de volgende manieren bepalen welke velden in een weergave kunnen worden opgenomen:

* Gebruik de [API Explorer](../../../wf-api/general/api-explorer.md) om andere objecten te zoeken waarnaar in de tekstmodus kan worden verwezen.\
   Niet alle velden die in de API Explorer worden beschreven, zijn geldige velden voor de tekstmodus. Sommige velden worden alleen gemeld via de API.

* Zoek het veld Id van het object in een kolom. De meeste objecten met een veld-id hebben ook een corresponderende kolom- of veldnaam die niet toegankelijk is via de standaardmodusinterface.

   U kunt de tekstmodus gebruiken om in een weergave de kolom- of veldnaam op te nemen in plaats van de id door de naam `fieldnameID` met de `fieldname:name`.

   In de standaardmodus kunt u bijvoorbeeld de opdracht **Portfolio-eigenaar-id** is beschikbaar voor een projectweergave, maar de **Naam Portfolio-eigenaar** niet. U kunt de tekstmodus gebruiken om de **Naam Portfolio-eigenaar** in de kolom van een weergave.

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

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Voorbeeld: Voeg de kolom Naam eigenaar Portfolio toe aan een projectweergave

1. Ga naar een lijst met projecten.
1. Van de **Weergave** vervolgkeuzelijst, klikt u op **Nieuwe weergave**.

1. Klikken **Kolom toevoegen** typ vervolgens &quot;Portfolio Eigenaar-id&quot; in het dialoogvenster **Tonen in deze kolom** en selecteert u deze wanneer deze in de lijst wordt weergegeven.

1. Klikken **Overschakelen naar tekstmodus**.
1. Houd de cursor boven het gebied van de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Vervang de `valuefield` line (`valuefield=portfolio:ownerID`) met de volgende regel:

   ```
   valuefield=portfolio:owner:name
   ```

   of

   Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   In dit specifieke voorbeeld wordt het rapport gesorteerd op de Portfolio Eigenaar-id, zoals aangegeven door de `querysort` lijn.

   >[!TIP]
   >
   >Een veld vervangen `ID` met het veld `name` in tekstmodus gebruiken, altijd vervangen `ID` with `:name` in de `valuefield` lijn.

1. Klikken **Opslaan** vervolgens **Weergave opslaan**.
