---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Overzicht van de voltooiingsstatus
description: De voltooiingsinformatie die in dit artikel wordt beschreven wordt getoond boven de burndown grafiek.
author: Lisa
feature: Agile
exl-id: cc6bebdb-f2aa-4e85-9f9f-15e7753d84cb
source-git-commit: 373f2522b85196d6395f189ae6cfe03449cac61a
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# Overzicht van de voltooiingsstatus

De voltooiingsinformatie die in dit artikel wordt beschreven wordt getoond boven de burndown grafiek.

Voltooiingspercentage van een herhaling:

![](assets/burndown-percentcomplete-350x47.png)

Deze informatie wijst op de voltooiingsstatus van de herhaling voor de dag die momenteel in de burndown grafiek wordt geselecteerd. Standaard wordt de voltooiingsstatus weergegeven op basis van de datum van de huidige dag.

De volgende informatie is beschikbaar:

* **[!UICONTROL Percent Complete]:** Algemene voortgang van de herhaling

   [!UICONTROL Percent Complete] wordt aangepast op basis van het percentage dat is voltooid voor elk artikel of elke taak binnen de herhaling, inclusief artikelen of taken die slechts gedeeltelijk zijn voltooid.

   De kleur van de [!UICONTROL Percent Complete] wordt de statusbalk weergegeven als rood of groen, zodat deze overeenkomt met de kleur van de daadwerkelijke burndown-snelheid. Het wordt in rood weergegeven wanneer de burndown rate minder is dan het ideale (meer punten of uren resterend per dag dan de ideale burndown berekening), en het wordt in groen getoond wanneer het burndown tarief aan of beter dan het ideale (gelijk of minder punten resterend per dag dan de ideale burndown berekening) is.

* **[!UICONTROL Completed Stories]:** (Alleen beschikbaar in herhalingen) Het aantal gemarkeerde artikelen [!UICONTROL Complete]. Dit wordt weergegeven in verhouding tot het totale aantal artikelen in de herhaling. Zo geeft &quot;3 van 6&quot; aan dat 3 van de 6 artikelen in de herhaling zijn gemarkeerd [!UICONTROL Complete].
* **[!UICONTROL Completed Points / Hours]:** (Alleen beschikbaar in herhalingen) Het aantal punten of uren dat is gemarkeerd [!UICONTROL Complete]. Wordt weergegeven in verhouding tot het totale aantal punten of uren in de herhaling. Zo geeft &quot;5 van 11&quot; aan dat 5 van de 11 artikelen in de herhaling zijn gemarkeerd [!UICONTROL Complete]. Dit nummer houdt rechtstreeks verband met de [!UICONTROL Percent Complete] en tegelijkertijd wordt bijgewerkt [!UICONTROL Percent Complete] wordt bijgewerkt.

   Punten en uren zijn gekoppeld aan artikelen. Wanneer een artikel is gemarkeerd [!UICONTROL Complete], worden de punten of uren die aan dat artikel zijn gekoppeld, gemarkeerd als Voltooid.

   Standaard worden punten gebruikt. U kunt dit wijzigen door de instellingen voor uw team te wijzigen, zoals wordt beschreven in [Een bestandsteam maken](../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

* **[!UICONTROL Points / Hours Per Day]:** (Alleen beschikbaar in herhalingen) Het gemiddelde aantal punten of gemarkeerde uren [!UICONTROL Complete] elke dag sinds het begin van de herhaling tot en met de huidige dag.

   Dit wordt berekend door het totale aantal punten of uren dat is voltooid, gedeeld door het totale aantal dagen tot en met de huidige dag. (Gedeeltelijke dagen worden als een hele dag geregistreerd.)

   Deze informatie kan nuttig zijn wanneer het plannen van een toekomstige herhaling.

* **[!UICONTROL Estimated Completion]:** De geschatte datum waarop de herhaling zal worden voltooid, op basis van de huidige frequentie in de punten/uren per dag (voor herhalingen).

   Wanneer de [!UICONTROL Estimated Completion] De datum is later dan de einddatum die voor de herhaling is gedefinieerd, het aantal resterende werkdagen wordt tussen haakjes weergegeven als een rood aantal werkdagen naast de [!UICONTROL Estimated Completion] datum.

   Wanneer de [!UICONTROL Estimated Completion] de datum eerder is dan de geplande einddatum van de herhaling, wordt het aantal resterende werkdagen groen weergegeven. (De einddatum voor de herhaling wordt opgegeven wanneer de herhaling wordt gepland, zoals beschreven in [Een herhaling maken](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md); de einddatum van het project is [!UICONTROL Planned Completion Date]of het is de huidige datum als de [!UICONTROL Planned Completion Date] is in het verleden. De [!UICONTROL Planned Completion Date] voor het project wordt berekend op basis van de duur van de taken in het project.) Wanneer u de herhaling plant, als u de einddatum van de herhaling voor een niet-werkende dag plaatst en de herhaling op tijd eindigt, wordt de Geschatte datum van de Voltooiing geplaatst voor de laatste werkdag voorafgaand aan de datum van het herhalingseind die u plaatst (omdat het werk niet gepland is om op niet-werkende dagen te worden gebrand).

   &quot;(+9 dagen)&quot; geeft bijvoorbeeld aan dat de geschatte einddatum 9 werkdagen later is dan de geplande einddatum van de herhaling.

   Zie voor meer informatie [Overzicht van de voltooiingsstatus](#Understanding-How-Days-Off-Affect-the-Burndown-Chart).
