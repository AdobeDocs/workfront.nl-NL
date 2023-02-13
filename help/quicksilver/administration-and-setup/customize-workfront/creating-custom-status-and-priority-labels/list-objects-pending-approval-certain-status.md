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

Als u probeert om een status te schrappen, zou een foutenmelding u kunnen vertellen dat het niet kan worden geschrapt omdat het in minstens één hangende goedkeuringsprocessen in uw systeem is. U kunt een rapport uitvoeren om de objecten weer te geven waar het zich in een goedkeuringsproces bevindt dat in behandeling is en vervolgens bepalen wat u voor elk rapport moet doen.

## In de standaardmodus

1. Ga naar de **Rapportage** in de algemene navigatiebalk selecteert u vervolgens het gebied **Rapporten** tab.
1. Klik op het pictogram Hoofdmenu ![](assets/main-menu-icon.png) in de rechterbovenhoek klikt u op **Rapporten**.
1. Klikken **Nieuw rapport** selecteert u vervolgens **Projectrapport**, **Taakrapport**, of **Probleemrapport**.
1. Open de **Filters** tab.
1. Klikken **Filterregel toevoegen** Voer vervolgens de volgende handelingen uit om de regel in te stellen:
   1. Begin met typen `status`selecteert u vervolgens **Status** wanneer deze wordt weergegeven.
   1. Verlaten **Gelijk** in het tweede veld.
   1. Selecteer de naam van de status in het derde veld.
1. Klikken **Filterregel toevoegen** opnieuw, dan doe het volgende aan opstelling de regel
   1. Begin met typen `pending status`selecteert u vervolgens dat item wanneer het onder het objecttype wordt weergegeven waarin u kijkt (**Project**, **Taak**, of **Probleem**).
   1. Verlaten **Gelijk** in het tweede veld.
   1. Type `in` in het derde veld.
1. Klikken **Filterregel toevoegen** opnieuw, dan doe het volgende aan opstelling de regel
   1. Begin goedkeuringsproces te typen en selecteer vervolgens **Groep-id** wanneer het wordt weergegeven onder **Goedkeuringsproces**.
   1. Selecteren **Is leeg** in het tweede veld.
1. Klikken **Opslaan + Sluiten** om het rapport uit te voeren en om het even welke voorwerpen van het type te vermelden u met goedkeuringsprocessen in hangende staat op basis van de status specificeerde u (**Project**, **Taak**, of **Probleem**).
1. Herhaal deze stappen om dezelfde informatie te zoeken voor de andere twee objecttypen.


## In tekstmodus

1. Klik op het pictogram Hoofdmenu ![](assets/main-menu-icon.png) in de rechterbovenhoek klikt u op **Rapporten**.
1. Klikken **Nieuw rapport** selecteert u vervolgens **Projectrapport**, **Taakrapport**, of **Probleemrapport**.
1. Open de **Filters** tab.
1. Selecteren **Overschakelen naar tekstmodus**.
1. Kopieer en plak het volgende in het bewerkingsvenster, waarbij XXX wordt vervangen door de 3-letterige sleutel voor de status:

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   U kunt de sleutel weergeven in de lijst met statussen, zoals in de volgende artikelen wordt getoond:
   * [Heb toegang tot de lijst van de statussen van het systeemproject](project-statuses.md)
   * [De lijst met taakstatussen van het systeem openen](task-statuses.md)
   * [Toegang krijgen tot de lijst met systeemuitgiftestatussen](issue-statuses.md)

1. Klikken **Opslaan + Sluiten** om het rapport uit te voeren en om het even welke voorwerpen van het type te vermelden u met goedkeuringsprocessen in hangende staat op basis van de status specificeerde u (**Project**, **Taak**, of **Probleem**).
1. Herhaal deze stappen om dezelfde informatie te zoeken voor de andere twee objecttypen.
