---
content-type: overview
product-area: projects
navigation-topic: financials
title: Een overloopverhouding definiëren
description: U kunt een overloopverhouding op een taak bepalen om de Geplande berekening van de Inkomsten voor de taaktaken aan te passen.
author: Lisa
feature: Work Management
source-git-commit: bf8dcc9dfa9697c8d212072bb511c57aa01e7529
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Een overloopverhouding definiëren

{{highlighted-preview-article-level}}

Wanneer een overloopverhouding aan een taak wordt toegevoegd, wordt het toegepast op alle taken op de taak. Het vermenigvuldigt alle Geplande Uren voor die taak en beïnvloedt de Geplande berekeningen van de Inkomsten.

De overloopverhouding kan niet variëren voor toewijzingen binnen dezelfde taak. Als verschillende overloopmultipliers worden vereist, moet u afzonderlijke subtaken onder een oudertaak tot stand brengen.

>[!NOTE]
>
>Er is geen validatie die voorkomt dat de overloopverhouding wordt toegevoegd aan een niet-overlopende taak.

## Berekening van de overuren van de geplande inkomsten

Het systeem bepaalt eerst het factureringstarief gebruikend de standaardhet facturerings tariefhiërarchie. Voor meer informatie, zie [ Overzicht van opbrengst en kostenhiërarchie ](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

Als de overloopverhouding op de taak bestaat, dan is de berekening:
Geplande inkomsten = Facturerings- × overloopratio × Geplande uren

Als de overloopverhouding leeg is, wordt de berekening als volgt berekend:
Geplande inkomsten = Factureringsgraad × geplande uren

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>Toegang tot taken, projecten en financiële gegevens bewerken</td> 
  </tr> 
  <tr> 
   <td>Objectmachtigingen</td> 
   <td><p>Machtigingen beheren voor een taak die factureringssnelheden bewerken bevat</p>
     <p>Contribute of hoger machtigingen voor het project</p></td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Het type van taakopbrengst moet Gebruiker en Rol Uur zijn. Voor meer informatie, zie [ Overzicht van opbrengst en kostenhiërarchie ](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

Het **gebied van de Verhouding van de Overuren** moet op uw lay-outmalplaatje worden toegelaten.

1. In het lay-outmalplaatje, klik de benedenpijl onder **aanpassen welke gebruikers** zien, dan **Taak** klikken.
1. In de **sectie van Details**, selecteer het **gebied van de Verhouding van de Overuren** in het **Financiën** gebied.

   Voor meer informatie, zie [ de mening van Details aanpassen gebruikend een lay-outmalplaatje ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

## De overloopverhouding voor een taak definiëren

1. Ga naar de taak die u wilt bewerken.

   Voor meer informatie, zie [ taakfinanciën in de sectie van de Details van de Taak beheren ](/help/quicksilver/manage-work/tasks/manage-tasks/task-finances-in-details.md).

1. Klik **Details van de Taak** in het linkerpaneel.
1. Op het **gebied van de Financiën**, ga overtime vermenigvuldiger op het **gebied van de Verhouding van de Overuren** in.
1. Klik **sparen Veranderingen**.

