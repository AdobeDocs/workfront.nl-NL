---
title: Verwijderde records herstellen
description: U kunt verwijderde records uit het onlangs verwijderde gebied in Adobe Workfront Planning herstellen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Verwijderde records herstellen

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

U kunt verwijderde records uit het onlangs verwijderde gebied in Adobe Workfront Planning herstellen.

Voor informatie over het schrappen van verslagen, zie [ verslagen van de Schrapping ](/help/quicksilver/planning/records/delete-records.md).

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

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
   <td>   <p>Contribute of hogere toestemmingen aan een werkruimte <span class="preview"> en verslagtype </span> </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>In het milieu van de Productie, moeten alle gebruikers met inbegrip van de Beheerders van het Systeem aan een lay-outmalplaatje worden toegewezen dat Planning omvat.</p>
<p><span class="preview">In het milieu van de Voorproef, hebben de Standaardgebruikers en de Beheerders van het Systeem Planning die door gebrek wordt toegelaten.</span></p></td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Overwegingen bij het herstellen van verwijderde records

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
1. Klik **ongedaan maken** pictogram ![ pictogram ](assets/undo-icon.png) in de hoger-juiste hoek van om het even welke verslagtype paginamening, dan klik onlangs geschrapt **&#x200B;**.

   De **onlangs geschrapte** vakvertoningen.

   ![ onlangs geschrapt doos ](assets/recently-deleted-box.png)

1. Selecteer de verslagen u wilt schrappen, dan **herstellen** > **herstellen**. U kunt meerdere records selecteren.

   Als het herstellen is gelukt, ontvangt u een melding van een geslaagde bewerking onder aan het scherm.
1. Ga naar de tabelweergave en bekijk de herstelde records.
