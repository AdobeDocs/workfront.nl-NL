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
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Tijdlijnherberekeningen voor projecten configureren

Het opnieuw berekenen van chronologie staat managers toe om te zien hoe de krachten buiten het project de chronologie van het project beïnvloeden. De tijdlijn van een project verwijst naar de geplande en geplande data voor het project.

Als [!DNL Adobe Workfront] beheerder, kunt u chronologie voor alle projecten in het systeem manueel opnieuw berekenen. De eigenaars van projecten kunnen chronologie voor individuele projecten manueel opnieuw berekenen. Voor meer informatie, zie [ projectchronologie ](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md) opnieuw berekenen.

In dit artikel wordt beschreven hoe u als [!DNL Workfront] beheerder kunt bepalen hoe en wanneer [!DNL Workfront] automatisch projecttijdlijnen berekent door projectvoorkeuren in het [!UICONTROL Setup] -gebied te configureren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegangsniveau voor systeembeheerder</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Automatische herberekeningen configureren

Als [!DNL Adobe Workfront] -beheerder kunt u configureren wanneer [!DNL Workfront] de projecttijdlijnen automatisch opnieuw berekent. [!DNL Workfront] kan projectchronologie of elke nacht opnieuw berekenen of wanneer het projectwerkingsgebied verandert, of allebei.

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Project Preferences]** > **[!UICONTROL Projects].**

1. Schakel in de sectie **[!UICONTROL Timelines]** een van de onderstaande instellingen in of uit. Beide instellingen zijn standaard ingeschakeld.

   * **elke nacht:** [!DNL Workfront&#x200B;&#x200B;&#x200B;] herberekent chronologie eens om de 24 uur, bij nacht, slechts voor projecten die een status van [!UICONTROL Current] hebben en die in de afgelopen drie maanden werden bijgewerkt. Afhankelijk van de systeembelasting en andere factoren kan de herberekeningstijd meer dan 24 uur worden uitgesteld.

     In dit geval berekent [!DNL Workfront] de tijdlijn opnieuw voor alle projecten met een [!UICONTROL Update Type] van [!UICONTROL Automatic] of [!UICONTROL Automatic and On Change] .

   * **wanneer het werkingsgebied van een project** verandert: Voor informatie over wat een verandering van het projectwerkingsgebied vormt, zie [ projectchronologie ](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md) opnieuw berekenen.

     In dit geval berekent [!DNL Workfront] de tijdlijn opnieuw voor alle projecten met het updatetype [!UICONTROL Automatic and On Change] of [!UICONTROL On Change Only] .
Voor informatie over de Types van Update van het project, zie [ Overzicht van het Type van Update van het Project ](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Klik op **[!UICONTROL Save]**.

   De chronologie van alle projecten in het systeem herberekent automatisch gebaseerd op het Type van Update van elk project.

## Tijdlijnen voor de gehele [!DNL Workfront] -instantie opnieuw berekenen

U kunt de diagnose [!UICONTROL Recalculate Timeline] uitvoeren om alle tijdlijnen in het [!DNL Workfront] -systeem handmatig opnieuw te berekenen. Hierdoor kunnen alle projectbeheerders de invloed van externe wijzigingen direct zien op zowel geplande als geplande data. Voor meer informatie, zie [ Diagnose van het Gebruik om geautomatiseerde processen ](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md) teweeg te brengen.
