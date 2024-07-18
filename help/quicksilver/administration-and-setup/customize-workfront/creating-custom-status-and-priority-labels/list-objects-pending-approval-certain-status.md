---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Objecten met een bepaalde status weergeven die in behandeling zijn
description: Als u probeert om een status te schrappen, zou een foutenmelding u kunnen vertellen dat het niet kan worden geschrapt omdat het in hangende goedkeuringsprocessen op voorwerpen in uw systeem wordt gebruikt. Als u die voorwerpen wilt vinden en herzien om te beslissen wat u moet doen, kunt u een rapport in werking stellen dat hen een lijst maakt.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Objecten met een bepaalde status weergeven die in behandeling zijn

Als u probeert om een status te schrappen, zou een foutenmelding u kunnen vertellen dat het niet kan worden geschrapt omdat het in minstens één hangende goedkeuringsprocessen in uw systeem is. U kunt een rapport uitvoeren om de objecten weer te geven waar het zich in een goedkeuringsproces bevindt dat in behandeling is, en vervolgens bepalen wat u voor elk rapport moet doen.

## In de standaardmodus

1. Ga naar het **Meldend** gebied in de Globale Bar van de Navigatie, dan selecteer de **Rapporten** tabel.
1. Klik het Belangrijkste pictogram van het Menu ![](assets/main-menu-icon.png) in de hoger-juiste hoek, dan klik **Rapporten**.
1. Klik **Nieuw Rapport**, dan selecteren **Rapport van het Project**, **Rapport van de Taak**, of **Rapport van de Uitgave**.
1. Open de **Filters** tabel.
1. Klik **toevoegen een Regel van de Filter**, dan doe het volgende aan opstelling de regel:
   1. Begin het typen `status`, dan selecteren **Status** wanneer het toont.
   1. Verlaat **Gelijk** op het tweede gebied.
   1. Selecteer de naam van de status in het derde veld.
1. Klik **voeg opnieuw een Regel van de Filter** toe, dan doe het volgende aan opstelling de regel
   1. Begin het typen `pending status`, dan selecteren dat punt wanneer het onder het objecten type toont waar u (**Project** kijkt, **Taak**, of **Uitgave**).
   1. Verlaat **Gelijk** op het tweede gebied.
   1. Typ `in` in het derde veld.
1. Klik **voeg opnieuw een Regel van de Filter** toe, dan doe het volgende aan opstelling de regel
   1. Begin goedkeuringsproces te typen, dan uitgezochte **identiteitskaart van de Groep** wanneer het onder **het Proces van de Goedkeuring** toont.
   1. Selecteer **is Lege** op het tweede gebied.
1. Klik **sparen + Sluiten** om het rapport in werking te stellen en van om het even welke voorwerpen van het type een lijst te maken u met goedkeuringsprocessen in hangende staat die op de status wordt gebaseerd u (**specificeerde Project**, **Taak**, of **Uitgave**).
1. Herhaal deze stappen om dezelfde informatie te zoeken voor de andere twee objecttypen.


## In tekstmodus

1. Klik het Belangrijkste pictogram van het Menu ![](assets/main-menu-icon.png) in de hoger-juiste hoek, dan klik **Rapporten**.
1. Klik **Nieuw Rapport**, dan selecteren **Rapport van het Project**, **Rapport van de Taak**, of **Rapport van de Uitgave**.
1. Open de **Filters** tabel.
1. Selecteer **Schakelaar aan de Wijze van de Tekst**.
1. Kopieer en plak het volgende in het bewerkingsvenster, waarbij XXX wordt vervangen door de 3-letterige sleutel voor de status:

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   U kunt de sleutel weergeven in de lijst met statussen, zoals in de volgende artikelen wordt getoond:
   * [Heb toegang tot de lijst van de statussen van het systeemproject](project-statuses.md)
   * [De lijst met taakstatussen van het systeem openen](task-statuses.md)
   * [Toegang krijgen tot de lijst met systeemuitgiftestatussen](issue-statuses.md)

1. Klik **sparen + Sluiten** om het rapport in werking te stellen en van om het even welke voorwerpen van het type een lijst te maken u met goedkeuringsprocessen in hangende staat die op de status wordt gebaseerd u (**specificeerde Project**, **Taak**, of **Uitgave**).
1. Herhaal deze stappen om dezelfde informatie te zoeken voor de andere twee objecttypen.
