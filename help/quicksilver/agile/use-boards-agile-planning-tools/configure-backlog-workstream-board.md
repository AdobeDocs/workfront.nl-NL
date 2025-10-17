---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: De back-up op een werkstroomkaart configureren
description: U kunt verkiezen om een backlogkolom op een raad in een werkstroom te tonen, en een vraag voor de kaarten te bepalen die in de bordbacklog van de werkstroomkaartlijst worden getrokken.
author: Jenny
feature: Agile
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# De achterstand op een werkstroomgebied configureren

>[!IMPORTANT]
>
>Workstreams zijn alleen beschikbaar voor een specifieke groep klanten.

U kunt verkiezen om een backlogkolom op een raad in een werkstroom te tonen, en een vraag voor de kaarten te bepalen die in de bordbacklog van de werkstroomkaartlijst worden getrokken.

>[!NOTE]
>
>Als u een nieuwe kaart in de backlogkolom toevoegt die niet de vraagcriteria aanpast, zal de kaart van backlog verdwijnen wanneer de raad wordt verfrist en het zal slechts in de kaartlijst beschikbaar zijn. U kunt de vraag op elk ogenblik veranderen om aan te passen welke kaarten in de backlogkolom verschijnen.

De backlogkolom en de vraag zijn niet beschikbaar op standalone borden. Voor informatie over het toevoegen van een inlaatkolom aan een standalone raad, zie [ een inlaatkolom aan een raad ](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md) toevoegen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Medewerker of hoger</p> 
   <p>Aanvraag of hoger</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## De achterstand op een werkstroomgebied configureren

{{step1-to-boards}}

1. Open de werkstroom waarin u wilt werken. Om een werkstroom te openen, klik [!UICONTROL **de werkstroom van de Mening**].
1. Klik op een willekeurige kaart in de werkstream om deze te openen.
1. Klik [!UICONTROL **vormen**] op het recht van de raad om het Configure paneel te openen.
1. Zet [!UICONTROL **op omvat een backlogkolom op deze raad**].

   De achtergrondkolom wordt links van de board toegevoegd. Het blijft leeg totdat u een query op het bestand toepast.

1. Vouw [!UICONTROL **Vraag Backlog**] uit.

   >[!NOTE]
   >
   >Er kan al een standaardquery op de achtergrond worden toegepast, waarbij alle werkitems uit de kaartlijst worden weergegeven die een status hebben en de status niet Voltooid is.

1. Klik [!UICONTROL **toevoegen voorwaarde**] en klik op het &quot;lege&quot;gebied.
1. Selecteer het veld waarop u een query wilt uitvoeren.

   De velden waaruit u kunt kiezen, zijn de standaardvelden op een kaart.

1. Selecteer de queryoptie.

   De opties voor wijzigingstoetsen zijn afhankelijk van de velden waarop ze kunnen worden toegepast. Het veld &quot;name&quot; heeft bijvoorbeeld niet de optie &quot;groter dan&quot; of &quot;kleiner dan&quot; als optie, omdat deze modifiers alleen op getallen van toepassing zijn.

1. Selecteer de waarde.

   De waarde is niet beschikbaar als u &quot;bestaat&quot;of &quot;niet bestaat&quot;als bepaling gebruikt.

   Als u bijvoorbeeld &quot;Vervaldatum&quot; en &quot;bestaan&quot; kiest, worden in de backlog kaarten weergegeven met toegewezen vervaldatums. Een kaart zonder vervaldatum wordt niet op de achterstand gezet.

1. (Facultatief) klik [!UICONTROL **toevoegen voorwaarde**] om een andere voorwaarde aan de vraag toe te voegen.

   ![ Backlog vraag ](assets/backlog-query-wrkstrm-board.png)

1. (Facultatief) klik [!UICONTROL **maken groep**] om een groep voorwaarden toe te voegen die met de eerste voorwaarde met OF exploitant worden verbonden.
1. Klik [!UICONTROL **sparen vraag**].

   De vraag wordt toegepast en de kaarten die aan de criteria voldoen verschijnen in de backlogkolom.
