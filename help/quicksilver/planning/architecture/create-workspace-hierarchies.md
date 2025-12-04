---
title: Workspace-hiërarchieën maken
description: Als werkruimtemanager kunt u meerdere werkruimtemhiërarchieën maken tussen de recordtypen in Adobe Workfront Planning. Nadat u recordtypes in een werkruimte verbindt en een hiërarchie creeert, worden de verslagtypes verbonden met elkaar, met één verslagtype dat als ouder en tot 6 andere verslagtypes wordt aangewezen die als kinderen worden gevormd.
hide: true
hidefromtoc: true
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: ff9371b639e7684a94c08b8cd6293b632fac9edf
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Create Workspace Hierarchies
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---

-->

# Hiërarchieën voor werkruimten maken

Als werkruimtemanager kunt u meerdere werkruimtemhiërarchieën maken tussen de recordtypen in Adobe Workfront Planning.

Nadat u recordtypes in een werkruimte verbindt en een hiërarchie creeert, worden de verslagtypes verbonden met elkaar, met één verslagtype dat als ouder en tot 6 andere verslagtypes wordt aangewezen die als kinderen worden gevormd. <!--asking Robert how many we can have in one hierarchy; I think 7 total but not sure-->

Hierarchieën genereren broodkruimels voor de recordtypen en records <!--ensure this is the case: does the breadcrumb show for both the RT and the record??--> die in de koppen worden weergegeven. Op deze manier weten gebruikers waar ze zich in de hiërarchie bevinden in elk stadium van hun workflow.

Voor algemene informatie over hiërarchieën en broodkruimels, zie [&#x200B; Hiërarchie en breadcrumb overzicht &#x200B;](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).


## Toegangsvereisten

<!--check the access to see if you oversimplified???-->

<!--Update the TOC for this to publish-->

+++ Breid uit om de toegangsvereisten te bekijken om de stappen in dit artikel uit te voeren:  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<ul> 
<li><p>Alle Workfront en alle planningspakketten</p></li>
of
<li><p>Willekeurige workflow en planningspakket</p></li></ul>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Machtigingen beheren in een werkruimte</p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr>  
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een werkruimtehiërarchie maken
