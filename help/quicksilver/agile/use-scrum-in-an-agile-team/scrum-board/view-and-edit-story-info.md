---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Artikelinformatie weergeven en bewerken op het plakbord
description: Wanneer u een artikeltegel weergeeft op het Kanban-bord, kunt u bepaalde informatie inline bewerken, rechtstreeks vanuit de artikeltegel.
author: Jenny
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Artikelinformatie op de [!UICONTROL Scrum] -board weergeven en bewerken

## Begrijp welke informatie kan worden bekeken en worden uitgegeven

Wanneer u een artikeltegel weergeeft op het artikelbord, is de informatie in de volgende tabel beschikbaar. U kunt de meeste informatie inline bewerken, rechtstreeks vanuit de artikeltegel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong> Informatie </strong> </th> 
   <th><strong> Zichtbaar </strong> </th> 
   <th><strong> Bewerkbaar Inline </strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>De artikelnaam met een koppeling die rechtstreeks naar de taak of uitgave verwijst</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>De projectnaam met een verbinding direct aan het project <br> Deze verbinding wordt getoond slechts op verhalen (oudertaken, niet subtasks) wanneer het gebruiken van de mening van de Gelijkheid op een herhaling; het wordt niet getoond wanneer het gebruiken van een Gelijke mening op een project.</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Het aantal punten of uren volledig op het verhaal en het aantal punten of uren die aan het verhaal <br> worden toegewezen Deze aantallen worden gebruikt om [!UICONTROL Percent Complete] voor elk verhaal te berekenen en te tonen.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>De [!UICONTROL Percent Complete] voor elk artikel en elke uitgave.<br> [!UICONTROL Percent Complete] voor de herhaling wordt berekend gebaseerd op [!UICONTROL Percent Complete] voor elk verhaal.</p> <p>Wanneer u [!UICONTROL Percent Complete] bijwerkt voor een artikel of uitgave, kunt u een willekeurig getal tussen 0 en 100 kiezen.</p> </td> 
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
   <td> <p>Om het even welke extra gebieden (met inbegrip van douanevelden) die aan de Gelijke mening door de Gelijke mening te wijzigen zouden kunnen zijn toegevoegd, zoals die in "het Creëren van en het Aanpassen van een [!UICONTROL Agile] Mening"in <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref"> overzicht van Meningen in [!UICONTROL Adobe Workfront]</a> wordt beschreven.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> <p>Nieuw: [!UICONTROL Standard]</p> 
   of
   <p>Huidig: [!UICONTROL Work] of hoger</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>[!UICONTROL Contribute] of [!UICONTROL Manage] toegang tot de taak of uitgave</td> 
  </tr>
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informatie over een artikeltegel weergeven en bewerken

{{step1-to-team}}

1. (Facultatief) klik het **[!UICONTROL Switch team]** pictogram van de pictogram ![&#x200B; Schakelaar teampictogram &#x200B;](assets/switch-team-icon.png), dan of selecteer een nieuw team van het Trommel van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

1. Selecteer in het linkerdeelvenster **[!UICONTROL Iterations]** om een specifieke herhaling te kiezen of selecteer **[!UICONTROL Current Iteration]** .

1. Ga naar het [!UICONTROL Scrum] artikel.
1. Vouw het element [!UICONTROL story] uit om alle velden weer te geven die aan het artikel zijn gekoppeld.

   ![&#x200B; verhaalkaart &#x200B;](assets/agile-storycard-scrum-2021-350x333.png)

1. (Optioneel) Als u een veld wilt bewerken, klikt u op het veld en brengt u de gewenste wijzigingen aan.

   U moet [!UICONTROL Edit] rechten op de taak of uitgave hebben om de artikeltegel te bewerken.

>[!NOTE]
>
>Als u [!UICONTROL Percent Complete] wilt wijzigen, moet u een getal tussen 0 en 100 invoeren. Het veld is geen schuifregelaar die u kunt verplaatsen.
