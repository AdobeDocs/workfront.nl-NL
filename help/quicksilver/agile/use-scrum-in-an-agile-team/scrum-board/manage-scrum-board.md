---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: Artikelen en problemen beheren op het schrombord
description: U kunt een artikel of uitgave van het Klembord naar een andere herhaling of naar de achtergrond verplaatsen of van het Klembord verwijderen. Wanneer u een artikel of uitgave verwijdert, wordt het artikel of de uitgave 30 dagen naar de prullenbak verplaatst en kan het alleen door de systeembeheerder worden hersteld.
author: Jenny
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Artikelen en problemen beheren op het [!UICONTROL Scrum] -bord

U kunt een artikel of uitgave van het [!UICONTROL Scrum] board naar een andere herhaling of naar de achtergrond verplaatsen, of het verwijderen van de [!UICONTROL Scrum] board. Wanneer u een artikel of uitgave verwijdert, wordt het artikel of de uitgave 30 dagen naar de prullenbak verplaatst en kan het alleen door de systeembeheerder worden hersteld.

Om een taak of een kwestie uit de herhaling te verwijderen zonder het te schrappen of het te verzenden naar de backlog, ga naar het project en verwijder het team van Ariel uit de taakkolom. Hierdoor wordt de taak of het probleem verwijderd van het Klembord, maar blijft het bestand op het project staan.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> <p>Nieuw: [!UICONTROL Standard]</p> 
   of
   <p>Huidig: [!UICONTROL Work] of hoger</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>[!UICONTROL Manage] toegang tot de taak of afgifte </td> 
  </tr>
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een artikel of uitgave vanaf het [!UICONTROL Scrum] -bord verplaatsen

{{step1-to-team}}

1. Klik het **[!UICONTROL Switch team]** pictogram van de pictogram ![ Schakelaar teampictogram ](assets/switch-team-icon.png), dan of selecteer een team van het Trommel van het drop-down menu of onderzoek naar een team in de onderzoeksbar.
1. Selecteer in het linkerdeelvenster **[!UICONTROL Iterations]** om een specifieke herhaling te kiezen of selecteer **[!UICONTROL Current Iteration]** .
1. Klik op het pictogram **[!UICONTROL More]** in het artikel of de uitgave en selecteer **[!UICONTROL Move to]** .

   ![ Schrap of beweeg verhaal van het Klembord van het Trommel ](assets/scrum-delete-move-story.png)

1. Kies in het bevestigingsbericht een van de volgende opties:

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Another iteration]</strong></td>
        <td>Selecteer deze optie om het item naar een andere herhaling te verplaatsen en kies naar welke herhaling het artikel of de uitgave wordt verplaatst. Als er geen herhalingen in de toekomst worden gedefinieerd, kunt u het item niet verplaatsen.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Backlog]</strong></td>
        <td>Selecteer deze optie om het artikel of het probleem naar de achtergrond van het team te verplaatsen.</td>
    </tr>
   </table>

   >[!NOTE]
   >
   >Het werkitem [!UICONTROL Planned Start Date] en [!UICONTROL Planned Completion Date] worden beïnvloed door een instelling op de pagina [!UICONTROL Edit Team] . Voor informatie, zie de sectie [[!UICONTROL Configure] hoe de data worden toegepast wanneer het toevoegen van het werkpunten aan een herhaling ](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) in het artikel [ vormen de Trommel ](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Klik op **[!UICONTROL Move]**.

## Een artikel of uitgave van het [!UICONTROL Scrum] -bord verwijderen

{{step1-to-team}}

1. Klik het **[!UICONTROL Switch team]** pictogram van de pictogram ![ Schakelaar teampictogram ](assets/switch-team-icon.png), dan of selecteer een team van het Trommel van het drop-down menu of onderzoek naar een team in de onderzoeksbar.
1. Selecteer in het linkerdeelvenster **[!UICONTROL Iterations]** om een specifieke herhaling te kiezen of selecteer **[!UICONTROL Current Iteration]** .
1. Klik op het pictogram **[!UICONTROL More]** in het artikel of de uitgave en selecteer **[!UICONTROL Delete Story]** of **[!UICONTROL Delete Issue]** .

   ![ Schrap of beweeg verhaal van het Klembord van het Trommel ](assets/scrum-delete-move-story.png)

1. Klik op **[!UICONTROL Yes, delete it]** in het bevestigingsbericht.
