---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: De achterstand op een werkstroomgebied configureren
description: U kunt verkiezen om een backlogkolom op een raad in een werkstroom te tonen, en een vraag voor de kaarten te bepalen die in de bordbacklog van de werkstroomkaartlijst worden getrokken.
author: Lisa
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: 75bb5af9564947a39e1cb46f9d6be2c03eb07acc
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# De achterstand op een werkstroomgebied configureren

U kunt verkiezen om een backlogkolom op een raad in een werkstroom te tonen, en een vraag voor de kaarten te bepalen die in de bordbacklog van de werkstroomkaartlijst worden getrokken. Deze opties zijn niet beschikbaar op zelfstandige borden. Voor informatie over het toevoegen van een inlaatkolom aan een standalone board, zie [Een inlaatkolom aan een bord toevoegen](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>[!UICONTROL Request] of hoger</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## De achterstand op een werkstroomgebied configureren

{{step1-to-boards}}

1. Open de werkstroom waarin u wilt werken. Als u een werkstroom wilt openen, klikt u op [!UICONTROL **Werkstroom weergeven**].
1. Klik op een willekeurige kaart in de werkstream om deze te openen.
1. Klikken [!UICONTROL **Configureren**] rechts van de board om het Configure paneel te openen.
1. Inschakelen [!UICONTROL **Een achtergrondkolom opnemen in deze kaart**].

   De achtergrondkolom wordt links van de board toegevoegd. Het blijft leeg totdat u een query op het bestand toepast.

1. Uitbreiden [!UICONTROL **Backlogquery**].

   >[!NOTE]
   >
   >Een standaardvraag kan reeds op de achterstand worden toegepast, die alle het werkpunten van de kaartlijst toont die niet tot een herhaling behoren en niet in Volledige status zijn.

1. Klikken [!UICONTROL **Voorwaarde toevoegen**] en klik in het veld &quot;leeg&quot;.
1. Selecteer het veld waarop u een query wilt uitvoeren.

   De velden waaruit u kunt kiezen, zijn de standaardvelden op een kaart.

1. Selecteer de queryoptie.

   De opties voor wijzigingstoetsen zijn afhankelijk van de velden waarop ze kunnen worden toegepast. Het veld &quot;name&quot; heeft bijvoorbeeld niet de optie &quot;groter dan&quot; of &quot;kleiner dan&quot; als optie, omdat deze modifiers alleen op getallen van toepassing zijn.

1. Selecteer de waarde.

   De waarde is niet beschikbaar als u &quot;bestaat&quot;of &quot;niet bestaat&quot;als bepaling gebruikt.

   Als u bijvoorbeeld &quot;Vervaldatum&quot; en &quot;bestaat&quot; kiest, worden in de backlog kaarten weergegeven met toegewezen vervaldatums. Een kaart zonder vervaldatum wordt niet op de achterstand gezet.

1. (Optioneel) Klik op [!UICONTROL **Voorwaarde toevoegen**] om een andere voorwaarde aan de vraag toe te voegen.

   ![Backlogquery](assets/backlog-query-wrkstrm-board.png)

1. (Optioneel) Klik op [!UICONTROL **Groep maken**] om een groep voorwaarden toe te voegen die met de eerste voorwaarde met een exploitant OR wordt verbonden.
1. Klikken [!UICONTROL **Query opslaan**].

   De vraag wordt toegepast en de kaarten die aan de criteria voldoen verschijnen in de backlogkolom.
