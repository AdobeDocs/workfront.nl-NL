---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Het percentage gebruikers- of roltoewijzingen beheren voor taken
description: Het percentage van de toewijzing vertegenwoordigt de hoeveelheid tijd een toegewezen middel wordt gepland om aan een taak in een dag te werken. Het is het percentage van een het werkdag (volgens het gebruikers of projectprogramma) waarbij een middel door de duur van de taak wordt toegewezen.
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: ad5d6bfda24119076df8336ed291c0ba63e2c88a
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# Het percentage gebruikers- of roltoewijzingen beheren voor taken

{{highlighted-preview}}

Het percentage van de toewijzing vertegenwoordigt de hoeveelheid tijd een toegewezen middel wordt gepland om aan een taak in een dag te werken. Het is het percentage van een het werkdag (volgens het gebruikers of projectprogramma) waarbij een middel door de duur van de taak wordt toegewezen.

>[!NOTE]
>
>Wanneer gebruikers aan het werk worden toegewezen, heeft hun beschikbaarheid volgens hun programma&#39;s invloed op de geplande en verwachte datum van taken en problemen. Voor informatie over programma&#39;s, zie [Een schema maken](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

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
   <td> <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot taken bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute of hoger machtigingen voor de taak</p> <p>Machtigingen bewerken om het toewijzingspercentage bij te werken in het vak Taak bewerken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Overwegingen bij het wijzigen van percentagetoewijzingen voor taken

* De gebruikers worden toegewezen een gelijk percentage van tijd aan taken zij worden toegewezen, door gebrek.
* U kunt het toewijzingspercentage voor gebruikers en baanrollen manueel wijzigen die aan taken slechts worden toegewezen wanneer het Type van Duur van de taak Berekend Werk of Gedreven Inspanning is.

  Zie voor meer informatie [Overzicht van het Type van Duur en van de Duur van de Taak](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* U kunt niet de percententoewijzing voor teams wijzigen die aan taken worden toegewezen.
* U kunt niet de percentaletoewijzing voor gebruikers en baanrollen wijzigen die aan kwesties worden toegewezen.

## Wijzig de gebruiker of rolpercenten toewijzing voor een taak

1. Ga naar een taak waarvoor de middelen u de percententoewijzing veranderen.
1. Klik op de knop **Meer** menu ![](assets/qs-more-icon-on-an-object.png) naast de naam van de taak klikt u op **Bewerken**.

   of

   Klik op de knop **Toewijzingen** gebied in de taakkopbal, dan klik **Geavanceerd**.

1. Zorg ervoor dat de **Duur** van de taak is één van de volgende:

   * Berekend werk
   * Inzet gedreven

   >[!TIP]
   >
   >* Voor het berekende Type Duur van Toewijzing gebruikt Workfront de volgende formule om het toewijzingspercentage van elke toegewezen persoon te berekenen: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Voor het Eenvoudige Type van Duur, kunt u de uren schatten die aan elk middel worden toegewezen, niet het toewijzingspercentage.

1. Klikken **Toewijzingen** en wijzigt u vervolgens de **Toewijzingen** voor elke aan te wijzen taak.

   U kunt het toewijzingspercentage voor gebruikers en taakroltoewijzingen alleen wijzigen.

   U kunt niet het toewijzingspercentage voor een team wijzigen dat aan een taak wordt toegewezen.

   Voorbeeldafbeelding in de productieomgeving:
   ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

   <span class="preview">Voorbeeldafbeelding in de voorvertoningsomgeving:</span>
   ![Toewijzingspercentage wijzigen](assets/advanced-assignments-allocation-percentage.png)

1. Klikken **Opslaan**.
