---
product-area: projects
navigation-topic: manage-tasks
title: Taken verwijderen
description: U kunt taken verwijderen die mogelijk duplicaten zijn of die ten onrechte zijn gemaakt.
author: Alina
feature: Work Management
exl-id: aee5c293-e5fa-413e-9d9b-c62528941be7
source-git-commit: 7c373707f6e5ec1431e38cc0e103e25cd8cf2309
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Taken verwijderen

U kunt taken verwijderen die mogelijk duplicaten zijn of die ten onrechte zijn gemaakt.

Voor taken die historische informatie (updates, veranderingen van programma, status, of andere gebieden) hebben, adviseren wij dat u hen sluit of hen Dode merkt, in plaats van hen te schrappen. Dit helpt u de historische informatie voor uw projecten houden.

## Toegangsvereisten

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
   <td> <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot taken en projecten bewerken met toegang tot Verwijderen</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over toegang tot taken raadpleegt u <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Toegang verlenen tot taken</a>. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute-machtigingen voor het project met de mogelijkheid om taken of hoger toe te voegen</p> <p>Als u een taak maakt, ontvangt u automatisch beheermachtigingen voor de taak</p> <p> Voor informatie over taaktoestemmingen, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Een taak delen </a>. </p> <p>Voor informatie over het aanvragen van aanvullende machtigingen raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Begrijp het proces om taken te schrappen

* [Beperkingen voor het verwijderen van taken](#limitations-for-deleting-tasks)
* [Het effect van het verwijderen van taken](#the-impact-of-deleting-tasks)

### Beperkingen voor het verwijderen van taken  {#limitations-for-deleting-tasks}

* Wanneer een project de status Voltooid heeft, kunt u taken alleen verwijderen als uw Workfront-beheerder of een groepsbeheerder dit heeft toegestaan in het gebied met projectvoorkeuren. Voor informatie over het instellen van projectvoorkeuren raadpleegt u [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Als de taak uren heeft geregistreerd, moet de Workfront of groepsbeheerder de schrapping van deze taken toestaan door de Voorkeur van de Taak &amp; van de Uitgave in uw instantie van Workfront te vormen. Dit is ook van toepassing wanneer u probeert om projecten te schrappen die taken met het programma geopende uren hebben hen.

  <!--
  (NOTE: the last statement is NWE&nbsp;only; not possible in classic)
  -->

  Voor meer informatie over het toelaten van de schrapping van taken waar de uren worden geregistreerd, zie de &quot;Schrapping&quot;sectie in [Taak- en probleemvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Het effect van het verwijderen van taken {#the-impact-of-deleting-tasks}

Wanneer u een taak verwijdert, heeft dat invloed op andere objecten die aan de taak zijn gekoppeld.

De volgende objecten die aan een taak zijn gekoppeld, worden ook verwijderd wanneer u een taak verwijdert:

* Documenten

  U kunt een taak waarvoor een document is uitgecheckt, niet verwijderen. Zie voor meer informatie over het uitchecken van documenten [Documenten uitchecken](../../../documents/managing-documents/check-out-documents.md).

* Problemen
* Subtaken
* Notities
* Goedkeuringen

Afhankelijk van hoe uw beheerder van Workfront de Voorkeur van het Project, van de Taak, of van de Schrapping van de Uitgave in de Voorkeur van de Tijdopname &amp; van het Uur van uw instantie van Workfront vormt, worden de uren die voor de taken worden geregistreerd behandeld op één van de volgende manieren wanneer het schrappen van een taak:

* Ga naar het project en herstel de taak niet als de taak later wordt hersteld.
* worden verwijderd en worden op de taak hersteld als de taak later wordt hersteld.

  Dit is ook van toepassing wanneer u probeert om projecten te schrappen die taken met het programma geopende uren hebben hen.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this stays NWE; not possible in classic;)
  </MadCap:conditionalText>
  -->

  Voor meer informatie over het vormen van de schrappingsvoorkeur voor uren het programma geopende kwesties, zie [Voorkeuren voor tijdpagina&#39;s en uren configureren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* De kosten van de taak zullen naar het project worden verplaatst.

* De gebruikers die aan de taak of aan de taakgoedkeuring worden toegewezen blijven op het projectteam.

  Voor meer informatie over projectteams, zie [Overzicht van het projectteam](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Taken verwijderen

* [Meerdere taken in een project tegelijk verwijderen](#delete-multiple-tasks-in-a-project-simultaneously)
* [Eén taak verwijderen](#delete-a-single-task)

### Meerdere taken in een project tegelijk verwijderen  {#delete-multiple-tasks-in-a-project-simultaneously}

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront.

1. Klikken **Projecten**.
1. Klik op de projectnaam die de taken bevat die u wilt verwijderen.
1. Klikken **Taken** in het linkerdeelvenster.
1. Voer een van de volgende handelingen uit:

   1. (Voorwaardelijk) Als de optie **Automatisch opslaan** toggle is ingeschakeld:

      1. Selecteer de taken die u wilt verwijderen en klik vervolgens op **Meer**
      1. Klikken **Verwijderen** vervolgens **Ja, verwijderen** om de schrapping te bevestigen.

         De taken worden verwijderd.

   1. (Voorwaardelijk) Klik op de knop **Abonnementsmodus** pictogram en selecteer **Handmatig opslaan** als u de wijzigingen die u in de takenlijst aanbrengt, wilt omkeren.

      ![Handmatig opslaan selecteren](assets/manual-save-option.png)

      Ga als volgt te werk:

      1. Selecteer de taken die u wilt verwijderen.
      1. Klikken **Verwijderen**.
      1. (Optioneel) Klik op **Ongedaan maken** om de wijziging om te keren en niet de taken te verwijderen.
      1. Klikken **Opnieuw** als u de wijziging wilt behouden en de taak wilt verwijderen.
      1. Klikken **Opslaan** om de taken te verwijderen.

         Taken worden pas verwijderd nadat u de wijzigingen hebt opgeslagen.

### Eén taak verwijderen {#delete-a-single-task}

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront.

1. Klikken **Projecten**.
1. Klik op de projectnaam die de taak bevat die u wilt verwijderen.
1. Klikken **Taken** in het linkerdeelvenster.
1. Klik op de naam van de taak die u wilt verwijderen.
1. Klik op de knop **Meer** pictogram ![](assets/qs-more-menu.png)in de rechterbovenhoek.

   ![](assets/delete-tasks-task-level-nwe-350x225.png)

1. Klikken **Taak verwijderen**.
1. Als het verwijderen is toegestaan, klikt u op **Ja, verwijderen**.

   Uw Workfront-beheerder of groepsbeheerder staat mogelijk niet toe dat taken worden verwijderd waarvoor uren zijn geregistreerd.

   Voor meer informatie over de toegang en de toestemmingen nodig om een taak te schrappen, zie de sectie [Beperkingen voor het verwijderen van taken](#limitations-for-deleting-tasks) in dit artikel.

## Verwijderde taken herstellen

Een Workfront of groepsbeheerder kan taken herstellen binnen 30 dagen nadat ze zijn verwijderd, zoals beschreven in [Verwijderde items herstellen](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
