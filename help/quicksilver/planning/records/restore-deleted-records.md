---
title: Verwijderde records herstellen
description: U kunt verwijderde records uit het onlangs verwijderde gebied in Adobe Workfront Planning herstellen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Verwijderde records herstellen

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> -->

{{planning-important-intro}}

U kunt verwijderde records uit het onlangs verwijderde gebied in Adobe Workfront Planning herstellen.

Voor informatie over het schrappen van verslagen, zie [ verslagen van de Schrapping ](/help/quicksilver/planning/records/delete-records.md).

## Toegangsvereisten

+++ Breid uit om de toegangsvereisten voor de functionaliteit in dit artikel te bekijken. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<ul> 
<li><p>Alle Workfront en alle planningspakketten</p></li>
of
<li><p>Willekeurige workflow en planningspakket</p></li></ul>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Contribute of hoger machtigingen voor een werkruimte en recordtype  </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p> </td> 
  </tr>   
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Contribute or higher permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## Overwegingen bij het herstellen van verwijderde records

* U kunt records herstellen die u of andere gebruikers hebben verwijderd.
* Records worden gedurende 30 dagen in de recent verwijderde opslagruimte opgeslagen. Na 30 dagen worden de records definitief verwijderd uit Workfront Planning.
* Als de verwijderde records zijn gekoppeld aan andere records, worden de gekoppelde records niet verwijderd, maar worden de gegevens uit de verwijderde record ook verwijderd. Door de verwijderde records te herstellen, worden de gegevens uit de verbonden records hersteld.
* U kunt records bulksgewijs herstellen.
* Wanneer de records worden verwijderd, wordt de volgende informatie opgeslagen in het vak Onlangs verwijderd:
   * **Naam**: Dit is de informatie op het Primaire gebied van het verslag. Voor meer informatie over primaire gebieden van het verslag, zie [ Primair gebiedsoverzicht ](/help/quicksilver/planning/fields/primary-field-overview.md).
   * **Geschrapte datum**: De tijd en de datum toen het verslag werd geschrapt.
   * **Tijd in onlangs geschrapt**: De tijd sinds het verslag werd geschrapt. Records die meer dan 30 dagen vóór de huidige datum zijn verwijderd, worden niet weergegeven in het recent verwijderde vak.
   * **die door** wordt geschrapt: De naam van de gebruiker die het verslag schrapte.

## Verwijderde records herstellen

1. Ga naar de pagina met recordtypen waarop u records hebt verwijderd.
1. Klik **ongedaan maken** pictogram ![ pictogram ](assets/undo-icon.png) in de hoger-juiste hoek van om het even welke verslagtype paginamening, dan klik onlangs geschrapt ****.

   De **onlangs geschrapte** vakvertoningen.

   ![ onlangs geschrapt doos ](assets/recently-deleted-box.png)

1. Selecteer de verslagen u wilt schrappen, dan **herstellen** > **herstellen**. U kunt meerdere records selecteren.

   Als het herstellen is gelukt, ontvangt u een melding van een geslaagde bewerking onder aan het scherm.
1. Ga naar de tabelweergave en bekijk de herstelde records.
