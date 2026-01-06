---
content-type: overview;how-to-procedural
product-area: projects
keywords: analyses, metriek, project, taken, ontvanger, volledig, status, achterstallig, komende
navigation-topic: manage-projects
title: Projectmetriek begrijpen
description: De metriek van het project geeft u een visualisatie van wat in een project gebeurt, toestaand u snel de behoeften en de status van een project beoordeelt. Ontdek hoe u het gedeelte Metriek in het linkerdeelvenster van een project kunt interpreteren.
author: Alina
feature: Work Management
exl-id: 54c2a59d-9f6b-4126-9526-5169aeda8517
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1206'
ht-degree: 0%

---

# Projectmetriek begrijpen

De metriek van het project geeft u een algemene mening in grafiekformaat over hoe een project presteert.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Licht of hoger</p>
   <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten weergeven</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven voor een project</p> </td> 
  </tr> 
 </tbody> 
</table>

*Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>New: Light or higher </p>
   <p>Current: Review or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration</td> 
   <td> <p>View access to Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a project</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Vereisten

Als u het gebied Metriek wilt openen vanuit het linkerdeelvenster van een project, moet u:

* De optie Metrische gegevens voor de linkerdeelvensteroptie is ingeschakeld in het gedeelte Projecten van uw lay-outsjabloon.

  Leren hoe een beheerder van Workfront of groepsbeheerder het linkerpaneel met een Malplaatje van de Lay-out kan aanpassen, zie [ het linkerpaneel aanpassen gebruikend een lay-outmalplaatje ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

## Overzicht van het gebied Metriek van het project

De metriek van het project geeft u een visualisatie van wat in een project gebeurt, toestaand u snel de behoeften en de status van een project beoordeelt.

![ metriek van het Project ](assets/project-metrics-full-screen-350x238.png)

In het gebied Metriek, kunt u de algemene gezondheid van een project zien, evenals:

* Waar werk actief of gestagneerd is
* Wie aan hen toegewezen open werkpunten heeft
* Details over taken of problemen die achterstallig zijn of die dicht bij de geplande afsluitdatum liggen

U kunt ook naar elk diagram gaan om taken of problemen in een bepaalde categorie nader te bekijken.

Meer leren over het bekijken van deze taken of kwesties, zie {de details van Metriek van 0} Mening [.](#view-metrics-details)

<!--this was deprecated: 
>[!TIP]
>
>To see metrics at a higher level for a group of projects within a program, portfolio, etc., navigate to the Enhanced analytics area.  
>To learn more about Enhanced analytics, see [Enhanced analytics overview](../../../enhanced-analytics/enhanced-analytics-overview.md).-->

## KPI&#39;s voor projecten

KPI&#39;s (Key Performance Indicators) worden boven aan het gebied Metrics weergegeven.

![ metriek van het Project ](assets/project-metrics-kpis-350x52.png)

Deze KPI&#39;s worden onderverdeeld in de volgende categorieën:

| Voltooide taken | **Voltooide taken** toont het aantal taken in een Volledige status. Dit nummer bevat ook taken met een aangepaste status die gelijk is aan Voltooien. |
|---|---|
| Onvolledige taken | **Onvolledige taken** toont het aantal taken die niet in een Volledige of Gesloten status of een status zijn die met Voltooid evenaart. |
| Achterstallige taken | **achterstallige taken** toont het aantal taken die voorbij de Geplande Datum van de Voltooiing zijn en niet in een Volledige of Gesloten status of een status zijn die met Voltooid of Gesloten evenaart. |
| Totaal aantal taken | **Totale taken** toont het totale aantal taken in het project. |

>[!TIP]
>
>Om een lijst van het werkpunten voor specifieke KPI te tonen, klik dat KPI. In die lijst kunt u op een specifiek werkitem klikken om meer details op een nieuw tabblad weer te geven.\
>![ Voltooide taken ](assets/completed-tasks-dialog-350x75.png)\
>Voor meer informatie, zie [ de details van Metriek van de Mening ](#view-metrics-details).

## Taakgrafiek of werkbalkgrafiek

In het staafdiagram dat onder het project KPIs verschijnt, kunt u de status of de prioriteit van het werkpunten in het project bekijken. De taakweergave is standaard geselecteerd.

Wanneer de status in dit diagram wordt geselecteerd, kunt u alle statussen van taken of kwesties in een project bekijken. Elke status wordt gegroepeerd in een balk in het diagram. Alle standaardsysteemstatussen en aangepaste statussen worden in dit diagram weergegeven.

![ kwestie van de Taak door status ](assets/project-metrics-task-issue-by-status-350x120.png)

Wanneer de prioriteit in deze grafiek wordt geselecteerd, kunt u alle prioriteiten van taken of kwesties in een project bekijken.

![ Taken en kwesties door prioriteit ](assets/project-metrics-task-issue-by-priority-350x121.png)

>[!TIP]
>
>Als u een lijst met werkitems met een bepaalde status of prioriteit wilt weergeven, klikt u op een balk in het diagram. In die lijst kunt u op een specifiek werkitem klikken om meer details op een nieuw tabblad weer te geven.\
>![ Voltooide takendoos ](assets/completed-tasks-dialog-350x75.png)\
>Voor meer informatie, zie [ de details van Metriek van de Mening ](#view-metrics-details).

## Donut-diagram

De donutgrafiek onder het project KPIs wordt gevestigd staat u toe om de verhouding van voltooide het werkpunten tegenover onvolledige het werkpunten in een project te bekijken dat.

![ Taken of kwesties door volledige status ](assets/tasks-issues-by-complete-status-350x250.png)

In het drop-down menu boven de grafiek, kunt u selecteren:

| Alle taken | Het selecteren van **taken** toont u het totale aantal taken in het project, evenals de verhouding tussen voltooide en onvolledige taken. |
|---|---|
| Alle problemen | Het selecteren van **kwesties** toont u het totale aantal kwesties in het project, evenals de verhouding tussen voltooide en onvolledige kwesties. |

>[!TIP]
>
>Als u een lijst met voltooide of onvolledige werkitems wilt weergeven, klikt u op die sectie in het donutdiagram. In die lijst kunt u op een specifiek werkitem klikken om meer details op een nieuw tabblad weer te geven.\
>![ Voltooide takendoos ](assets/completed-tasks-dialog-350x75.png)\
>Voor meer informatie, zie [ de details van Metriek van de Mening ](#view-metrics-details).

## Toegewezen staafdiagram

Het grafiek van de bestemmingsbar toont u het aantal taken die aan elke persoon in het project worden toegewezen. Dit aantal varieert op basis van de categorie die u selecteert in het keuzemenu.

![ Taak en kwesties door toegewezen ](assets/tasks-issues-by-assignee-350x104.png)

U kunt taaktoewijzingen voor een project in de volgende categorieën bekijken:

| Voltooid | Het selecteren **Volledige** toont het aantal taken die aan elke gebruiker worden toegewezen die zijn voltooid. |
|---|---|
| Onvolledig | Het selecteren van **Onvolledige** toont het aantal taken die aan elke gebruiker worden toegewezen die nog niet zijn voltooid. |
| Binnenkort | Het selecteren **Komende** toont het aantal taken die aan elke gebruiker worden toegewezen die nog niet de Geplande Datum van het Begin hebben bereikt. |
| Achterstallig | Het selecteren van **Achterstallig** toont het aantal taken die aan elke gebruiker worden toegewezen die voorbij de Geplande Datum van de Voltooiing zijn en nog niet zijn voltooid. |

>[!TIP]
>
>Als u een lijst met werkitems in de geselecteerde categorie wilt weergeven die aan een specifieke gebruiker zijn toegewezen, klikt u op de balk naast de naam van de gebruiker in het diagram. In die lijst kunt u op een specifiek werkitem klikken om meer details op een nieuw tabblad weer te geven.\
>![ Voltooide takendoos ](assets/completed-tasks-dialog-350x75.png)\
>Voor meer informatie, zie [ de details van Metriek van de Mening ](#view-metrics-details).

## Metrische details weergeven {#view-metrics-details}

U kunt met de grafieken in het gebied van Metriek in wisselwerking staan om verschillende aspecten van een grafiek te bekijken of nauwkeuriger te kijken naar de taken en de kwesties binnen een grafiek.

1. Ga naar het project u metriek voor wilt zien.
1. In het linkerpaneel, klik **Metriek**.\
   In grafieken in het gebied Metriek wordt standaard informatie voor taken weergegeven.\
   ![ sectie van Metriek ](assets/metrics-section-350x298.png)

1. (Voorwaardelijk) als een drop-down pijlvertoningen op een grafiek, de **drop-down pijl** pictogram ![ Dropdown pijl ](assets/dropdown-arrow.png) op de grafiek klikken en de optie selecteren u van het menu wilt.\
   Zie de desbetreffende sectie hierboven voor informatie over de opties die in de menu&#39;s op elk diagram worden weergegeven.

1. (Optioneel) Ga als volgt te werk om taken of problemen voor metrische gegevens op de pagina nader te bekijken:

   1. Klik het element-zulke zoals taken die aan een specifieke gebruiker worden toegewezen, kwesties met een hoge prioriteit, of alle achterstallige taken-die u details voor wilt zien.

      Er wordt een lijst met taken of problemen weergegeven.

      ![ Voltooide takendoos ](assets/completed-tasks-dialog-350x75.png)

   1. Gebruik de pijlen onder aan de lijst om de taak of uitgave te zoeken die u wilt bekijken.

      of

      Selecteer een specifiek nummer om taken of problemen op een specifieke pagina weer te geven.

      ![ Paginering ](assets/pagination-300x152.png)

   1. Selecteer een taak of kwestie om meer details te bekijken.

      De taak of kwestie opent in een nieuw lusje.

1. (Facultatief) om het dashboard van projectmetriek naar een.png- dossier uit te voeren, klik het **pictogram van de Uitvoer** ![, dan uitgezochte ](assets/export.png) Uitvoer als PNG **van het drop-down menu.**

   >[!TIP]
   >
   >Wanneer u het dashboard exporteert, bevat het geëxporteerde bestand alleen de gegevens die op dat moment in uw viewport worden weergegeven. Als u bepaalde onderdelen in het geëxporteerde bestand wilt opnemen, moet u mogelijk omhoog of omlaag schuiven op de pagina of de zoominstellingen van uw browser aanpassen.
