---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Artikelen toevoegen aan een bestaande herhaling
description: U kunt op verschillende manieren artikelen aan een herhaling toevoegen.
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Artikelen toevoegen aan een bestaande herhaling

U kunt op de volgende manieren artikelen toevoegen aan een herhaling:

* Van de backlog nadat de herhaling is gemaakt, zoals beschreven in het dialoogvenster [Artikelen van de achtergrond verplaatsen naar een herhaling of [!UICONTROL Kanban] board](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog) sectie in [De logboekregistratie voor bestanden beheren](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Van de [!UICONTROL Details] pagina van de afzonderlijke taak of uitgave
* Van een taak of uitgiftenlijst
* Uit een rapport
* Van een dashboard

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>[!UICONTROL Work] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>[!UICONTROL Worker] of hoger</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>[!UICONTROL Manage] toegang tot het project waarop het verhaal zich bevindt</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Begrijp hoe het toevoegen van artikelen takendatums beïnvloedt

Wanneer u een bestaande taak aan een herhaling toevoegt, wordt standaard de taak [!UICONTROL Planned Start Date] en [!UICONTROL Planned Completion Date] worden als volgt ingesteld:

### Taak [!UICONTROL Planned Start Date]

* De taak gebruikt de Datum van het Begin van de herhaling wanneer:

   * Het project heeft geen [!UICONTROL Planned Start Date] set.
   * De projecten [!UICONTROL Planned Start Date] is *voor* of *op* de begindatum van de herhaling.

* De taak gebruikt de projecten [!UICONTROL Planned Start Date] wanneer:

   * De projecten [!UICONTROL Planned Start Date] is *na* de begindatum van de herhaling.

### Taak [!UICONTROL Planned Completion Date]

* De taak gebruikt de Einddatum van de herhaling wanneer:

   * Het project heeft geen [!UICONTROL Planned Completion Date] set.
   * De projecten [!UICONTROL Planned Start Date] is *voor of op* de begindatum van de herhaling of de projectnaam [!UICONTROL Planned Completion Date] is *voor of op* de einddatum van de herhaling.

* De taak gebruikt de projecten [!UICONTROL Planned Completion Date] wanneer:

   * De projecten [!UICONTROL Planned Start Date] is *na* de begindatum van de herhaling en de [!UICONTROL Planned Completion Date] is *na* de einddatum van de herhaling.

U kunt de individuele teams van het Trommel vormen om de projectdata door gebrek, eerder dan de herhalingsdata te gebruiken. Zie de sectie [Configureer hoe datums worden toegepast bij het toevoegen van werkitems aan een herhaling](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) in het artikel [Scrum configureren](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Een artikel toevoegen aan een bestaande herhaling

Artikelen rechtstreeks vanuit de taak of uitgave aan een herhaling toevoegen:

>[!IMPORTANT]
>
>Nadat de taak naar de herhaling is verplaatst, kunt u het dialoogvenster [!UICONTROL Duration Type] of [!UICONTROL Task Constraint]. [!UICONTROL Duration Type] is ingesteld op [!UICONTROL Simple] en [!UICONTROL Task Constraint] is ingesteld op [!UICONTROL Fixed Dates] om de tijdlijn van de taak consistent te houden met de tijdlijn van de herhaling.

### Via het tabblad Taken of Problemen

U kunt om het even welke taak of kwestie aan om het even welke herhaling toevoegen als u hebt leidt toegang tot het project. Houd rekening met het volgende wanneer u een taak of probleem naar een herhaling verplaatst:

* Als u meerdere teams toevoegt, kan de taak of uitgave slechts op de iteratie van één team worden weergegeven. Dit is de herhaling die u kiest in stap 3 hieronder.
* Als de taak of de kwestie aan een flexibel team wordt toegewezen en aan de herhaling van een ander team wordt bewogen, verandert de teamtaak niet.
* Als de taak of de kwestie niet aan een team wordt toegewezen, wordt de taak of de kwestie toegewezen aan het team dat de herhaling bezit.
* U kunt geen bovenliggende taken aan de herhaling toevoegen. Als u onderliggende taken toevoegt, wordt de bovenliggende taak als een zwembad op het gebied van het scrum weergegeven.

1. Ga naar het project, het rapport, of het dashboard dat de taak of de kwestie bevat u aan een herhaling wilt toevoegen.
1. Selecteer een of meer taken of problemen.
1. Klik op **[!UICONTROL More]** ![](assets/more-icon.png) > **[!UICONTROL Add to Iteration]**.\
   U kunt geen taken of kwesties toewijzen die aan niet-flexibele teams worden toegewezen.

1. In de **[!UICONTROL Add Stories]** typt u de naam van de herhaling.

   >[!NOTE]
   >
   >U kunt een artikel van een bestaande herhaling naar een nieuwe herhaling verplaatsen.

1. Als u taken toevoegt, klikt u op **[!UICONTROL Add Stories]**.\
   of\
   Klik op **[!UICONTROL Add Issues]**.
