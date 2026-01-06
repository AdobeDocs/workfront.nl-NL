---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Een doel delen in Workfront-doelen
description: Als u een doel deelt, geeft u beheermachtigingen voor een doel aan iemand die dit niet heeft gemaakt.
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 0%

---

# Een doel delen in Adobe Workfront-doelen

Als u een doel deelt, geeft u beheermachtigingen voor een doel aan iemand die dit niet heeft gemaakt.

## Toegangsvereisten

>[!NOTE]
>
>Uw bedrijf zou kunnen verkiezen om de Doelen van Adobe Workfront verder te gebruiken als zij dit pakket in het verleden kochten. U moet voor meer informatie contact opnemen met uw accountvertegenwoordiger.
>
>Adobe Workfront Goals kan niet meer worden aangeschaft.

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Adobe Workfront-pakket</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-licentie</td>
 <td>
 <p>Medewerker of hoger</p>
<p>Aanvraag of hoger</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configuratie op toegangsniveau</td>
 <td> <p>Toegang tot doelen bewerken</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objectmachtigingen</td>
 <td>
  <div>
  <p>De toestemmingen van de mening of hoger aan het doel om het te bekijken</p>
  <p>Machtigingen beheren om het te bewerken</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Systeembeheerders, moet een lay-outsjabloon worden toegewezen die het gebied Doelen in het hoofdmenu bevat. </p>  
</td>
  </tr>
</tbody>
</table>

Voor meer informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
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
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

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

* Als u beheerdersmachtigingen voor een doel hebt, kunt u de machtigingen voor het doel wijzigen voor de maker van het doel. Standaard beschikken zij over de machtiging Beheren wanneer zij het doel maken, maar u kunt hun machtigingen wijzigen in Weergeven.

## Een doel delen

{{step1-to-goals}}

De vertoningen van de Lijst van het Doel.

1. Klik op de naam van een doel in de lijst. De doelpagina wordt geopend.

1. Klik het **Meer pictogram** naast de doelnaam, dan klik **Aandeel**.

   ![&#x200B; Meer menu &#x200B;](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   Het vak Goal Access wordt weergegeven.

   ![&#x200B; Toegang van het Doel &#x200B;](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. Voer een van de volgende handelingen uit:

   * Selecteer **beheer systeem-breed** plaatsen om te geven leidt toestemmingen aan iedereen in het systeem die toegang tot Doelen in hun toegangsniveau heeft uitgeven. Deze optie is standaard uitgeschakeld voor alle nieuwe doelen.
   * Begin de naam van een gebruiker te typen die u beheertoestemmingen aan in **wilt geven leidt toegang tot** doos. Selecteer de naam wanneer deze in de lijst wordt weergegeven.

     >[!TIP]
     >
     >U kunt een doel alleen met andere gebruikers delen. U kunt geen doelstellingen met groepen, teams, of uw bedrijf delen.

1. Klik **Aandeel**.

   Het doel wordt gedeeld met de gebruikers u specificeerde. Een label voor het hele systeem of de naam van de gebruikers die beheermachtigingen hebben voor de doelweergave in het veld Toegang tot beheren in het deelvenster Algemene details.

## Opties voor algemene machtigingen

De volgende lijst maakt een lijst van de toestemmingen die u kunt verlenen wanneer het delen van een doel. Voor meer informatie over de toegangsgebruikers die op hun vergunning worden gebaseerd, zie [&#x200B; de toegang van de Verlening tot de Doelen van Adobe Workfront &#x200B;](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p><strong> Acties </strong> </p> </th> 
   <th> <p><strong> leiden </strong> </p> </th> 
   <th> <p><strong> Mening </strong> </p> </th> 
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
   <td> </td> 
  </tr> 
  <tr> 
   <td>Resultaten of activiteiten toevoegen voor het doel</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Een project koppelen als een activiteit aan het doel**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Doel verwijderen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Resultaten of activiteiten verwijderen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Maak projecten van het doel los</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*U moet Edit toegang tot Doelen in uw toegangsniveau hebben om resultaten en activiteiten in doelstellingen kunnen omzetten.

**U moet toegang tot de Projecten van de Mening hebben en toestemming van de Mening aan de toegevoegde projecten of die u aan het doel wilt toevoegen om hen te bekijken.

Voor informatie over het niveau van de projecttoegang, zie [&#x200B; Toegang van de Verlening tot projecten &#x200B;](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Voor informatie over projecttoestemmingen, zie [&#x200B; een project in Adobe Workfront &#x200B;](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md) delen.


