---
product-area: projects
navigation-topic: manage-issues
title: Problemen verwijderen
description: In Adobe Workfront kunt u problemen of aanvragen verwijderen als u hiervoor de juiste toegangsrechten en machtigingen hebt.
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# Problemen verwijderen

<!--Audited: 01/2024-->

In Adobe Workfront kunt u problemen of aanvragen verwijderen als u hiervoor de juiste toegangsrechten en machtigingen hebt.

>[!TIP]
>
>&quot;Issues&quot; en &quot;request&quot; worden door elkaar gebruikt in Workfront. U kunt kwesties over zowel projecten als taken registreren om op onvoorzien werk te wijzen dat moet worden gericht. U kunt verzoeken ook voorleggen die als kwesties op een project worden geregistreerd dat als Rij van het Verzoek wordt aangewezen.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Nieuw: Medewerker of hoger</p>
   <p>Huidig: Verzoek of hoger</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuratie op toegangsniveau</td> 
   <td> <p>Toegang tot problemen bewerken</p> <p>De mening of hogere toegang tot Projecten en Taken</p>  <p>Voor informatie over toegang tot kwesties in uw Niveau van de Toegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref"> Toegang van de Verlening tot kwesties </a>.  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het probleem beheren</p> <p>Contribute of hoger machtigingen voor het project of de taak</p> <p> Voor informatie over het verlenen van toestemmingen aan kwesties, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref"> een kwestie delen </a></p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront. Voor meer informatie over toegangsvereisten, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Overwegingen bij het verwijderen van problemen

* Uw Workfront-beheerder of groepsbeheerder moet het verwijderen van problemen inschakelen in een project met de status Voltooid in het gedeelte Projectvoorkeuren. Voor informatie over vestiging projectvoorkeur, zie [ systeem-brede projectvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

* Als de uitgave uren heeft geregistreerd, moet de beheerder van Workfront of een groepsbeheerder de schrapping van deze kwesties toestaan door de Voorkeur van de Taak &amp; van de Uitgave in uw instantie van Workfront te vormen. Dit is ook van toepassing wanneer u probeert om projecten te schrappen die kwesties met het programma geopende uren hebben.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  Voor meer informatie over het toelaten van de schrapping van kwesties waar de uren worden geregistreerd, zie de &quot;Schrapping&quot;sectie in [ de taak van het hele systeem vormen en voorkeur uitgeven ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Het effect van het verwijderen van problemen

Wanneer u een uitgave verwijdert, heeft dit invloed op andere objecten die aan de uitgave zijn gekoppeld.

De volgende objecten die aan een uitgave zijn gekoppeld, worden ook verwijderd wanneer u een uitgave verwijdert:

* Documenten

  Het is niet mogelijk een uitgave te verwijderen waaraan een document is toegevoegd dat is uitgecheckt. Voor meer informatie over het controleren van documenten, zie [ Controle uit documenten ](../../../documents/managing-documents/check-out-documents.md).

* Notities
* Goedkeuringen

Afhankelijk van hoe uw Workfront of groepsbeheerder het Project, de Taak, of de Voorkeur van de Schrapping van de Uitgave in de **Voorkeur van de Tijdopname &amp; van het Uur** van uw instantie van Workfront vormt, worden de uren die voor de kwesties worden geregistreerd behandeld op één van de volgende manieren wanneer het schrappen van een kwestie:

* Ga naar het project en wordt niet hersteld bij de uitgave als de uitgave later wordt hersteld.
* Verwijder het bestand en wordt hersteld bij het probleem als het probleem later wordt hersteld.

  Dit is ook van toepassing wanneer u probeert om projecten te schrappen die taken met het programma geopende uren hebben hen.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  Voor meer informatie over het vormen van de schrappingsvoorkeur voor uren het programma geopende kwesties, zie [ timesheet en uurvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) vormen.

* De gebruikers die aan de kwestie of aan de uitgiftegoedkeuring worden toegewezen blijven op het projectteam.\
  Voor meer informatie over projectteams, zie [ Overzicht van het Team van het Project ](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Problemen verwijderen

* [ Schrap veelvoudige kwesties in een project gelijktijdig ](#delete-multiple-issues-in-a-project-simultaneously)
* [Eén uitgave verwijderen](#delete-a-single-issue)

### Meerdere problemen in een project tegelijk verwijderen  {#delete-multiple-issues-in-a-project-simultaneously}

1. Ga naar het **Belangrijkste menu**.
1. Klik **Projecten**.
1. Klik op de projectnaam die de problemen bevat die u wilt verwijderen.
1. Klik **Kwesties** in het linkerpaneel.
1. Selecteer een kwestie, dan klik het **pictogram van de Schrapping ![ pictogram van de Schrapping ](assets/delete.png) bij de bovenkant van de lijst.**

1. Als de schrapping wordt toegestaan, klik ja **, schrap het**.\
   Uw Workfront-beheerder staat mogelijk niet toe dat problemen worden verwijderd waarvoor uren zijn geregistreerd.\
   Voor meer informatie over de toegang en de toestemmingen nodig om een kwestie te schrappen, zie [ kwesties van de Schrapping ](#access-and-permissions-needed).

### Eén uitgave verwijderen {#delete-a-single-issue}

{{step1-to-projects}}

1. Klik de projectnaam die de kwestie bevat u wilt schrappen.
1. Klik **Kwesties** in het linkerpaneel.

   ![ pictogram van Kwesties ](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. Klik op de naam van het probleem dat u wilt verwijderen.
1. Klik het **Meer** menu rechts van de voorwaardennaam.

   ![ Uitgave Meer menu ](assets/qs-issue-more-menu-highlighted-350x469.png)

1. Klik **Uitgave van de Schrapping**.
1. Als de schrapping wordt toegestaan, klik ja **, schrap het**.

   Uw Workfront-beheerder staat mogelijk niet toe dat problemen worden verwijderd waarvoor uren zijn geregistreerd.\
   Voor meer informatie over de toegang en de toestemmingen nodig om een kwestie te schrappen, zie [ kwesties van de Schrapping ](#access-and-permissions-needed).

## Verwijderde problemen herstellen

Een Workfront of groepsbeheerder kan de problemen binnen 30 dagen nadat ze zijn verwijderd, herstellen. Voor meer informatie over het herstellen van punten in Workfront, zie [ geschrapte punten ](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md) herstellen.
