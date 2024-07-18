---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groeperen: lijstresultaten ordenen met een berekende waarde die hetzelfde is voor alle objecten in de groep'
description: U zou uw taken kunnen willen bekijken die door Percentage wordt gegroepeerd Voltooien in waaiers van 0-25, 26-50, 51-75, 75-99, en 100. Hiervoor kunt u een groepering maken in de tekstmodus.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 93b743ce-7e54-4a96-933b-912e2107a84f
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---

# Groeperen: lijstresultaten ordenen met een berekende waarde die hetzelfde is voor alle objecten in de groep

U zou uw taken kunnen willen bekijken die door Percentage wordt gegroepeerd Voltooien in waaiers van 0-25, 26-50, 51-75, 75-99, en 100. Hiervoor kunt u een groepering maken in de tekstmodus.

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
   <td> <p>Verzoek om een groepering te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een groep te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## De lijstresultaten organiseren met een berekende waarde die voor alle voorwerpen in de groepering gemeenschappelijk is

Deze groepering toepassen op een lijst met taken:

1. Ga naar een takenlijst.
1. Van **het Groeperen** drop-down menu, uitgezochte **Nieuwe Groepering**.

1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. Voeg de volgende code toe in de beschikbare ruimte:

   ```
   textmode=true<br>group.0.valueexpression=IF({percentComplete}>=0&&{percentComplete}<=25,'0-25%',IF({
   ```

   ```
   percentComplete
   ```

   ```
   }>25&&{percentComplete}<=50,'26-50%',IF({percentComplete}>50&&{percentComplete}<=75,'51-75%',IF({percentComplete}>75&&{percentComplete}<=100,'76-100%',''))))<br>group.0.linkedname=direct<br>group.0.valueformat=doubleAsString<br>group.0.namekey=percentComplete
   ```

1. Klik **Gedaan**, dan **sparen Groepering**.
