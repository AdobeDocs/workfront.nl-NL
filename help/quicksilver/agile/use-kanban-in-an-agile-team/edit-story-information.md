---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Artikelgegevens bewerken
description: Wanneer u een artikeltegel weergeeft op het Kanban-bord, kunt u bepaalde informatie inline bewerken, rechtstreeks vanuit de artikeltegel.
author: Jenny
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Artikelgegevens bewerken

## Begrijp welke informatie kan worden bekeken en worden uitgegeven {#understand-what-information-can-be-viewed-and-edited}

Wanneer u een artikeltegel weergeeft op het [!UICONTROL Kanban] -bord, is de informatie in de volgende tabel beschikbaar. U kunt de meeste informatie inline bewerken, rechtstreeks vanuit de artikeltegel.

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
   <td> <p>De projectnaam met een verbinding direct aan het project</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Het aantal punten of uren volledig op het verhaal en het aantal punten of uren die aan het verhaal <br> worden toegewezen Deze aantallen worden gebruikt om Percentage te berekenen en te tonen voltooit voor elk verhaal.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>De [!UICONTROL Percent Complete] voor elk artikel en elke uitgave.<br>[!UICONTROL The Percent Complete] voor de herhaling wordt berekend op basis van [!UICONTROL Percent Complete] voor elk artikel.<br></p> <p>Wanneer u [!UICONTROL Percent Complete] bijwerkt voor een artikel of uitgave, kunt u een willekeurig getal tussen 0 en 100 kiezen.</p> </td> 
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
   <td> <p>Om het even welke extra gebieden (met inbegrip van douanevelden) die aan de Gelijke mening door de Gelijke mening te wijzigen zouden kunnen zijn toegevoegd, zoals die in "het Creëren van en het Aanpassen van een Gelijke Mening"in <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref"> Overzicht van Mening in [!DNL Adobe Workfront]</a> wordt beschreven</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p> 
   <p>Werk of hoger</p> </td> 
  </tr>
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informatie over een artikeltegel weergeven en bewerken

{{step1-to-team}}

1. (Facultatief) klik het **[!UICONTROL Switch team]** pictogram van de pictogram ![ Schakelaar teampictogram ](assets/switch-team-icon.png), dan of selecteer een nieuw team Kanban van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

1. Ga naar het [!UICONTROL Kanban] board.
1. Vouw de artikeltegel uit om alle velden weer te geven die aan het artikel zijn gekoppeld.

   ![ kaart van het Verhaal ](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (Optioneel) Als u een veld wilt bewerken, klikt u op het veld en brengt u de gewenste wijzigingen aan.
U moet [!UICONTROL Edit] rechten op de taak of uitgave hebben om de artikeltegel te kunnen bewerken.
Voor meer informatie over elk gebied en of het kan worden uitgegeven, zie [ begrijpen welke informatie kan worden bekeken en worden uitgegeven ](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>Als u [!UICONTROL Percent Complete] wilt wijzigen, moet u een getal tussen 0 en 100 invoeren. Het veld is geen schuifregelaar die u kunt verplaatsen.
