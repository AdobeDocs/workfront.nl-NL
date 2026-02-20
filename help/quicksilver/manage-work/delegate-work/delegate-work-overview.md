---
filename: delegate-work-overview
content-type: overview
navigation-topic: delegate-work
title: Overzicht van werkzaamheden delegeren
description: Wanneer u van plan bent om voor een korte periode uit het bureau te zijn, kunt u uw werk aan andere gebruikers tijdelijk delegeren om ervoor te zorgen dat uw afwezigheid geen wegbelemmering wordt om het werk te voltooien.
author: Becky
feature: Work Management
exl-id: aec2ce78-278f-48d2-af8c-e4e5b31ac856
source-git-commit: a5f33f914dabaa9368dea919510375bcb6ee03e2
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 0%

---

# Overzicht van werkzaamheden delegeren

Wanneer u van plan bent om voor een korte periode uit het bureau te zijn, kunt u uw werk aan andere gebruikers tijdelijk delegeren om ervoor te zorgen dat uw afwezigheid geen wegbelemmering wordt om het werk te voltooien.

Bijvoorbeeld, als bepaalde taken vóór u terugkeren maar u hebt niet de tijd om hen te voltooien alvorens u weggaat, kunt u uw taken aan een andere gebruiker delegeren zodat kunnen zij hen op tijd voltooien en niet de voltooiing van het project vertragen tot nadat u terugkeert.

U kunt de volgende objecten delegeren in [!DNL Adobe Workfront] :

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Projects where you are designated as the Project Owner (not yet, not for the MVP)</p> </li>
  -->

* Taken die aan u zijn toegewezen
* Aan u toegewezen problemen
* Goedkeuringen voor projecten, taken of uitgaven die aan u zijn toegewezen.

  >[!TIP]
  >
  >   U kunt geen timesheet-, document- of proefdrukgoedkeuringen delegeren.


Dit artikel bevat algemene informatie over het delegeren van taken en kwesties die aan u worden toegewezen.

Voor informatie over het delegeren van project, taak, en geeft goedkeuringen uit, zie [ de goedkeuringsverzoek van de Afgevaardigde ](../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

Voor informatie over hoe te om taken en kwesties te delegeren, zie [ de taken en kwesties van de Afgevaardigde ](../../manage-work/delegate-work/how-to-delegate-work.md).

## Overzicht van taken en problemen delegeren

Overweeg het volgende wanneer u taken en kwesties delegeert:

* Uw [!DNL Workfront] - of groepsbeheerder moet de delegatievoorkeuren in het [!UICONTROL Setup] -gebied inschakelen voordat u uw werk aan anderen kunt delegeren.

  Voor informatie, zie [ de taak en de uitgevende voorkeur van het systeem brede ](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) vormen.

* U kunt taken en problemen alleen delegeren vanuit het [!UICONTROL Home] -gebied.
* Bij het delegeren van werk, zijn er uitzonderingen voor de volgende vergunningstypes:

   * U kunt het werk delegeren aan Revisoren of Aanvragers, hoewel [!DNL Workfront] het niet aanbeveelt.
   * Revisoren kunnen het werk delegeren aan anderen. Ze kunnen werkitems in hun [!UICONTROL Home] -gebied niet weergeven. Ze kunnen alleen goedkeuringen bekijken.
   * Aanvragers kunnen hun werk niet delegeren aan anderen. Ze kunnen werkitems in hun [!UICONTROL Home] -gebied niet weergeven
* U kunt de taken en de kwesties slechts delegeren die aan u worden toegewezen. U kunt geen taken en kwesties delegeren die aan andere gebruikers, teams, of baanrollen worden toegewezen.
* U kunt taken en kwesties slechts delegeren die niet vóór de begindatum van de delegatie worden voltooid.
* Als een het werkpunt tijdens het tijdkader van de delegatie voltooit, blijft het punt in het gebied van het Huis van de afgevaardigde en van de toegewezen persoon twee weken alvorens [!DNL Workfront] automatisch het verwijdert.
* De gebruikers die u als afgevaardigden selecteert, ontvangen de zelfde toestemmingen zoals uw toestemmingen op de taken en de kwesties u aan hen delegeert. De toestemmingen moeten binnen hun toegangsniveaus werken, en soms zouden hun toegangsniveaus lager kunnen zijn dan van u.

>[!NOTE]
>
>  Voor punten die worden toegewezen nadat de delegatie reeds is begonnen, kan het tot één uur nadat het punt voor [!DNL Workfront] werd toegewezen duren om de onlangs-toegewezen punten met de afgevaardigde te delen.

* Als extra taken en kwesties aan u tijdens de tijd worden toegewezen u hebt geselecteerd om uw werk aan andere gebruikers te laten afgevaardigen, wordt het nieuwe toegewezen werk automatisch gedelegeerd aan de zelfde persoon voor het tijdkader u selecteerde als de taak of de uitgiftedata binnen dat tijdkader zijn.
* De zelfde gebruiker kan als afgevaardigde door veelvoudige gebruikers worden geselecteerd.
* Gedelegeerde taken en uitgaven worden niet weergegeven in hulpmiddelen voor resourcebeheer, zoals de [!UICONTROL Workload Balancer] of de [!UICONTROL Resource Planner] voor gedelegeerde gebruikers.
* U kunt gedelegeerde werk en gedelegeerde namen bekijken in verschillende gebieden van [!DNL Workfront] . Voor meer informatie, zie de sectie &quot;van de plaats bepalen van gedelegeerd werk en van afgevaardigden informatie&quot;in het artikel [ de taken en de kwesties van de Afgevaardigde ](../delegate-work/how-to-delegate-work.md).


  >[!IMPORTANT]
  >
  >  Als een gebruiker slechts de toegang van de Mening tot taken op hun toegangsniveau heeft en u hebt leiden toestemmingen op de taken u aan hen delegeert, ontvangen zij leiden toestemmingen aan de taken u aan hen delegeert. Ze kunnen echter niet dezelfde handelingen uitvoeren als u met betrekking tot gedelegeerde taken. Zij moeten om Edit toegang tot Taken van de systeembeheerder verzoeken om taken in uw afwezigheid bij te werken.

* Als de delegatie wordt gestopt, worden de machtigingen die aan de gedelegeerde gebruikers zijn verleend voor de taken en problemen waaraan ze zijn gedelegeerd, niet verwijderd.
* Als een systeem of de instelling [!UICONTROL Allow users to delegate their tasks & issues] in het [!UICONTROL Setup] -gebied uitschakelt, worden de momenteel gedelegeerde gebruikers verwijderd uit de taken en problemen waaraan zij eerder zijn gedelegeerd. Hun machtigingen voor de taken of uitgaven worden niet verwijderd.

## Verschillen en overeenkomsten tussen taken en delegaties

| Actie | Toewijzingen | Delegaties |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------------------------|
| Een toegewezen of gedelegeerde gebruiker kan het werkitem bewerken of verwijderen waaraan deze is toegewezen | Gebaseerd op machtigingen en toegangsniveau | Gebaseerd op machtigingen en toegangsniveau |
| Een toegewezen of gedelegeerde gebruiker wordt weergegeven in de koptekst van het werkitem | Ja | Ja |
| De toegewezen of gedelegeerde taken of uitgaven worden weergegeven in het thuisgebied van de ontvanger of gedelegeerde | Ja, totdat het item is voltooid | Ja, alleen voor het tijdsbestek van de delegatie |
| U kunt het werk aan gebruikers van het gebied van het Huis toewijzen of delegeren | Ja | Ja |
| U kunt het werk aan gebruikers toewijzen of delegeren gebruikend de Balancer van de Werkbelasting | Ja | Nee |
| U kunt het werk aan gebruikers in een lijst, of van de kopbal van een het werkpunt toewijzen of delegeren | Ja | Nee |
| Om het even welke gebruiker kan andere gebruikers met het werkpunten toewijzen of afvaardigen die zij niet met associëren | Gebaseerd op machtigingen en toegangsniveau | Nee. Alleen de toegewezen persoon kan zijn of haar eigen items delegeren. |
| Gepland, Ware, of Gefabriceerde Uren voor het werk dat aan een gebruikersvertoning voor die gebruiker in middelbeheersinstrumenten wordt toegewezen of wordt gedelegeerd | Ja | Nee |
