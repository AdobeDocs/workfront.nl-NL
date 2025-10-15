---
product-area: reporting
navigation-topic: reporting-elements
title: De milestone-weergave gebruiken
description: U kunt de mening van de Mijlpaal op een projectlijst of een rapport toepassen. U kunt de mening van de Mijlpaal gebruiken om alle mijlpalen te bekijken die met taken binnen de projecten worden geassocieerd u bekijkt.
author: Courtney, Alina
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 0%

---

# De milestone-weergave gebruiken

<!-- Audited: 11/2024 -->

<!--remove Preview and Production mentions from the article when this comes out live-->

<div class="preview">

De gemarkeerde informatie op deze pagina verwijst naar functionaliteit die nog niet algemeen beschikbaar is. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Dezelfde functies zijn ook beschikbaar in de productieomgeving voor alle klanten vanaf een week na de release Preview.

Voor meer informatie, zie [ modernisering van de Interface ](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

U kunt de mening van de Mijlpaal op een projectlijst of een rapport toepassen. U kunt de mening van de Mijlpaal gebruiken om alle mijlpalen te bekijken die met taken binnen de projecten worden geassocieerd u bekijkt.

Voordat u de milestone-weergave kunt gebruiken, moeten de volgende elementen bestaan:

* De wegen van mijlpalen worden gevormd. Voor informatie, zie [ een milestone weg ](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) creëren.
* Mijlpaden die nodig zijn, worden toegevoegd aan projecten. Voor informatie, zie [ projecten ](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md) uitgeven.
* Mijlpalen zijn gekoppeld aan taken. Voor informatie, zie [ mijlpalen met taken ](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md) associëren.

De mening van de Mijlpaal is beschikbaar wanneer het bekijken van een projectlijst of een projectrapport. De volgende secties beschrijven om de milestone mening te bekijken en te gebruiken.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</strong></td> 
   <td> 
    <p>Standard</p>
    <p>Werk of hoger</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders weergeven of vergroten</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
    <td> <p>De toestemmingen van de mening op een projectrapport om de mening van de Mijlpaal op een rapport toe te passen</p></td> 
   </td> 
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

<div class="preview">

De mening van de Mijlpaal is beschikbaar op projectlijsten en projectrapporten. U kunt snel alle mijlpalen bekijken die met taken binnen de projecten worden geassocieerd u bekijkt.

![ Project met milestone mening ](assets/project-with-milestone-view-with-complete.png)

</div>

>[!NOTE]
>
>De milestone-weergave is niet beschikbaar in de volgende gebieden:
>
>* Tijdschema&#39;s, in de projectlijst wanneer het toevoegen van een project.

Voor informatie over hoe te om aan de mening van de Mijlpaal over te schakelen, zie de sectie [ Schakelaar aan de mening van de Mijlpaal ](#switch-to-the-milestone-view) in dit artikel.


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
  Datums worden weergegeven voor de begin- en einddatum van het project en voor de voltooiing van elke mijlpaaltaak in het pad van de mijlpaal.

  Als u Geprojecteerde datums weergeeft, kunnen de datums niet worden bewerkt. Geprojecteerde datums worden berekend door Workfront en kunnen niet handmatig worden gewijzigd.

  Als u Geplande Datums bekijkt en u hebt ook Manage toegang tot het project, kunt u de volgende data direct van de mening van de Mijlpaal uitgeven:

   * **Datums van het Begin van het Project:** als een project van de Datum van het Begin wordt gepland, kunt u de Geplande Datum van het Begin van het project manueel veranderen, en de Geplande Datum van de Voltooiing wordt dan berekend.
   * **de Datums van de Voltooiing van het Project:** als een project van de Geplande Datum van de Voltooiing wordt gepland, kunt u de Geplande Datum van de Voltooiing van het project manueel veranderen, en de Geplande Datum van het Begin wordt dan berekend.
   * **Datums van de Voltooiing van de Taak:** u kunt de Geplande Datum van de Voltooiing voor taken direct van de mening van de Mijlpaal manueel bijwerken.

* **Volledige Percentage:** toont het voltooiingspercentage van elke taak en project.

  U kunt het voltooiingspercentage van worden getoond onbruikbaar maken, zoals die in de sectie [ wordt beschreven vormt welke informatie in de mening van de Mijlpaal ](#configure-what-information-displays-in-the-milestone-view) in dit artikel toont.

  U kunt het voltooiingspercentage direct van de mening van de Mijlpaal aanpassen, zoals die in de sectie [ wordt beschreven Pas Percentage volledig voor taken in de mening van de Mijlpaal ](#adjust-percent-complete-for-tasks-in-the-milestone-view) in dit artikel aan.

* **de statuspictogrammen van de Taakvooruitgang:** Afhankelijk van welk milieu u gebruikt om de milestone mening te bekijken, zijn het volgende pictogrammen die op de vooruitgangstatus van de taken wijzen:

   * In het milieu van de Productie, tonen de volgende statuspictogrammen naast elk project en taak in de mening van de Mijlpaal:

      * Op tijd\
        ![ op tijdpictogram ](assets/gantt-ontime.png)

      * Achter\
        ![ Achter pictogram ](assets/gantt-behind.png)

      * Risico\
        ![ Bij risicopictogram ](assets/gantt-atrisk.png)

      * Late\
        ![ Te laat pictogram ](assets/gantt-late.png)

     <!--get new screen shots or hide them for preview or production - could not display all in devtest; idea: use color dots from Task Details tab - New status is blue; Some concerns condition is yellow etc-->

  <div class="preview">

   * In het milieu van de Voorproef, tonen de volgende gekleurde cirkels naast elk project en taak in de mening van de Mijlpaal:

      * Op tijd - groen
      * Achter, geel
      * Risico - blauw
      * Late - rood

  </div>

  U kunt deze statuspictogrammen van worden getoond onbruikbaar maken, zoals die in de sectie [ wordt beschreven vormt welke informatie in de mening van de Mijlpaal ](#configure-what-information-displays-in-the-milestone-view) in dit artikel toont.

  Voor meer gedetailleerde informatie over elk statustype, zie het overzicht van de Status van de Voortgang van de taak van artikel [ ](../../../manage-work/tasks/task-information/task-progress-status.md).

* **de status die van de Taak voor voltooide taken** wordt in de schaduw gesteld: Nadat een taak voltooid is, wordt de achtergrond van de taak gearceerd in de mening van de Mijlpaal om erop te wijzen of de taak op tijd of laat werd voltooid:

   * **Rode schaduwen voor taakkolom**: De achtergrond van een taak is rood wanneer de Status van de Voortgang **Late** is.

   * **Groene het in de schaduw stellen voor taakkolom**: De achtergrond van een taak is groen wanneer de Status van de Voortgang **op Tijd** is.

* **de status die van het Project voor de kolommen van het Begin en van de Voltooiing van het Project** wordt in de schaduw gesteld:

   * **Kolom van het Begin van het Project**: De achtergrond van de kolom van het Begin van het Project is rood of groen slechts wanneer de Ware Datum van het Begin wordt bevolkt:

      * **Rode schaduwen voor de kolom van het Begin van het Project**: De achtergrond van de kolom van het Begin van het Project is rood wanneer de Voortgangsstatus van het project **Late** is.

      * **Groene schaduw voor de kolom van het Begin van het Project**: De achtergrond van de kolom van het Begin van het Project is groen wanneer de Voortgangsstatus van het project **op Tijd** is.

     >[!TIP]
     >
     >U moet naar de pagina van de Details van het Project gaan om de Ware Datum van het Begin van het project te bekijken.

   * **de kolom van de Voltooiing van het Project**: De achtergrond van de kolom van de Voltooiing van het Project is rood of groen slechts wanneer de Ware Datum van de Voltooiing wordt bevolkt:

      * **Rood het Schaduwen voor de kolom van de Voltooiing van het Project**: De achtergrond van de kolom van de Voltooiing van het Project is rood wanneer de Voortgangsstatus van het project **Late** is.

      * **Groene het in de schaduw stellen voor de kolom van de Voltooiing van het Project**: De achtergrond van de kolom van de Voltooiing van het Project is groen wanneer de Voortgangsstatus van het project **op Tijd** is.

     >[!TIP]
     >
     >U moet naar de pagina van de Details van het Project gaan om de Ware Datum van de Voltooiing van het project te bekijken.

   * Er wordt geen kleurschaduw toegewezen aan de kolommen Start en Voltooiing wanneer de taken de status Voortgang hebben van Op risico of Achter.

  <!--add new screen shot for preview or production release; logged a bug as this is not happening in the new view - if at prod this is still missing, hide this screen shot-->

  ![ Mijlsteenmening met het in de schaduw stellen ](assets/milestone-view-with-shading.png)

* **naam van het Project**: De projectnaam wordt getoond met een verbinding aan het project.
* **pictogram van de Voorwaarde van het Project**: Afhankelijk van het milieu hebt u toegang tot de mening van de Mijlpaal van de volgende indicatoren toont de projectvoorwaarde:

   * In het milieu van de Productie, toont een pictogram naast de projectnaam, die op de voorwaarde van het project wijzen. De voorwaarde van het project kan één van het volgende zijn:

      * Op doel
      * Risico
      * In problemen

  <div class="preview">

   * In de voorvertoningsomgeving wordt naast elk project een voorwaardepictogram in de vorm van een gekleurde cirkel weergegeven. De mogelijke projectvoorwaarden en cirkelkleuren zijn:

      * Op doel - groen
      * Risicogeel
      * In problemen - rood

     </div>


## Vorm welke informatie in de mening van de Mijlpaal toont {#configure-what-information-displays-in-the-milestone-view}

U kunt vormen of de volgende elementen in de mening van de Mijlpaal worden getoond:

* Pictogrammen voor de voortgangsstatus
* Percentage voltooide projecten en taken

Standaard worden de statuspictogrammen voor de voortgang en het percentage voltooide projecten en taken weergegeven.

Wijzigingen die u aanbrengt in deze opties zijn alleen op u van toepassing. Dit heeft geen invloed op andere gebruikers. De wijzigingen die u aanbrengt, blijven behouden wanneer u zich opnieuw aanmeldt bij Workfront.

Om te vormen of de pictogrammen van de projectstatus en voltooiingspercentage van projecten tonen:

{{step1-to-projects}}

1. Klik het **drop-down menu van de Mening**, dan klik **Mijlpaal**.

1. In het milieu van de Productie, klik **Opties** in de hoger-juiste hoek van de mening van de Mijlpaal, dan selecteer van de opties in de volgende stap.

   ![ milestone_view_options.png ](assets/milestone-view-options-350x141.png)

   <div class="preview">Selecteer in de voorvertoningsomgeving een van de opties in de volgende stap in de rechterbovenhoek van de milestone-weergave.</div>

   <!--at Production release, replace this screen shot and adjust the Production/ Preview text above-->


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

U kunt het percentage Voltooien aanpassen voor taken in de mening van de Mijlpaal. U kunt niet Percentage aanpassen voltooit voor een oudertaak (een taak die subtaken bevat) of voor een project.

Om het percentage aan te passen volledig voor een taak in de mening van de Mijlpaal:

{{step1-to-projects}}

1. Klik het **drop-down menu van de Mening**, dan klik **Mijlpaal**.

1. (Voorwaardelijk) als de voltooiingspercentages niet huidig zijn die in de mening van de Mijlpaal tonen, laat het bekijken van Percentage van taken en projecten toe, zoals die in de sectie [ worden beschreven vormt welke informatievertoningen in de mening van de Mijlpaal ](#configure-what-information-displays-in-the-milestone-view) in dit artikel.

1. Klik in de productieomgeving op het voltooiingspercentage onder een taak, geef een nieuw percentage op en druk op Enter.

   <div class="preview">Verplaats in de voorvertoningsomgeving de dia Percentage voltooid naar het nieuwe percentage voltooid om deze bij te werken. </div>
