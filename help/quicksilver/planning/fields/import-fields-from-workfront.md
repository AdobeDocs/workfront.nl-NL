---
title: Velden importeren uit Adobe Workfront
description: In de Planning van Adobe Workfront, kunt u douanevelden voor elk type van verslag tot stand brengen. U kunt het gebied met de verslagen van de Planning van Workfront dan associëren.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 994594f2-a888-423a-bf66-0d14baf57c55
source-git-commit: 8425f8be7d30d36986ac1c062603e680c69902c6
workflow-type: tm+mt
source-wordcount: '760'
ht-degree: 0%

---

<!--add to TOC-->

# Velden importeren uit Adobe Workfront

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>


{{planning-important-intro}}

U kunt kopieën van bestaande Workfront-velden importeren. Als u velden importeert uit Workfront, wordt een kopie van elk veld gemaakt voor een recordtype voor Workfront Planning.


## Toegangsvereisten

+++ Breid uit om toegangsvereisten voor de Planning van Workfront te bekijken.

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
<li>Eerste</li> 
<li>Ultieme</li></ul> 
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
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden genegeerd om tot alle mogelijkheden van de Planning van Workfront te kunnen toegang hebben.</p> 
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td><p> Standaard </p>
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
   <td>   <p>Rechten beheren in een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het importeren van velden uit Workfront

* U kunt native of aangepaste Workfront-velden importeren naar een recordtype in Workfront Planning.
* Als u Workfront-velden importeert, worden kopieën van dezelfde velden gemaakt en blijft de veldnaam behouden in Workfront Planning. Nadat ze naar Workfront Planning zijn gekopieerd, zijn de velden onafhankelijk van de originele Workfront-velden en delen ze geen informatie meer.
<!--check this: * You do not need permissions or access to Workfront objects to be able to add their fields to Workfront Planning. -->
* U kunt eigen of aangepaste velden toevoegen vanuit de volgende Workfront-objecten:
   * Portfolio
   * Programma
   * Project
   * Taak
   * Probleem
   * Document
   * Bedrijf
   * Groep
   * Gebruiker
   * Functie
   * Toewijzing
   * Uur
   * Factureringsrecord
     <!--Available only to Preview, but might not come to Prod:* Rate card-->
   * Kosten
   * Iteratie
     <!--* Non-labor resource-->
     <!--* Non-labour resource category-->
* Het veldtype van Workfront-velden blijft mogelijk niet behouden nadat deze zijn geïmporteerd in Workfront Planning.

  In de onderstaande tabel worden de veldtypen van Workfront en het corresponderende veldtype voor Workfront Planning weergegeven.

  | Workfront-veldtype | Het veldtype Workfront Planning |
  |------------------------------------------|-------------------------------|
  | Tekst met enkele regel opmaak | Tekst met één regel |
  | Tekst met enkele regel met nummeropmaak | Getal |
  | Tekst met enkele regel in de notatie van valuta | Valuta |
  | Alinea | Alinea |
  | Tekst met opmaak | Alinea |
  | Vervolgkeuzelijst met één keuze | Enkel selecteren |
  | Vervolgkeuzelijst met meerdere selecties | Meerdere selecties |
  | Typeahead-filters van gebruikers worden niet ondersteund | Mensen |
  | Berekend* | Formule |
  | Datum | Datum |
  | Groep selectievakjes | Meerdere selecties |
  | Keuzerondje | Meerdere selecties |

  *Berekende velden zijn later beschikbaar.
Alle andere Workfront-veldtypen worden niet ondersteund in Workfront Planning.


## Velden importeren uit Workfront

<!--the first 3 steps are the same as in Create fields-->

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u recordtypen wilt maken.

   De werkruimte wordt geopend en de recordtypen worden weergegeven.

1. Klik op de kaart van een recordtype.

   Alle bestaande records die aan het recordtype zijn gekoppeld, worden in de rijen van de tabelweergave weergegeven.

   >[!TIP]
   >
   >    Sommige velden zijn mogelijk verborgen. Klik **Gebieden** en laat knevel voor de gebieden toe u als kolommen in de lijstmening wilt bekijken.

1. Klik op het pictogram **+** rechtsboven in de tabelweergave

   of

   Beweeg over de kopbal van om het even welke kolom, klik de naar beneden wijzende pijl na de gebiedsnaam, dan klik links **of** Tussenvoegsel rechts **om het nieuwe gebied toe te voegen.**
1. Klik **toevoegen bestaand** in de laag-juiste hoek van het **Nieuwe gebied** tabel. <!--check UI - did they change this??-->

   ![](assets/add-existing-fields-from-workfront-modal.png)

1. Typ de naam van een bestaand Workfront-veld in het zoekgebied en klik vervolgens op **+** wanneer het veld in de lijst wordt weergegeven.
1. (Optioneel) Typ een ander veld en klik op **+** wanneer dit in de lijst wordt weergegeven.
1. (Optioneel) Klik op het **pictogram ![](assets/filters-in-import-fields-icon.png) Filters** en werk vervolgens een of beide van de volgende velden bij:

   * Objecttype: selecteer een Workfront-objecttype waarvan u de velden wilt importeren.
   * Aangepast formulier: selecteer een of meer aangepaste formulieren in Workfront. U kunt een aangepast formulier selecteren zonder eerst een objecttype te selecteren.
1. Klik **+**, dan **voegt gebieden** toe.
De velden worden toegevoegd aan de tabelweergave en aan de detailpagina&#39;s van de records.

   >[!IMPORTANT]
   >
   >    Er geldt een limiet van 500 velden voor elk recordtype. De bestaande velden en de geïmporteerde velden dragen bij aan deze limiet.

   De toegevoegde velden zijn kopieën van de Workfront-velden en maken geen verbinding meer met de oorspronkelijke velden in Workfront.