---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: de inhoud van een kolom verbergen'
description: U kunt informatie in de kolom van een mening willen verbergen. U kunt dit doen door de tekstwijze van de kolom te wijzigen.
author: Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Weergave: de inhoud van een kolom verbergen

<!--Audited: 11/2024-->

U kunt informatie in de kolom van een mening willen verbergen. U kunt dit doen door de tekstwijze van de kolom te wijzigen.

>[!NOTE]
>
>* U kunt verborgen kolommen gebruiken om te sorteren op een bepaald object dat u niet wilt weergeven in de weergave.\
>  U kunt bijvoorbeeld sorteren op Taaknummer in een taakweergave en de gegevens van Taaknummer verbergen in de weergave. In dit geval helpt het object waarnaar in de kolom wordt verwezen, de weergave te sorteren, maar wordt de informatie van dat object niet weergegeven in de weergave.
>* Als u een kolom verbergt, ziet u dat de informatie in de kolom verborgen is, maar dat de kolom nog steeds in de weergave voorkomt.
>

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
   <td> <p>Nieuw:<ul><li>Medewerker om een weergave te wijzigen</li><li>Standaard voor het wijzigen van een rapport</li></ul></p><p>of</p>Huidige:<ul><li>Verzoek om een weergave te wijzigen</li><li>Plan om een rapport te wijzigen</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
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

## Voorbeeld: U kunt de kolom Taaknummer in een taakweergave sorteren en verbergen:

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Mening**, klik **Nieuwe Mening**.

1. Klik **toevoegen Kolom** en beginnen &quot;Aantal van de Taak&quot;in **tonen in dit kolom** gebied dan selecteren het wanneer het in de lijst toont.

1. Klik **Schakelaar aan de Wijze van de Tekst**, dan **geef Tekst** uit.
1. Verwijder de tekst u in **vindt geef de Wijze van de Tekst** vakje uit, en vervang het met de volgende code:

   ```
   displayname=
   linkedname=direct
   querysort=taskNumber
   sortOrder=1
   sortType=asc
   textmode=true
   value=
   valueformat=int
   width=0
   ```

   De belangrijkste wijzigingen in deze code waardoor de kolom verborgen wordt, zijn:

   * `displayname=`: deze regel moet leeg zijn.
   * `valuefield=`: deze is vervangen door `value` en moet leeg zijn.
   * `width=`: Afhankelijk van het gebied, moet dit een waarde van **0** of **1** hebben.

1. Klik **Gedaan**, dan **sparen Mening**.
