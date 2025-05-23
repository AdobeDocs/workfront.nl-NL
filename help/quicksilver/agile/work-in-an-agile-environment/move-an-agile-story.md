---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Een flexibel artikel verplaatsen
description: U kunt een flexibel artikel verplaatsen naar een andere herhaling (voor Scrum-teams) of naar de achtergrond (voor Kanban- en Scrum-teams).
author: Lisa
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
source-git-commit: 68aafe63ff8b60a542ed9dd0900b3742c26a1e4f
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Een stapel artikel verplaatsen

U kunt een flexibel artikel verplaatsen naar een andere herhaling (voor Scrum-teams) of naar de achtergrond (voor Kanban- en Scrum-teams).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td>[!UICONTROL Manage] toegang tot het artikel</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een artikel van een iteratie of Kanban-bord naar de achtergrond verplaatsen

1. Ga naar de iteratie of het Kanban-bord met het artikel dat u naar de achtergrond wilt verplaatsen.
1. Klik op de herhalingskop boven aan de pagina.
1. Selecteer op het tabblad **[!UICONTROL Stories]** de artikelen die u wilt verplaatsen.
1. Klik op **[!UICONTROL More]** > **[!UICONTROL Move to]** . Het dialoogvenster **[!UICONTROL Move To]** wordt weergegeven.

   ![ de dialoog van het Artikel van de Beweging ](assets/iteration-story-move.png)

1. Selecteer **team_name Achterlog**. In het bovenstaande voorbeeld, is de teamnaam **Marketing**.

1. Klik op **[!UICONTROL Move]**.

## Een artikel naar een andere herhaling verplaatsen

U kunt een verhaal naar een verschillende herhaling voor uw team van het Trommel verplaatsen als u een systeembeheerder of een lid van het team bent de herhaling met wordt geassocieerd.

>[!NOTE]
>
> De optie **[!UICONTROL Move to]** is niet beschikbaar voor bovenliggende artikelen in een herhaling. U kunt subtaken alleen naar een andere herhaling verplaatsen.


1. Ga naar de herhaling die het artikel bevat dat u wilt verplaatsen.
1. Klik op de herhalingskop boven aan de pagina.
1. Selecteer op het tabblad **[!UICONTROL Stories]** de artikelen die u wilt verplaatsen.
1. Klik op **[!UICONTROL More]** > **[!UICONTROL Move to]** . Het dialoogvenster **[!UICONTROL Move To]** wordt weergegeven.

   ![ de dialoog van het Artikel van de Beweging ](assets/iteration-story-move.png)

1. Selecteer **[!UICONTROL Another Iteration]** .
1. Selecteer in het keuzemenu dat wordt weergegeven de herhaling waarnaar u het artikel wilt verplaatsen.

   >[!NOTE]
   >
   >Het werkitem [!UICONTROL Planned Start Date] en [!UICONTROL Planned Completion Date] worden beïnvloed door een instelling op de pagina [!UICONTROL Edit Team] . Voor informatie, zie de sectie [[!UICONTROL Configure] hoe de data worden toegepast wanneer het toevoegen van het werkpunten aan een herhaling ](../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) in het artikel [ vormen de Trommel ](../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Klik op **[!UICONTROL Move]**.
