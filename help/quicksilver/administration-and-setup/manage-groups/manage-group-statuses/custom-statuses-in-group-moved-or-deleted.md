---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Aangepaste statussen in een groep die wordt verplaatst of verwijderd
description: In dit artikel wordt uitgelegd wat er gebeurt met het groeperen van aangepaste statussen wanneer u een groep verplaatst of verwijdert.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 83885d86-eb00-46cc-93e9-e3364b6125e8
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# Aangepaste statussen in een groep die wordt verplaatst of verwijderd

In dit artikel wordt uitgelegd wat er gebeurt met het groeperen van aangepaste statussen wanneer u een groep verplaatst of verwijdert.

## Aangepaste statussen in een groep die wordt verplaatst

Overweeg de volgende scenario&#39;s die beschrijven wat aan de status van de groepsdouane gebeurt wanneer u één groep naar een nieuwe plaats onder een andere groep beweegt.

Voor informatie over het bewegen van een groep, zie [ een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md) bewegen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Wanneer u een groep onder een andere groep verplaatst </td> 
   <td> <p>Alle statussen van de verplaatste groep blijven behouden. Ze worden niet toegevoegd aan de status van de nieuwe bovenliggende groep van de groep.</p> <p>Maar de verplaatste groep erft vergrendelde statussen in de groep of groepen die nu hoger in de hiërarchie zijn. En vanaf nu, als een beheerder een hogere status in de hiërarchie vergrendelt, erft de verplaatste groep die status.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Wanneer een status in beide groepen dezelfde sleutel maar verschillende kenmerken heeft</td> 
   <td> <p>Stel dat twee verschillende subgroepen dezelfde niet-vergrendelde status overerven van een bovenliggende groep. De groepsbeheerders van de twee groepen passen dan de status voor hun groepen op verschillende manieren aan.</p> <p>Later wordt een van de twee groepen onder de andere verplaatst. Nu hebben ze beide een status met dezelfde sleutel, maar ze hebben verschillende kenmerken in de twee groepen.</p> <p>In dit geval is een van de volgende situaties waar:</p> 
    <ul> 
     <li>Als de status in de nieuwe bovenliggende groep ontgrendeld is, behoudt de status in de verplaatste groep zijn kenmerken, zonder dat dit door de verplaatsing wordt beïnvloed.</li> 
     <li>Als de status in de nieuwe bovenliggende groep is vergrendeld, overschrijven de kenmerken van de status in de bovenliggende groep die van de status in de verplaatste groep.</li> 
    </ul> <p>Voor informatie over statussleutels, zie <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref"> een status </a> creëren of uitgeven.</p> </td> 
  </tr> 
  <tr> 
   <td>Wanneer een verplaatste groep statussen heeft die van zijn vorige oudergroep worden geërft </td> 
   <td> <p>Alle aangepaste statussen die zijn overgeërfd van de vorige bovenliggende groep worden geleverd met de verplaatste groep en worden de eigen aangepaste statussen. Ze zijn niet meer verbonden met de vorige bovenliggende groep.</p> 
    <ul> 
     <li>Als de vorige bovenliggende groep na de verplaatsing een vergrendelde aangepaste status bewerkt, hebben de wijzigingen geen invloed op de status van de verplaatste subgroep.</li> 
     <li>Als de vorige bovenliggende groep een aangepaste status vergrendelt die was ontgrendeld toen de groep werd verplaatst, is de status van de verplaatste subgroep niet vergrendeld.</li> 
     <li>De verplaatste groep kan nu statussen ontgrendelen die zijn vergrendeld toen deze werden overgeërfd van de vorige bovenliggende groep.</li> 
    </ul> 
     <p><b>VOORBEELD</b><p> 
     <p>Olivia, de groepsbeheerder voor de marketinggroep, maakt twee statussen voor de groep. Ze noemt een Eerste Review, met de sleutel ABC, en vergrendelt het. Ze noemt de andere Final Review, met de sleutel XYZ, en sluit het niet.</p> 
     <p>Zij leidt ook tot een subgroep onder de Marketing groep genoemd Product Marketing. Op het ogenblik dat het wordt gecreeerd, erft het automatisch zowel Eerste Overzicht als Definitieve Overzicht van de Groep van de Marketing.</p> 
     <p>Later verplaatst Olivia de subgroep Product Marketing onder de productgroep. Zowel het Eerste Overzicht als het Definitieve Overzicht gaan met de Groep van de Marketing van het Product aan zijn nieuwe plaats onder de Groep van het Product.</p> 
     <p>Hoewel de Eerste Controle vóór de beweging werd gesloten, kan de de groepsbeheerder van de Marketing van het Product het nu uitgeven omdat het niet meer een geërfte status die door de oudergroep wordt gecontroleerd het van oorsprong was.</p> 
     <p>Definitieve revisie is ontgrendeld en bewerkbaar zoals altijd.</p> 
     <p>Voor de marketinggroep wijzigt Olivia de kleuren van Eerste controle en Laatste controle en wijzigt ze in Eerste controle en Laatste controle bewerkt. Ze vergrendelt ook de voltooide revisie. Ondertussen, in de groep van de Marketing van het Product, veranderen de kleuren en de namen van de statussen Eerste Overzicht en Definitieve Overzicht niet.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Aangepaste statussen in een groep die wordt verwijderd

Wanneer u een groep of subgroep verwijdert, wijst u de bijbehorende informatie, inclusief de aangepaste status, opnieuw toe aan een andere groep of subgroep. De statussen van de verwijderde groep worden toegevoegd aan die van de doelgroep.

Als een van de statussen van de verwijderde groep ook door de bestemmingsgroep werd gebruikt (de status in beide groepen heeft dezelfde sleutel), en de bestemmingsgroep de status op verschillende manieren aanpast, treden de montages van de versie van de bestemmingsgroep de montages van de versie van de verplaatste groep met voeten.

>[!INFO]
>
>**VOORBEELD:**
>
>De groepsbeheerder van Groep A wijzigt een ontgrendelde status op systeemniveau voor haar groep. De groepsbeheerder van Groep B wijzigt ook de naam van die status voor zijn groep. Hoewel de status verschillende namen heeft in de twee groepen, heeft de status dezelfde sleutel.
>
>Later, wordt Groep A geschrapt en al zijn informatie wordt opnieuw toegewezen aan Groep B.
>
>* De naam van de versie van Groep B van de status treedt de naam van de versie van Groep A met voeten.
>* Als de status op een object is toegepast door iemand in groep A voordat die groep is verwijderd, wordt de statusnaam op het object bijgewerkt met de naam voor de status die wordt gebruikt door groep B.
>
>Voor informatie over de sleutel voor een status, zie de lijst in dit artikel onder [ creeer of geef een douanestatus ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md#create) uit [ creeer of geef een status voor een groep ](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create) uit.
>
>Voor informatie over het schrappen van een groep, zie [ een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md) schrappen.
