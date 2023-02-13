---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Het configureren van beïnvloeding wordt toegepast op uren dat een object wordt verwijderd en hersteld
description: U kunt vormen wat met uren gebeurt wanneer iemand een project, een taak, of een kwestie schrapt die de uren tegen worden geregistreerd. De optie die u kiest, bepaalt ook wat er met de uren gebeurt als het project, de taak of de uitgave op een later tijdstip wordt hersteld. (Zie Verwijderde items herstellen voor meer informatie over het herstellen van items in Workfront.)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Het configureren van beïnvloeding wordt toegepast op uren dat een object wordt verwijderd en hersteld

U kunt vormen wat met uren gebeurt wanneer iemand een project, een taak, of een kwestie schrapt die de uren tegen worden geregistreerd. De optie die u kiest, bepaalt ook wat er met de uren gebeurt als het project, de taak of de uitgave op een later tijdstip wordt hersteld. (Zie voor meer informatie over het herstellen van objecten in Workfront [Verwijderde items herstellen](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

## Toegangsvereisten

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
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configureer hoe uren worden beheerd wanneer een item wordt verwijderd en hersteld

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Uitbreiden **Timesheets en uren** en klik vervolgens op **Voorkeuren**.

1. Zoek de **Voorkeuren voor project-, taak- of probleemverwijdering** sectie.
1. (Voorwaardelijk) om te vormen hoe de uren worden beheerd wanneer een project wordt geschrapt, selecteer één van de volgende opties in **Bij het verwijderen van projecten** sectie:

   * De geregistreerde uren houden die reeds aan timesheets als algemene uren worden toegevoegd (als dit project op een recentere tijd wordt hersteld, blijven de uren op timesheet)\
      Deze optie is standaard ingeschakeld.
   * Schrap om het even welke geregistreerde uren (als dit project op een recentere tijd wordt hersteld, worden de geregistreerde uren hersteld aan het project)

1. (Voorwaardelijk) Om te vormen hoe de uren worden beheerd wanneer een taak of een kwestie wordt geschrapt, selecteer één van de volgende opties in **Bij het verwijderen van taken of problemen** sectie:

   * Verplaats om het even welke geregistreerde uren naar het project waar de taak of de kwestie verblijft (als deze taak of kwestie op een recentere tijd wordt hersteld, blijven de uren op het project)\
      Deze optie is standaard ingeschakeld.
   * Alle geregistreerde uren verwijderen (als deze taak of uitgave later wordt hersteld, worden de geregistreerde uren teruggezet naar de taak of uitgave)

1. Klikken **Opslaan**.
