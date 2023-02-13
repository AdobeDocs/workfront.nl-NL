---
product-area: projects
navigation-topic: use-predecessors
title: Predecessors voor meerdere projecten maken
description: Een voorganger voor meerdere projecten is een taak waarvan een andere taak (een opvolgertaak genoemd) in een ander project afhankelijk is. De voorganger is de taak die voorrang heeft op de afhankelijke (opvolger)taak. Bijvoorbeeld, kunt u tot een gebiedsdeel leiden dat vereist dat de voorgangertaak wordt duidelijk Voltooid alvorens de afhankelijke taak kan beginnen.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Predecessors voor meerdere projecten maken

Een voorganger voor meerdere projecten is een taak waarvan een andere taak (een opvolgertaak genoemd) in een ander project afhankelijk is. De voorganger is de taak die voorrang heeft op de afhankelijke (opvolger)taak. Bijvoorbeeld, kunt u tot een gebiedsdeel leiden dat vereist dat de voorgangertaak wordt duidelijk Voltooid alvorens de afhankelijke taak kan beginnen.

Net als voorgangers binnen één project, staat Adobe Workfront toe dat taken afhankelijk zijn van taken in andere projecten.

**VOORBEELD**

Als een gravend bedrijf slechts één graafmachine heeft, en twee gezamenlijke projecten taken hebben die het gebruik van de graafmachine vereisen, kan de projectmanager de taak in het eerste project afhankelijk van de taak in het tweede project maken om te illustreren dat het graven kan beginnen wanneer het vorige project de graafmachine zal verlaten.
Wanneer het verbinden van projecten door dwars-project predecessors, zullen de data van het primaire project (die de voorgangertaak heeft) het secundaire project (die de opvolgertaak heeft) beïnvloeden.

>[!TIP]
>
>U moet chronologie voor de projecten opnieuw berekenen om data te zien die voor het secundaire project worden bijgewerkt. Zie voor meer informatie over het opnieuw berekenen van tijdlijnen [Tijdlijnherberekeningen voor projecten configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Voor meer informatie over vorige relaties raadpleegt u [Overzicht van voorgangers van taken](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Toegangsvereisten

<!--drafted - replace table for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Toegang tot taken en projecten bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor de taken en projecten beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Een voorganger voor meerdere projecten maken

1. Ga naar de taak die uw opvolger zal zijn.
1. Klikken **Predecessors** in het linkerdeelvenster.
1. Klikken **Voorganger toevoegen.**
1. In de **Bovenliggend project** veld, typt u de naam van het project dat de taak bevat die u afhankelijk wilt maken van uw huidige taak.
1. Klik op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.
1. In de **Taken** veld, typt u de naam van de taak die u afhankelijk wilt maken van de huidige taak.
1. Geef de volgende informatie op voor het definiëren van de relatie tussen de voorganger en de afhankelijke taak:

   * **Type afhankelijkheid:** Selecteer de verhouding die u de taak met de afhankelijke taak wilt hebben. De standaardverhouding is &quot;eind-Begin,&quot;betekenend dat de voorgangerstaak moet beëindigen alvorens de afhankelijke taak kan beginnen. Voor meer informatie over de diverse gebiedstypes, zie [Overzicht van typen taakafhankelijkheid](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)

   * **Lag:** Geef de hoeveelheid tijd op die moet verstrijken na de voltooiing van een afgedwongen voorganger totdat de afhankelijke taak kan beginnen. Voor meer informatie over de verschillende soorten vertraging raadpleegt u [Overzicht van labeltypen](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **Afgedwongen:** Wanneer deze optie wordt geselecteerd, kan het gebiedsverband tussen de twee taken niet worden omzeild door gebruikers die taken beginnen vroeg. Bijvoorbeeld, als u een verband tussen Taak A en Taak B afdwingt, kan de Taak B niet worden begonnen tot Taak A volledig is. Voor meer informatie over het afdwingen van predecessors raadpleegt u [Voorgangers afdwingen](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

      Als deze optie niet is geselecteerd, wordt de afhankelijkheid behandeld als een suggestie voor gebruikers. Bijvoorbeeld, kunnen de gebruikers Taak B beginnen alvorens Taak A volledig is.

1. Klikken **Opslaan**.

   De taken die een dwars-projectvoorganger hebben tonen het verwijzingsaantal van het project predecessor tot en het aantal van de taak behoort, die door een dubbelpunt in de kolom van Predecessors op een taaklijst wordt gescheiden.

   ![Predecessor met meerdere projecten](assets/cross-project-predecessor-in-list-view.png)

   Het voorgangspictogram wordt groen als de voorganger de markering Voltooid heeft. Dit wijst erop dat de afhankelijke taak klaar voor het werk is.

   Houd de muisaanwijzer boven deze waarde voor meer informatie over de voorganger, het project en de datums. Klik op de voorganger voor meerdere projecten in het vak Details om de taak te openen. Klikken **Zie Project** het project te openen.

   ![Details voorganger van meerdere projecten](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   De **Zie Project** Deze optie wordt alleen weergegeven wanneer u een voorganger voor meerdere projecten weergeeft.

