---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: De teams van een groep maken en wijzigen
description: Wanneer u een groep bekijkt die u in het gebied Groepen beheert, kunt u met teams bekijken en werken verbonden aan de groep en om het even welk van zijn subgroepen.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: 6f9eddd46430990e11d5d661ea09f0595a9acebc
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 0%

---

# De teams van een groep maken en wijzigen

Wanneer u een groep bekijkt die u in het gebied Groepen beheert, kunt u met teams bekijken en werken verbonden aan de groep en om het even welk van zijn subgroepen.

Als er om het even welke groepen boven uw groep zijn, kunnen hun beheerders deze dingen voor uw groep ook doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

Voor informatie over hoe de gebruikers met een vergunning van het Plan een team kunnen tot stand brengen, zie [Een team maken](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Voor informatie over hoe een beheerder van Workfront een team kan creëren, zie [Een team maken vanuit het gedeelte Setup](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md).

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-abonnement*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> <p>U moet een groepsbeheerder van de groep of een beheerder van Workfront zijn. Zie voor meer informatie <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Groepbeheerders</a> en <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de Workfront-beheerder als u wilt weten welk abonnement- of licentietype u hebt.

## U kunt vanuit het gebied Groepen teams voor uw groep weergeven, werken met en maken

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Groepen** ![](assets/groups-icon.png).

1. Klik op de naam van de groep waarvoor u teams wilt maken of wijzigen.
1. Klik in het linkerdeelvenster op **Teams** ![](assets/teams.png) om de teams te vermelden verbonden aan de groep en met om het even welke subgroepen het kan hebben.

1. Voer een van de volgende handelingen uit:

   * **Een team toevoegen**: Klikken **Nieuw team** en gebruik vervolgens de volgende opties om het te configureren:

   <!-- WRITER please check table below. I stripped out wonky conditions-->

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
       <td role="rowheader">Teamnaam</td> 
       <td>Typ een naam voor het team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Groep</td> 
       <td> <p> Het systeem vult het gebied van de Groep voor het nieuwe team met de groep op u bekijkt. Als u het team aan een verschillende groep wilt associëren, begin de naam van de groep te typen, dan selecteer de naam wanneer het verschijnt.</p> <p>U kunt ervoor zorgen u de juiste groep met het team associeert door over het te hangen en het informatiepictogram te klikken <img src="assets/info-icon.png"> die ernaast wordt weergegeven. Hier wordt knopinfo weergegeven met informatie over de groep, zoals de hiërarchie van de bovenliggende groepen en de bijbehorende beheerders.</p> <p><b>OPMERKING</b>: Wanneer een team aan een groep of een subgroep wordt toegewezen, kunnen om het even welke groepsbeheerders van die groep of subgroep het team beheren zonder een lid van het te zijn. De beheerders van de groep kunnen naar het gebied van Teams van het Belangrijkste Menu gaan en de pijl van de Teams van de Schakelaar klikken <img src="assets/switch-team-icon.png" alt="Teampictogram wisselen"> om van alle teams een lijst te maken die aan de groepen worden toegewezen die zij leiden.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Teamleden</td> 
       <td> <p>Typ de naam van een gebruiker die zich in het team moet bevinden en selecteer vervolgens de naam in de vervolgkeuzelijst. Herhaal dit proces om meerdere gebruikers aan het team toe te voegen.</p> <p>Er is geen limiet voor het aantal gebruikers dat u aan een team kunt toevoegen. Nochtans, adviseren wij om geen bovenmatig groot aantal gebruikers in één team te hebben, omdat het het werkbeheer van het team te complex zou kunnen worden.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Beschrijving</td> 
       <td>Typ een beschrijving voor het team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Kalender</td> 
       <td>Kies welk kalendertabblad wordt weergegeven voor dit team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">eraan werken</td> 
       <td>Wijzig de knop Aan de werkbalk in een knop Start. Wanneer een gebruiker op Start klikt, wordt de status van het item automatisch bijgewerkt.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Gereed, knop</td> 
       <td>Selecteer de status die u voor items wilt instellen wanneer op de knop Gereed wordt geklikt.</td> 
       </tr> 
      </tbody> 
     </table>

   * **Teams bewerken**: Selecteer minstens één team, klik **de** Pictogram Bewerken ![](assets/edit-icon.png)en gebruik vervolgens de volgende opties om het te configureren:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
       <td role="rowheader">Teamnaam</td> 
       <td>Typ een naam voor het team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Groep</td> 
       <td> <p>Associeer het team met een groep. Typ de naam van de groep en selecteer vervolgens de naam wanneer deze wordt weergegeven.</p> <p>U kunt ervoor zorgen u de juiste groep met het team associeert door over het te hangen en het informatiepictogram te klikken <img src="assets/info-icon.png"> die ernaast wordt weergegeven. Hier wordt knopinfo weergegeven met informatie over de groep, zoals de hiërarchie van de bovenliggende groepen en de bijbehorende beheerders.</p> <p><b>OPMERKING</b>: Wanneer een team aan een groep of een subgroep wordt toegewezen, kunnen om het even welke groepsbeheerders van die groep of subgroep het team beheren zonder een lid van het te zijn. De beheerders van de groep kunnen naar het gebied van Teams van het Belangrijkste Menu gaan en de pijl van de Teams van de Schakelaar klikken <img src="assets/switch-team-icon.png" alt="Teampictogram wisselen"> om van alle teams een lijst te maken die aan de groepen worden toegewezen die zij leiden.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Eigenaar</td> 
       <td>Selecteer een eigenaar voor het team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Teamleden</td> 
       <td> <p>Toevoegen en teamleden. Typ de naam van een gebruiker en selecteer vervolgens de naam wanneer deze wordt weergegeven. Herhaal dit proces om meerdere gebruikers aan het team toe te voegen.</p> <p><b>TIP</b>: Er is geen limiet voor het aantal gebruikers dat u aan een team kunt toevoegen. Nochtans, adviseren wij om geen bovenmatig groot aantal gebruikers in één team te hebben, omdat het het werkbeheer van het team te complex zou kunnen worden.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Beschrijving</td> 
       <td>Typ een beschrijving voor het team.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Lay-outsjabloon</td> 
       <td> <p>Typ de naam van de lay-outsjabloon die het team moet gebruiken en klik vervolgens op de naam wanneer deze wordt weergegeven.</p> <p>Wanneer u het team met dit lay-outmalplaatje als Team van het Huis van gebruikers aanwijst, zullen alle gebruikers in dit team de aanpassingen in dit lay-outmalplaatje zien.<br>Hun individuele montages van het lay-outmalplaatje zullen de montages van het de lay-outmalplaatje van het huisteam met voeten treden. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Agile</td> 
       <td>Geef op of dit een flexibel team is. Voor informatie over bestandsteams en hoe ze hun werk kunnen beheren, raadpleegt u <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Een bestandsteam maken</a>.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">eraan werken</td> 
       <td> <p>Wijzig de knop Aan de werkbalk in een knop Start. Wanneer een gebruiker op Start klikt, wordt de status van het item automatisch bijgewerkt.</p> <p>Voor meer informatie over hoe te om de knoop van het Begin te vormen, zie <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">De knop Aan de werkbalk vervangen door de knop Start</a>.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Gereed, knop</td> 
       <td> <p>Pas de knop Gereed aan. Zie voor meer informatie:</p> 
       <ul> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">De knop Gereed configureren voor taken</a> </li> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">De knop Gereed configureren voor problemen</a> </li> 
       </ul> </td> 
       </tr> 
      </tbody> 
     </table>

   * **Teams verwijderen**: Selecteer ten minste één team en klik op het pictogram Verwijderen ![](assets/delete.png).
   * **De lijst met teams exporteren**: Klikken **Exporteren** ![](assets/export.png)selecteert u vervolgens de gewenste bestandsindeling voor de geëxporteerde lijst.
