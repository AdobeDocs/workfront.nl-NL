---
product-area: projects
navigation-topic: use-predecessors
title: Een eerdere relatie maken met het gebied Voorgangers
description: U kunt voorgangstaken (of alleen voorgangers) gebruiken om taken te koppelen die afhankelijk zijn van andere taken die moeten worden gestart of voltooid. U wilt bijvoorbeeld geen partij (afhankelijke taak) hosten voordat u de uitnodigingen (voorgangstaak) verzendt.
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Een eerdere relatie maken met het gebied Voorgangers

U kunt voorgangstaken (of alleen voorgangers) gebruiken om taken te koppelen die afhankelijk zijn van andere taken die moeten worden gestart of voltooid. U wilt bijvoorbeeld geen partij (afhankelijke taak) hosten voordat u de uitnodigingen (voorgangstaak) verzendt.

In dit artikel wordt weergegeven hoe u voordecessors kunt instellen met het tabblad Voorgangers in een taak.

Voor informatie over het plaatsen van predecessors in een lijst van taken, zie [Een voorganger-relatie maken in de takenlijst](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

U kunt de voorgangers van taken in de volgende gebieden van Adobe Workfront bekijken:

* In de sectie Predecessors van de afhankelijke taken
* In de Gantt-grafiek
* In de takenlijst in de kolom Voorgangers

Voor informatie over predecessors raadpleegt u [Overzicht van voorgangers van taken](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot taken en projecten bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor de taken en het project beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Een voorganger maken voor een taak

1. Ga naar een taak die u als afhankelijke taak wilt aanwijzen, dan klik **Predecessors** in het linkerdeelvenster.

   Mogelijk moet u op **Meer weergeven** vervolgens **Predecessors**.

1. Klikken **+Voorganger toevoegen**.
1. (Optioneel) Als u een voorganger voor meerdere projecten wilt toevoegen, vervangt u de naam van het project in het dialoogvenster **Bovenliggend project** veld met een ander project, typt u vervolgens de naam van de taak of taken die u als voorgangers wilt uitvoeren.

   Voor informatie over het toevoegen van predecessors voor meerdere projecten raadpleegt u [Predecessors voor meerdere projecten maken](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. Typ de naam van de taak of taken die u als voorgangers wilt aanwijzen.

   ![](assets/add-predecessor-box-nwe-350x465.png)

1. Selecteer een **Type afhankelijkheid**.

   Voor informatie over de Types van Afhankelijkheid van de taak, zie a [Overzicht van typen taakafhankelijkheid](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Geef een **Lag** bedrag in dagen.

   Voor informatie over de Types van Lag, zie &#x200B; [Overzicht van labeltypen](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

1. Selecteren **Afgedwongen** als u de voorafgaande verhouding tussen de twee taken wilt afdwingen.

   Voor informatie over het afdwingen van voorgangers raadpleegt u [Voorgangers afdwingen](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Klikken **Opslaan**.
