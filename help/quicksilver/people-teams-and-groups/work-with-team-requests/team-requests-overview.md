---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Overzicht van teamverzoeken
description: De verzoeken van het team worden gevonden in het gebied van Teams in het Belangrijkste Menu.
author: Lisa
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Overzicht van teamverzoeken

## Inzicht krijgen in teamverzoeken

Teamaanvragen vindt u in het gebied [!UICONTROL Teams] in [!UICONTROL Main Menu] . Klik op het [!UICONTROL Team Requests] pictogram van het pictogram ![ Verzoek ](assets/request-icon.png) in het linkerpaneel om teamverzoeken te bekijken.

>[!NOTE]
>
>Gegraveerde teams hebben geen teamaanvragen.

Op het tabblad [!UICONTROL Team Requests] worden de aanvragen weergegeven die op toewijzing wachten voor het team dat momenteel is geselecteerd in de vervolgkeuzelijst. Het getal tussen haakjes geeft aan hoeveel items klaar zijn om te worden bewerkt.

Een teamverzoek vertegenwoordigt een in afwachting van het werkpunt dat niet aan een specifieke gebruiker wordt toegewezen. In plaats daarvan, wordt het toegewezen aan een team, en om het even welk lid van dat team kan vrijwilliger zijn om verantwoordelijkheid voor het punt te aanvaarden. Als een gebruiker zich ertoe aanzet om aan een teamverzoek te werken, accepteert de gebruiker de werktoewijzing als zijn eigen. De taak wordt toegewezen aan de individuele gebruiker naast het team.

>[!NOTE]
>
>Een teamverzoek zou niet voor samenwerkende taaktaken moeten worden gebruikt. Als u veelvoudige gebruikers moet toewijzen om aan een taak samen te werken, doe dit door [!UICONTROL Advanced Assignments] en niet door de verzoeken van het Team. Voor meer informatie, zie [ Geavanceerde taken ](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md) creëren.

## De opties [!UICONTROL Ready to Start] en [!UICONTROL All] begrijpen

De sectie Teamverzoeken bevat twee opties: [!UICONTROL Ready to Start] en [!UICONTROL All] .

De optie [!UICONTROL Ready to Start] geeft alleen taken en problemen weer die aan alle volgende criteria voldoen:

* Alle voorgangers hebben aan de voorwaarden voor hun voorganger afhankelijkheidstypen voldaan.\
  Als het type van de voorgangerrelatie bijvoorbeeld [!UICONTROL Finish-Start] is (de voorgangertaak moet zijn voltooid voordat de afhankelijke taak kan worden gestart), moet de voorganger zijn gemarkeerd als [!UICONTROL Complete] . (Voor meer informatie over de types van voorgangsafhankelijkheid, zie [ Overzicht van de types van taakgebiedsdeel ](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).)

* De het programma geopende gebruiker is de persoon die aan deze taken en kwesties (voor het werkverzoeken) wordt toegewezen, of het geselecteerde team wordt toegewezen aan deze taken en kwesties (voor teamverzoeken).
* De status van het project is ingesteld op [!UICONTROL Current] .
* [!UICONTROL Projected Start Date] of [!UICONTROL Planned Start Date] is overgegaan of zal volgens planning binnen twee weken na de datum van vandaag (of er is geen [!UICONTROL Projected Start Date] of [!UICONTROL Planned Start Date] gedefinieerd) beginnen.
* [!UICONTROL Handoff Date] is al opgetreden of zal binnen twee weken na de huidige datum voorkomen.

>[!NOTE]
>
>Als de taak aan de eerste drie criteria voldoet en binnen twee weken na de huidige datum een Handoff-datum heeft, wordt deze weergegeven als [!UICONTROL Ready to Start], zelfs als de geplande/geprojecteerde data verder zijn dan twee weken. Als de taak geen Handoff datum heeft, dan moeten de Geplande/Geprojecteerde data binnen twee weken na de huidige datum zijn.

De optie [!UICONTROL All] toont alle taken en kwesties op huidige projecten die aan de het programma geopende gebruiker of alle taken of kwesties worden toegewezen die aan het team worden toegewezen.
