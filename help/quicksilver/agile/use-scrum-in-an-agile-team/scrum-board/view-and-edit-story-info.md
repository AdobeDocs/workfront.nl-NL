---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Artikelgegevens weergeven en bewerken op het scrollbord
description: Wanneer u een artikeltegel weergeeft op het Kanban-bord, kunt u bepaalde informatie inline bewerken, rechtstreeks vanuit de artikeltegel.
author: Lisa
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# Artikelgegevens weergeven en bewerken in het dialoogvenster [!UICONTROL Scrum] board

## Begrijp welke informatie kan worden bekeken en worden uitgegeven

Wanneer u een artikeltegel weergeeft op het artikelbord, is de informatie in de volgende tabel beschikbaar. U kunt de meeste informatie inline bewerken, rechtstreeks vanuit de artikeltegel.

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
   <td> <p>De projectnaam met een verbinding direct aan het project<br>Deze koppeling wordt alleen weergegeven in artikelen (bovenliggende taken, niet in subtaken) wanneer de schakelweergave voor een herhaling wordt gebruikt. deze wordt niet weergegeven wanneer een flexibele weergave wordt gebruikt voor een project.</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Het aantal punten of uren dat is voltooid in het artikel en het aantal punten of uren dat is toegewezen aan het artikel<br>Deze getallen worden gebruikt om de [!UICONTROL Percent Complete] voor elk artikel.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>De [!UICONTROL Percent Complete] voor elk artikel en elke uitgave.<br>De [!UICONTROL Percent Complete] voor de iteratie wordt berekend op basis van de [!UICONTROL Percent Complete] voor elk artikel.</p> <p>Bij bijwerken [!UICONTROL Percent Complete] voor een artikel of uitgave kunt u een willekeurig nummer tussen 0 en 100 kiezen.</p> </td> 
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
   <td> <p>Eventuele extra velden (inclusief aangepaste velden) die mogelijk zijn toegevoegd aan de bestandsweergave door de bestandsweergave te wijzigen, zoals wordt beschreven in "Een bestand maken en aanpassen [!UICONTROL Agile] Weergeven" in <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Overzicht van weergaven in [!UICONTROL Adobe Workfront]</a>.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

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
   <td> <p>[!UICONTROL Work] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>[!UICONTROL Worker] of hoger</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Toegang tot de taak of uitgave bewerken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Informatie over een artikeltegel weergeven en bewerken

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Teams]**.

1. (Optioneel) Klik op de knop **[!UICONTROL Switch team]** pictogram ![Teampictogram wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw scrubteam in het keuzemenu of zoek naar een team op de zoekbalk.

1. Selecteer in het linkerdeelvenster de optie **[!UICONTROL Iterations]** om een specifieke herhaling te kiezen, of **[!UICONTROL Current Iteration]**.

1. Ga naar de [!UICONTROL Scrum] &#39;agile story board&#39;.
1. Breid uit [!UICONTROL story] tegel om alle velden weer te geven die aan het artikel zijn gekoppeld.

   ![](assets/agile-storycard-scrum-2021-350x333.png)

1. (Optioneel) Als u een veld wilt bewerken, klikt u op het veld en brengt u de gewenste wijzigingen aan.

   U moet [!UICONTROL Edit] rechten op de taak of uitgave om de artikeltegel te bewerken.

>[!NOTE]
>
>Als u het dialoogvenster [!UICONTROL Percent Complete], moet u een getal tussen 0 en 100 invoeren. Het veld is geen schuifregelaar die u kunt verplaatsen.
