---
product-area: projects
navigation-topic: create-projects
title: Een project importeren uit Microsoft Project
description: U kunt projecten van het Project van Microsoft in Adobe Workfront invoeren en al uw projecten in één toepassing beheren. Telkens wanneer u een project van het Project van Microsoft invoert, wordt een nieuw project gecreeerd in Workfront.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Een project importeren uit Microsoft Project

U kunt projecten van het Project van Microsoft in Adobe Workfront invoeren en al uw projecten in één toepassing beheren. Telkens wanneer u een project van het Project van Microsoft invoert, wordt een nieuw project gecreeerd in Workfront.

>[!IMPORTANT]
>
>Niet alle Microsoft-projectvelden worden overgedragen naar Workfront.
>
>Ga voor meer informatie over de compatibiliteit van velden tussen Workfront en Microsoft Project naar [Microsoft-projectvelden toewijzen aan Adobe Workfront-projecten](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## Toegangsvereisten

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
   <td> <p>Nieuwe licentie: standaard </p> 
   of
   <p>Huidige licentie: abonnement </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau*</td> 
   <td> <p>Toegang tot projecten bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over toegang tot projecten, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Toegang verlenen tot projecten</a>. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Wanneer u een project maakt, ontvangt u automatisch beheermachtigingen voor het project </p> <p> Zie voor informatie over projectmachtigingen <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Een project delen in Adobe Workfront</a>.</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

<!--old permissions model: 

You must have the following access to perform the steps in this article:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## Een project maken van een MS-project

U kunt een project van het gebied van Projecten in het Belangrijkste Menu, of van het gebied van Projecten van een portefeuille of een programma tot stand brengen.

1. Ga naar Microsoft Project en open een project waaruit u wilt importeren in Workfront.
1. Klikken **Bestand** vervolgens **Opslaan als** om het project als .xml- dossier op te slaan.

1. Meld u aan bij Workfront.
1. Voer een van de volgende handelingen uit:

   * Klik op de knop **Hoofdmenu** ![](assets/main-menu-icon.png), klikt u op **Projecten** vervolgens uitvouwen **Nieuw project**.
   * Naar een portfolio gaan en vervolgens uitvouwen **Nieuw project**.
   * Naar een programma gaan en vervolgens uitvouwen **Nieuw project**.
   * Als u een groepsbeheerder bent, kunt u een project in de sectie van Projecten van een groep ook tot stand brengen u beheert. Zie voor meer informatie [Projecten van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Kies de optie **MS-project importeren** -optie.

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. Klikken **Bestand selecteren** Blader vervolgens naar het .xml-bestand op uw computer dat u uit Microsoft Project hebt geëxporteerd.
1. Het geselecteerde bestand importeren.

   Workfront begint het importproces en maakt een nieuw project op basis van het bestand dat is geëxporteerd uit Microsoft Project.

   Nadat het importproces is voltooid, wordt u naar de nieuwe projectpagina geleid die een bevestiging toont dat de import is voltooid.

   >[!NOTE]
   >
   >Workfront heeft een tijdlimiet van 15 minuten voor het uploaden van bestanden. Als het uploaden van het bestand langer duurt dan dat, raden we u aan uw project in kleinere projecten op te delen en afzonderlijk te importeren. Zodra zij in Workfront zijn ingevoerd, verplaats de taken van één project naar het andere project om hen in één project te combineren. Voor informatie over het verplaatsen van taken raadpleegt u [Taken verplaatsen](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. (Optioneel) Ga door met het bewerken van het project in Workfront. Zie voor informatie over het bewerken van projecten [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).

   De status van een nieuw project dat van een malplaatje wordt gecreeerd beantwoordt aan de status door uw beheerder van Workfront in het gebied van de Voorkeur van het Project of door een groepsbeheerder in het gebied van de Voorkeur van het Project van de Groep wordt bepaald. Voor informatie over het vormen van projectvoorkeur, zie [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
