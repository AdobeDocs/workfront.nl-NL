---
product-area: projects
navigation-topic: create-projects
title: Projectbasislijnen maken
description: Een basislijn is een projectmomentopname die zeer belangrijke stukken van informatie inbegrepen in het aanvankelijke projectplan of op om het even welk bepaald ogenblik tijdens het leven van het project vertegenwoordigt.
author: Alina
feature: Work Management
exl-id: 422bd7a5-d7a0-4c24-8624-bd0fe6e79d7b
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Projectbasislijnen maken

<!-- Audited: 12/2023 -->

Een basislijn is een projectmomentopname die zeer belangrijke stukken van informatie inbegrepen in het aanvankelijke projectplan of op om het even welk bepaald ogenblik tijdens het leven van het project vertegenwoordigt.

U kunt basislijn gebruiken om die stukken van informatie van het huidige plan met het originele plan of een ander punt in tijd te vergelijken, om probleemtaken, werkingsgebiedkneep, en andere tendensen in tijd te identificeren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<!--
drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher to view baselines</p> <p>Manage permissions to the project to create baselines</p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
    <td><p>Nieuw: Standaard</p>
        <p>of</p>
        <p>Huidig: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau</td> 
   <td> <p>Toegang tot projecten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven voor het project of hoger om basislijnen weer te geven</p> <p>Rechten voor het project beheren om basislijnen te maken</p> </td> 
  </tr> 
 </tbody> 
</table>

*For meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het werken met basislijnen

* U kunt een momentopname van de vooruitgang op een project vangen veelvoudige tijden tijdens het leven van het project, creërend veelvoudige basislijnen.
* U kunt de informatie bekijken inbegrepen in de basislijnen van een project door een basislijn te creëren of door een rapport van de Basislijn te bouwen.
* Wanneer u een basislijn maakt, worden de taakgegevens ook vastgelegd op de basislijntaken van die basislijn.
* U kunt de informatie van de basislijntaken bekijken door een rapport van de Taak van de Basislijn te bouwen.

>[!IMPORTANT]
>
>Een basislijn neemt een momentopname van de naam, de data, en de financiële informatie van het project. De basislijn omvat niet de waarden van douanegebieden op het project. Voor informatie over financiële informatie inbegrepen in de basislijn, zie [ de financiën van het Project inbegrepen in projectbasislijnen ](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Een basislijn maken

U kunt op de volgende manieren een basislijn maken:

* **automatisch**: Uw beheerder van Workfront of een groepsbeheerder plaatst de projectvoorkeur voor Workfront om een basislijn automatisch tot stand te brengen wanneer een project Huidig wordt. Wanneer deze instelling is ingeschakeld, wordt een basislijn gemaakt wanneer de projectstatus Huidig wordt. Als deze instelling niet is ingeschakeld, moet u handmatig basislijnen maken.

  Voor meer informatie over het vormen van projectvoorkeur en vestiging automatische basislijnverwezenlijking, zie [ systeem-brede projectvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

  >[!CAUTION]
  >
  >Als u deze instelling inschakelt, wordt automatisch een basislijn voor een project gemaakt telkens wanneer de status van een project verandert in Huidig. De eerste gemaakte basislijn is de standaard. Tijdens de levensduur van het project moet u handmatig alle andere basislijnen maken.

* **manueel**: U kunt nieuwe basislijnen voor het project tot stand brengen zoals nodig aangezien het project vordert. U kunt dan basislijnen vergelijken om te zien hoe het project in tijd vorderde.

Een basislijn maken:

1. Ga naar een project.
1. In het linkerpaneel, klik **Basislijnen**.

   ![ sectie van Baselines op project ](assets/baselines-section-on-project-with-header.png)

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

1. (Facultatief) klik de **knoop van de Mening**, dan creeer een nieuwe mening of geef de huidige mening uit om gebieden aan de mening toe te voegen en extra informatie tussen basislijnen te vergelijken. Voor informatie, zie [ meningen in Adobe Workfront ](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) creëren of uitgeven.

## Creeer een Baseline of een rapport van de Taak van de Basislijn

Om basislijninformatie te bekijken, kunt u een rapport van de Taak van de Basislijn of van de Basislijn ook tot stand brengen. Hierdoor kunt u een willekeurig aantal velden weergeven over de basislijnen of basislijntaken om deze in één weergave te vergelijken.

>[!TIP]
>
>U moet een basislijn creëren alvorens u een rapport van de Taak van de Basislijn of van de Basislijn kunt tot stand brengen.

Voor informatie over het creëren van een rapport, zie [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

Wij adviseren dat u een groepering van de Naam van het Project aan uw rapport van de Taak van de Basislijn of van de Basislijn toevoegt om het gemakkelijker te maken te lezen.

Voor informatie over het creëren van een groepering, zie [ groepen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md) creëren.
