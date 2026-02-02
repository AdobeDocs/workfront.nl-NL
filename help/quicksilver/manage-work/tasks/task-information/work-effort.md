---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Overzicht van de werkprestaties
description: Overzicht van de werkprestaties
author: Alina
feature: Work Management
exl-id: 70f51e4b-43cc-427a-99e4-ebb056bb1070
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '1488'
ht-degree: 0%

---

# Overzicht van de werkprestaties

<!--Audited: 01/2024-->

<!--
(NOTE: Linked to the UI >> in the Project/ Template edit box > Tasks area> Learn more)
-->

Als projectmanager, kunt u beslissen hoe u de hoeveelheid werk wilt schatten nodig voor taken om in een project te voltooien. Schatting van de hoeveelheid werk die nodig is om de taken uit te voeren aan de hand van een van de volgende indicatoren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Geplande uren</td> 
   <td> <p> Een handmatige numerieke ingang of een berekening van Adobe Workfront die het aantal uren toont dat het voor de middelen zou nemen die aan een taak worden toegewezen om het te voltooien. </p> <p>Overweeg het volgende over Geplande Uren: </p> 
    <ul> 
     <li>Dit is de standaardmethode. </li> 
     <li>U kunt Geplande uren manueel bijwerken slechts voor taken met een Type van Duur van Berekende Toewijzing of Eenvoudig. </li> 
    </ul> <p>Voor informatie over Geplande Uren, zie <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref"> Gepland overzicht van Uren </a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Werkinspanning </td> 
   <td> <p>Een handmatig label waarmee wordt gedefinieerd of een gebruiker een kleine, middelgrote of grote hoeveelheid dagelijkse inspanning nodig heeft om een taak te voltooien. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The level of effort is estimated to be a percentage of the daily amount of working time. (NOTE: keep this drafted. Vazgen said it's not needed, but waiting for feedback from users)
      </MadCap:conditionalText>
     --> </p> <p>Overweeg het volgende over de Werkinspanning van het Werk:</p> 
    <ul> 
     <li>Dit veld is alleen beschikbaar voor taken met het type Eenvoudige duur. </li> 
     <li>U kunt het gebruik van dit etiket toelaten en het percentage van arbeidstijd bepalen verbonden aan het op het projectniveau. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

In dit artikel wordt beschreven wat de werkinspanning is en hoe u deze moet gebruiken bij het schatten van de hoeveelheid werk voor uw taken.

>[!NOTE]
>
>De geplande uren en de Werkinspanning van het Werk beïnvloeden elkaar. Door de geplande uren bij te werken, kunt u de werkinspanning bijwerken en de werkinspanning bijwerken, kunt u de geplande uren van de taak bijwerken.

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
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p>
   <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten en taken bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een project en de taken ervan beheren</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current: Plan </p>
   Or
   <p>New: Standard </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration</td> 
   <td> <p>Edit access to Projects and Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project and its tasks</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Overwegingen bij het gebruik van werkinspanningen

* Wanneer de projecttaken 0 Geplande Uren hebben en u de Werkinspanning van het Gebruik toelaat om taak Geplande Uren automatisch te berekenen die op het project plaatsen, zal het standaardniveau van de Werkinspanning verbonden aan hen Medium zijn. De geplande uren worden automatisch bijgewerkt voor eenvoudige taken van het Type van Duur. Voor meer informatie, zie de sectie [&#x200B; Niveaus van de Werkinspanning &#x200B;](#levels-of-work-effort) in dit artikel.
* Wanneer de projecttaken Geplande Uren hebben die meer dan 0 zijn en u de Werkinspanning van het Gebruik toelaat om taak Geplande Uren automatisch te berekenen die op het project plaatsen, het niveau van de Inspanning van het Werk volgens de hoeveelheid Geplande Uren zonder de hoeveelheid Geplande Uren voor de Eenvoudige taken van het Type van Duur te veranderen. Voor meer informatie, zie de sectie [&#x200B; Hoe Workfront de Werkinspanning berekent die op Geplande Uren &#x200B;](#how-workfront-calculates-work-effort-based-on-planned-hours) in dit artikel wordt gebaseerd.
* Wanneer de projecttaken 0 Geplande Uren hebben en u de Werkinspanning van het Gebruik toelaat om taak Geplande Uren automatisch te berekenen die op het project plaatsen, dan update het niveau van de Werkinspanning van Medium aan Klein of Groot, de Geplande Uren ook bijwerken. Voor meer informatie, zie de sectie [&#x200B; hoe Workfront Geplande Uren berekent die op de Werkinspanning &#x200B;](#how-workfront-calculates-planned-hours-based-on-work-effort) in dit artikel worden gebaseerd.
* Wanneer u inline taken uitgeeft en zowel de Geplande Uren als het gebied van de Werkinspanning voor taak tezelfdertijd wijzigt, zullen de Geplande Uren met de waarde worden bijgewerkt u specificeert, terwijl de waarde van de Werkinspanning wordt berekend gebaseerd op uw bijgewerkte Geplande Uren.
* Wanneer u de waarde voor Werkinspanning van een taak bijwerkt, wordt de duur niet meer automatisch berekend op basis van de geplande uren. Voor meer informatie over hoe de Duur voor de Eenvoudige taken van de Duur berekent, zie [&#x200B; Overzicht van het Type van Duur: Eenvoudig &#x200B;](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).
* Wanneer u het Type van Duur van een taak van Eenvoudig in om het even welk ander type verandert, wordt het gebied van de Werkinspanning verborgen op de taak. De geplande uren blijven ongewijzigd.
* U kunt het werkinspanningsniveau niet bijwerken op een bovenliggende taak. Het niveau van de Werkinspanning voor een oudertaak wordt automatisch berekend gebaseerd op het aantal Geplande Uren voor de taken die een rollup van alle kindtaken is. Voor informatie over oudertaken, zie [&#x200B; subtasks &#x200B;](../../../manage-work/tasks/create-tasks/create-subtasks.md) creëren.

## Inschakelen met Werkinspanning in plaats van Geplande uren

1. Ga naar een project en klik **Meer** menu ![&#x200B; Meer pictogram &#x200B;](assets/more-icon.png), dan klik **uitgeven**.
1. Klik **Montages van de Taak**, dan selecteren de optie **Werkinspanning van het Gebruik om taak Geplande uren** automatisch te berekenen. Deze optie is standaard uitgeschakeld.

   ![&#x200B; de inspanning van het werk aan projecten &#x200B;](assets/nwe-work-effort-on-projects-350x182.png)

   Voor meer informatie over het toelaten van het gebruik van de Werkinspanning op een project, zie de &quot;sectie van de Montages van Taken&quot;in [&#x200B; projecten &#x200B;](../../../manage-work/projects/manage-projects/edit-projects.md) artikel uitgeven.

1. Klik **Taken** op het linkerpaneel, dan klik de naam van een taak om tot het toegang te hebben.
1. Klik het **Meer** menu ![&#x200B; Meer pictogram &#x200B;](assets/more-icon.png), dan klik **uitgeven**. Zorg ervoor dat de taak een eenvoudig type duur heeft.

   >[!TIP]
   >
   >U kunt de Werkinspanning voor een taak in de sectie van de Details van de Taak ook bijwerken.

1. In het **gebied van het Overzicht**, klik het drop-down menu van de Werkinspanning van het Werk om de hoeveelheid inspanning te verbeteren nodig om de taak te voltooien.

   ![&#x200B; de inspanning van het Werk op Edit de pagina van de Taak &#x200B;](assets/work-effort-on-edit-task-page-350x239.png)

   Raadpleeg de volgende artikelen voor meer informatie over het bijwerken van het veld Werkinspanning op een taak:

   * De &quot;sectie van het Overzicht&quot;in [&#x200B; geeft taken &#x200B;](../../../manage-work/tasks/manage-tasks/edit-tasks.md) artikel uit
   * [Taakgegevens beheren in het gebied Overzicht van taakdetails](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)

## Niveaus van de Werkinspanning {#levels-of-work-effort}

Als projectmanager, kunt u drie niveaus van de Inspanning van het Werk voor uw projecten identificeren. Elk inspanningsniveau is gelijk aan een percentage van dagelijkse tijd dat de gebruikers de taak moeten voltooien.

Bij het instellen van het niveau van de werkinspanning moet u zich de vraag stellen: &quot;Hoeveel tijd zou een gebruiker die aan deze taak wordt toegewezen dagelijks aan het moeten besteden om het in tijd te krijgen?&quot;

In de volgende tabel worden de mogelijke niveaus van de werkinspanning en de bijbehorende standaardpercentages weergegeven. Als projectmanager, kunt u de percentages bijwerken om aan de behoeften van uw organisatie te passen. U doet dit terwijl u een project bewerkt. Voor informatie over het uitgeven van projecten, zie [&#x200B; projecten &#x200B;](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

Als beheerder van Workfront, bepaalt u de Typische uren per het werkdag in het gebied van de Voorkeur van het Project van Opstelling. Dit is de dagelijkse hoeveelheid tijd die als arbeidstijd wordt beschouwd. Voor informatie over het vormen van de Voorkeur van het Project voor uw geval van Workfront, zie [&#x200B; systeem-brede projectvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

>[!NOTE]
>
>In de onderstaande voorbeelden gaan we ervan uit dat de Workfront-beheerder het aantal normale uren per werkdag op 8 uur heeft ingesteld.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Niveau van de Werkinspanning</td> 
   <td>Procentuele waarden</td> 
  </tr> 
  <tr> 
   <td>Klein </td> 
   <td>Een klein inspanningsniveau voor het voltooien van een taak is ingesteld op 25% van de typische uren per werkdag. Dit betekent dat een taak die is toegewezen aan dit niveau van de arbeidsintensie, maximaal 2 uur per dag moet duren om in één dag te voltooien. <code>(0.25*8=2)</code></td> 
  </tr> 
  <tr> 
   <td>Medium</td> 
   <td> <p>Een Medium-inspanningsniveau voor het voltooien van een taak is ingesteld op 50% van de normale uren per werkdag. Dit betekent dat een taak die op dit niveau van de Werkinspanning wordt toegewezen meer dan 2 en minder dan 6 uren zou moeten vergen om in één dag te voltooien. <code>(0.50*80=4)</code> </p> <p>Opmerking: wanneer de optie Werktijd automatisch berekenen voor taak geplande uren is ingeschakeld voor het project, is dit de standaardinstelling voor een taak als de taak 0 geplande uren had voordat deze instelling was ingeschakeld. Hierdoor wordt de taak Geplande uren bijgewerkt naar 4 uur. </p> </td> 
  </tr> 
  <tr> 
   <td>Groot</td> 
   <td>Een grote inspanning voor de voltooiing van een taak wordt geplaatst aan 75% van de Typische uren per het werkdag. Dit houdt in dat een taak die is toegewezen aan dit niveau van de arbeidsintensie in één dag 6 uur of meer moet duren om te worden voltooid. <code>(0.75*8=6)</code></td> 
  </tr> 
 </tbody> 
</table>

## Hoe Workfront de geplande uren berekent op basis van de werkinspanning {#how-workfront-calculates-planned-hours-based-on-work-effort}

Wanneer u de Werkinspanning van het Gebruik toelaat om taak Geplande Uren automatisch te berekenen die op een project plaatsen, berekent Workfront het aantal Geplande Uren voor een taak met een Eenvoudige Type van Duur gebruikend de volgende formule:

```
Task Planned Hours = Number of days in task Duration * Work Effort percentage * Typical hours per work day
```

Een taak met een duur van 3 dagen en een werkinspanning van Medium heeft bijvoorbeeld 12 geplande uren:

```
Planned Hours = 3*4=12
```

waarbij de waarde van de normale uren per werkdag 8 uur bedraagt.

>[!TIP]
>
>Wanneer een taak aan veelvoudige middelen wordt toegewezen, worden de Geplande Uren gelijkmatig verdeeld aan elke middel voor elke dag van de duur van de taak.

## Hoe Workfront de werkinspanning berekent op basis van de geplande uren {#how-workfront-calculates-work-effort-based-on-planned-hours}

Wanneer u de Werkinspanning van het Gebruik toelaat om taak Geplande Uren automatisch te berekenen die op een project plaatsen en u reeds Uren op de taak geplant hebt of u het aantal Geplande Uren op de taak uitgeeft, werkt Workfront de waarde van de Werkinspanning bij.

Workfront gebruikt de volgende formule om het niveau van de Werkinspanning volgens de Geplande Uren bij te werken:

```
Work Effort level = Task Planned Hours / Duration / Typical hours per work day
```

Als u bijvoorbeeld een taak hebt met een duur van 2 dagen en u de geplande uren bijwerkt van 8 tot 20 uur, wordt de werkinspanning voor de taak bijgewerkt van Medium naar Groot:

```
Work Effort level = 20 / 2 / 8 = 125 % = Large
```

## Werkinspanning zoeken voor taken en projecten

* [&#x200B; Werkinspanning voor projecten &#x200B;](#work-effort-for-projects)
* [Werkinspanning voor taken](#work-effort-for-tasks)

### Werkinspanning voor projecten {#work-effort-for-projects}

U kunt de sectie Werkinspanning op een project in het volgende gebied vinden:

* Het gebied Taakinstellingen in het vak Project bewerken

### Werkinspanning voor taken {#work-effort-for-tasks}

U kunt het veld Werkinspanning voor een taak als volgt opzoeken:

* Het gedeelte Overzicht in het vak Taak bewerken
* Het gebied van het Overzicht van de sectie van de Details van de Taak, in het gebied van de Werktijd
* Een takenlijst of rapport
