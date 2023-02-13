---
product-area: projects
navigation-topic: update-work-in-a-project
title: Taakstatus bijwerken
description: U kunt de status van een taak bijwerken om anderen te informeren over waar de taak is (en het algemene project) en hoe de taak vordert.
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Taakstatus bijwerken

U kunt de status van een taak bijwerken om anderen te informeren over waar de taak is (en het algemene project) en hoe de taak vordert.

De standaardstatussen zijn Nieuw, Bezig en Voltooid. Uw Adobe Workfront-beheerder kan aangepaste statussen toevoegen aan uw organisatie. Zie voor meer informatie [Een status maken of bewerken](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

U kunt taakstatussen handmatig bijwerken of u kunt Workfront toestaan deze automatisch bij te werken wanneer bepaalde handelingen plaatsvinden.

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

## Taakstatus handmatig bijwerken

Wanneer u een taakstatus bijwerkt, kunt u ook een uitleg over de nieuwe status typen en andere taakgegevens wijzigen, zoals de vervaldatum.

1. Ga naar een taak waaraan u wordt toegewezen waarvoor u de status wilt bijwerken.
1. Klik op de knop **Status** in de taakkopbal en selecteer een nieuwe status.
1. (Optioneel) Voer een van de volgende handelingen uit om aanvullende informatie over de update op te geven en klik vervolgens op **Bijwerken** of als de taak **Voltooid** status, klik op **Gereed:**

   * Als u een notitie over de update wilt toevoegen, gaat u naar de **Updates** gebied en klik **Een nieuwe update starten** Typ uw notitie.

   * Als u bepaalde gebruikers op de hoogte wilt stellen van de update, typt u hun namen in het dialoogvenster **Waarschuwen** wordt weergegeven wanneer u een notitie over de update typt. Zie voor meer informatie [Andere tags toepassen op updates](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Klik op **Voorwaarde selecteren** rechts van de **Waarschuwen** (deze worden weergegeven wanneer u een opmerking over de update typt) en selecteer vervolgens de voorwaarde die het best overeenkomt met de huidige toestand van de taak.

   * Als u de taakdatum vastleggen wilt bijwerken, vouwt u de opdracht **Vastlegdatum** en selecteer een nieuwe datum vastleggen.
   * Om een visuele aanwijzing van taakvoltooiing te verstrekken, sleep de bel onder Percentage Voltooid of klik het tweemaal om een percentagewaarde in te gaan.\
      ![](assets/drag-the-progress-bar-350x155.png)

## Taakstatus automatisch bijwerken

Workfront werkt de bestaande status van een taak automatisch bij naar een andere status wanneer de in de onderstaande tabel vermelde handelingen plaatsvinden.

>[!NOTE]
>
>De statussen in de volgende tabel zijn standaardsysteemstatussen. Uw Workfront-beheerder of een groepsbeheerder kan de naam van de statussen in uw exemplaar van Workfront wijzigen. Voor informatie over het maken en beheren van statussen in Workfront raadpleegt u [Een status maken of bewerken](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Handeling</td> 
   <td>Oorspronkelijke status</td> 
   <td>Nieuwe status</td> 
  </tr> 
  <tr> 
   <td>Het taakpercentage bijwerken tot 100%</td> 
   <td>Nieuw of Bezig</td> 
   <td>Voltooid</td> 
  </tr> 
  <tr> 
   <td>Werk het taakpercentage bij dat is voltooid van 100% tot een lager getal</td> 
   <td>Voltooid</td> 
   <td>In uitvoering</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Klik op de knop Taak starten om te accepteren dat u aan een taak werkt die aan u is toegewezen</span> </td> 
   <td><span>Nieuw</span> </td> 
   <td> <p>Om het even welke status verbonden aan de knoop van de Taak van het Begin in uw montages van het Team van het Huis.</p> <p>Voor informatie over het vervangen van het Werk op het met een knoop van de Taak van het Begin, zie <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">De knop Aan de werkbalk vervangen door de knop Start</a></span>.</p> <p>Tip: <span>Klikken</span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">de knop Ongedaan maken</span>nadat u op Taak starten hebt geklikt, wordt de status teruggezet naar Nieuw. </p> </td> 
  </tr> 
 </tbody> 
</table>
