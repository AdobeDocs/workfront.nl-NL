---
product-area: projects
navigation-topic: manage-issues
title: Problemen verwijderen
description: In Adobe Workfront kunt u problemen of aanvragen verwijderen als u hiervoor de juiste toegangsrechten en machtigingen hebt.
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '728'
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
   <td> <p>Toegang tot problemen bewerken</p> <p>De mening of hogere toegang tot Projecten en Taken</p>  <p>Voor informatie over toegang tot kwesties in uw Niveau van de Toegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Toegang verlenen tot kwesties</a>.  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het probleem beheren</p> <p>Contribute of hoger machtigingen voor het project of de taak</p> <p> Voor informatie over het verlenen van machtigingen voor uitgaven raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Een uitgave delen </a></p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt. Voor meer informatie over toegangsvereisten, zie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Overwegingen bij het verwijderen van problemen

* Uw Workfront-beheerder of groepsbeheerder moet het verwijderen van problemen inschakelen in een project met de status Voltooid in het gedeelte Projectvoorkeuren. Voor informatie over het instellen van projectvoorkeuren raadpleegt u [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Als de uitgave uren heeft geregistreerd, moet de beheerder van Workfront of een groepsbeheerder de schrapping van deze kwesties toestaan door de Voorkeur van de Taak &amp; van de Uitgave in uw instantie van Workfront te vormen. Dit is ook van toepassing wanneer u probeert om projecten te schrappen die kwesties met het programma geopende uren hebben.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  Voor meer informatie over het toelaten van de schrapping van kwesties waar de uren worden geregistreerd, zie de &quot;Schrapping&quot;sectie in [Taak- en probleemvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Het effect van het verwijderen van problemen

Wanneer u een uitgave verwijdert, heeft dit invloed op andere objecten die aan de uitgave zijn gekoppeld.

De volgende objecten die aan een uitgave zijn gekoppeld, worden ook verwijderd wanneer u een uitgave verwijdert:

* Documenten

  Het is niet mogelijk een uitgave te verwijderen waaraan een document is toegevoegd dat is uitgecheckt. Zie voor meer informatie over het uitchecken van documenten [Documenten controleren](../../../documents/managing-documents/check-out-documents.md).

* Notities
* Goedkeuringen

Afhankelijk van hoe uw Workfront of groepsbeheerder de voorkeuren voor Project, Taak of Uitgave verwijderen configureert in het dialoogvenster **Voorkeuren voor tijdpagina&#39;s en uren** van uw Workfront-exemplaar worden uren die voor de problemen zijn aangemeld, op een van de volgende manieren afgehandeld wanneer u een probleem verwijdert:

* Ga naar het project en wordt niet hersteld bij de uitgave als de uitgave later wordt hersteld.
* Verwijder het bestand en wordt hersteld bij het probleem als het probleem later wordt hersteld.

  Dit is ook van toepassing wanneer u probeert om projecten te schrappen die taken met het programma geopende uren hebben hen.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  Voor meer informatie over het vormen van de schrappingsvoorkeur voor uren het programma geopende kwesties, zie [Voorkeuren voor tijdpagina&#39;s en uren configureren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* De gebruikers die aan de kwestie of aan de uitgiftegoedkeuring worden toegewezen blijven op het projectteam.\
  Voor meer informatie over projectteams, zie [Overzicht van het projectteam](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Problemen verwijderen

* [Meerdere problemen in een project tegelijk verwijderen](#delete-multiple-issues-in-a-project-simultaneously)
* [Eén uitgave verwijderen](#delete-a-single-issue)

### Meerdere problemen in een project tegelijk verwijderen  {#delete-multiple-issues-in-a-project-simultaneously}

1. Ga naar de **Hoofdmenu**.
1. Klikken **Projecten**.
1. Klik op de projectnaam die de problemen bevat die u wilt verwijderen.
1. Klikken **Problemen** in het linkerdeelvenster.
1. Selecteer een probleem en klik op de knop **Verwijderen** pictogram ![](assets/delete.png) boven aan de lijst.

1. Als het verwijderen is toegestaan, klikt u op **Ja, verwijderen**.\
   Uw Workfront-beheerder staat mogelijk niet toe dat problemen worden verwijderd waarvoor uren zijn geregistreerd.\
   Voor meer informatie over de toegang en de toestemmingen nodig om een kwestie te schrappen, zie [Problemen verwijderen](#access-and-permissions-needed).

### Eén uitgave verwijderen {#delete-a-single-issue}

{{step1-to-projects}}

1. Klik de projectnaam die de kwestie bevat u wilt schrappen.
1. Klikken **Problemen** in het linkerdeelvenster.

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. Klik op de naam van het probleem dat u wilt verwijderen.
1. Klik op de knop **Meer** rechts van de naam van de uitgave.

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

1. Klikken **Probleem verwijderen**.
1. Als het verwijderen is toegestaan, klikt u op **Ja, verwijderen**.

   Uw Workfront-beheerder staat mogelijk niet toe dat problemen worden verwijderd waarvoor uren zijn geregistreerd.\
   Voor meer informatie over de toegang en de toestemmingen nodig om een kwestie te schrappen, zie [Problemen verwijderen](#access-and-permissions-needed).

## Verwijderde problemen herstellen

Een Workfront of groepsbeheerder kan de problemen binnen 30 dagen nadat ze zijn verwijderd, herstellen. Ga voor meer informatie over het herstellen van objecten in Workfront naar [Verwijderde items herstellen](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
