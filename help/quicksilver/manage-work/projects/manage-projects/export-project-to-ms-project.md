---
product-area: projects
navigation-topic: manage-projects
title: Een project exporteren naar Microsoft Project
description: U kunt Adobe Workfront-projecten exporteren naar Microsoft Project.
author: Alina
feature: Work Management
exl-id: 3f0f3644-a763-4b72-a93a-85af8626b5b3
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Een project exporteren naar Microsoft Project

U kunt Adobe Workfront-projecten exporteren naar Microsoft Project. 

>[!IMPORTANT]
>
>* Niet alle Workfront-velden worden overgebracht naar het Microsoft-projectbestand.\
>  Voor meer informatie over de verenigbaarheid van gebieden tussen het Project van Workfront en van Microsoft, zie de gebieden van het Project van Microsoft van de artikel [ Kaart aan de projecten van Adobe Workfront ](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).
>* Wij adviseren dat u het aantal tijden beperkt u projecten van één toepassing aan een andere overbrengt. 
>

## Toegangsvereisten

<!--drafted for P&P:

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
   <td>  <p>Current license: Light or higher</p>
   Or
   <p>Legacy license: Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the project</p> <p>For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten weergeven of vergroten</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over toegang tot projecten, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref"> toegang van de Verlening tot projecten </a>. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p> De toestemmingen van de mening of hoger aan het project</p> <p>Voor informatie over projecttoestemmingen, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref"> een project in Adobe Workfront </a> delen.</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Een project exporteren van Workfront naar Microsoft Project

U kunt een project van Workfront van de projectpagina of van een projectlijst of een rapport uitvoeren.

1. Ga naar het project u wilt uitvoeren en **klikken Meer** pictogram ![](assets/qs-more-menu.png) rechts van de projectnaam

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   of

   Ga naar een projectlijst of een rapport en selecteer een project, dan klik het Meer pictogram ![](assets/qs-more-menu.png) bij de bovenkant van de lijst.

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. Klik **het Project van MS van de Uitvoer**.

   Het project wordt als een XML-bestand naar uw computer gedownload en kan worden geïmporteerd in Microsoft Project. 
