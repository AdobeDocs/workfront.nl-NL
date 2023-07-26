---
filename: delegate-work-overview
content-type: overview
navigation-topic: delegate-work
title: Overzicht van werkzaamheden delegeren
description: Wanneer u van plan bent om voor een korte periode uit het bureau te zijn, kunt u uw werk aan andere gebruikers tijdelijk delegeren om ervoor te zorgen dat uw afwezigheid geen wegbelemmering wordt om het werk te voltooien.
author: Alina
feature: Work Management
exl-id: aec2ce78-278f-48d2-af8c-e4e5b31ac856
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 0%

---

# Overzicht van werkzaamheden delegeren

Wanneer u van plan bent om voor een korte periode uit het bureau te zijn, kunt u uw werk aan andere gebruikers tijdelijk delegeren om ervoor te zorgen dat uw afwezigheid geen wegbelemmering wordt om het werk te voltooien.

Bijvoorbeeld, als bepaalde taken vóór u terugkeren maar u hebt niet de tijd om hen te voltooien alvorens u weggaat, kunt u uw taken aan een andere gebruiker delegeren zodat kunnen zij hen op tijd voltooien en niet de voltooiing van het project vertragen tot nadat u terugkeert.

U kunt in [!DNL Adobe Workfront]:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Projects where you are designated as the Project Owner (not yet, not for the MVP)</p> </li>
  -->

* Taken die aan u zijn toegewezen
* Aan u toegewezen problemen
* Goedkeuringen voor projecten, taken, uitgaven en documenten die aan u zijn toegewezen.

Dit artikel bevat algemene informatie over het delegeren van taken en kwesties.

Voor informatie over het delegeren van project, taak, kwestie, en documentgoedkeuringen, zie [Goedkeuringsaanvraag delegeren](../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

Voor informatie over hoe te om taken en kwesties te delegeren zie [Taken en problemen delegeren](../../manage-work/delegate-work/how-to-delegate-work.md).

## Overzicht van werkzaamheden delegeren

Overweeg het volgende wanneer u taken en kwesties delegeert:

* Uw [!DNL Workfront] of groepsbeheerder moet de delegatievoorkeuren inschakelen in het dialoogvenster [!UICONTROL Setup] voordat u uw werk aan anderen kunt delegeren.

  Zie voor meer informatie [Taak- en probleemvoorkeuren voor het hele systeem configureren](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* U kunt taken en problemen alleen delegeren vanuit de [!UICONTROL Home] gebied.
* Er zijn uitzonderingen voor de volgende licentietypen:

   * U kunt uw werk delegeren aan revisoren of aanvragers, hoewel [!DNL Workfront] adviseert het niet.
   * Revisoren kunnen het werk delegeren aan anderen. Ze kunnen geen werkitems weergeven in hun [!UICONTROL Home] gebied. Ze kunnen alleen goedkeuringen bekijken.
   * Aanvragers kunnen hun werk niet delegeren aan anderen. Ze kunnen geen werkitems weergeven in hun [!UICONTROL Home] gebied
* U kunt de taken en de kwesties slechts delegeren die aan u worden toegewezen. U kunt geen taken en kwesties delegeren die aan andere gebruikers, teams, of baanrollen worden toegewezen.
* U kunt taken en kwesties slechts delegeren die niet vóór de begindatum van de delegatie worden voltooid.
* Als een het werkpunt tijdens het tijdkader van de delegatie voltooit, blijft het punt op het gebied van het Huis van de afgevaardigde en van de toegewezen persoon 2 weken vóór [!DNL Workfront] wordt automatisch verwijderd.
* De gebruikers die u als afgevaardigden selecteert, ontvangen de zelfde toestemmingen zoals uw toestemmingen op de taken en de kwesties u aan hen delegeert. De toestemmingen moeten binnen hun toegangsniveaus werken, en soms zouden hun toegangsniveaus lager kunnen zijn dan van u.

>[!NOTE]
>
>  Voor punten die na de delegatie reeds begonnen worden toegewezen, kan het tot één uur duren nadat het punt werd toegewezen voor [!DNL Workfront] om de onlangs-toegewezen punten met de afgevaardigde te delen.

* Als extra taken en kwesties aan u tijdens de tijd worden toegewezen u hebt geselecteerd om uw werk aan andere gebruikers te laten afgevaardigen, wordt het nieuwe toegewezen werk automatisch gedelegeerd aan de zelfde persoon voor het tijdkader u selecteerde als de taak of de uitgiftedata binnen dat tijdkader zijn.
* De zelfde gebruiker kan als afgevaardigde door veelvoudige gebruikers worden geselecteerd.
* Gedelegeerde taken en uitgaven worden niet weergegeven in hulpmiddelen voor middelenbeheer, zoals de [!UICONTROL Workload Balancer] of de [!UICONTROL Resource Planner] voor de gedelegeerde gebruikers.
* U kunt gedelegeerde werk en gedelegeerde namen weergeven op verschillende gebieden van [!DNL Workfront]. Voor meer informatie, zie de sectie &quot;van de plaats de plaats van gedelegeerd werk en van afgevaardigden informatie&quot;in het artikel [Taak beheren en taken delegeren](../delegate-work/how-to-delegate-work.md).


  >[!IMPORTANT]
  >
  >  Als een gebruiker slechts de toegang van de Mening tot taken op hun toegangsniveau heeft en u hebt leiden toestemmingen op de taken u aan hen delegeert, ontvangen zij leiden toestemmingen aan de taken u aan hen delegeert. Ze kunnen echter niet dezelfde handelingen uitvoeren als u met betrekking tot gedelegeerde taken. Zij moeten om Edit toegang tot Taken van de systeembeheerder verzoeken om taken in uw afwezigheid bij te werken.

* Als de delegatie wordt gestopt, worden de machtigingen die aan de gedelegeerde gebruikers zijn verleend voor de taken en problemen waaraan ze zijn gedelegeerd, niet verwijderd.
* Als een systeem of het [!UICONTROL Allow users to delegate their tasks & issues] in het dialoogvenster [!UICONTROL Setup] , worden de momenteel gedelegeerde gebruikers verwijderd van de taken en problemen waaraan zij eerder zijn gedelegeerd. Hun machtigingen voor de taken of uitgaven worden niet verwijderd.

## Verschillen en overeenkomsten tussen taken en delegaties

| Handeling | Toewijzingen | Delegaties |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------------------------|
| Een toegewezen of gedelegeerde gebruiker kan het werkitem bewerken of verwijderen waaraan deze is toegewezen | Gebaseerd op machtigingen en toegangsniveau | Gebaseerd op machtigingen en toegangsniveau |
| Een toegewezen of gedelegeerde gebruiker wordt weergegeven in de koptekst van het werkitem | Ja | Ja |
| De toegewezen of gedelegeerde taken of uitgaven worden weergegeven in het thuisgebied van de ontvanger of gedelegeerde | Ja, totdat het item is voltooid | Ja, alleen voor het tijdsbestek van de delegatie |
| U kunt het werk aan gebruikers van het gebied van het Huis toewijzen of delegeren | Ja | Ja |
| U kunt het werk aan gebruikers toewijzen of delegeren gebruikend | Ja | Nee |
| U kunt het werk aan gebruikers in een lijst, of van de kopbal van een het werkpunt toewijzen of delegeren | Ja | Nee |
| Om het even welke gebruiker kan andere gebruikers met het werkpunten toewijzen of afvaardigen die zij niet met associëren | Gebaseerd op machtigingen en toegangsniveau | Nee. Alleen de toegewezen persoon kan zijn of haar eigen items delegeren. |
| Gepland, Ware, of Gefabriceerde Uren voor het werk dat aan een gebruikersvertoning voor die gebruiker in middelbeheersinstrumenten wordt toegewezen of wordt gedelegeerd | Ja | Nee |
