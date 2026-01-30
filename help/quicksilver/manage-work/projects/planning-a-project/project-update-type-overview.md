---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Overzicht van het type projectupdate
description: Het updatetype van een project geeft aan hoe Adobe Workfront de tijdlijn van een project berekent. Wijzigingen in het projectplan kunnen wijzigingen in de tijdlijn van het project veroorzaken. De tijdlijn van het project moet automatisch of handmatig opnieuw worden berekend om ervoor te zorgen dat deze aan deze wijzigingen voldoet.
author: Alina
feature: Work Management
exl-id: a6394961-2ac8-4b95-aa1b-dba8108c612f
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Overzicht van het type projectupdate

Het updatetype van een project geeft aan hoe Adobe Workfront de tijdlijn van een project berekent. Wijzigingen in het projectplan kunnen wijzigingen in de tijdlijn van het project veroorzaken. De tijdlijn van het project moet automatisch of handmatig opnieuw worden berekend om ervoor te zorgen dat deze aan deze wijzigingen voldoet.

Voor informatie over het opnieuw berekenen van de projectchronologie, zie [ projectchronologie ](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md) opnieuw berekenen.

## Typen projectupdate

Er zijn vier updatetypen voor een project, afhankelijk van wanneer u Workfront wilt de projectchronologie opnieuw berekenen. Kies een updatetype in de onderstaande lijst.

Voor informatie over hoe te om het Type van Update van het project bij te werken, zie [ het Type van projectupdate ](../../../manage-work/projects/manage-projects/select-project-update-type.md) selecteren.

>[!IMPORTANT]
>
>Als de tijdlijn van een project langer is dan 15 jaar, berekent Workfront de tijdlijn niet automatisch of bij wijziging. Het updatetype van een project langer dan 15 jaar is altijd Handmatig.

* **Automatisch en op Verandering:** dit is het gebrek dat plaatst. De projectchronologie wordt bijgewerkt telkens als een verandering in het project of in een ander project voorkomt dat de chronologie van afhankelijk is. De projecttijdlijn wordt ook elke avond bijgewerkt.\
  Dit is de aanbevolen instelling omdat de tijdlijn van het project altijd up-to-date is.

  Wanneer u een taak of het project bijwerkt en een tijdlijnherberekening activeert, worden alle beschikbare datums onmiddellijk weergegeven, zodat u kunt doorgaan met werken. Voor projecten met meer dan 100 taken worden datums die langere berekeningen vereisen, grijs weergegeven.

  ![ Verduisterde Data wanneer het inlineuitgeven ](assets/dates-dimmed-when-insline-editing-350x146.png)

  Dit geeft aan dat de herberekening nog niet is voltooid en dat de datums kunnen worden gewijzigd.

* **Verandering slechts:** de projectchronologie wordt bijgewerkt telkens als een verandering in het project of in een ander project voorkomt dat de chronologie afhankelijk is; de geplande updates komen niet voor.\
  U zou deze optie kunnen willen selecteren als u zich over systeemprestaties ongerust maakt en als de veranderingen zelden in het project of in andere projecten voorkomen dat de chronologie van afhankelijk is.

* **Automatisch slechts:** de projectchronologie wordt bijgewerkt elke nacht; het wordt niet onmiddellijk bijgewerkt nadat de veranderingen worden aangebracht.\
  U zou deze optie kunnen willen selecteren als u zich over systeemprestaties ongerust maakt en als vele veranderingen elke dag in het project of in andere projecten voorkomen dat de chronologie van afhankelijk is.

  >[!NOTE]
  >
  >Een project herberekent niet automatisch elke nacht als het in de status van de Planning is. Het herberekent alleen op verandering.

* **Hand slechts:** de projectchronologie wordt bijgewerkt slechts wanneer u de optie om **Chronologie** opnieuw te berekenen, zoals die in de sectie &quot;Handmatige herberekening&quot;in de artikel [ wordt beschreven projectchronologie ](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md) opnieuw berekent.\
  U kunt deze optie selecteren als u in één keer veel wijzigingen aanbrengt in het project en u wilt dat de tijdlijnherberekening plaatsvindt nadat alle wijzigingen zijn aangebracht (in plaats van na elke afzonderlijke wijziging).
