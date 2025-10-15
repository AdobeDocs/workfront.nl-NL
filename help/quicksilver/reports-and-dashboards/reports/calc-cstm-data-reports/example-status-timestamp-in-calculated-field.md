---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Voorbeeld van een berekend aangepast veld: een statustijdstempel weergeven in een aangepast formulier'
description: In het volgende berekende veld wordt de datum weergegeven waarop de objectstatus wordt gemarkeerd als Bezig (INP). U kunt de zelfde informatie voor berekende douanevelden voor kwesties, taken, of projecten gebruiken.
author: Jenny
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Voorbeeld van een berekend aangepast veld: een statustijdstempel weergeven in een aangepast formulier

In het volgende berekende veld wordt de datum weergegeven waarop de objectstatus wordt gemarkeerd als Bezig (INP). U kunt de zelfde informatie voor berekende douanevelden voor kwesties, taken, of projecten gebruiken.

>[!NOTE]
>
>Als de status van het object verandert in INP, verandert deze in een andere status en vervolgens weer in INP, legt Adobe Workfront alleen de tijdstempel van de eerste wijziging vast in INP.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-pakket</p> </td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-licentie</p> </td> 
   <td>
      <p>Standard</p>
      <p>Plan</p></td>
  </tr> 
  <tr> 
   <td><p>Configuraties op toegangsniveau</p></td> 
   <td> <p>Toegang bewerken tot rapporten, dashboards en kalenders maken</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objectmachtigingen</p> </td> 
   <td> <p>Rechten beheren voor het object waaraan het formulier is gekoppeld</p></td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
