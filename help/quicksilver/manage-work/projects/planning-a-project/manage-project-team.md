---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Het projectteam beheren
description: Het team van het Project bestaat uit gebruikers die met het project worden geassocieerd. De leden van de vertoning van het Team van het Project in de sectie van Mensen van het project.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# Het projectteam beheren

Het team van het Project bestaat uit gebruikers die met het project worden geassocieerd. De leden van de vertoning van het Team van het Project in de sectie van Mensen van het project.

## Toegangsvereisten

<!--drafted for P&P:
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
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>View or higher access to Users</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten bewerken</p> <p>Toegang tot gebruikers weergeven of vergroten</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening of hoger aan het project</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Gebruikers toevoegen aan een projectteam

Wanneer u gebruikers aan het projectteam toevoegt, krijgen zij de toestemmingen van de Mening over het project en de taken, de kwesties, en de documenten van het project. Zie het artikel voor meer informatie [Overzicht van het projectteam](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>De gebruikers op het Team van het Project worden niet automatisch toegevoegd aan de hulpmiddelen van het middelbeheer voor het project.

U kunt gebruikers aan het projectteam op de volgende manieren toevoegen:

* [Automatisch gebruikers toevoegen aan een projectteam](#automatically-add-users-to-a-project-team)
* [Voeg handmatig gebruikers toe aan een projectteam](#manually-add-users-to-a-project-team)

### Automatisch gebruikers toevoegen aan een projectteam {#automatically-add-users-to-a-project-team}

De gebruikers die de volgende rollen op het project vervullen worden automatisch toegevoegd aan het projectteam en in de sectie van Mensen verschijnen wanneer het project wordt gecreeerd:

* De maker van het project
* De eigenaar van het project
* De projectsponsor

De gebruikers worden ook automatisch toegevoegd aan het projectteam wanneer zij aan het volgende worden toegewezen:

* Taken
* Problemen

### Voeg handmatig gebruikers toe aan een projectteam {#manually-add-users-to-a-project-team}

Als de gebruikers die geen rol op het project vervullen over bepaalde updates of veranderingen tijdens het leven van het project op de hoogte willen worden gebracht, kunt u hen aan het projectteam manueel toevoegen.

Voor meer informatie over welke berichten voor gebruikers op het projectteam kunnen worden toegelaten, zie [Gebeurtenismeldingen beschikbaar in Adobe Workfront](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

<!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

1. Ga naar het project u gebruikers aan wilt toevoegen.

1. Klikken **Mensen** in het linkerdeelvenster. Mogelijk moet u op **Meer weergeven** eerst.

1. Klikken **Gebruikers toevoegen**.

   De Add gebruikers aan de dialoogdoos van het Team van het Project toont.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. In de **Gebruikers toevoegen** typt u de naam van een actieve Workfront-gebruiker die u aan het projectteam wilt toevoegen. Klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.

   Herhaal deze stap om meerdere gebruikers aan het projectteam toe te voegen. De gebruikers moeten tot de groep behoren verbonden aan het project.

   >[!TIP]
   >
   >* U kunt geen gebruikers toevoegen door hun teams, groepen, bedrijven, of baanrollen toe te voegen.
   >* Terwijl u de gebruikers toevoegt, ziet u de avatar, de primaire rol van de gebruiker en hun e-mailadres om onderscheid te maken tussen gebruikers met identieke namen. Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze toevoegt.
   >
   >  De instelling Contactinfo weergeven moet zijn ingeschakeld op uw toegangsniveau zodat gebruikers de e-mails van gebruikers kunnen bekijken. Zie voor meer informatie [Toegang verlenen aan gebruikers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


1. Klikken **Toevoegen**.

   De gebruikers krijgen de toestemmingen van de Mening aan het project en ontvangen berichten over het project als deel van het projectteam.

## Gebruikers verwijderen uit een projectteam

Wanneer u gebruikers uit hun rollen op het project verwijdert, blijven zij deel van het projectteam.

Als u een gebruiker uit het projectteam verwijdert en de gebruiker aan taken of kwesties in het project wordt toegewezen, wordt de gebruiker unassigned van de taken en de kwesties die niet worden voltooid. In dit geval worden de taken en uitgaven teruggezet naar het gedeelte Niet toegewezen werk in de werklastbalans.

De gebruikers die aan voltooide taken en kwesties worden toegewezen blijven toegewezen zelfs nadat u hen uit het projectteam verwijdert.

Voor meer informatie over het verwijderen van gebruikers uit het projectteam, zie [Gebruikers uit projecten verwijderen](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).
