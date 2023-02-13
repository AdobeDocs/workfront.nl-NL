---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Overzicht van het type projectupdate
description: Het updatetype van een project geeft aan hoe Adobe Workfront de tijdlijn van een project berekent. De veranderingen in het projectplan zouden veranderingen in de chronologie van het project kunnen teweegbrengen. De tijdlijn van het project moet automatisch of handmatig opnieuw worden berekend om ervoor te zorgen dat deze aan deze wijzigingen voldoet.
author: Alina
feature: Work Management
exl-id: a6394961-2ac8-4b95-aa1b-dba8108c612f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Overzicht van het type projectupdate

Het updatetype van een project geeft aan hoe Adobe Workfront de tijdlijn van een project berekent. De veranderingen in het projectplan zouden veranderingen in de chronologie van het project kunnen teweegbrengen. De tijdlijn van het project moet automatisch of handmatig opnieuw worden berekend om ervoor te zorgen dat deze aan deze wijzigingen voldoet.

Voor informatie over het opnieuw berekenen van de projecttijdlijn raadpleegt u [Projecttijdlijnen opnieuw berekenen](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

## Typen projectupdate

Er zijn vier updatetypen voor een project, afhankelijk van wanneer u Workfront wilt de projectchronologie opnieuw berekenen. Kies een updatetype in de onderstaande lijst.

Voor informatie over hoe te om het Type van Update van het project bij te werken, zie [Selecteer het Type van projectupdate](../../../manage-work/projects/manage-projects/select-project-update-type.md).

>[!IMPORTANT]
>
>Als de tijdlijn van een project langer is dan 15 jaar, berekent Workfront de tijdlijn niet automatisch of bij wijziging. Het updatetype van een project langer dan 15 jaar is altijd Handmatig.

* **Automatisch en bij wijziging:** Dit is de standaardinstelling. De projectchronologie wordt bijgewerkt telkens als een verandering in het project of in een ander project voorkomt dat de chronologie van afhankelijk is. De projecttijdlijn wordt ook elke avond bijgewerkt. \
   Dit is de aanbevolen instelling omdat de tijdlijn van het project altijd up-to-date is.

   Wanneer u een taak of het project bijwerkt en een tijdlijnherberekening activeert, worden alle beschikbare datums onmiddellijk weergegeven, zodat u kunt doorgaan met werken. Voor projecten met meer dan 100 taken worden datums die langere berekeningen vereisen, grijs weergegeven.

   ![](assets/dates-dimmed-when-insline-editing-350x146.png)

   Dit geeft aan dat de herberekening nog niet is voltooid en dat de datums kunnen worden gewijzigd.

* **Alleen wijzigen:** De projecttijdlijn wordt bijgewerkt telkens wanneer een wijziging optreedt in het project of in een ander project waarvan de tijdlijn afhankelijk is; geplande updates vinden niet plaats.\
   U zou deze optie kunnen willen selecteren als u zich over systeemprestaties ongerust maakt en als de veranderingen zelden in het project of in andere projecten voorkomen dat de chronologie van afhankelijk is.

* **Alleen automatisch:** Het projecttijdschema wordt elke avond bijgewerkt; het wordt niet onmiddellijk bijgewerkt nadat wijzigingen zijn aangebracht.\
   U zou deze optie kunnen willen selecteren als u zich over systeemprestaties ongerust maakt en als vele veranderingen elke dag in het project of in andere projecten voorkomen dat de chronologie van afhankelijk is.

   >[!NOTE]
   >
   >Een project herberekent niet automatisch elke nacht als het in de status van de Planning is. Het herberekent alleen op verandering.

* **Alleen handmatig:** De projecttijdlijn wordt alleen bijgewerkt wanneer u de optie selecteert om **Tijdlijnen opnieuw berekenen**, zoals beschreven in de rubriek &quot;Handmatige herberekening&quot; in het artikel [Projecttijdlijnen opnieuw berekenen](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
   U kunt deze optie selecteren als u in één keer veel wijzigingen aanbrengt in het project en u wilt dat de tijdlijnherberekening plaatsvindt nadat alle wijzigingen zijn aangebracht (in plaats van na elke afzonderlijke wijziging).
