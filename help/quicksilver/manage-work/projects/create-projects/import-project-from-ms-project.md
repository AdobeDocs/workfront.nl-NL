---
product-area: projects
navigation-topic: create-projects
title: Een project importeren uit Microsoft Project
description: U kunt projecten van het Project van Microsoft in Adobe Workfront invoeren en al uw projecten in één toepassing beheren. Telkens wanneer u een project van het Project van Microsoft invoert, wordt een nieuw project gecreeerd in Workfront.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

# Een project importeren uit Microsoft Project

<!-- Audited: 10/2025 -->

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
   <td role="rowheader">Configuratie op toegangsniveau</td> 
   <td> <p>Toegang tot projecten bewerken</p> 
   <p>Als u een project toevoegt aan een portfolio of programma, moet u toegang tot portfolio's en programma's hebben.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Wanneer u een project maakt, ontvangt u automatisch beheermachtigingen voor het project</p>
   <p>Als u een project toevoegt aan een portfolio of programma, moet u beheermachtigingen hebben voor het portfolio en het programma.</p>
   </td> 
    </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--old permissions model: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p> 
   Or
   <p>Current: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> </td> 
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

   * Klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, of het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, als beschikbaar, dan klik **Projecten** en breid **Nieuw Project** uit.
   * Ga naar een portefeuille, dan breid **Nieuw Project** uit.
   * Ga naar een programma, dan breid **Nieuw Project** uit.
   * Als u een groepsbeheerder bent, kunt u een project in de **sectie van Projecten** van een groep tot stand brengen u beheert. Voor meer informatie, zie [&#x200B; tot stand brengen en wijzigen de projecten van een groep &#x200B;](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Klik **het Project van MS van de Invoer**.

   ![&#x200B; Nieuwe projectdropdown &#x200B;](assets/import-ms-project-option.png)

   Het **vakje van het Dossier van de Invoer MS** opent.

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
