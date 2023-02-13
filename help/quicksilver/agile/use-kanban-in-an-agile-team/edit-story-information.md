---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Artikelgegevens bewerken
description: Wanneer u een artikeltegel weergeeft op het Kanban-bord, kunt u bepaalde informatie inline bewerken, rechtstreeks vanuit de artikeltegel.
author: Lisa
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Artikelgegevens bewerken

## Begrijp welke informatie kan worden bekeken en worden uitgegeven {#understand-what-information-can-be-viewed-and-edited}

Wanneer u een artikeltegel weergeeft op de knop [!UICONTROL Kanban] de informatie in de volgende tabel beschikbaar is. U kunt de meeste informatie inline bewerken, rechtstreeks vanuit de artikeltegel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Informatie</strong> </th> 
   <th><strong>Zichtbaar</strong> </th> 
   <th><strong>Bewerkbaar inline</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>De artikelnaam met een koppeling die rechtstreeks naar de taak of uitgave verwijst</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>De projectnaam met een verbinding direct aan het project</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Het aantal punten of uren dat is voltooid in het artikel en het aantal punten of uren dat is toegewezen aan het artikel<br>Deze getallen worden gebruikt om het percentage Voltooid voor elk artikel te berekenen en weer te geven.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>De [!UICONTROL Percent Complete] voor elk artikel en elke uitgave.<br>[!UICONTROL The Percent Complete] voor de iteratie wordt berekend op basis van de [!UICONTROL Percent Complete] voor elk artikel.<br></p> <p>Bij bijwerken [!UICONTROL Percent Complete] voor een artikel of uitgave kunt u een willekeurig nummer tussen 0 en 100 kiezen.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Aan wie is het artikel toegewezen</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>De kleur of categorie van de tegel</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Eventuele extra velden (inclusief aangepaste velden) die mogelijk zijn toegevoegd aan de bestandsweergave door de bestandsweergave te wijzigen, zoals wordt beschreven in "Een flexibele weergave maken en aanpassen" in <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Overzicht van weergaven in [!DNL Adobe Workfront]</a></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>[!UICONTROL Work] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>[!UICONTROL Worker] of hoger</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau veranderen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Informatie over een artikeltegel weergeven en bewerken

1. Klik op de knop *[!UICONTROL *Main Menu]**, pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Teams]**.

1. (Optioneel) Klik op de knop **[!UICONTROL Switch team]** pictogram ![Teampictogram wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw Kanban-team in het keuzemenu of zoek naar een team op de zoekbalk.

1. Ga naar de [!UICONTROL Kanban] bord.
1. Vouw de artikeltegel uit om alle velden weer te geven die aan het artikel zijn gekoppeld.

   ![](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (Optioneel) Als u een veld wilt bewerken, klikt u op het veld en brengt u de gewenste wijzigingen aan.\
   U moet [!UICONTROL Edit] rechten op de taak of uitgave om de artikeltegel te bewerken.\
   Voor meer informatie over elk gebied en of het kan uitgeven, zie [Begrijp welke informatie kan worden bekeken en worden uitgegeven](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>Als u het dialoogvenster [!UICONTROL Percent Complete], moet u een getal tussen 0 en 100 invoeren. Het veld is geen schuifregelaar die u kunt verplaatsen.
