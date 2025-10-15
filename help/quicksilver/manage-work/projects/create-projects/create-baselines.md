---
product-area: projects
navigation-topic: create-projects
title: Projectbasislijnen maken
description: Een basislijn is een projectmomentopname die zeer belangrijke stukken van informatie inbegrepen in het aanvankelijke projectplan of op om het even welk bepaald ogenblik tijdens het leven van het project vertegenwoordigt.
author: Alina
feature: Work Management
exl-id: 422bd7a5-d7a0-4c24-8624-bd0fe6e79d7b
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# Projectbasislijnen maken

<!-- Audited: 08/2025 -->

Een basislijn is een projectmomentopname die zeer belangrijke stukken van informatie inbegrepen in het aanvankelijke projectplan of op om het even welk bepaald ogenblik tijdens het leven van het project vertegenwoordigt.

U kunt basislijn gebruiken om die stukken van informatie van het huidige plan met het originele plan of een ander punt in tijd te vergelijken, om probleemtaken, werkingsgebiedkneep, en andere tendensen in tijd te identificeren.

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
    <td><p>Standard</p>
        <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuratie op toegangsniveau</td> 
   <td> <p>Toegang tot projecten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven voor het project of hoger om basislijnen weer te geven</p> <p>Rechten voor het project beheren om basislijnen te maken</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
    <td><p>New: Standard</p>
        <p>or</p>
        <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher to view baselines</p> <p>Manage permissions to the project to create baselines</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Overwegingen bij het werken met basislijnen

* U kunt een momentopname van de vooruitgang op een project vangen veelvoudige tijden tijdens het leven van het project, creërend veelvoudige basislijnen.
* U kunt de informatie bekijken inbegrepen in de basislijnen van een project door een basislijn te creëren of door een rapport van de Basislijn te bouwen.
* Wanneer u een basislijn maakt, worden de taakgegevens ook vastgelegd op de basislijntaken van die basislijn.
* U kunt de informatie van de basislijntaken bekijken door een rapport van de Taak van de Basislijn te bouwen.

>[!IMPORTANT]
>
>Een basislijn neemt een momentopname van de naam, de data, en de financiële informatie van het project. De basislijn omvat niet de waarden van douanegebieden op het project. Voor informatie over financiële informatie inbegrepen in de basislijn, zie [&#x200B; de financiën van het Project inbegrepen in projectbasislijnen &#x200B;](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Een basislijn maken

U kunt op de volgende manieren een basislijn maken:

* **automatisch**: Uw beheerder van Workfront of een groepsbeheerder plaatst de projectvoorkeur voor Workfront om een basislijn automatisch tot stand te brengen wanneer een project Huidig wordt. Wanneer deze instelling is ingeschakeld, wordt een basislijn gemaakt wanneer de projectstatus Huidig wordt. Als deze instelling niet is ingeschakeld, moet u handmatig basislijnen maken.

  Voor meer informatie over het vormen van projectvoorkeur en vestiging automatische basislijnverwezenlijking, zie [&#x200B; systeem-brede projectvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

  >[!CAUTION]
  >
  >Als u deze instelling inschakelt, wordt automatisch een basislijn voor een project gemaakt telkens wanneer de status van een project verandert in Huidig. De eerste gemaakte basislijn is de standaard. Tijdens de levensduur van het project moet u handmatig alle andere basislijnen maken.

* **manueel**: U kunt nieuwe basislijnen voor het project tot stand brengen zoals nodig aangezien het project vordert. U kunt dan basislijnen vergelijken om te zien hoe het project in tijd vorderde.

Een basislijn maken:

1. Ga naar een project.
1. In het linkerpaneel, klik **Basislijnen**.

   ![&#x200B; sectie van Baselines op project &#x200B;](assets/baselines-section-on-project-with-header.png)

1. Klik **Nieuwe Basislijn.**
1. Geef de naam voor de basislijn op.
1. (Optioneel) Als dit de eerste basislijn is, kunt u deze als de standaardbasislijn kiezen.
1. Klik **sparen**.

   Standaard wordt de volgende informatie weergegeven over de basislijn die u hebt gemaakt:

   * Naam basislijn
   * Datum basislijninvoer
   * Geplande begindatum van het project toen de basislijn werd gecreeerd
   * Geprojecteerde begindatum van het project toen de basislijn werd gecreeerd
   * Werkelijke duur van het project toen de basislijn werd gecreeerd
   * % Voltooien van het project toen de basislijn werd gecreeerd
   * Standaardbasislijnindicator die aangeeft of een basislijn de standaardbasislijn van het project is

     >[!TIP]
     >
     >U kunt geen informatie van om het even welke twee basislijnen tezelfdertijd in de zelfde mening of het rapport bekijken. U kunt informatie van een bepaalde basislijn en de Standaard basislijn slechts bekijken in het zelfde rapport. U kunt wijzigen welke basislijn u als Standaardbasislijn beschouwt wanneer tijdens het leven van het project.

1. (Facultatief) klik de **knoop van de Mening**, dan creeer een nieuwe mening of geef de huidige mening uit om gebieden aan de mening toe te voegen en extra informatie tussen basislijnen te vergelijken. Voor informatie, zie [&#x200B; meningen in Adobe Workfront &#x200B;](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) creëren of uitgeven.

## Creeer een Baseline of een rapport van de Taak van de Basislijn

Om basislijninformatie te bekijken, kunt u een rapport van de Taak van de Basislijn of van de Basislijn ook tot stand brengen. Hierdoor kunt u een willekeurig aantal velden weergeven over de basislijnen of basislijntaken om deze in één weergave te vergelijken.

>[!TIP]
>
>U moet een basislijn creëren alvorens u een rapport van de Taak van de Basislijn of van de Basislijn kunt tot stand brengen.

Voor informatie over het creëren van een rapport, zie [&#x200B; een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

Wij adviseren dat u een groepering van de Naam van het Project aan uw rapport van de Taak van de Basislijn of van de Basislijn toevoegt om het gemakkelijker te maken te lezen.

Voor informatie over het creëren van een groepering, zie [&#x200B; groepen in Adobe Workfront &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md) creëren.
