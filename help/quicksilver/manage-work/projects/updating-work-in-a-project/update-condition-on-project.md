---
product-area: projects
navigation-topic: update-work-in-a-project
title: Voorwaarde voor bijwerken voor een project
description: De voorwaarde van een project is een vlag die op het wordt geplaatst om erop te wijzen of het werk verbonden aan het regelmatig verloopt of of u om het even welke wegblokkades hebt ontmoet. Dit is anders dan de Status van het project, die erop wijst of u actief aan het of niet werkt.
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---

# Voorwaarde voor bijwerken voor een project

De voorwaarde van een project is een vlag die op het wordt geplaatst om erop te wijzen of het werk verbonden aan het regelmatig verloopt of of u om het even welke wegblokkades hebt ontmoet. Dit is anders dan de Status van het project, die erop wijst of u actief aan het of niet werkt.

U kunt de Voorwaarde van een project of automatisch of manueel plaatsen. Als u de voorwaarde van een project handmatig wilt wijzigen, moet u de eigenaar van het project zijn of over beheerrechten beschikken.

De Adobe Workfront-beheerder kan aangepaste voorwaarden voor uw omgeving maken, zoals beschreven in [Een aangepaste voorwaarde maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Toegangsvereisten

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the current licenses:
  <p>Standard</p>
   
   For legacy licenses:
   <ul><li><p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
    <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Toegang tot projecten bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het project beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## De voorwaarde automatisch instellen

Het automatisch plaatsen van de Voorwaarde van een project wordt bepaald door het Type van Voorwaarde van het project. Het voorwaardetype moet aan de Status van de Voortgang voor Workfront worden geplaatst om de Voorwaarde van het Project automatisch te plaatsen.

Uw Workfront of de beheerder van de Groep bepaalt het gebrek van het gebied van het Type van Voorwaarde voor nieuwe projecten in uw systeem wanneer het plaatsen van projectvoorkeur in het gebied van de Opstelling. Zie voor meer informatie [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Wanneer u een project creeert, wordt de Voorwaarde van het project automatisch geplaatst om de Voortgangsstatus van het project op dat ogenblik aan te passen. De status van de voortgang van het project is gebaseerd op de voortgang van de taken van het project.

Voor informatie over projectvoorwaarden en hoe zij gebaseerd op de Status van de Voortgang worden berekend, zie [Overzicht van voortgang van project](../../../manage-work/projects/planning-a-project/project-progress-status.md).

## De voorwaarde voor een project handmatig bijwerken

Als u het Type van Voorwaarde van uw project aan Handboek in plaats van de Status van de Voortgang plaatst, kunt u de Voorwaarde van een project manueel bijwerken.

1. Ga naar het project waarvoor u de Voorwaarde wilt bijwerken.
1. Klik op de knop **Projectdetails** sectie.

   ![](assets/project-details-overview-edit-enabled-with-condition-shot-nwe-350x251.png)

1. Zorg ervoor dat de **Type voorwaarde** veld is ingesteld op **Handmatig**.

1. In de **Voorwaarde** in het veld selecteert u uit de volgende opties de optie die aansluit bij uw inzicht in de vraag of het bijbehorende werk vloeiend verloopt of dat er vertraging optreedt:

   * **Op doel**
   * **Risico**
   * **In problemen**

   Voor meer informatie over projectvoorwaarden, zie [Overzicht van het type Projectvoorwaarde en Voorwaarde](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >De voorwaarden kunnen voor uw milieu worden aangepast, zodat kunt u meer dan drie opties voor Voorwaarde in uw milieu vinden. De namen van de Voorwaarden kunnen verschillen van de hierboven vermelde. Voor informatie over het aanpassen van Voorwaarden in Workfront raadpleegt u [Een aangepaste voorwaarde maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. Klikken **Opslaan**.click **Wijzigingen opslaan**.
