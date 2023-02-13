---
product-previous: workfront-goals
navigation-topic: goal-management
title: De lijst met doelstellingen van Adobe Workfront afdrukken
description: U kunt een lijst met doelen afdrukken in het gedeelte Lijst met doelen van Adobe Workfront. Bij het afdrukken wordt een bestand naar de printer verzonden of wordt een .pdf-bestand gemaakt als de afdrukbestemming van de browser is ingesteld op Opslaan als PDF.
author: Alina
feature: Workfront Goals
exl-id: 66488d2f-ed35-4571-93e3-e0e025da7b33
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 0%

---

# De lijst met doelstellingen van Adobe Workfront afdrukken

>[!IMPORTANT]
>
>De in dit artikel beschreven functionaliteit is uit Workfront verwijderd, vanaf de release 23.1.
>
>Dit artikel wordt ook verwijderd kort na de release van 23.1, begin 2023. Op dit moment raden we u aan eventuele bladwijzers dienovereenkomstig bij te werken.

U kunt een lijst met doelen afdrukken in het gedeelte Lijst met doelen van Adobe Workfront. Bij het afdrukken wordt een bestand naar de printer verzonden of wordt een .pdf-bestand gemaakt als de afdrukbestemming van de browser is ingesteld op Opslaan als PDF.

## Toegangsvereisten

<!--drafted - replace the table below with this one when P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>
-->

U moet de volgende toegang hebben om de handelingen uit te voeren die in dit artikel worden beschreven:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Pro of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Aanvraag of hoger</p> <p>Zie voor meer informatie <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Overzicht van Adobe Workfront-licenties</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>U moet een extra licentie voor de Adobe Workfront Goals aanschaffen om toegang te krijgen tot de functionaliteit die in dit artikel wordt beschreven. </p> <p>Zie voor meer informatie <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Vereisten voor het gebruik van Workfront-doelen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau*</td> 
   <td> <p>Toegang tot doelen weergeven of vergroten</p> <p><b>OPMERKING</b><p>Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Toegang tot Adobe Workfront-doelen verlenen</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> 
    <div> 
     <p>De toestemmingen van de mening of hoger op doelstellingen</p> 
     <p>Voor informatie over het delen van doelstellingen, zie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Een doel delen in Workfront-doelen</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Vereisten

U moet het volgende hebben voordat u kunt beginnen:

* Een lay-outsjabloon die het gebied Doelen in het hoofdmenu bevat.

## De doellijst afdrukken

>[!TIP]
>
>* Wanneer u een lijst met doelen afdrukt, bevat het geproduceerde bestand alleen de informatie die op het scherm wordt weergegeven. De punten die door een lijst van doelstellingen worden geëlimineerd te filtreren tonen niet in het .pdf- dossier.
>* Wanneer u de doelstellingen in de lijst niet breidt alvorens de lijst te drukken, toont het .pdf- dossier slechts doelstellingen zonder hun resultaten en activiteiten.
>


1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) > **Doelen** in de rechterbovenhoek.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Dit opent het gebied van de Doelen van Workfront.

   De vertoningen van de Lijst van het Goal door gebrek.

1. (Optioneel) Pas filters toe op de lijst met doelen om de voor u relevante doelen weer te geven.

   Voor informatie over het filtreren van informatie in de Lijst van het Doel, zie [Gegevens filteren in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. Klikken **Afdrukken**. Het vak Afdrukken wordt weergegeven.
1. (Voorwaardelijk) Afhankelijk van browser gebruikt u en andere toepassingen u op uw computer hebt geïnstalleerd, kunt u uit de volgende bestemmingen selecteren:

   * Afdrukken op een printer
   * Afdrukken naar PDF
   * De lijst met doelen opslaan op een lokaal of online station (bijvoorbeeld Google Drive)
   * De lijst met doelen naar een andere toepassing verzenden (bijvoorbeeld Eén opmerking)

1. (Optioneel) Pas de afdrukopties aan.
1. Klikken **Afdrukken**.

   De lijst met doelen wordt aan de geselecteerde bestemming geleverd.
