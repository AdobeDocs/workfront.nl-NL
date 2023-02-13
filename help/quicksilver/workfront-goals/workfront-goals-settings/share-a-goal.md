---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Een doel delen in Workfront-doelen
description: Als u een doel deelt, geeft u beheermachtigingen voor een doel aan iemand die dit niet heeft gemaakt.
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 0%

---

# Een doel delen in Adobe Workfront-doelen

Als u een doel deelt, geeft u beheermachtigingen voor een doel aan iemand die dit niet heeft gemaakt.

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

U moet het volgende hebben:

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
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot doelen of hoger bewerken</p> <p><b>OPMERKING</b><p>Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Toegang tot Adobe Workfront-doelen verlenen</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> 
    <div> 
     <p>Rechten voor het doel beheren</p> 
     <p>Voor informatie over het delen van doelstellingen, zie <a href="#" class="MCXref xref selected">Een doel delen in Workfront-doelen</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Vereisten

Voordat u begint, moet u over het volgende beschikken:

* Een lay-outsjabloon die het gebied Doelen in het hoofdmenu bevat.

## Overwegingen over het delen van doelstellingen

* De gebruikers kunnen de volgende toestemmingen aan een doel hebben:

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Doelmachtigingen</b></p></td> 
      <td>
      <p><b>Beschrijving</b></p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Weergave</p></td> 
      <td>
      <p>De gebruikers hebben toestemmingen om het doel te bekijken, maar zij kunnen geen informatie voor het doel uitgeven, kunnen zij geen informatie voor resultaten, of activiteiten toevoegen of uitgeven, status bijwerken, of het doel schrappen.</p>      
      <p>Door gebrek, kunnen alle gebruikers met toegang tot Doelen alle doelstellingen in het systeem bekijken. De gebruikers kunnen het doel kopiëren, als zij Edit toegang tot Doelen in hun toegangsniveau hebben.</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Beheren</p></td> 
      <td> <p>Gebruikers kunnen alle informatie voor het doel bewerken, inclusief voor de resultaten of activiteiten, inclusief het verwijderen van de resultaten.</p> 
      <p>Alleen makers of gebruikers die specifiek beheermachtigingen voor een bepaald doel hebben, kunnen een doel beheren.</p> 
      Alleen gebruikers met de machtiging Beheren voor een bepaald doel kunnen het doel met anderen delen om hen beheerdersmachtigingen voor het doel te geven. </p> </td> 
   </tr> 
   </tbody> 
   </table>

* U kunt de volgende typen doelen met anderen delen:

   * Een doel dat u hebt gemaakt
   * Een doel dat is gemaakt door iemand anders aan wie u machtigingen hebt verleend om te beheren.

* Als u beheerdersmachtigingen voor een doel hebt, kunt u de machtigingen voor het doel wijzigen voor de maker van het doel. Standaard beschikken zij over beheermachtigingen wanneer zij het doel maken, maar u kunt hun machtigingen wijzigen in Weergeven.

## Een doel delen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) > **Doelen** in de rechterbovenhoek.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../workfront-goals-settings/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   De vertoningen van de Lijst van het Doel.

1. Klik op de naam van een doel in de lijst. De doelpagina wordt geopend.

1. Klik op de knop **Meer pictogram** naast de naam van het doel klikt u op **Delen**.

   ![](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   Het vak Goal Access wordt weergegeven.

   ![](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. Voer een van de volgende handelingen uit:

   * Selecteer **Systeembreed beheren** het plaatsen om te geven leidt toestemmingen aan iedereen in het systeem die Edit toegang tot Doelen op hun toegangsniveau heeft. Deze optie is standaard uitgeschakeld voor alle nieuwe doelen.
   * Typ de naam van een gebruiker die u beheerdersrechten wilt geven in het dialoogvenster **Geef Beheer toegang tot** doos. Selecteer de naam wanneer deze in de lijst wordt weergegeven.

      >[!TIP]
      >
      >U kunt een doel alleen met andere gebruikers delen. U kunt geen doelstellingen met groepen, teams, of uw bedrijf delen.

1. Klikken **Delen**.

   Het doel wordt gedeeld met de gebruikers u specificeerde. Een label voor het hele systeem of de naam van de gebruikers die beheermachtigingen hebben voor de doelweergave in het veld Toegang tot beheren in het deelvenster Algemene details.

## Opties voor algemene machtigingen

De volgende lijst maakt een lijst van de toestemmingen die u kunt verlenen wanneer het delen van een doel. Voor meer informatie over de toegang krijgen de gebruikers gebaseerd op hun vergunning, zie [Toegang tot Adobe Workfront-doelen verlenen](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p><strong>Handelingen</strong> </p> </th> 
   <th> <p><strong>Beheren</strong> </p> </th> 
   <th> <p><strong>Weergave</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Doel weergeven</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Resultaten of activiteiten weergeven</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Doel kopiëren* </td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Resultaten of activiteiten omzetten in andere doelen*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Projecten weergeven die zijn toegevoegd als activiteiten** </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Doel bewerken</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Resultaten of activiteiten bewerken</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Resultaten of activiteiten toevoegen voor het doel</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Een project koppelen als een activiteit aan het doel**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Doel verwijderen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Resultaten of activiteiten verwijderen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Maak projecten van het doel los</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*U moet Edit toegang tot Doelen in uw toegangsniveau hebben om resultaten en activiteiten in doelstellingen kunnen omzetten.

**U moet toegang tot de Projecten van de Mening hebben en toestemming van de Mening aan de toegevoegde projecten of die u aan het doel wilt toevoegen om hen te bekijken.

Voor informatie over het niveau van de projecttoegang, zie [Toegang verlenen tot projecten](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Voor informatie over projecttoestemmingen, zie [Een project delen in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

 
