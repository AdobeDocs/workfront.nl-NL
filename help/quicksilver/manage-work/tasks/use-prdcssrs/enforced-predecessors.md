---
product-area: projects
navigation-topic: use-predecessors
title: Voorgangers afdwingen
description: Predecessors zijn taken waarvan andere taken afhankelijk zijn voor voltooiing. Relaties van vorige versies zijn van invloed op de start- en voltooiingsdatums van de taken en hebben uiteindelijk invloed op de tijdlijn van het project.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: 7a9232f59e4c6f2eac2995be7d7862295b6bab2c
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Voorgangers afdwingen

<!-- Audited: 2/2024 -->

Predecessors zijn taken waarvan andere taken afhankelijk zijn voor voltooiing. Relaties van vorige versies zijn van invloed op de start- en voltooiingsdatums van de taken en hebben uiteindelijk invloed op de tijdlijn van het project.

Voor informatie over predecessors raadpleegt u [Overzicht van voorgangers van taken](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Door voorgangerrelaties tussen taken in te stellen, definieert u hoe het begin of einde van een afhankelijke taak afhankelijk is van het begin of einde van hun voorgangertaken. Dit wordt gedaan door verschillende Types van Afhankelijkheid te gebruiken.

Voor informatie over de Types van Afhankelijkheid, zie [Overzicht van typen taakafhankelijkheid](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Overzicht van gedwongen voorgangers

>[!IMPORTANT]
>
>U moet predecessors afdwingen om te vereisen dat de vorige verhoudingen worden gerespecteerd. Zonder de voorgangers af te dwingen, kunnen afhankelijke taken onafhankelijk van het begin en einde van hun voorgangers beginnen en eindigen, ongeacht het type afhankelijkheid.

U kunt de voorgaande relatie afdwingen wanneer u voorgangers voor een project instelt.

Als een voorganger wordt afgedwongen, kan de opvolgertaak niet worden gestart voordat de voorganger is voltooid. Bijvoorbeeld, het afdwingen van een eind-Begin verhouding tussen Taak A en Taak B betekent dat Taak B niet kan beginnen (de Status moet Nieuw blijven, en Percent moet 0%) blijven tot Taak A zoals voltooid duidelijk is. Het afdwingen van verhoudingen is op alle voorgangstypen van toepassing.

## Toegangsvereisten

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

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Een voorganger op taakniveau afdwingen

1. Ga naar de opvolgertaak waarvan voorganger u wilt afdwingen.
1. Klikken **Predecessors** in het linkerdeelvenster en klik vervolgens op **Voorganger toevoegen**. Mogelijk moet u op **Meer weergeven** vervolgens **Predecessors**.
1. (Voorwaardelijk) Als u een voorganger voor meerdere projecten wilt toevoegen, verwijdert u de naam van het project in het dialoogvenster **Bovenliggend project** veld en vervangen door een ander project.
1. Geef de naam op van de vorige taak of taken in het dialoogvenster **Taken** veld.
1. Geef de **Type afhankelijkheid** tussen deze twee taken.

   De standaardwaarde **Type afhankelijkheid** is **Voltooien**.

1. Selecteer de **Afgedwongen** om de voorganger af te dwingen.
1. Klikken **Opslaan**.

## Een voorganger afdwingen in een takenlijst

1. Ga naar een taaklijst in een project.
1. Van de **Weergave** vervolgkeuzelijst, selecteert u de **Standaardweergave**.

1. Neem nota van het aantal taak die u als voorganger zult aanwijzen.
1. Zoek de opvolgertaak waarvan u de voorganger wilt afdwingen.
1. In de **Predecessors** kolom, begin het aantal van de voorgangstaak in te gaan die door &quot;e&quot;wordt gevolgd. Typ bijvoorbeeld &quot;1e&quot; om taaknummer 1 als voorganger aan de geselecteerde taak toe te voegen.
1. Klik op Enter om uw voorganger-informatie voor de taak op te slaan.

   ![predecessor_required_in_list.png](assets/predecessor-enforced-in-list-350x308.png)
