---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Tijdlijnherberekeningen voor projecten configureren
description: Het opnieuw berekenen van chronologie staat managers toe om te zien hoe de krachten buiten het project de chronologie van het project beïnvloeden. De tijdlijn van een project verwijst naar de geplande en geplande data voor het project.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Tijdlijnherberekeningen voor projecten configureren

Het opnieuw berekenen van chronologie staat managers toe om te zien hoe de krachten buiten het project de chronologie van het project beïnvloeden. De tijdlijn van een project verwijst naar de geplande en geplande data voor het project.

Als [!DNL Adobe Workfront] beheerder, kunt u chronologie voor alle projecten in het systeem manueel opnieuw berekenen. De eigenaars van projecten kunnen chronologie voor individuele projecten manueel opnieuw berekenen. Voor meer informatie, zie [&#x200B; projectchronologie &#x200B;](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md) opnieuw berekenen.

In dit artikel wordt beschreven hoe u als [!DNL Workfront] beheerder kunt bepalen hoe en wanneer [!DNL Workfront] automatisch projecttijdlijnen berekent door projectvoorkeuren in het [!UICONTROL Setup] -gebied te configureren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licentie</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Automatische herberekeningen configureren

Als [!DNL Adobe Workfront] -beheerder kunt u configureren wanneer [!DNL Workfront] de projecttijdlijnen automatisch opnieuw berekent. [!DNL Workfront] kan projectchronologie of elke nacht opnieuw berekenen of wanneer het projectwerkingsgebied verandert, of allebei.

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Project Preferences]** > **[!UICONTROL Projects].**

1. Schakel in de sectie **[!UICONTROL Timelines]** een van de onderstaande instellingen in of uit. Beide instellingen zijn standaard ingeschakeld.

   * **elke nacht:** [!DNL Workfront&#x200B;&#x200B;&#x200B;] herberekent chronologie eens om de 24 uur, bij nacht, slechts voor projecten die een status van [!UICONTROL Current] hebben en die in de afgelopen drie maanden werden bijgewerkt. Afhankelijk van de systeembelasting en andere factoren kan de herberekeningstijd meer dan 24 uur worden uitgesteld.

     In dit geval berekent [!DNL Workfront] de tijdlijn opnieuw voor alle projecten met een [!UICONTROL Update Type] van [!UICONTROL Automatic] of [!UICONTROL Automatic and On Change] .

   * **wanneer het werkingsgebied van een project** verandert: Voor informatie over wat een verandering van het projectwerkingsgebied vormt, zie [&#x200B; projectchronologie &#x200B;](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md) opnieuw berekenen.

     In dit geval berekent [!DNL Workfront] de tijdlijn opnieuw voor alle projecten met het updatetype [!UICONTROL Automatic and On Change] of [!UICONTROL On Change Only] .
Voor informatie over de Types van Update van het project, zie [&#x200B; Overzicht van het Type van Update van het Project &#x200B;](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Klik op **[!UICONTROL Save]**.

   De chronologie van alle projecten in het systeem herberekent automatisch gebaseerd op het Type van Update van elk project.

>[!IMPORTANT]
>
>Voor de milieu&#39;s van de Sandbox van de Voorproef en van de Douane verfrissen, wordt de niight herberekening onbruikbaar gemaakt, en de projectchronologie worden niet automatisch opnieuw berekend. U moet de projectchronologie voor de Voorproef en de Douane manueel opnieuw berekenen vernieuwt Sandbox milieu&#39;s. Voor informatie, zie [&#x200B; projectchronologie &#x200B;](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md) opnieuw berekenen.


## Tijdlijnen voor de gehele [!DNL Workfront] -instantie opnieuw berekenen

U kunt de diagnose [!UICONTROL Recalculate Timeline] uitvoeren om alle tijdlijnen in het [!DNL Workfront] -systeem handmatig opnieuw te berekenen. Hierdoor kunnen alle projectbeheerders de invloed van externe wijzigingen direct zien op zowel geplande als geplande data. Voor meer informatie, zie [&#x200B; Diagnose van het Gebruik om geautomatiseerde processen &#x200B;](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md) teweeg te brengen.
