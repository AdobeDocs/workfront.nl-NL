---
product-area: projects
navigation-topic: use-predecessors
title: Voorgangers afdwingen
description: Predecessors zijn taken waarvan andere taken afhankelijk zijn voor voltooiing. Relaties van vorige versies zijn van invloed op de start- en voltooiingsdatums van de taken en hebben uiteindelijk invloed op de tijdlijn van het project.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Voorgangers afdwingen

<!-- Audited: 2/2024 -->

Predecessors zijn taken waarvan andere taken afhankelijk zijn voor voltooiing. Relaties van vorige versies zijn van invloed op de start- en voltooiingsdatums van de taken en hebben uiteindelijk invloed op de tijdlijn van het project.

Voor informatie over predecessors, zie [&#x200B; Overzicht van taakvoordecessors &#x200B;](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Door voorgangerrelaties tussen taken in te stellen, definieert u hoe het begin of einde van een afhankelijke taak afhankelijk is van het begin of einde van hun voorgangertaken. Dit wordt gedaan door verschillende Types van Afhankelijkheid te gebruiken.

Voor informatie over de Types van Afhankelijkheid, zie [&#x200B; Overzicht van de types van taakgebiedsdeel &#x200B;](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Overzicht van gedwongen voorgangers

>[!IMPORTANT]
>
>U moet predecessors afdwingen om te vereisen dat de vorige verhoudingen worden gerespecteerd. Zonder de voorgangers af te dwingen, kunnen afhankelijke taken onafhankelijk van het begin en einde van hun voorgangers beginnen en eindigen, ongeacht het type afhankelijkheid.

U kunt de voorgaande relatie afdwingen wanneer u voorgangers voor een project instelt.

Als een voorganger wordt afgedwongen, kan de opvolgertaak niet worden gestart voordat de voorganger is voltooid. Bijvoorbeeld, het afdwingen van een eind-Begin verhouding tussen Taak A en Taak B betekent dat Taak B niet kan beginnen (de Status moet Nieuw blijven, en Percent moet 0%) blijven tot Taak A zoals voltooid duidelijk is. Het afdwingen van verhoudingen is op alle voorgangstypen van toepassing.

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
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
      <p>Nieuw: Standaard</p> 
      <p>OF</p>
      <p>Huidig: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot taken en projecten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td><p>Rechten voor de taken en het project beheren</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een voorganger op taakniveau afdwingen

1. Ga naar de opvolgertaak waarvan voorganger u wilt afdwingen.
1. Klik **Voorgangers** in het linkerpaneel, dan klik **toevoegen Voorganger**.
1. (Voorwaardelijk) Als u een dwars-projectvoorganger wilt toevoegen, verwijder de naam van het project op het **gebied van het Project van de Ouder 1&rbrace; en vervang het met een ander project.**
1. Specificeer de naam van de voorgangerstaak of de taken op het **gebied van Taken**.
1. Specificeer het **Type van Afhankelijkheid** tussen deze twee taken.

   Het standaard **Type van Afhankelijkheid** is **eind-Begin**.

1. Selecteer het **Gedwongen** gebied om predecessor af te dwingen.
1. Klik **sparen**.

## Een voorganger afdwingen in een takenlijst

1. Ga naar een taaklijst in een project.
1. Van het **drop-down menu van de Mening**, selecteer de **StandaardMening**.

1. Neem nota van het aantal taak die u als voorganger zult aanwijzen.
1. Zoek de opvolgertaak waarvan u de voorganger wilt afdwingen.
1. In de **kolom van Predecessors**, begin het aantal van de voorgangertaak in te gaan die door &quot;e&quot;wordt gevolgd. Typ bijvoorbeeld &quot;1e&quot; om taaknummer 1 als voorganger aan de geselecteerde taak toe te voegen.
1. Klik op Enter om uw voorganger-informatie voor de taak op te slaan.

   ![&#x200B; predecessor_required_in_list.png &#x200B;](assets/predecessor-enforced-in-list-350x308.png)
