---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Tijdlijnherberekeningen voor projecten configureren
description: Het opnieuw berekenen van chronologie staat managers toe om te zien hoe de krachten buiten het project de chronologie van het project beïnvloeden. De tijdlijn van een project verwijst naar de geplande en geplande data voor het project.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 4705c3fc76c1544f8c71e70a773432f164282abb
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# Tijdlijnherberekeningen voor projecten configureren

Het opnieuw berekenen van chronologie staat managers toe om te zien hoe de krachten buiten het project de chronologie van het project beïnvloeden. De tijdlijn van een project verwijst naar de geplande en geplande data voor het project.

Als [!DNL Adobe Workfront] beheerder, kunt u chronologie voor alle projecten in het systeem manueel opnieuw berekenen. De eigenaars van projecten kunnen chronologie voor individuele projecten manueel opnieuw berekenen. Zie voor meer informatie [Projecttijdlijnen opnieuw berekenen](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

In dit artikel wordt beschreven hoe u [!DNL Workfront] beheerder, kan bepalen hoe en wanneer [!DNL Workfront] berekent automatisch projectchronologie door projectvoorkeur in te vormen [!UICONTROL Setup] gebied.

## Toegangsvereisten

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
   <td> <p>Toegangsniveau voor systeembeheerder</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Automatische herberekeningen configureren

Als [!DNL Adobe Workfront] beheerder, kunt u vormen wanneer [!DNL Workfront] worden de projecttijdlijnen automatisch opnieuw berekend. [!DNL Workfront] U kunt projectchronologie of elke nacht opnieuw berekenen of wanneer het projectwerkingsgebied verandert, of allebei.

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek, of de [!UICONTROL **Hoofdmenu**] pictogram ![](assets/lines-main-menu.png) in de linkerbovenhoek van [!DNL Workfront], indien beschikbaar, klikt u op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik op **[!UICONTROL Project Preferences]** > **[!UICONTROL Projects].**

1. In de **[!UICONTROL Timelines]** in- of uitschakelen van een van de instellingen hieronder. Beide instellingen zijn standaard ingeschakeld.

   * **Elke avond:** [!DNL Workfront&#x200B;&#x200B;&#x200B;] herberekent de tijdlijnen eenmaal om de 24 uur, &#39;s nachts, alleen voor projecten met de status [!UICONTROL Current] en die in de afgelopen drie maanden zijn bijgewerkt. Afhankelijk van de systeembelasting en andere factoren kan de herberekeningstijd meer dan 24 uur worden uitgesteld.

     In dit geval: [!DNL Workfront] herberekent de tijdlijn voor alle projecten met een [!UICONTROL Update Type] van [!UICONTROL Automatic] of [!UICONTROL Automatic and On Change].

   * **Wanneer het bereik van een project verandert**: Voor informatie over wat een wijziging van het projectbereik is, raadpleegt u [Projecttijdlijnen opnieuw berekenen](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

     In dit geval: [!DNL Workfront] herberekent de chronologie voor alle projecten die een Type van Update van hebben [!UICONTROL Automatic and On Change] of [!UICONTROL On Change Only].
Voor informatie over de Types van projectupdate, zie [Overzicht van het type projectupdate](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Klik op **[!UICONTROL Save]**.

   De chronologie van alle projecten in het systeem herberekent automatisch gebaseerd op het Type van Update van elk project.

## Tijdlijnen opnieuw berekenen voor de gehele [!DNL Workfront] instance

U kunt de [!UICONTROL Recalculate Timeline] diagnostisch om alle chronologie in [!DNL Workfront] systeem. Hierdoor kunnen alle projectbeheerders de invloed van externe wijzigingen direct zien op zowel geplande als geplande data. Zie voor meer informatie [Diagnostiek gebruiken om geautomatiseerde processen te activeren](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
