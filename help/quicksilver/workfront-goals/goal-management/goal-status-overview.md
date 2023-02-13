---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Overzicht van de status van objecten in Adobe Workfront Goals
description: De status van het doel geeft aan of een doel actief is en momenteel vooruitgang registreert, of inactief is, is opgesteld, of reeds bereikt.
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---

# Overzicht van de status van objecten in Adobe Workfront Goals

<!--drafted for P&P new model: the note at the top will need to be replaced with this:    
    
Your organization must have the following to use the functionality described in this article:    
    
* For the legacy plan and license structure:     
    
  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans).     
  * An Adobe Workfront Goals license in addition to a Workfront license.    
    
* For the current plan and license structure:    
    
  * An Ultimate plan     
        
    Or    
        
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>    
    
Contact your Workfront account manager to learn about a Workfront Goals license.    
    
For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../workfront-goals/goal-management/access-needed-for-wf-goals.md).    
-->

>[!NOTE]
>
>Uw organisatie moet het volgende hebben om de functionaliteit te gebruiken die in dit artikel wordt beschreven:
>
>* Een Pro of hoger [Adobe Workfront-plan](https://www.workfront.com/plans).
>* Een Adobe Workfront Goals-licentie in aanvulling op een Workfront-licentie.
>
>Neem contact op met uw Workfront-accountmanager voor meer informatie over een Workfront Goals-licentie.

Voor meer informatie over toegang tot Workfront Goals raadpleegt u [Vereisten voor het gebruik van Workfront-doelen](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


De status van het doel geeft aan of een doel actief is en momenteel vooruitgang registreert, of inactief is, is opgesteld, of reeds bereikt.

## Overwegingen bij het bijwerken van doelstatussen in Workfront-doelen

* U kunt de status van doelen die u hebt gemaakt of die met u zijn gedeeld, niet handmatig bijwerken. De status van doelen wordt bijgewerkt, afhankelijk van de acties die u uitvoert om het doel te bereiken. Als u bijvoorbeeld een doel activeert, verandert de conceptstatus in Actief.
* Sommige beperkingen bestaan en soms kunt u niet de status van een doel in een andere status veranderen, volgens de volgende regels:

   | Van/naar | Concept | Actief | Inactief | Gesloten |
   |---|---|---|---|---|
   | Concept | - | Ja | Nee | Nee |
   | Actief | Nee | - | Ja | Ja |
   | Inactief | Nee | Ja | - | Nee |
   | Gesloten | Nee | Ja | Nee | - |

* Als u een gesloten doel opent, wordt ook de voortgang van het doel bijgewerkt.
* Bepaalde acties die u uitvoert op een doel werken ook zijn status bij. Raadpleeg de volgende artikelen voor informatie over het bijwerken van de status van doelen:

   * [Doelen maken voor Adobe Workfront-doelen](../../workfront-goals/goal-management/create-goals.md)
   * [Doelen in Adobe Workfront-doelen activeren](../../workfront-goals/goal-management/activate-goals.md)
   * [Doelen verwijderen en deactiveren in Adobe Workfront-doelen](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [Doelen sluiten en opnieuw openen in Adobe Workfront-doelen](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Overzicht van doelstatussen in Workfront-doelen

Ga voor informatie over het maken van Workfront Goals naar [Doelen maken voor Adobe Workfront-doelen](../../workfront-goals/goal-management/create-goals.md).

Voor informatie over het activeren van doelstellingen, zie [Doelen in Adobe Workfront-doelen activeren](../../workfront-goals/goal-management/activate-goals.md).

De doelstellingen kunnen één van de volgende statussen in de Doelen van Workfront hebben:

* [Concept](#draft)
* [Actief](#active)
* [Inactief](#inactive)
* [Gesloten](#closed)

### Concept {#draft}

* Dit is de standaardstatus voor een pas gecreëerd doel. Voor informatie over het creëren van doelstellingen, zie [Doelen maken voor Adobe Workfront-doelen](../../workfront-goals/goal-management/create-goals.md).
* De Workfront-doelstellingen boeken geen vooruitgang op een geformuleerd doel.
* U kunt de voortgang van een geformuleerd doel niet bijwerken.
* U kunt gestelde doelen niet sluiten of deactiveren, omdat ze geen voortgangsgegevens bevatten.
* Opgestelde doelen dragen niet bij tot de voortgangsberekening van andere doelen en worden in grafieken niet in aanmerking genomen.
* Tekendoelstellingen worden weergegeven op de volgende gebieden van Workfront Goals:

   * Lijst met doelen
   * Sectie voor uitlijning van doelen (alleen als een uitgelijnd doel)


>[!IMPORTANT]
>
>Nadat u de status van een doel hebt gewijzigd in een andere status, kan het doel nooit meer in een conceptstatus worden geplaatst.

### Actief {#active}

* U kunt een opgesteld doel slechts activeren wanneer u het met een resultaat associeert, een activiteit, of een ander doel aan het richten. Als u het doel activeert, verandert de status in Actief. Voor informatie over het activeren van doelstellingen, zie [Doelen in Adobe Workfront-doelen activeren](../../workfront-goals/goal-management/activate-goals.md).
* De Doelen van Workfront registreert vooruitgang op actieve doelstellingen.
* Actieve doelstellingen dragen bij tot de voortgangsberekening van andere doelstellingen en worden in grafieken in aanmerking genomen.
* Actieve doelstellingen worden weergegeven op de volgende gebieden van Workfront Goals:

   * Lijst met doelen
   * Sectie Goal Alignment
   * De voortgang van actieve doelen wordt weergegeven in grafieken

* U kunt een gesloten of inactief doel opnieuw activeren.

### Inactief {#inactive}

* U kunt een actief doel deactiveren wanneer de eigenaar er tijdelijk of permanent aan heeft gewerkt. U kunt het voor historische informatie bewaren. Hiermee wordt de status van het doel bijgewerkt naar Inactief.

   Voor informatie over het deactiveren van doelstellingen, zie de &quot;Deactivate doelstellingen&quot;sectie in het artikel [Doelen verwijderen en deactiveren in Adobe Workfront-doelen](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* U kunt een geschreven of gesloten doel niet deactiveren.
* U kunt een inactief doel opnieuw activeren en eraan blijven werken.
* Workfront-doelen berekenen geen vooruitgang bij inactieve doelen.
* U kunt de voortgang van een inactief doel niet bijwerken.
* Inactieve doelstellingen dragen niet bij aan de voortgangsberekening van andere doelstellingen en worden niet in grafieken in aanmerking genomen.
* Inactieve doelen hebben een geschiedenis van vooruitgang omdat ze ooit actief waren, in tegenstelling tot gestelde doelen.
* Inactieve doelen worden weergegeven op de volgende gebieden van Workfront Goals:

   * Lijst met doelen
   * Sectie voor uitlijning van doelen (alleen als uitgelijnde doelen)

### Gesloten {#closed}

* U kunt een doel sluiten als u wilt aangeven dat u het hebt bereikt of dat u er niet meer aan werkt, en dat u dat ook in de toekomst niet zult doen. Voor informatie over het sluiten van doelstellingen, zie [Doelen sluiten en opnieuw openen in Adobe Workfront-doelen](../../workfront-goals/goal-management/close-and-reopen-goals.md).

   >[!TIP]
   >
   >Als u van plan bent om later aan een doel te werken dat nog niet wordt bereikt, adviseren wij u de status in Inactief in plaats van Gesloten te veranderen.

* Je kunt geen doelen sluiten die nooit zijn geactiveerd, zoals geschreven doelen.
* U kunt een gesloten doel opnieuw openen en er verder aan blijven werken.
* Workfront Goals houdt op met het vastleggen van voortgang bij gesloten doelen.
* U kunt de voortgang van een gesloten doel niet bijwerken.
* De gesloten doelstellingen tonen op het volgende gebied van de Doelstellingen van Workfront:

   * Lijst met doelen
   * Sectie voor uitlijning van doelen (alleen als uitgelijnde doelen)
   * Informatie van gesloten doelstellingen wordt ook in de sectie van Grafieken in aanmerking genomen.
