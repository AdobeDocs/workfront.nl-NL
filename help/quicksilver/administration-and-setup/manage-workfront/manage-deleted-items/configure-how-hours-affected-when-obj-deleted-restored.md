---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Effect op uren configureren wanneer een object wordt verwijderd en hersteld
description: U kunt vormen wat met uren gebeurt wanneer iemand een project, een taak, of een kwestie schrapt die de uren tegen worden geregistreerd. De optie die u kiest, bepaalt ook wat er met de uren gebeurt als het project, de taak of de uitgave op een later tijdstip wordt hersteld. (Zie Verwijderde items herstellen voor meer informatie over het herstellen van items in Workfront.)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Effect configureren op uren dat een object wordt verwijderd en hersteld

U kunt vormen wat met uren gebeurt wanneer iemand een project, een taak, of een kwestie schrapt die de uren tegen worden geregistreerd. De optie die u kiest, bepaalt ook wat er met de uren gebeurt als het project, de taak of de uitgave op een later tijdstip wordt hersteld. (Voor meer informatie over het herstellen van punten in Workfront, zie [ geschrapte punten ](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md) herstellen.)

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configureer hoe uren worden beheerd wanneer een item wordt verwijderd en hersteld

{{step-1-to-setup}}

1. Breid **Tijdopnamen &amp; Uren** uit, dan klik **Voorkeur**.

1. Bepaal de plaats van het **Project, de Taak of de sectie van de Schrapping van de Uitgave van de Voorkeur**.
1. (Voorwaardelijk) om te vormen hoe de uren worden beheerd wanneer een project wordt geschrapt, selecteer één van de volgende opties in **wanneer het schrappen van projecten** sectie:

   * De geregistreerde uren houden die reeds aan timesheets als algemene uren worden toegevoegd (als dit project op een recentere tijd wordt hersteld, blijven de uren op timesheet)\
     Deze optie is standaard ingeschakeld.
   * Schrap om het even welke geregistreerde uren (als dit project op een recentere tijd wordt hersteld, worden de geregistreerde uren hersteld aan het project)

1. (Voorwaardelijk) om te vormen hoe de uren worden beheerd wanneer een taak of een kwestie wordt geschrapt, selecteer één van de volgende opties in **wanneer het schrappen van taken of kwesties** sectie:

   * Verplaats om het even welke geregistreerde uren naar het project waar de taak of de kwestie verblijft (als deze taak of kwestie op een recentere tijd wordt hersteld, blijven de uren op het project)\
     Deze optie is standaard ingeschakeld.
   * Alle geregistreerde uren verwijderen (als deze taak of uitgave later wordt hersteld, worden de geregistreerde uren teruggezet naar de taak of uitgave)

1. Klik **sparen**.
