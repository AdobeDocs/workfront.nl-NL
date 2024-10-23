---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Voorbeeld van berekend aangepast veld: een tijdstempel voor status weergeven in een aangepast formulier'
description: In het volgende berekende veld wordt de datum weergegeven waarop de objectstatus wordt gemarkeerd als Bezig (INP.) U kunt de zelfde informatie voor berekende douanevelden voor kwesties, taken, of projecten gebruiken.
author: Nolan
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# Voorbeeld van een berekend aangepast veld: een statustijdstempel weergeven in een aangepast formulier

In het volgende berekende veld wordt de datum weergegeven waarop de objectstatus wordt gemarkeerd als Bezig (INP.) U kunt de zelfde informatie voor berekende douanevelden voor kwesties, taken, of projecten gebruiken.

>[!NOTE]
>
>Als de status van het object verandert in INP, verandert deze in een andere status en vervolgens weer in INP, legt Adobe Workfront alleen de tijdstempel van de eerste wijziging vast in INP.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-abonnement*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-licentie*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td><strong> het niveauconfiguraties van de Toegang* </strong> </td> 
   <td> <p>Toegang bewerken tot rapporten, dashboards en kalenders maken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> de toestemmingen van Objecten </strong> </p> </td> 
   <td> <p>Rechten beheren voor het object waaraan het formulier is gekoppeld</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.<br> voor meer informatie over toestemmingen voor dashboards, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref"> de rapporten van het Aandeel, dashboards, en kalenders </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Vereiste

Als u een berekend veld met de bewerkingsgeschiedenis van een veld wilt toevoegen aan een aangepast formulier, moet u eerst het aangepaste formulier maken.

## Een statustijdstempel weergeven in een aangepast formulier

1. Ga naar een aangepast formulier waaraan u het veld wilt toevoegen.
1. Klik **Berekend** om een berekend douanegebied aan de vorm toe te voegen.
1. Typ a **Etiket** voor het douanegebied. Bijvoorbeeld &#39;Aangepast veld voor tijdstempel van status&#39;.
1. Klik **sparen+Sluiten**.
1. Heropen de douanevorm, dan selecteer het nieuwe **Gebied van de Tijdstempel van de Status Tijdstempel van de Status** op de vorm.
1. In het **vakje van de Berekening**, kopieer en kleef de volgende berekening voor uw douanegebied:

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >Deze berekening is identiek voor alle objecten en voor alle statussen. U moet altijd de drie-letterige sleutel gebruiken, en niet de statusnaam voor de objecten status in deze berekening.
   >
   >Voor meer informatie over de sleutels voor Statussen, zie [ een status ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) creëren of uitgeven.

1. Klik **sparen+Sluiten**.

   U kunt nu rapporteren over het veld Aangepast tijdstempel voor status of dit gebruiken in andere berekeningen, rapporten of aangepaste velden.
