---
product-area: projects
navigation-topic: create-projects
title: Een project importeren uit Microsoft Project
description: U kunt projecten van het Project van Microsoft in Adobe Workfront invoeren en al uw projecten in één toepassing beheren. Telkens wanneer u een project van het Project van Microsoft invoert, wordt een nieuw project gecreeerd in Workfront.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: b38c98ec79617a78c76510bcb109da2ff83247af
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 0%

---

# Een project importeren uit Microsoft Project

<!-- Audited: 4/2025 -->

U kunt projecten van het Project van Microsoft in Adobe Workfront invoeren en al uw projecten in één toepassing beheren. Telkens wanneer u een project van het Project van Microsoft invoert, wordt een nieuw project gecreeerd in Workfront.

>[!IMPORTANT]
>
>Niet alle Microsoft-projectvelden worden overgedragen naar Workfront.
>
>Voor meer informatie over de verenigbaarheid van gebieden tussen het Project van Workfront en van Microsoft, zie [&#x200B; de gebieden van het Project van Microsoft van de Kaart aan de projecten van Adobe Workfront &#x200B;](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Nieuw: Standaard </p> 
   of
   <p>Huidig: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau</td> 
   <td> <p>Toegang tot projecten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Wanneer u een project maakt, ontvangt u automatisch beheermachtigingen voor het project </p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

U kunt een project van het **gebied van Projecten** in het **Belangrijkste Menu**, of van het **gebied van Projecten** van een portefeuille of een programma tot stand brengen.

1. Meld u aan bij Microsoft Project en open een project waaruit u wilt importeren in Workfront.
1. Klik **Dossier**, dan **sparen als** om het project als .xml- dossier te bewaren.

1. Meld u aan bij Workfront.
1. Voer een van de volgende handelingen uit:

   * Klik het **Belangrijkste pictogram van het Menu** ![&#x200B; Belangrijkste pictogram van het Menu &#x200B;](assets/main-menu-icon.png) in de hoger-juiste hoek van Workfront, of klik de **Belangrijkste Lijnen van het Menu** ![&#x200B; Belangrijkste Menu &#x200B;](assets/lines-main-menu.png) in de upper-left hoek, als beschikbaar, klik **Projecten**, dan breid **Nieuw Project** uit.
   * Ga naar een portefeuille, dan breid **Nieuw Project** uit.
   * Ga naar een programma, dan breid **Nieuw Project** uit.
   * Als u een groepsbeheerder bent, kunt u een project in de **sectie van Projecten** van een groep tot stand brengen u beheert. Voor meer informatie, zie [&#x200B; tot stand brengen en wijzigen de projecten van een groep &#x200B;](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Klik **het Project van MS van de Invoer**. Het **de dialoogvakje van het Dossier van de Invoer MS** verschijnt.

   ![&#x200B; Nieuwe projectdropdown &#x200B;](assets/import-ms-project-option.png)

1. Klik **Uitgezochte Dossier**, dan doorblader voor het .xml- dossier op uw computer die u van het Project van Microsoft uitvoerde.
1. Het geselecteerde bestand importeren. Workfront begint het importproces en maakt een nieuw project op basis van het bestand dat is geëxporteerd uit Microsoft Project.

   Nadat het importproces is voltooid, wordt u naar de nieuwe projectpagina geleid die een bevestiging toont dat de import is voltooid.

   >[!NOTE]
   >
   >Workfront heeft een tijdlimiet van 15 minuten voor het uploaden van bestanden. Als het uploaden van het bestand langer duurt dan dat, raden we u aan uw project in kleinere projecten op te delen en afzonderlijk te importeren. Zodra zij in Workfront zijn ingevoerd, verplaats de taken van één project naar het andere project om hen in één project te combineren. Voor informatie bij het bewegen van taken, zie [&#x200B; de taken van de Beweging &#x200B;](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. (Optioneel) Ga door met het bewerken van het project in Workfront. Voor informatie over het uitgeven van projecten, zie [&#x200B; projecten &#x200B;](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.


   >[!NOTE]
   >
   >Het statuut van een nieuw die project van een malplaatje wordt gecreeerd beantwoordt met de status door uw beheerder van Workfront in het **wordt bepaald gebied van de Voorkeur van het Project** of door een groepsbeheerder in het **gebied van de Voorkeur van het Project van de Groep**. Voor informatie over het vormen van projectvoorkeur, zie [&#x200B; systeem-brede projectvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.
