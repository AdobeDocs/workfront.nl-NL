---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Het projectteam beheren
description: Het team van het Project bestaat uit gebruikers die met het project worden geassocieerd. De leden van de vertoning van het Team van het Project in de sectie van Mensen van het project of op de sectie van Mensen van het malplaatje dat zou kunnen worden gebruikt om een project tot stand te brengen.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: 00e693fc8b35a59f6ed212bc30da7f85cc78c845
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# Het projectteam beheren

<!--take preview and production references out at production - August 7-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>

-->

Het team van het Project bestaat uit gebruikers die met het project worden geassocieerd. Voor meer informatie, zie [ Overzicht van het Team van het Project ](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md).

De leden van de vertoning van het Team van het Project in de sectie van Mensen van het project.

De gebruikers die in de sectie van Mensen van een projectmalplaatje worden getoond zullen het projectteam worden nadat het project van het malplaatje wordt gecreeerd.

De volgende gebruikers worden automatisch toegevoegd aan het projectteam, voor zowel projecten als malplaatjes:

* Eigenaar
* Sponsor
* Gebruikers die zijn toegewezen aan taken
* Gebruikers die zijn toegewezen aan problemen (alleen voor een project)

De gebruikers in het projectteam ontvangen berichten over het project. Voor meer informatie, zie [ de berichttypes van de Gebeurtenis ](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

U kunt de gebruikers in het project en de teams van het malplaatje beheren door hen (slechts voor het project) toe te voegen, hen te verwijderen, of hen te verzenden een update.

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
   <td> <p>Toegang tot projecten en sjablonen bewerken</p> <p>Toegang tot gebruikers weergeven of vergroten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening of hoger aan een project of aan een malplaatje</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old access: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Standard </p>
    <p>Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects and Templates</p> <p>View or higher access to Users</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project or to a template</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).



## Add users to a Project Team

When you add users to the project team, they gain View permissions on the project and the tasks, issues, and documents of the project. For more information, see the article [Project Team overview](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>Users on the Project Team are not automatically added to the resource management tools for the project.

You can add users to the project team in the following ways:

* [Automatically add users to a Project Team](#automatically-add-users-to-a-project-team) 
* [Manually add users to a Project Team](#manually-add-users-to-a-project-team)

### Automatically add users to a Project Team {#automatically-add-users-to-a-project-team}

The users that fulfill the following roles on the project are automatically added to the project team and appear  in the People section when the project is created:

* The creator of the project
* The project owner
* The project sponsor

Users are also automatically added to the project team when they are assigned to the following:

* Tasks
* Issues

### Manually add users to a Project Team {#manually-add-users-to-a-project-team}

If users that don't fulfill any role on the project want to be notified about certain updates or changes during the life of the project, you can manually add them to the project team. 

 For more information about what notifications can be enabled for users on the project team, see [Event notification types](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md). 

 <!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 



## Manage people on a project

1. Go to the project you want to manage the project team for.

   >[!TIP]
   >
   >You must have users assigned to tasks, issues or as stakeholders on the project to have them display in the People section.

1. Click **People** in the left panel. 

1. Click **Add users**. 

   The **Add users to Project Team** box displays.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. In the **Add users** box, begin typing the name of an active Workfront user that you want to add to the project team, then click the name when it appears in the list.

   Repeat this step to add multiple users to the project team. The users must belong to the group associated with the project. 

   >[!TIP]
   >
   >* You cannot add users by adding their teams, groups, companies, or job roles.
   >* As you add the users, notice the avatar, the user's Primary Role, and their email address to distinguish between users with identical names. Users must be associated with at least one job role to view it as you add them.
   >
   >  You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

1. Click **Add**.

   The users gain View permissions to the project and receive notifications about the project as part of the project team.

1. (Optional) If you want a user to receive a  notification when their job role is added to a task, issue, or project approval, click inside the **Job Role** column for the user, and select a job role that will be associated with the approval. 

   The users will receive notifications related to the approvals assigned to the selected job role. 

   For more information see the "Role-based approvals" section in the article [Project Team overview](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md).

1. Select one or several users in the list, then click the **Remove** icon ![Remove icon](assets/remove-icon.png) to remove them from the team. 
 
1. Click **Yes, Remove Selected Users** to confirm and remove the users.

   Users are removed and unassigned from incomplete work items.

   For more information, see the [Considerations for removing users from a project team](#considerations-for-removing-users-from-a-project-team) section in this article.
1. (Optional) To send an update for this project to users, click **Update All** to send the update to everyone on the team

   Or 

   Select one or multiple users in the list, then click **Send Update to User**.

   <!--update screen shot when they fix the bug - the text above the box needs to match the OLD box, below-->

![ verzendt update naar gebruikersdoos op het project ](assets/send-update-to-user-on-project-box-2025.png)

<!--Old UI for projects but the text above the comment box is right and matches the functionality):
   ![OLD Send update to user on a project](assets/send-update-to-user-on-project-box.png)-->

**verzendt update naar gebruiker** opent doos.

1. Voer een van de volgende handelingen uit:

   * Voeg een update toe voor de geselecteerde gebruikers.
   * Klik op het slotpictogram om de update privé te maken voor de gebruikers in uw bedrijf.
   * Geef extra gebruikers de tag om dezelfde update te ontvangen.
   * Klik **verzenden**.

   De update wordt toegevoegd aan de **sectie van Updates** van het project en alle geselecteerde gebruikers tonen als geëtiketteerde gebruikers.

   Gebruikers ontvangen mogelijk een e-mailbericht als ze hiervoor zijn ingeschakeld en ontvangen een melding in de app over de nieuwe update.

1. (Facultatief) klik het **pictogram van de Uitvoer** Uitvoer ![ om de lijst van gebruikers naar een dossier uit te voeren](assets/export-icon.png)

   of

   Selecteer gebruikers, dan klik het **pictogram van de Uitvoer** om slechts specifieke gebruikers uit te voeren.

## Personen op een sjabloon beheren

1. Ga naar het malplaatje u het projectteam voor wilt beheren.

   >[!TIP]
   >
   >U moet gebruikers hebben die aan taken of als belanghebbenden op het malplaatje worden toegewezen om hen te hebben tonen in de sectie van Mensen.

1. Klik **Mensen** in het linkerpaneel.

1. Selecteer één of verscheidene gebruikers in de lijst, dan klik **verwijderen** pictogram om hen uit het team te verwijderen.

1. Klik **ja, verwijder Geselecteerde Gebruikers** om de gebruikers te bevestigen en te verwijderen.

   De gebruikers worden verwijderd en unassigned van de malplaatjetaken.

   Voor meer informatie, zie de [ Overwegingen voor het verwijderen van gebruikers uit een sectie van het projectteam ](#considerations-for-removing-users-from-a-project-team) in dit artikel.

1. (Facultatief) om een update naar gebruikers te verzenden, klik **Update allen** om de update naar alle gebruikers in de lijst te verzenden

   of

   Selecteer één of veelvoudige gebruikers in de lijst, dan klik **verzenden Update naar Gebruiker**.

   <!--update screen shot for unshim production, notice the text above the box - it needs to say "Post an update to each person's profile"-->

   ![ verzendt update naar gebruikersdoos op malplaatje ](assets/send-update-to-user-on-template-box.png)

   **verzendt update naar gebruiker** opent doos.

1. Ga als volgt te werk:

   * Voeg een update toe voor de geselecteerde gebruikers.
   * Klik **de mensen van de Markering** om extra gebruikers te etiketteren om de zelfde update te ontvangen.
   * Selecteer de **Privé aan mijn bedrijf** optie om de update privé aan de gebruikers in uw bedrijf te maken.
   * Klik **verzenden**.

     >[!TIP]
     >
     >**Privé aan mijn bedrijf** het plaatsen is slechts beschikbaar wanneer uw profiel van Workfront met een bedrijf wordt geassocieerd.

   De update wordt toegevoegd aan de **sectie van Updates** van elk geëtiketteerd gebruikersprofiel.

   Gebruikers ontvangen mogelijk een e-mailbericht als ze hiervoor zijn ingeschakeld en ontvangen een melding in de app over de nieuwe update.

1. Klik het **pictogram van de Uitvoer** pictogram van de Uitvoer ![ om de lijst van gebruikers naar een dossier uit te voeren](assets/export-icon.png)

   of

   Selecteer gebruikers, dan klik het **pictogram van de Uitvoer** om slechts specifieke gebruikers uit te voeren.

## Overwegingen voor het verwijderen van gebruikers uit een Team van het Project

Wanneer u gebruikers uit hun rollen op het project verwijdert, blijven zij deel van het projectteam.

U moet hen uit het projectteam, uit de sectie van Mensen van het project verwijderen, voor hen ophouden ontvangend berichten die naar het projectteam worden verzonden.

Als u een gebruiker uit het projectteam verwijdert en de gebruiker aan taken of kwesties in het project wordt toegewezen, wordt de gebruiker unassigned van de taken en de kwesties die niet worden voltooid. In dit geval worden de taken en uitgaven teruggezet naar het gedeelte Niet toegewezen werk in de werklastbalans.

De gebruikers die aan voltooide taken en kwesties worden toegewezen blijven toegewezen aan de taken en de kwesties, zelfs nadat u hen uit het projectteam verwijdert.

De volgende gebruikers worden verwijderd uit hun rollen op het project wanneer u hen uit de sectie van Mensen van een project of een malplaatje verwijdert:

* Gebruikers die zijn toegewezen aan onvolledige taken
* Gebruikers die zijn toegewezen aan onvolledige problemen

De volgende gebruikers worden niet verwijderd uit hun rollen op het project wanneer u hen uit de sectie van Mensen van een project of een malplaatje verwijdert:

* Eigenaar
* Sponsor

Voor meer informatie over het verwijderen van gebruikers uit het projectteam, zie [ gebruikers uit projecten ](../../../manage-work/projects/manage-projects/remove-users-from-projects.md) verwijderen.

