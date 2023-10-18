---
product-area: projects
navigation-topic: update-work-in-a-project
title: Percentage van voltooiing weergeven en bijwerken voor taken
description: U kunt het percentage van voltooiing van een taak bijwerken om de vooruitgang aan te geven die u op de taak hebt gemaakt om het te voltooien.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Percentage van voltooiing weergeven en bijwerken voor taken

U kunt het percentage van voltooiing van een taak bijwerken om de vooruitgang aan te geven die u op de taak hebt gemaakt om het te voltooien.

## Toegangsvereisten

<!--drafted for P&P:

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
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

U moet de volgende toegang hebben om taken handmatig bij te werken:

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
   <td> <p>Toegang tot taken bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor de taak beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.


## Gebieden waar u het percentage van voltooiing van een taak kunt bijwerken

U kunt het voltooide percentage voor een taak op een van de volgende gebieden bijwerken:

* **In een takenlijst**: U kunt het voltooide percentage van een taak bijwerken wanneer de kolom Percentage voltooid wordt weergegeven.\
  Zie voor meer informatie over inline bewerken [Items inline bewerken in een lijst in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **In de milestone-weergave**: U kunt het percentage bijwerken voltooide van een taak wanneer het gebruiken van de mening van de Mijlpaal op een projectlijst of een projectrapport. Zie voor meer informatie [De milestone-weergave gebruiken](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **Terwijl u de taak bijwerkt**: U kunt de optie voor het percentage van een taak bijwerken wanneer u een update aan de taak toevoegt.

  >[!IMPORTANT]
  >
  >Deze optie wordt alleen weergegeven nadat u de optie Percentage tonen hebt ingeschakeld.\
  >Ga als volgt te werk om het percentage van de volledige updatebalk voor taken in te schakelen:
  >
  >1. Ga naar de **Hoofd** menu>uw naam>**Meer** pictogram naast uw naam >**Bewerken** > selecteren **Percentage volledig tonen bij updatestatus**.\
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >

* **In de taakkoptekst**: U kunt het percentage van een taak bijwerken in de taakkoptekst. Zie voor meer informatie [Taken bewerken](../../tasks/manage-tasks/edit-tasks.md).

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)


## Overwegingen bij het bijwerken van het percentage voltooide taken

* Wanneer u een taak markeert als 100% voltooid, wordt de taakstatus bijgewerkt naar Voltooid.
* De volgende scenario&#39;s bestaan voor oudertaken:
   * U kunt niet het percentage bijwerken volledig van een oudertaak aan 100% wanneer de Summiere Wijze van de Voltooiing van het project aan Automatisch wordt geplaatst en de subtaken niet worden voltooid.
   * U kunt het percentage volledig van een oudertaak aan 100% bijwerken wanneer de Summiere Wijze van de Voltooiing van het project aan Handboek wordt geplaatst en subtaken worden voltooid of onvolledig.

  Zie voor meer informatie [Projecten bewerken](../manage-projects/edit-projects.md).

## Het percentage van een taak bijwerken

1. Ga naar een van de volgende gebieden in Workfront:

   * Een takenlijst
   * Een lijst met projecten en past de Mijlpaal-weergave toe
   * Een taak, door tot de taakpagina toegang te hebben
1. Zoek de **Percentage voltooid** veld voor de taak waarvan het percentage is voltooid dat u wilt bijwerken.
1. Klik in het veld Percentage voltooid en typ een getal tussen 0 en 100

   of

   Klik en sleep de **Percentage voltooid** bar aan het noodzakelijke aantal om te wijzen op hoeveel van de taak u voltooide.

   >[!NOTE]
   >
   >Als u aangeeft dat 100% van de taak is voltooid, wordt de status van de taak ook bijgewerkt naar Voltooien.


1. Druk op Enter op het toetsenbord om het volledige percentage op te slaan.

