---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Toegang vereist voor het beheren van bronnen in de werklastverhouding
description: Als u niet beschikt over de juiste toegang of machtigingen, kunt u uw werktoewijzingen mogelijk niet weergeven of beheren in Workload Balancer.
author: Lisa
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---

# Toegang vereist voor het beheer van bronnen in het werklastevenwicht

{{preview-fast-release-general}}

Als u niet beschikt over de juiste toegang of machtigingen, kunt u uw werktoewijzingen mogelijk niet weergeven of beheren in Workload Balancer.

U moet toegang hebben om de gebruikers te bekijken waarvan werkbelasting u in de Balancer van de Werkbelasting wilt bekijken of beheren. Bovendien moet u het correcte toegangsniveau en de correcte toestemmingen op de projecten hebben het werk met wordt geassocieerd.

<!--## Adobe Workfront package needed to use the Workload Balancer for different areas

The following table illustrates the connection between the Workfront plan your company has and where in the system you can use the Workload Balancer:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><p><b>Workfront Plan (Current)</b></p></td> 
   <td> <p><b>Areas where you can access the Workload Balancer</b></p> </td> 
  </tr> 
  <tr> 
   <td>Team or higher </td> 
   <td>Workload Balancer for a team or a project</td> 
  </tr> 
  <tr> 
   <td>Pro or higher</td> 
   <td>Workload Balancer for multiple projects, at the system level</td> 
  </tr> 
  <tr> 
   <td><p><b>Workfront Plan (New)</b></p></td> 
   <td> <p><b>Areas where you can access the Workload Balancer</b></p> </td> 
  </tr>
  <tr> 
   <td>Any </td> 
   <td>Access the Workload Balancer anywhere in Workfront</td> 
  </tr> 
 </tbody> 
</table>

For information about the Workfront plans, see [Our Plans](https://business.adobe.com/products/workfront/pricing.html).

For information about where you can locate the Workload Balancer in Workfront, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).-->

## Toegang nodig om werklastbalans weer te geven

U moet de volgende toegang hebben om de werklastbalans te kunnen bekijken:

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
   <td><p>Standard</p>
       <p>Plan, om de Balancer van de Werkbelasting in het gebied van Middelen te bekijken; het werk, om de Balancer van de Werkbelasting van een team of een project te bekijken</p></td>
  </tr>  
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot resourcebeheer weergeven of vergroten</p> <p>Voor informatie over het de toegangsniveau van het Beheer van het Middel, zie de artikel <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md"> toegang van de Verlening tot het Beheer van het Middel </a>.</p></td> 
  </tr> 
  <tr> 
   <td>Objectmachtigingen</td> 
   <td> <p>U moet de toestemmingen van de Mening op het project hebben waarvan taken u wilt bekijken. </p> <p>Voor informatie over projecttoestemmingen, zie het artikel <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md"> een project in Adobe Workfront </a> delen.</p></td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<span class="preview"> alle gebruikers hebben toegang om de Balancer van de Werkbelasting op hun eigen profielen te bekijken. Dit wordt niet beperkt door vergunning of toegangsniveau. Merk op dat de Balancer van de Werkbelasting op een gebruikersprofiel read-only is, en de taken en de toewijzingen kunnen niet worden veranderd.</span>

## Toegang nodig voor het beheer van toewijzingen in Workload Balancer

U moet de volgende toegang hebben om de werklastverdeling te beheren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td>
  </tr>
  <tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan, om taken in de Balancer van de Werkbelasting in het gebied van de Middelen te beheren; het werk, om taken in de Balancer van de Werkbelasting van een team of een project te beheren</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td>
   <td> <p>Toegang tot resourcebeheer bewerken</p>
     <p>Voor informatie over het de toegangsniveau van het Beheer van het Middel, zie de artikel <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" > toegang van de Verlening tot het Beheer van het Middel </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Objectmachtigingen</td> 
   <td> <p> Draag of hogere toestemmingen op het project bij waarvan taken u wilt beheren die toestemmingen omvat om taken te maken. </p> <p>Voor informatie over projecttoestemmingen, zie het artikel <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md"> een project in Adobe Workfront </a> delen.</p></td>
  </tr> 
 </tbody>
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->
