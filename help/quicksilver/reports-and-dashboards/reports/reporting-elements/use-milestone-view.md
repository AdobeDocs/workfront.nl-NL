---
product-area: reporting
navigation-topic: reporting-elements
title: De milestone-weergave gebruiken
description: U kunt de mening van de Mijlpaal op een projectlijst of een rapport toepassen.
author: Nolan
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1312'
ht-degree: 0%

---

# De milestone-weergave gebruiken

<!-- Audited: 11/2024 -->

U kunt de mening van de Mijlpaal op een projectlijst of een rapport toepassen.

Alvorens u de milestone mening kunt gebruiken, moeten de Mijlpalen worden gevormd, moeten de Wegen van de Mijlsteen aan projecten worden toegevoegd, en de Mijlpalen moeten met taken worden geassocieerd, zoals die in de artikelen [ worden beschreven leidt tot een milestone weg ](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) en [ Verwante mijlpalen met taken ](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

De mening van de Mijlpaal is beschikbaar wanneer het bekijken van een projectlijst of een projectrapport. De volgende secties beschrijven om de milestone mening te bekijken en te gebruiken.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie</strong></td> 
   <td> 
      <p>Nieuw:</p>
         <ul>
         <li><p>Standaard</p></li>
         </ul>
      <p>Huidige:</p>
         <ul>
         <li><p>Werk of hoger</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders weergeven of vergroten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>De toestemmingen van de mening op een projectrapport om de mening van de Mijlpaal op een rapport toe te passen</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overschakelen naar de milestone-weergave {#switch-to-the-milestone-view}

{{step1-to-projects}}

1. Klik het **drop-down menu van de Mening**, dan klik **Mijlpaal**.

   De lijst of het rapport wordt weergegeven in een Mijlsteenweergave.

   Voor informatie over de milestone mening, zie het overzicht van de sectie [ mening Mijlsteen ](#milestone-view-overview) in dit artikel.

## Overzicht van de mijlpaalweergave {#milestone-view-overview}

De mening van de Mijlpaal is beschikbaar op projectlijsten en projectrapporten. In deze weergave kunt u snel alle mijlpalen weergeven die zijn gekoppeld aan taken binnen de projecten die u bekijkt.


>[!NOTE]
>
>De milestone-weergave is niet beschikbaar in de volgende gebieden:
>
>* Tijdschema&#39;s, in de projectlijst wanneer het toevoegen van een project.


Voor informatie over hoe te om aan de mening van de Mijlpaal over te schakelen, zie de sectie [ Schakelaar aan de mening van de Mijlpaal ](#switch-to-the-milestone-view) in dit artikel.

![ Project met milestone mening ](assets/project-with-milestone-view-with-complete.png)

### Fragmenten uit de Mijlsteenweergave

Wanneer het toepassen van de mening van de Mijlpaal op een lijst van projecten, tonen de projecten in de volgende secties:

* De projecten die met een Weg van de Mijlpaal worden geassocieerd worden eerst getoond, die onder de naam van hun respectieve Wegen van de Mijlsteen worden vermeld.

  Workfront sorteert de projecten in de eerste sectie aan de volgende criteria, in deze orde:

   1. Mijlpad-id. U kunt identiteitskaart van de Weg van de Mijlpaal in een rapport van de Weg van de Mijlpaal bekijken.

   2. Het gebied selecteerde als eerste sorterend gebied voor de projectlijst in de mening eerder toegepast op de projectlijst, alvorens u de mening van de Mijlpaal selecteerde.

* De projecten niet verbonden aan een vertoning van de Weg van Milestobe daarna, in de Niet toegewezen sectie. Workfront sorteert de projecten in de Unassiged sectie door het gebied dat als eerste sorterend gebied voor de projectlijst in de mening eerder op de projectlijst wordt toegepast, alvorens u de mening van de Mijlpaal selecteerde.

### Projectinformatie in de milestone-weergave

Wanneer het bekijken van een projectlijst of een projectrapport in de mening van de Mijlpaal, is de volgende informatie beschikbaar:

* **Geplande Data of Geprojecteerde Datums:** specificeer of u Geplande Data of Geprojecteerde Datums in de mening van de Mijlpaal wilt tonen.\
  Datums worden weergegeven voor het begin en de voltooiing en voor elke mijlpaal in het pad van de mijlpaal.\
  Als u Geplande Data bekijkt en u hebt ook beheertoegang tot het project, kunt u de volgende datums rechtstreeks vanuit de Mijlpaal-weergave bewerken: (Als u Geprojecteerde datums weergeeft, kunnen de datums niet worden bewerkt omdat Geprojecteerde datums worden berekend en niet handmatig kunnen worden gewijzigd.)

   * **Datums van het Begin van het Project:** als een project van de Datum van het Begin wordt gepland, kunt u de Datum van het Begin van het project manueel veranderen, en de Datum van de Voltooiing wordt dan berekend.
   * **de Datums van de Voltooiing van het Project:** als een project van de Datum van de Voltooiing wordt gepland, kunt u de Datum van de Voltooiing van het project manueel veranderen, en de Datum van het Begin wordt dan berekend.
   * **Datums van de Voltooiing van de Taak:** u kunt Voltooiing voor taken direct van de mening van de Mijlpaal manueel bijwerken.

* **Volledige Percentage:** toont het voltooiingspercentage van elke taak en project.\
  U kunt het voltooiingspercentage van worden getoond onbruikbaar maken, zoals die in de sectie [ wordt beschreven vormt welke informatie in de mening van de Mijlpaal ](#configure-what-information-displays-in-the-milestone-view) in dit artikel toont.\
  U kunt het voltooiingspercentage direct van de mening van de Mijlpaal aanpassen, zoals die in de sectie [ wordt beschreven Pas Percentage volledig voor taken in de mening van de Mijlpaal ](#adjust-percent-complete-for-tasks-in-the-milestone-view) in dit artikel aan.

* **de statuspictogrammen van de Taak:** A statuspictogram wordt getoond naast elk project en taak in de mening van de Mijlpaal.

   * Op tijd\
     ![ op tijdpictogram ](assets/gantt-ontime.png)

   * Achter\
     ![ Achter pictogram ](assets/gantt-behind.png)

   * Risico\
     ![ Bij risicopictogram ](assets/gantt-atrisk.png)

   * Late\
     ![ Te laat pictogram ](assets/gantt-late.png)

  U kunt deze statuspictogrammen van worden getoond onbruikbaar maken, zoals die in de sectie [ wordt beschreven vormt welke informatie in de mening van de Mijlpaal ](#configure-what-information-displays-in-the-milestone-view) in dit artikel toont.\
  Voor meer gedetailleerde informatie over elk statustype, zie het overzicht van de Status van de Voortgang van de taak van artikel [ ](../../../manage-work/tasks/task-information/task-progress-status.md).

* **de status die van de Taak voor voltooide taken** wordt in de schaduw gesteld: Nadat een taak voltooid is, wordt de achtergrond van de taak gearceerd in de mening van de Mijlpaal om erop te wijzen of de taak op tijd of laat werd voltooid:

   * **Rode schaduwen voor taakkolom**: De achtergrond van een taak is rood wanneer de Status van de Voortgang **Late** is.

   * **Groene het in de schaduw stellen voor taakkolom**: De achtergrond van een taak is groen wanneer de Status van de Voortgang **op Tijd** is.

* **de status die van het Project voor de kolommen van het Begin en van de Voltooiing van het Project** wordt in de schaduw gesteld:

   * **Kolom van het Begin van het Project**: De achtergrond van de kolom van het Begin van het Project is rood of groen slechts wanneer de Ware Datum van het Begin wordt bevolkt:

      * **Rode schaduwen voor de kolom van het Begin van het Project**: De achtergrond van de kolom van het Begin van het Project is rood wanneer de Voortgangsstatus van het project **Late** is.

      * **Groene schaduw voor de kolom van het Begin van het Project**: De achtergrond van de kolom van het Begin van het Project is groen wanneer de Voortgangsstatus van het project **op Tijd** is.

   * **de kolom van de Voltooiing van het Project**: De achtergrond van de kolom van de Voltooiing van het Project is rood of groen slechts wanneer de Ware Datum van de Voltooiing wordt bevolkt:

      * **Rood het Schaduwen voor de kolom van de Voltooiing van het Project**: De achtergrond van de kolom van de Voltooiing van het Project is rood wanneer de Voortgangsstatus van het project **Late** is.

      * **Groene het in de schaduw stellen voor de kolom van de Voltooiing van het Project**: De achtergrond van de kolom van de Voltooiing van het Project is groen wanneer de Voortgangsstatus van het project **op Tijd** is.

   * Er wordt geen kleurschaduw toegewezen aan de kolommen Start en Voltooiing wanneer de taken de status Voortgang hebben van Op risico of Achter.

  ![ Mijlsteenmening met het in de schaduw stellen ](assets/milestone-view-with-shading.png)

* **naam van het Project**: De projectnaam wordt getoond met een verbinding aan het project.
* **het pictogram van de Voorwaarde van het Project**: Een pictogram wordt getoond naast de projectnaam, die op de voorwaarde van het project wijzen.

## Vorm welke informatie in de mening van de Mijlpaal toont {#configure-what-information-displays-in-the-milestone-view}

U kunt vormen of de volgende elementen in de mening van de Mijlpaal worden getoond:

* Pictogrammen voor de voortgangsstatus
* Percentage voltooide projecten en taken

Door gebrek, de pictogrammen van de projectstatus en het percentage voltooide van projecten tonen.

Wijzigingen die u aanbrengt in deze opties zijn alleen op u van toepassing. Dit heeft geen invloed op andere gebruikers. De wijzigingen die u aanbrengt, blijven behouden wanneer u zich opnieuw aanmeldt bij Adobe Workfront.

Om te vormen of de pictogrammen van de projectstatus en voltooiingspercentage van projecten tonen:

{{step1-to-projects}}

1. Klik het **drop-down menu van de Mening**, dan klik **Mijlpaal**.\
   Als u een lijst van projecten binnen een Portfolio of een Programma bekijkt, selecteer **Mijlsteen** subtab.

1. Klik **Opties** in de hoger-juiste hoek van de mening van de Mijlpaal.\
   ![ milestone_view_options.png ](assets/milestone-view-options-350x141.png)

1. Selecteer een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Voortgangsstatus</td> 
      <td> <p>Selecteer deze optie om statuspictogrammen voor de voortgang weer te geven naast elk project en elke taak.</p> <p>Deze optie is standaard ingeschakeld.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percentage voltooid</td> 
      <td> <p>Selecteer deze optie om het voltooiingspercentage naast elk project en elke taak weer te geven.</p> <p>Deze optie is standaard ingeschakeld.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Percentage van voltooiing aanpassen voor taken in de weergave Mijlpaal {#adjust-percent-complete-for-tasks-in-the-milestone-view}

U kunt het percentage Voltooien aanpassen voor taken in de mening van de Mijlpaal. U kunt het percentage niet aanpassen voltooid voor een bovenliggende taak (een taak die subtaken bevat).

Om het percentage aan te passen volledig voor een taak in de mening van de Mijlpaal:

{{step1-to-projects}}

1. Klik het **drop-down menu van de Mening**, dan klik **Mijlpaal**.

1. (Voorwaardelijk) als de voltooiingspercentages niet huidig zijn die in de mening van de Mijlpaal tonen, klik **Opties** in de hoger-juiste hoek van de mening van de Mijlpaal, dan ervoor zorgen dat **Volledige Percentage** wordt toegelaten.

1. Klik op het voltooiingspercentage onder een taak, geef een nieuw percentage op en druk op Enter.
