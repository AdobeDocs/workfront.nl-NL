---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Toegang vereist voor het beheren van bronnen in de werklastverhouding
description: Als u niet beschikt over de juiste toegang of machtigingen, kunt u uw werktoewijzingen mogelijk niet weergeven of beheren in Workload Balancer.
author: Lisa
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: 78d73d0d7bd0ffc00ae1afed0adb324501e0c310
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Toegang vereist voor het beheer van bronnen in het werklastevenwicht

{{preview-fast-release-general}}

Als u niet beschikt over de juiste toegang of machtigingen, kunt u uw werktoewijzingen mogelijk niet weergeven of beheren in Workload Balancer.

U moet toegang hebben om de gebruikers te bekijken waarvan werkbelasting u in de Balancer van de Werkbelasting wilt bekijken of beheren. Bovendien moet u het correcte toegangsniveau en de correcte toestemmingen op de projecten hebben het werk met wordt geassocieerd.

## Adobe Workfront-plan vereist voor gebruik van de werklastverdeling voor verschillende gebieden

In de volgende tabel ziet u de verbinding tussen het Workfront-plan dat uw bedrijf heeft en de locatie in het systeem waar u de Workload Balancer kunt gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p><b>Workfront-abonnement (huidig)</b></p></td> 
   <td> <p><b>Gebieden waar u tot de Balancer van de Werkbelasting kunt toegang hebben</b></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Team of hoger </td> 
   <td>Werklastbalans voor een team of project</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pro of hoger</td> 
   <td>Werklastbalans voor meerdere projecten, op systeemniveau</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p><b>Workfront-abonnement (nieuw)</b></p></td> 
   <td> <p><b>Gebieden waar u tot de Balancer van de Werkbelasting kunt toegang hebben</b></p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Alle </td> 
   <td>Overal in Workfront toegang tot werklastbalans</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie over de plannen van Workfront, zie [&#x200B; Onze Plannen &#x200B;](https://business.adobe.com/nl/products/workfront/pricing.html).

Voor informatie over waar u van de Balancer van de Werkbelasting in Workfront kunt de plaats bepalen, zie [&#x200B; plaats van de Balancer van de Werkbelasting &#x200B;](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Toegang nodig om werklastbalans weer te geven

U moet de volgende toegang hebben om de werklastbalans te kunnen bekijken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan, om de Balancer van de Werkbelasting in het Bronsgebied te bekijken;</br>
       Het werk, om de Balancer van de Werkbelasting van een team of een project te bekijken</p></td>
  </tr>  
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot resourcebeheer weergeven of vergroten</p> <p>Voor informatie over het de toegangsniveau van het Beheer van het Middel, zie de artikel <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref"> toegang van de Verlening tot het Beheer van het Middel </a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>U moet de toestemmingen van de Mening op het project hebben waarvan taken u wilt bekijken. </p> <p>Voor informatie over projecttoestemmingen, zie het artikel <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref"> een project in Adobe Workfront </a> delen.</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<span class="preview"> alle gebruikers hebben toegang om de Balancer van de Werkbelasting op hun eigen profielen te bekijken. Dit wordt niet beperkt door vergunning of toegangsniveau. Merk op dat de Balancer van de Werkbelasting op een gebruikersprofiel read-only is, en de taken en de toewijzingen kunnen niet worden veranderd.</span>

## Toegang nodig voor het beheer van toewijzingen in Workload Balancer

U moet de volgende toegang hebben om de werklastverdeling te beheren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan, om taken in de Balancer van de Werkbelasting op het gebied van de Middelen te beheren;</br>
       Werk, om taken in de Balancer van de Werkbelasting van een team of een project te beheren</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot resourcebeheer bewerken</p> 
     <p>Voor informatie over het de toegangsniveau van het Beheer van het Middel, zie de artikel <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref"> toegang van de Verlening tot het Beheer van het Middel </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p> Draag of hogere toestemmingen op het project bij waarvan taken u wilt beheren die toestemmingen omvat om taken te maken. </p> <p>Voor informatie over projecttoestemmingen, zie het artikel <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref"> een project in Adobe Workfront </a> delen.</p></td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->
