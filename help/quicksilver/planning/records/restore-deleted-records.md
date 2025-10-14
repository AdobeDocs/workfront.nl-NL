---
title: Verwijderde records herstellen
description: U kunt verwijderde records uit het onlangs verwijderde gebied in Adobe Workfront Planning herstellen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# Verwijderde records herstellen

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> -->

{{planning-important-intro}}

U kunt verwijderde records uit het onlangs verwijderde gebied in Adobe Workfront Planning herstellen.

Voor informatie over het schrappen van verslagen, zie [&#x200B; verslagen van de Schrapping &#x200B;](/help/quicksilver/planning/records/delete-records.md).

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Producten</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-abonnement*</p></td> 
   <td> 
<p>Een van de volgende Workfront-plannen:</p> 
<ul><li>Selecteren</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is niet beschikbaar voor oudere Workfront-plannen</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-planningspakket*</p></td> 
   <td> 
<p>Alle </p> 
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningsplan is opgenomen. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-platform</p></td> 
   <td> 
<p>Het geval van Workfront van uw organisatie moet aan de Verenigde Ervaring van Adobe worden genegeerd om tot de Planning van Workfront te kunnen toegang hebben.</p> 
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td><p> Standaard</p>
   <p>Workfront Planning is niet beschikbaar voor oudere Workfront-licenties</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td> 
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Contribute of hoger machtigingen voor een werkruimte en recordtype </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Overwegingen bij het herstellen van verwijderde records

* U kunt records herstellen die u of andere gebruikers hebben verwijderd.
* Records worden gedurende 30 dagen in de recent verwijderde opslagruimte opgeslagen. Na 30 dagen worden de records definitief verwijderd uit Workfront Planning.
* Als de verwijderde records zijn gekoppeld aan andere records, worden de gekoppelde records niet verwijderd, maar worden de gegevens uit de verwijderde record ook verwijderd. Door de verwijderde records te herstellen, worden de gegevens uit de verbonden records hersteld.
* U kunt records bulksgewijs herstellen.
* Wanneer de records worden verwijderd, wordt de volgende informatie opgeslagen in het vak Onlangs verwijderd:
   * **Naam**: Dit is de informatie op het Primaire gebied van het verslag. Voor meer informatie over primaire gebieden van het verslag, zie [&#x200B; Primair gebiedsoverzicht &#x200B;](/help/quicksilver/planning/fields/primary-field-overview.md).
   * **Geschrapte datum**: De tijd en de datum toen het verslag werd geschrapt.
   * **Tijd in onlangs geschrapt**: De tijd sinds het verslag werd geschrapt. Records die meer dan 30 dagen vóór de huidige datum zijn verwijderd, worden niet weergegeven in het recent verwijderde vak.
   * **die door** wordt geschrapt: De naam van de gebruiker die het verslag schrapte.

## Verwijderde records herstellen

1. Ga naar de pagina met recordtypen waarop u records hebt verwijderd.
1. Klik **ongedaan maken** pictogram ![&#x200B; pictogram &#x200B;](assets/undo-icon.png) in de hoger-juiste hoek van om het even welke verslagtype paginamening, dan klik onlangs geschrapt **&#x200B;**.

   De **onlangs geschrapte** vakvertoningen.

   ![&#x200B; onlangs geschrapt doos &#x200B;](assets/recently-deleted-box.png)

1. Selecteer de verslagen u wilt schrappen, dan **herstellen** > **herstellen**. U kunt meerdere records selecteren.

   Als het herstellen is gelukt, ontvangt u een melding van een geslaagde bewerking onder aan het scherm.
1. Ga naar de tabelweergave en bekijk de herstelde records.
