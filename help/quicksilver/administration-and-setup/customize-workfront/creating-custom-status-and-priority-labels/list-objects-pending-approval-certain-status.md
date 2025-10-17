---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Objecten weergeven met een bepaalde status die in behandeling is voor een goedkeuringsproces
description: Als u probeert om een status te schrappen, zou een foutenmelding u kunnen vertellen dat het niet kan worden geschrapt omdat het in hangende goedkeuringsprocessen op voorwerpen in uw systeem wordt gebruikt. Als u die voorwerpen wilt vinden en herzien om te beslissen wat u moet doen, kunt u een rapport in werking stellen dat hen een lijst maakt.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Objecten met een bepaalde status weergeven waarvoor een goedkeuringsproces in behandeling is

Als u probeert om een status te schrappen, zou een foutenmelding u kunnen vertellen dat het niet kan worden geschrapt omdat het in minstens één handig goedkeuringsproces in uw systeem is. U kunt een rapport uitvoeren om de objecten weer te geven waar het zich in een goedkeuringsproces bevindt dat in behandeling is, en vervolgens bepalen wat u voor elk rapport moet doen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td>
     <p>Standard</p>
     <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td><p>Toegang tot rapporten, dashboards, kalenders bewerken</p><p>Toegang tot filters, weergaven, groepen bewerken</p></td>
  </tr>
  <tr> 
   <td>Objectmachtigingen</td> 
   <td>U krijgt beheermachtigingen voor de rapporten die u maakt.</td>
  </tr>
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## In de standaardmodus

{{step1-to-reports}}

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

{{step1-to-reports}}

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
