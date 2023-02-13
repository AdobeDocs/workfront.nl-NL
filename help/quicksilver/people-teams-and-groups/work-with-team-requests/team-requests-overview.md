---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Overzicht van teamverzoeken
description: De verzoeken van het team worden gevonden in het gebied van Teams in het Belangrijkste Menu.
author: Lisa
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: 9693ac3792fec3eca6218a228f2067519ed433ac
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Overzicht van teamverzoeken

## Inzicht krijgen in teamverzoeken

De verzoeken van het team worden gevonden in [!UICONTROL Teams] in het gebied [!UICONTROL Main Menu]. Klik op de knop [!UICONTROL Team Requests] pictogram ![Aanvraagpictogram](assets/request-icon.png) in het linkerpaneel om teamverzoeken te bekijken.

>[!NOTE]
>
>Gegraveerde teams hebben geen teamaanvragen.

De [!UICONTROL Team Requests] toont de verzoeken die op taak voor het team wachten dat momenteel in de drop-down lijst wordt geselecteerd. Het getal tussen haakjes geeft aan hoeveel items klaar zijn om te worden bewerkt.

Een teamverzoek vertegenwoordigt een in afwachting van het werkpunt dat niet aan een specifieke gebruiker wordt toegewezen. In plaats daarvan, wordt het toegewezen aan een team, en om het even welk lid van dat team kan vrijwilliger zijn om verantwoordelijkheid voor het punt te aanvaarden. Als een gebruiker zich ertoe aanzet om aan een teamverzoek te werken, accepteert de gebruiker de werktoewijzing als zijn eigen. De taak wordt toegewezen aan de individuele gebruiker naast het team.

>[!NOTE]
>
>Een teamverzoek zou niet voor samenwerkende taaktaken moeten worden gebruikt. Als u meerdere gebruikers wilt toewijzen om samen te werken aan een taak, doet u dit via [!UICONTROL Advanced Assignments] en niet door de verzoeken van het Team. Zie voor meer informatie [Geavanceerde toewijzingen maken](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## Begrijp het [!UICONTROL Ready to Start] en [!UICONTROL All] opties

Er zijn twee opties bij de bovenkant van de sectie van de Verzoeken van het Team: [!UICONTROL Ready to Start] en [!UICONTROL All].

De [!UICONTROL Ready to Start] alleen taken en problemen worden weergegeven die aan alle volgende criteria voldoen:

* Alle voorgangers hebben aan de voorwaarden voor hun voorganger afhankelijkheidstypen voldaan.\
   Bijvoorbeeld als het type van predecessor verhouding is [!UICONTROL Finish-Start] (de voorganger taak moet eindigen alvorens de afhankelijke taak kan beginnen), moet predecessor als duidelijk worden gemerkt [!UICONTROL Complete]. (Voor meer informatie over de types van predecessor gebiedsdeel, zie [Overzicht van typen taakafhankelijkheid](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).)

* De het programma geopende gebruiker is de persoon die aan deze taken en kwesties (voor het werkverzoeken) wordt toegewezen, of het geselecteerde team wordt toegewezen aan deze taken en kwesties (voor teamverzoeken).
* De projectstatus bevindt zich in een status van [!UICONTROL Current].
* De [!UICONTROL Projected Start Date] of [!UICONTROL Planned Start Date] is verstreken of is gepland binnen twee weken na de datum van vandaag (of [!UICONTROL Projected Start Date] of [!UICONTROL Planned Start Date] is gedefinieerd).
* De [!UICONTROL Handoff Date] heeft plaatsgevonden of zal binnen twee weken na de huidige datum voorkomen.

>[!NOTE]
>
>Als de taak aan de eerste drie criteria voldoet en binnen twee weken na de huidige datum een Handoff-datum heeft, zal het als [!UICONTROL Ready to Start] zelfs als de geplande/voorspelde data verder zijn dan twee weken. Als de taak geen Handoff datum heeft, dan moeten de Geplande/Geprojecteerde data binnen twee weken na de huidige datum zijn.

De [!UICONTROL All] de optie toont alle taken en kwesties op huidige projecten die aan de het programma geopende gebruiker of alle taken of kwesties worden toegewezen die aan het team worden toegewezen.
