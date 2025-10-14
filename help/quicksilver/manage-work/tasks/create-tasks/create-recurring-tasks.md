---
product-area: projects
navigation-topic: create-tasks
title: Herhalende taken maken
description: U kunt terugkomende taken voor taken tot stand brengen u als deel van één enkel project moet herhalen.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '917'
ht-degree: 0%

---

# Herhalende taken maken

<!--Audited: 01/2024-->

U kunt terugkomende taken voor taken tot stand brengen u als deel van één enkel project moet herhalen.

Voor algemene informatie over terugkomende taken, met inbegrip van het effect van het uitgeven van een bestaande terugkomende taak, zie [&#x200B; Terugkerende takenoverzicht &#x200B;](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Nieuw: Standaard</p> 
   <p>Huidig: Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot taken en projecten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute-machtigingen voor het project met de mogelijkheid om taken of hoger toe te voegen</p> 
   <p>Als u een taak maakt, ontvangt u automatisch beheermachtigingen voor de taak</p> 
   <p> Voor informatie over taaktoestemmingen, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref"> een taak delen </a>.</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront. Voor meer informatie over toegangsvereisten, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een terugkerende taak maken

>[!NOTE]
>
>U kunt geen terugkomende taak tot stand brengen door een bestaande taak te wijzigen. U moet een nieuwe taak maken.

1. Ga naar het project waar u een terugkomende taak wilt tot stand brengen, dan de **sectie van Taken** in het linkerpaneel klikken.
1. Klik **Nieuwe Taak**.

   Het dialoogvenster Nieuwe taak wordt weergegeven.

   ![](assets/nwe-create-task-small-screen-350x272.png)

1. Klik **Meer opties** dan ga een naam voor de taak op het **gebied van de Naam van de Taak** in.
1. Werk de taak verder bij op dezelfde manier als wanneer u een nieuwe taak toevoegt. Voor meer informatie over het toevoegen van een nieuwe taak, zie [&#x200B; tot taken in een project &#x200B;](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) leiden.

   >[!TIP]
   >
   >   De duur en de geplande uren die voor een nieuwe terugkerende taak worden vermeld zijn de Duur en de Geplande Uren van elk voorkomen. De Duur van de oudertaak is de tijd tussen de Geplande Datum van het Begin van de vroegste taak en de Geplande Datum van de Voltooiing van de recentste taak. De geplande uren van de bovenliggende taak is het totaal van alle geplande uren van alle voorvallen.

1. Klik **Overzicht** in het linkerpaneel.
1. De rol neer aan de **sectie van het Programma van de Herhaling**, dan selecteert **maakt dit een terugkomende taak** optie.

   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. In de **drop-down lijst van de Frequentie**, selecteer het aantal tijdeenheden wanneer u de taak en het type van tijdeenheden wilt voorkomen. Selecteer een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Type herhaling</th> 
      <th>Beschrijving</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong> Dag </strong> </td> 
      <td> <p>De taak wordt elke dag herhaald, elke 2 dagen, elke 3 dagen enzovoort, afhankelijk van de snelheid die u kiest. U kunt taken vormen om tot elke 6de dag te herhalen. De standaardinstelling is 1 dag. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Werkdag </strong> </td> 
      <td> <p> De taak wordt elke werkdag herhaald, elke twee werkdagen, elke drie werkdagen, enzovoort, afhankelijk van de snelheid die u kiest. U kunt taken vormen om tot elke 6de werkdag te herhalen.</p> <p>Deze optie gebruikt het standaardprogramma dat door de systeembeheerder wordt bepaald, zoals die in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref"> wordt beschreven creeer een programma </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Week </strong> </td> 
      <td> <p> De taak wordt elke week herhaald, elke 2 weken, elke 3 weken enzovoort, afhankelijk van de snelheid die u kiest.</p> <p>Op <strong> herhaalt </strong> gebied, selecteer de dag van de week wanneer u elke taak wilt voorkomen. U kunt meerdere dagen selecteren. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Maand </strong> </td> 
      <td> <p>De taak wordt elke maand herhaald, elke 2 maanden, elke 3 maanden, enzovoort, afhankelijk van de snelheid die u selecteert. U kunt kiezen tussen 1 en 12 maanden. </p> <p>Op <strong> herhaalt </strong> gebied, selecteer van de volgende opties wanneer u de taak wilt voorkomen:</p> 
       <ul> 
        <li> <p><strong> elke maand op dag &lt;month date&gt; </strong> </p> <p>U kunt dagen van 1 tot 30 selecteren of u kunt <strong> laatste </strong> selecteren. U kunt bijvoorbeeld "elke maand op de 30e" selecteren. </p> </li> 
        <li> <p><strong> elke maand op &lt;number&gt; &lt;dag van de week&gt; </strong> </p> <p>In het eerste drop-down menu, kunt u een aantal tussen 1 en 4 voor het aantal van de week in de maand selecteren, of u kunt "laatste"selecteren. </p> <p>In het tweede drop-down menu, kunt u om het even welke dag van de week selecteren. </p> <p>U kunt bijvoorbeeld "elke maand op de tweede dinsdag" selecteren. </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Als u een Uitzondering van het Programma verbonden aan het programma van het project hebt, kunnen de terugkomende taken niet tijdens de uitzondering beginnen. De terugkomende taken die tijdens de planningsuitzondering voorkomen zijn gepland om op de eerste werkdag te beginnen die de uitzondering volgt. Voor meer informatie over planningsuitzonderingen, zie het artikel [&#x200B; een programma &#x200B;](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.

1. Op **begint** gebied, selecteer de datum en de tijd wanneer u de terugkomende taken wilt beginnen.
1. Op **beëindigt** gebied, selecteer de datum en de tijd wanneer u de terugkomende taken wilt voltooien

   of

   Selecteer **na `<number>` voorkomen** om erop te wijzen hoe vaak de terugkomende taak zou moeten voorkomen. Workfront maakt hetzelfde aantal herhalingen voor de taken als het nummer dat u in dit veld opgeeft.

1. Klik **creëren Taak.**

   De takenlijst wordt weergegeven. De terugkomende taak wordt gecreeerd als ouder, en alle recurrences zijn zijn zijn kinderen. Workfront heeft de namen van de onderliggende taken automatisch gegenereerd. Hierbij wordt de naam gebruikt die u voor het bovenliggende onderdeel hebt opgegeven, gevolgd door een getal. De terugkomende taken worden geplaatst aan het eind van de taaklijst.

   Voor meer informatie over welke gebieden auto-gevuld van de ouder terugkomende taak zijn, zie [&#x200B; Terugkerende takenoverzicht &#x200B;](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. (Optioneel) Wijzig elke terugkerende taak op dezelfde manier als elke andere taak in het project.

   U kunt bijvoorbeeld toewijzingen, voordecessors, tijdsduur toevoegen en andere informatie over de taak wijzigen, inclusief aangepaste velden.

   >[!IMPORTANT]
   >
   >Het aanpassen van de bovenliggende recidieven nadat de kinderen individueel zijn aangepast kan leiden tot verschillende informatie tussen de kinderen of tussen de kinderen en de ouder. Voor meer informatie, zie [&#x200B; Terugkerende takenoverzicht &#x200B;](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).
