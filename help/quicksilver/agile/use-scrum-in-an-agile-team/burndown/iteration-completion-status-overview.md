---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Overzicht van de voltooiingsstatus van de herhaling
description: De voltooiingsinformatie die in dit artikel wordt beschreven wordt getoond boven de burndown grafiek.
author: Jenny
feature: Agile
exl-id: cc6bebdb-f2aa-4e85-9f9f-15e7753d84cb
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# Overzicht van de voltooiingsstatus

De voltooiingsinformatie die in dit artikel wordt beschreven wordt getoond boven de burndown grafiek.

Voltooiingspercentage van een herhaling:

![&#x200B; het paneel van herhalingsdetails &#x200B;](assets/burndown-percentcomplete-350x47.png)

Deze informatie wijst op de voltooiingsstatus van de herhaling voor de dag die momenteel in de burndown grafiek wordt geselecteerd. Standaard wordt de voltooiingsstatus weergegeven op basis van de datum van de huidige dag.

De volgende informatie is beschikbaar:

* **[!UICONTROL Percent Complete]:** Algemene voortgang van de herhaling

  [!UICONTROL Percent Complete] wordt aangepast op basis van het percentage dat is voltooid voor elk artikel of elke taak binnen de herhaling, inclusief artikelen of taken die slechts gedeeltelijk zijn voltooid.

  De kleur van de statusbalk van [!UICONTROL Percent Complete] wordt weergegeven als rood of groen, zodat deze overeenkomt met de kleur van de daadwerkelijke burndown-snelheid. Het wordt in rood weergegeven wanneer de burndown rate minder is dan het ideale (meer punten of uren resterend per dag dan de ideale burndown berekening), en het wordt in groen getoond wanneer het burndown tarief aan of beter dan het ideale (gelijk of minder punten resterend per dag dan de ideale burndown berekening) is.

* **[!UICONTROL Completed Stories]:** (Alleen beschikbaar in herhalingen) Het aantal artikelen dat is gemarkeerd [!UICONTROL Complete] . Dit wordt weergegeven in verhouding tot het totale aantal artikelen in de herhaling. Zo geeft &#39;3 van 6&#39; aan dat 3 van de 6 artikelen in de herhaling zijn gemarkeerd [!UICONTROL Complete] .
* **[!UICONTROL Completed Points / Hours]:** (Alleen beschikbaar in herhalingen) Het aantal punten of uren dat is gemarkeerd [!UICONTROL Complete] . Wordt weergegeven in verhouding tot het totale aantal punten of uren in de herhaling. &#39;5 van 11&#39; geeft bijvoorbeeld aan dat 5 van de 11 artikelen in de herhaling zijn gemarkeerd [!UICONTROL Complete] . Dit nummer houdt rechtstreeks verband met de [!UICONTROL Percent Complete] -berekening en wordt tegelijk bijgewerkt met [!UICONTROL Percent Complete] .

  Punten en uren zijn gekoppeld aan artikelen. Wanneer een artikel is gemarkeerd als [!UICONTROL Complete] , worden de punten of uren van dat artikel gemarkeerd als Voltooid.

  Standaard worden punten gebruikt. U kunt dit veranderen door de montages voor uw team te wijzigen, zoals die in [&#x200B; wordt beschreven leidt tot een Gelijk team &#x200B;](../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

* **[!UICONTROL Points / Hours Per Day]:** (Beschikbaar slechts in herhalingen) het gemiddelde aantal punten of uren duidelijk [!UICONTROL Complete] elke dag sinds het begin van de herhaling door de huidige dag.

  Dit wordt berekend door het totale aantal punten of uren dat is voltooid, gedeeld door het totale aantal dagen tot en met de huidige dag. (Deeldagen worden als een hele dag geregistreerd.)

  Deze informatie kan nuttig zijn wanneer het plannen van een toekomstige herhaling.

* **[!UICONTROL Estimated Completion]:** De geschatte datum waarop de herhaling wordt voltooid, op basis van de huidige snelheid in de punten/uren per dag (voor herhalingen).

  Wanneer de [!UICONTROL Estimated Completion] -datum later is dan de einddatum die voor de herhaling is gedefinieerd, wordt het aantal resterende werkdagen tussen haakjes weergegeven als een rood aantal werkdagen naast de [!UICONTROL Estimated Completion] -datum.

  Wanneer de [!UICONTROL Estimated Completion] -datum eerder is dan de geplande einddatum van de herhaling, wordt het aantal resterende werkdagen groen weergegeven. (De einddatum voor de herhaling wordt gespecificeerd wanneer de herhaling wordt gepland, zoals die in [&#x200B; wordt beschreven leidt tot een herhaling &#x200B;](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md); de einddatum voor het project is [!UICONTROL Planned Completion Date], of het is de huidige datum als [!UICONTROL Planned Completion Date] in het verleden is. [!UICONTROL Planned Completion Date] voor het project wordt berekend op basis van de duur van taken in het project.) Wanneer u de herhaling plant, als u de einddatum van de herhaling voor een niet-werkende dag plaatst en de herhaling op tijd eindigt, wordt de Geschatte datum van de Voltooiing geplaatst voor de laatste werkdag voorafgaand aan de datum van het herhalingseind die u plaatst (omdat het werk niet gepland is om op niet-werkende dagen te worden gebrand).

  &quot;(+9 dagen)&quot; geeft bijvoorbeeld aan dat de geschatte einddatum 9 werkdagen later is dan de geplande einddatum van de herhaling.

  Voor meer informatie, zie [&#x200B; overzicht van de voltooiingsvoltooiingsstatus &#x200B;](#Understanding-How-Days-Off-Affect-the-Burndown-Chart).
