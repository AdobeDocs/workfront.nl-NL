---
product-area: projects
navigation-topic: use-predecessors
title: Een eerdere relatie maken met het gebied Voorgangers
description: U kunt voorgangstaken (of alleen voorgangers) gebruiken om taken te koppelen die afhankelijk zijn van andere taken die moeten worden gestart of voltooid.
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: 6d02397a15b0b06c3c60fb5d71dfeb3cb0b0a30d
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Een eerdere relatie maken met het gebied Voorgangers

<!-- Audited: 5/2025 -->

U kunt voorgangstaken (of alleen voorgangers) gebruiken om taken te koppelen die afhankelijk zijn van andere taken die moeten worden gestart of voltooid. U wilt bijvoorbeeld geen partij (afhankelijke taak) hosten voordat u de uitnodigingen (voorgangstaak) verzendt.

In dit artikel wordt weergegeven hoe u voordecessors kunt instellen met het tabblad Voorgangers in een taak.

Voor informatie over het plaatsen van voorgangers in een lijst van taken, zie [ een voorgangersverhouding op de taaklijst ](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md) creëren.

U kunt de voorgangers van taken in de volgende gebieden van Adobe Workfront bekijken:

* In de sectie Predecessors van de afhankelijke taken
* In de Gantt-grafiek
* In de takenlijst in de kolom Voorgangers

Voor informatie over predecessors, zie [ Overzicht van taakvoordecessors ](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.

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
   <td> 
   <p>Standard </p>
    <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot taken en projecten bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor de taken en het project beheren</p> <p>Voor informatie bij het verzoeken van extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> Toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een voorganger maken voor een taak

Het creëren van een voorganger voor een projecttaak die het gebied van Predecessors gebruikt is gelijkaardig aan het creëren van predecessors voor een malplaatjetaak op een malplaatje.

Een voorgangertaak maken voor een projecttaak:

1. Navigeer aan de taak u als afhankelijke taak wilt aanwijzen.

1. In het linkerpaneel, klik **Predecessors**.

1. In de **sectie 0} Voorgangers {, klik** toevoegen Voorganger **.** **voegt de dialoogdoos van de Voorganger** toe opent.

1. (Facultatief) om een dwars-projectvoorganger toe te voegen, vervang de naam van het project op het **gebied van het Project van de 1} ouder** met een ander project.

   Voor informatie, zie [ tot dwars-project predecessors ](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md) leiden.

   >[!TIP]
   >
   >U kunt geen voordecessors voor meerdere sjablonen maken voor sjabloontaken.


1. Op het **gebied van Taken**, type in de naam van de taak of de taken u als predecessors wilt aanwijzen, dan hen selecteren wanneer zij in drop-down verschijnen.

1. Selecteer het Type van a **Afhankelijkheid**.

   Voor informatie, zie [ Overzicht van de types van taakgebiedsdeel ](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Ga a **bedrag van de a** Lag in.

   Voor informatie, zie &#x200B; [ overzicht van de Types van Lag ](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   ![ voeg de dialoogdoos van de Voorganger ](assets/add-predecessor-dialog-box.png) toe

1. Selecteer **gedwongen** checkbox als u de voorgangersverhouding tussen de twee taken wilt afdwingen.

   Voor informatie, zie [ predecessors ](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md) afdwingen.

1. Klik **sparen**.

1. (Facultatief) om een voorganger te verwijderen, selecteer het uit de lijst van voorgangers, dan klik **verwijderen** pictogram ![ verwijderen pictogram ](assets/remove-or-delete-icon.png).

   De voorganger wordt uit de lijst verwijderd. De voorgangstaak wordt niet geschrapt uit zijn project.
