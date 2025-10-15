---
product-area: projects
navigation-topic: manage-issues
title: Problemen verwijderen
description: In Adobe Workfront kunt u problemen of aanvragen verwijderen als u hiervoor de juiste toegangsrechten en machtigingen hebt en als u merkt dat deze niet langer nodig zijn. We raden u aan deze bestanden te sluiten in plaats van ze te verwijderen, zodat u de nauwkeurigheid van uw projecten kunt behouden.
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# Problemen verwijderen

<!--Audited: 08/2025-->

In Adobe Workfront kunt u problemen of aanvragen verwijderen als u hiervoor de juiste toegangsrechten en machtigingen hebt en als u merkt dat deze niet langer nodig zijn. We raden u aan deze bestanden te sluiten in plaats van ze te verwijderen, zodat u de nauwkeurigheid van uw projecten kunt behouden.

Workfront-beheerders kunnen verwijderde problemen herstellen.

>[!TIP]
>
>&quot;Issues&quot; en &quot;request&quot; worden door elkaar gebruikt in Workfront. U kunt kwesties over zowel projecten als taken registreren om op onvoorzien werk te wijzen dat moet worden gericht. U kunt verzoeken ook voorleggen die als kwesties op een project worden geregistreerd dat als Rij van het Verzoek wordt aangewezen.

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven. 

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
   <td> <p>Medewerker of hoger</p>
   <p>Aanvraag of hoger</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuratie op toegangsniveau</td> 
   <td> <p>Toegang tot problemen bewerken</p> <p>De mening of hogere toegang tot Projecten en Taken</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het probleem beheren</p> <p>Contribute of hoger machtigingen voor het project of de taak</p> </td> 
  </tr> 
 </tbody> 
</table>

*Voor meer informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het verwijderen van problemen

* Uw Workfront-beheerder of groepsbeheerder moet het verwijderen van problemen inschakelen in een project met de status Voltooid in het gedeelte Projectvoorkeuren.

  Voor informatie over vestiging projectvoorkeur, zie [&#x200B; systeem-brede projectvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

* Als de uitgave uren heeft geregistreerd, moet de beheerder van Workfront of een groepsbeheerder de schrapping van deze kwesties toestaan door de Voorkeur van de Taak &amp; van de Uitgave in uw instantie van Workfront te vormen. Dit is ook van toepassing wanneer u probeert om projecten te schrappen die kwesties met het programma geopende uren hebben.

  Voor meer informatie over het toelaten van de schrapping van kwesties waar de uren worden geregistreerd, zie de &quot;Schrapping&quot;sectie in [&#x200B; de taak van het hele systeem vormen en voorkeur uitgeven &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).


## Het effect van het verwijderen van problemen

Wanneer u een uitgave verwijdert, heeft dit invloed op andere objecten die aan de uitgave zijn gekoppeld.

De volgende objecten die aan een uitgave zijn gekoppeld, worden ook verwijderd wanneer u een uitgave verwijdert:

* Documenten

  Het is niet mogelijk een uitgave te verwijderen waaraan een document is toegevoegd dat is uitgecheckt. Voor meer informatie over het controleren van documenten, zie [&#x200B; Controle uit documenten &#x200B;](../../../documents/managing-documents/check-out-documents.md).

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

  Voor meer informatie over het vormen van de schrappingsvoorkeur voor uren het programma geopende kwesties, zie [&#x200B; timesheet en uurvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) vormen.

* De gebruikers die aan de kwestie of aan de uitgiftegoedkeuring worden toegewezen blijven op het projectteam.\
  Voor meer informatie over projectteams, zie [&#x200B; Overzicht van het Team van het Project &#x200B;](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Problemen verwijderen

### Meerdere problemen in een project tegelijk verwijderen  {#delete-multiple-issues-in-a-project-simultaneously}

1. Ga naar het **Belangrijkste menu**.
1. Klik **Projecten**.
1. Klik op de projectnaam die de problemen bevat die u wilt verwijderen.
1. Klik **Kwesties** in het linkerpaneel.

   Een lijst van kwesties verbonden aan het geselecteerde project toont aan het recht.
1. Selecteer één of veelvoudige kwesties in de lijst, dan klik het **pictogram van de Schrapping** pictogram van de Schrapping ![&#x200B; bij de bovenkant van de lijst.](assets/delete.png)

1. Als de schrapping wordt toegestaan, klik **Schrapping**.

   Uw Workfront-beheerder staat mogelijk niet toe dat problemen worden verwijderd waarvoor uren zijn geregistreerd.\
   Voor meer informatie over de toegang en de toestemmingen nodig om een kwestie te schrappen, zie de sectie [&#x200B; Overwegingen voor het schrappen van kwesties &#x200B;](#considerations-for-deleting-issues) in dit artikel.

### Eén uitgave verwijderen {#delete-a-single-issue}

{{step1-to-projects}}

1. Klik de projectnaam die de kwestie bevat u wilt schrappen.
1. Klik **Kwesties** in het linkerpaneel.

   ![&#x200B; sectie van Kwesties in linkerpaneel &#x200B;](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. Klik op de naam van het probleem dat u wilt verwijderen.
1. Klik het **Meer** menu rechts van de voorwaardennaam.

   ![&#x200B; Uitgave Meer menu &#x200B;](assets/qs-issue-more-menu-highlighted-350x469.png)

1. Klik **Uitgave van de Schrapping**.
1. Klik **Schrapping** aan.

   >[!NOTE]
   >
   >  Uw Workfront-beheerder staat mogelijk niet toe dat problemen worden verwijderd waarvoor uren zijn geregistreerd.\
   >  Voor meer informatie over de toegang en de toestemmingen nodig om een kwestie te schrappen, zie de sectie [&#x200B; Overwegingen voor het schrappen van kwesties &#x200B;](#considerations-for-deleting-issues) in dit artikel.

## Verwijderde problemen herstellen

Een Workfront of groepsbeheerder kan de problemen binnen 30 dagen nadat ze zijn verwijderd, herstellen.

Voor meer informatie over het herstellen van punten in Workfront, zie [&#x200B; geschrapte punten &#x200B;](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md) herstellen.
