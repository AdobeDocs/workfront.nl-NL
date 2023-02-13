---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Overzicht van het wijzigen van taaktaken
description: U kunt taken toewijzen aan of de toewijzing van taken door gebruikers, teams of taakrollen ongedaan maken. U kunt meerdere bronnen tegelijk toewijzen, of slechts één bron. U kunt één taak tegelijk toewijzen of meerdere taken in bulk.
author: Alina
feature: Work Management
exl-id: e774f2db-494d-4f93-8727-3c073e5f930b
source-git-commit: 7e77223595d3c9cf0d6592a09e893142439adb2c
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# Overzicht van het wijzigen van taaktaken

U kunt taken toewijzen aan of de toewijzing van taken door gebruikers, teams of taakrollen ongedaan maken. U kunt meerdere bronnen tegelijk toewijzen, of slechts één bron. U kunt één taak tegelijk toewijzen of meerdere taken in bulk.

>[!TIP]
>
>U kunt meerdere gebruikers, taakrollen of teams toewijzen. U kunt alleen actieve gebruikers, taakrollen en teams toewijzen.
>
>Als een gebruiker, een baanrol, of een team werd toegewezen alvorens zij werden gedeactiveerd, blijven zij toegewezen aan het het werkpunt. In dit geval raden we het volgende aan:
>
>* Wijs het werkitem opnieuw toe aan actieve bronnen.
>* Koppel de gebruikers in een gedeactiveerd team aan een actief team en wijs het het werkpunt aan het actieve team opnieuw toe.
>


Dit artikel bevat algemene informatie over het effect van het wijzigen van taaktaken. Raadpleeg de volgende artikelen voor informatie over het toewijzen van taken:

* Voor informatie over het toewijzen van taken raadpleegt u [Taken toewijzen](../../../manage-work/tasks/assign-tasks/assign-tasks.md) en [Meerdere gebruikerstoewijzingen in een takenlijst wijzigen](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

* Voor informatie over het wijzigen van taken op veelvoudige taken in het Plannende gebied, zie [Meerdere gebruikerstoewijzingen wijzigen voor taken in de planningsgebieden](../../../resource-mgmt/resource-scheduling/modify-multipl-assignments-scheduling-areas.md).
* Voor informatie over het toewijzen van taken met behulp van Workload Balancer raadpleegt u [Overzicht van het toewijzen van werk in de werklastverdeler](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Sommige informatie in dit artikel is ook van toepassing op toewijzingen aan kwesties. Voor meer informatie over het toewijzen van problemen, en extra overwegingen, zie [Overzicht van uitgaven wijzigen](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

## Wanneer moet u gebruikerstoewijzingen wijzigen voor taken

U kunt de gebruikerstaken voor taken om diverse redenen, met inbegrip van het volgende, willen wijzigen:

* Gebruikers nemen deel aan of verlaten uw team
* Een gebruiker neemt een vakantie die zich voorbij taakvervaldata uitbreidt

   >[!NOTE]
   >
   >Wanneer u gebruikers aan het werk toewijst, heeft de beschikbaarheid volgens hun planning invloed op de geplande en de verwachte taakdatum. Voor informatie over programma&#39;s, zie [Een schema maken](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Een specifieke rol of een gebruiker wordt geplaatst als ontvanger voor veelvoudige taken en u wilt snel alle punten wijzigen die aan een verschillende gebruiker of een rol moeten worden toegewezen

## Overwegingen voor veelvoudige taken aan baanrollen, teams, en gebruikers

Overweeg het volgende wanneer het toewijzen van veelvoudige middelen aan een het werkpunt:

* Gebruikers kunnen meer dan één taakrol aan hun profiel koppelen. Voor informatie over het associëren van gebruikers met baanrollen, zie [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Taken of problemen worden doorgaans eerst toegewezen aan een of meer functies of aan een team. Wanneer de projecten klaar zijn om te beginnen, zouden zij ook aan gebruikers kunnen moeten worden toegewezen.\
   Als een taak of een kwestie aan één of veelvoudige rollen wordt toegewezen en u dan ook een gebruiker toewijst, beslist Adobe Workfront welke baanrol aan de extra gebruiker (als om het even welk) te associëren volgens de volgende regels:

   * Als er slechts één taakrol is toegewezen en deze overeenkomt met de primaire rol van de gebruiker, wordt de taak of kwestie alleen toegewezen aan de gebruiker die zijn primaire rol vervult.
   * Als er veelvoudige toegewezen rollen zijn en minstens één van de rollen de secundaire rollen van de gebruiker aanpast, dan wordt de taak of de kwestie toegewezen aan de gebruiker die één van hun Andere Rollen vervult — die Workfront willekeurig selecteert als er veelvoudige gelijken zijn — evenals om het even welke extra rollen die worden toegewezen.
   * Als er een of meer toegewezen taakrollen zijn en er geen overeenkomsten met de rollen van de gebruiker zijn, dan wordt de taak of kwestie toegewezen aan zowel de rol of de rollen als aan de gebruiker.

* Als een taak of een kwestie aan een team wordt toegewezen en u ook een gebruiker toewijst, blijft de taak of de kwestie toegewezen aan zowel het team als de gebruiker.

## Hoe het verwijderen van toegewezen beïnvloedt taakuren en toewijzingspercentages

Het verwijderen van gebruikers kan taakuren en toewijzingspercentages beïnvloeden. Het effect dat het verwijderen van een gebruiker op de taak heeft hangt van het Type van Duur af dat voor de taak werd geselecteerd. Voor informatie over het Type van Duur, zie [Overzicht van het Type van Duur en van de Duur van de Taak](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Wanneer u een gebruiker uit een taak met de volgende Types van Duur schrapt:

* **Eenvoudig:** De geplande uren die aan die gebruiker worden toegewezen worden afgetrokken van het totaal van geplande uren van de taak.

   >[!IMPORTANT]
   >
   >Dit zou uw projectplan negatief kunnen beïnvloeden omdat het het totale geplande uren voor de taak en het project verandert.

* **Gedreven inspanning:** Het toewijzingspercentage verandert niet voor andere gebruikers.
* **Berekende toewijzing:** De toewijzingspercentages van andere gebruikers worden zodanig aangepast dat het totaal gelijk is aan 100%.
* **Berekend werk:** Het toewijzingspercentage verandert niet voor andere gebruikers.

## Overwegingen over het ongedaan maken van taken

U kunt toewijzingen van één taak tegelijk verwijderen of u kunt toewijzingen van meerdere taken bulksgewijs verwijderen.

Voor meer informatie over het verwijderen van taken uit taken in bulk, zie [Meerdere gebruikerstoewijzingen in een takenlijst wijzigen](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Houd rekening met het volgende wanneer u toewijzingen verwijdert uit taken:

* Wanneer u een gebruiker van een taak loskoppelt, blijft de taak toegewezen aan de baanrol die de gebruiker op de taak vervulde.
* Wanneer u een baanrol of een team van een taak unassign, blijft de taak unassigned als het niet aan andere middelen wordt toegewezen.
