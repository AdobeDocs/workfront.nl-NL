---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groeperen: projectsponsor voor uren'
description: Deze uurgroepering organiseert uren door de sponsor van het project waar de uren worden geregistreerd. De standaardinterface van de rapportbouwer voor uurgroepen verstrekt geen afbeelding aan het gebied van de Sponsor van het Project. U moet de interface van de Wijze van de Tekst gebruiken om tot dit gebied toegang te hebben.
author: Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: bc99e303047b989b972974b398420a9180e40874
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Groepering: projectsponsor voor uren

<!--Audited: 10/2024-->

Deze uurgroepering organiseert uren door de sponsor van het project waar de uren worden geregistreerd. De standaardinterface van de rapportbouwer voor uurgroepen verstrekt geen afbeelding aan het gebied van de Sponsor van het Project. U moet de interface van de Wijze van de Tekst gebruiken om tot dit gebied toegang te hebben.

![ hour_report_grouped_by_sponsor.png ](assets/hour-report-grouped-by-sponsor-350x39.png)

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

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
   <td> 
    <p>Nieuw:</p>
   <ul><li><p>Medewerker om een filter te wijzigen </p></li>
   <li><p>Standaard voor het wijzigen van een rapport</p></li> </ul>

<p>Huidige:</p>
   <ul><li><p>Verzoek om een filter te wijzigen </p></li>
   <li><p>Plan om een rapport te wijzigen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Uren groeperen op projectsponsor

Deze groep toepassen:

1. Ga naar een lijst met uren.
1. Van **het Groeperen** drop-down menu, uitgezochte **Nieuwe Groepering**.

1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. Verwijder de tekst in het gebied dat wordt weergegeven en vervang deze door de volgende code:

```
   group.0.linkedname=project:sponsor:name
   group.0.name=
   group.0.valuefield=project:sponsor:name
   group.0.valueformat=HTML
   textmode=true
```

1. Klik **Gedaan**.
1. Werk de groeperingsnaam bij, dan klik **sparen Groepering**.
