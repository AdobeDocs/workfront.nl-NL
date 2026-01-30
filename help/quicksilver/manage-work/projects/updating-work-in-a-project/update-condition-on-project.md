---
product-area: projects
navigation-topic: update-work-in-a-project
title: Voorwaarde voor bijwerken voor een project
description: De voorwaarde van een project is een vlag die op het wordt geplaatst om erop te wijzen of het werk verbonden aan het regelmatig verloopt of of u om het even welke wegblokkades hebt ontmoet. Dit is anders dan de Status van het project, die erop wijst of u actief aan het of niet werkt.
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 0%

---

# Voorwaarde voor bijwerken voor een project

De voorwaarde van een project is een vlag die op het wordt geplaatst om erop te wijzen of het werk verbonden aan het regelmatig verloopt of of u om het even welke wegblokkades hebt ontmoet. Dit is anders dan de Status van het project, die erop wijst of u actief aan het of niet werkt.

U kunt de Voorwaarde van een project of automatisch of manueel plaatsen. Als u de voorwaarde van een project handmatig wilt wijzigen, moet u de eigenaar van het project zijn of over beheerrechten beschikken.

De beheerder van Adobe Workfront kan douaneVoorwaarden voor uw milieu tot stand brengen, zoals die in [&#x200B; wordt beschreven creeer of geef een douanetoewijzing &#x200B;](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md) uit.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td><p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
  <p>Standard</p>
   <p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten weergeven of vergroten</p> <p>Toegang tot taken en problemen bewerken </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven voor taken en uitgaven om hun voorwaarde weer te geven</p>
   <p>Machtigingen beheren voor taken en uitgaven om de voorwaarde bij te werken</p>
     </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the new licenses:
  <p>Standard</p>
   
   For current licenses:
   <ul><li><p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
     </td> 
  </tr> 
 </tbody> 
</table>-->

## De voorwaarde automatisch instellen

Het automatisch plaatsen van de Voorwaarde van een project wordt bepaald door het Type van Voorwaarde van het project. Het voorwaardetype moet aan de Status van de Voortgang voor Workfront worden geplaatst om de Voorwaarde van het Project automatisch te plaatsen.

Uw Workfront of de beheerder van de Groep bepaalt het gebrek van het gebied van het Type van Voorwaarde voor nieuwe projecten in uw systeem wanneer het plaatsen van projectvoorkeur in het gebied van de Opstelling. Voor meer informatie, zie [&#x200B; systeem-brede projectvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

Wanneer u een project creeert, wordt de Voorwaarde van het project automatisch geplaatst om de Voortgangsstatus van het project op dat ogenblik aan te passen. De status van de voortgang van het project is gebaseerd op de voortgang van de taken van het project.

Voor informatie over projectvoorwaarden en hoe zij gebaseerd op de Status van de Voortgang worden berekend, zie [&#x200B; Overzicht van de Status van de Voortgang van het Project &#x200B;](../../../manage-work/projects/planning-a-project/project-progress-status.md).

## De voorwaarde voor een project handmatig bijwerken

Als u het Type van Voorwaarde van uw project aan Handboek in plaats van de Status van de Voortgang plaatst, kunt u de Voorwaarde van een project manueel bijwerken.

1. Ga naar het project waarvoor u de Voorwaarde wilt bijwerken.
1. Klik de **sectie van de Details van het Project** in het linkerpaneel.

1. Zorg ervoor dat het **gebied van het Type van Voorwaarde** aan **Handboek** wordt geplaatst.

   ![&#x200B; de details van het Project overzicht uitgezochte voorwaarde &#x200B;](assets/project-details-overview-select-condition.png)

1. Op het **gebied van de Voorwaarde**, selecteer van de volgende opties die uw begrip van aanpassen of het werk verbonden aan het vloeiend gaat of of er om het even welke vertragingen zijn:

   * **op Doel**
   * **Bij Risico**
   * **in Problemen**

   Voor meer informatie over projectvoorwaarden, zie [&#x200B; Overzicht van het Type van de Voorwaarde en van de Voorwaarde van het Project &#x200B;](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >De voorwaarden kunnen voor uw milieu worden aangepast, zodat kunt u meer dan drie opties voor Voorwaarde in uw milieu vinden. De namen van de Voorwaarden kunnen verschillen van de hierboven vermelde. Voor informatie over het aanpassen van Voorwaarden in Workfront, zie [&#x200B; creeer of geef een douanevoorwaarde &#x200B;](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md) uit.

1. Klik **sparen Veranderingen**.
