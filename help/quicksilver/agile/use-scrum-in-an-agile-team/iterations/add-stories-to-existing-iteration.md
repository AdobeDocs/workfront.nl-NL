---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Artikelen toevoegen aan een bestaande herhaling
description: U kunt op verschillende manieren artikelen aan een herhaling toevoegen.
author: Jenny
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Artikelen toevoegen aan een bestaande herhaling

U kunt op de volgende manieren artikelen toevoegen aan een herhaling:

* Van de achterstand nadat de herhaling wordt gecreeerd, zoals die in [ worden beschreven verhalen van de beweging van de achterstand aan een herhaling of [!UICONTROL Kanban] raad ](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or--board) sectie in [ beheert de Begeleidende backlog ](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Van de [!UICONTROL Details] pagina van de individuele taak of kwestie
* Van een taak of uitgiftenlijst
* Uit een rapport
* Van een dashboard

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p> 
   <p>Werk of hoger</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>Toegang beheren tot het project waarop het artikel zich bevindt </td> 
  </tr>
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Begrijp hoe het toevoegen van artikelen takendatums beïnvloedt

Wanneer u een bestaande taak aan een herhaling toevoegt, worden standaard de taakopties [!UICONTROL Planned Start Date] en [!UICONTROL Planned Completion Date] als volgt ingesteld:

### Taak [!UICONTROL Planned Start Date]

* De taak gebruikt de Datum van het Begin van de herhaling wanneer:

   * Het project heeft geen [!UICONTROL Planned Start Date] set.
   * Het project [!UICONTROL Planned Start Date] is *vóór* of *op* de de begindatum van de herhaling.

* De taak gebruikt [!UICONTROL Planned Start Date] van het project wanneer:

   * Het project [!UICONTROL Planned Start Date] is *na* de de begindatum van de herhaling.

### Taak [!UICONTROL Planned Completion Date]

* De taak gebruikt de Einddatum van de herhaling wanneer:

   * Het project heeft geen [!UICONTROL Planned Completion Date] set.
   * Het project [!UICONTROL Planned Start Date] is *vóór of op* de Datum van het Begin van de herhaling of [!UICONTROL Planned Completion Date] is van het Project *vóór of op* de Datum van het Eind van de herhaling.

* De taak gebruikt [!UICONTROL Planned Completion Date] van het project wanneer:

   * Het project [!UICONTROL Planned Start Date] is *na* de Datum van het Begin van de herhaling en het project [!UICONTROL Planned Completion Date] is *na* de Datum van het Eind van de herhaling.

U kunt de individuele teams van het Trommel vormen om de projectdata door gebrek, eerder dan de herhalingsdata te gebruiken. Voor informatie, zie de sectie [ vormen hoe de data worden toegepast wanneer het toevoegen van het werkpunten aan een herhaling ](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) in artikel [ Scrum ](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md) vormt.

## Een artikel toevoegen aan een bestaande herhaling

U kunt om het even welke taak of kwestie aan om het even welke herhaling toevoegen als u hebt leidt toegang tot het project. Houd rekening met het volgende wanneer u een taak of probleem naar een herhaling verplaatst:

* Als u meerdere teams toevoegt, kan de taak of uitgave slechts op de iteratie van één team worden weergegeven. Dit is de herhaling die u kiest in stap 3 hieronder.
* Als de taak of de kwestie aan een flexibel team wordt toegewezen en aan de herhaling van een ander team wordt bewogen, verandert de teamtaak niet.
* Als de taak of de kwestie niet aan een team wordt toegewezen, wordt de taak of de kwestie toegewezen aan het team dat de herhaling bezit.
* U kunt geen bovenliggende taken aan de herhaling toevoegen. Als u onderliggende taken toevoegt, wordt de bovenliggende taak als een zwembad op het gebied van het scrum weergegeven.

>[!IMPORTANT]
>
>Nadat de taak naar de herhaling is verplaatst, kunt u [!UICONTROL Duration Type] of [!UICONTROL Task Constraint] niet meer bijwerken. [!UICONTROL Duration Type] is ingesteld op [!UICONTROL Simple] en [!UICONTROL Task Constraint] is ingesteld op [!UICONTROL Fixed Dates] om de tijdlijn van de taak consistent te houden met de tijdlijn van de herhaling.

1. Open de taak of kwestie u aan een herhaling wilt toevoegen.
of
Ga naar het project, het rapport, of het dashboard dat de taak of de kwestie bevat u aan een herhaling wilt toevoegen. Selecteer vervolgens een of meer taken of problemen.

1. Klik **[!UICONTROL More]** ![ Meer pictogram ](assets/more-icon.png) > **[!UICONTROL Add to Iteration]**.
U kunt geen taken of kwesties toewijzen die aan niet-flexibele teams worden toegewezen.

1. Typ in het vak **[!UICONTROL Add To]** de naam van de herhaling en selecteer deze wanneer deze in de lijst wordt weergegeven.

   >[!NOTE]
   >
   >U kunt een artikel van een bestaande herhaling naar een nieuwe herhaling verplaatsen.

1. Klik op **[!UICONTROL Add]**.
