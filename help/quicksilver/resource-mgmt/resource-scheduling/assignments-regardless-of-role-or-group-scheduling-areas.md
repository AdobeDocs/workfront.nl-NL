---
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: Gebruikerstoewijzingen ongeacht rol en groepslidmaatschap in de planningsgebieden toestaan
description: In het Planning van het Middel, kunnen de taken slechts aan gebruikers worden gemaakt die een rol hebben die op hun gebruikersprofiel wordt bepaald dat de roltaak van de taak of de kwestie aanpast die aan hen wordt toegewezen.
author: Alina
feature: Resource Management
exl-id: 0f90ffde-6f07-4c3c-b963-de28b1b55dc1
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%

---

# Gebruikerstoewijzingen ongeacht rol en groepslidmaatschap in de planningsgebieden toestaan

>[!IMPORTANT]
>  
><span class="preview">De planningsfunctionaliteit die in dit artikel wordt beschreven, is vanaf de release 23.1 in januari 2023 vervangen en uit Adobe Workfront verwijderd.   </span>
>  
> <span class="preview"> Dit artikel wordt ook verwijderd kort na de release van 23.1, begin 2023. Op dit moment raden we u aan eventuele bladwijzers dienovereenkomstig bij te werken. </span>
> 
><span class="preview"> U kunt de werklastbalans nu gebruiken om werk voor uw bronnen te plannen. </span>
>  
> <span class="preview">Voor informatie over het plannen van middelen die de Balancer van de Werkbelasting gebruiken, zie de sectie [De werklastbalans](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!-- 

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer.</span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;***LINKED TO THE UI FROM Resource Scheduling (People> Teams>Working On>Settings>Limit Assignments to the Group Associated with the Project) - ALSO FROM THE WORKING ON TAB OF TEAMS and AT THE PROJECT STAFFING TAB TOO)</p>
<p>NOTE: Alina; broken off the original article; retitle, reformat, relink sections) </p>
</div>
-->

Door gebrek, kunnen de taken slechts aan gebruikers worden gemaakt die een rol hebben die op hun gebruikersprofiel wordt bepaald dat de roltaak van de taak of de kwestie aanpast die aan hen wanneer het gebruiken van het Middel dat hulpmiddelen plant wordt toegewezen.

U kunt Adobe Workfront zodanig configureren dat taken en problemen kunnen worden toegewezen aan elke gebruiker, ongeacht of die gebruiker een rol heeft gedefinieerd in zijn gebruikersprofiel die overeenkomt met de roltoewijzing van de taak of uitgave die aan hem of haar wordt toegewezen. Wanneer u een gebruiker aan een taak of een kwestie toewijst en die gebruiker geen rol heeft die de roltaak op de taak of de kwestie aanpast, wordt de originele roltaak verwijderd, en de roltaak verandert in de rol van de gebruiker u toewijst.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau*</td> 
   <td> <p>De mening of hogere toegang tot Projecten, Taken, en Kwesties</p> <p><strong>OPMERKING</strong>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute-machtigingen of hoger voor de projecten, taken en uitgaven waarvoor u toewijzingen bijwerkt</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Toewijzingen aan gebruikers ongeacht rol toestaan

1. Ga naar de het plannen chronologie voor veelvoudige projecten, voor een individueel project, of voor een team:

   * **Voor meerdere projecten**: Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Bronnen > Werklastverdeling** selecteert u vervolgens **Planning** in het drop-down menu linksboven.
   * **Voor een afzonderlijk project**: Ga naar een project, klik **Werklastverdeling** in het linkerdeelvenster en selecteer vervolgens **Planning** in het keuzemenu linksboven.
   * **Voor een team**: Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Teams**, selecteert u een team en klikt u op **Werklastverdeling** in het linkerdeelvenster selecteert u vervolgens **Planning** in het keuzemenu linksboven.

1. Klik op de knop **Instellingen** op de tijdlijn van de planning.
1. De optie uitschakelen **Toewijzingen beperken tot gebruikers met dezelfde rol**.
1. Klikken **Terugkeren naar planning**.

## Toewijzingen aan gebruikers ongeacht het groepslidmaatschap toestaan

<!--
<p>(NOTE: Alina: **^ This section is linked to the UI in a tooltip inside the Settings of the scheduler. do not rename/ remove/ edit the tag!!) </p>
-->

Door gebrek, kunnen de taken slechts aan gebruikers worden gemaakt die lid van de groep zijn die met het project wordt geassocieerd (dit is de groep die wanneer het uitgeven van het project wordt bepaald).

>[!IMPORTANT]
>
>Deze instelling houdt alleen rekening met de leden van de groep die bij het project horen, en niet met leden van subgroepen van die groep.

U kunt Workfront vormen om taken en kwesties toe te staan om aan om het even welke gebruiker worden toegewezen, ongeacht of die gebruiker een lid van de groep is die met het project wordt geassocieerd waar de taak of de kwestie verblijft.

1. Ga naar de het plannen chronologie voor veelvoudige projecten, voor een individueel project, of voor een team:

   * **Voor meerdere projecten**: Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Bronnen > Werklastverdeling** selecteert u vervolgens **Planning** in het drop-down menu linksboven.
   * **Voor een afzonderlijk project**: Ga naar een project, klik **Werklastverdeling** in het linkerdeelvenster en selecteer vervolgens **Planning** in het keuzemenu linksboven.
   * **Voor een team**: Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Teams**, selecteert u een team en klikt u op **Werklastverdeling** in het linkerdeelvenster selecteert u vervolgens **Planning** in het keuzemenu linksboven.

1. Klik op de knop **Instellingen** op de tijdlijn van de planning.
1. De optie uitschakelen **Toewijzingen beperken aan de groep die is gekoppeld aan het project**.
1. Klikken **Terugkeren naar planning**.

 
