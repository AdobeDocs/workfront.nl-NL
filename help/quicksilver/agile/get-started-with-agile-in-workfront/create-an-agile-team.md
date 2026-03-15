---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Een flexibel team maken
description: Adobe Workfront stelt Agile-teams in staat hun werk op een incrementele, georganiseerde manier te voltooien.
author: Courtney
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# Een flexibel team maken

<!--Audited: 01/2024-->

Met [!DNL Adobe Workfront] kunnen mobiele teams hun werk op een incrementele, georganiseerde manier voltooien.

Om het even welke gebruiker in de organisatie kan het team van Agile zien en alle componenten van Agile voor het team, met inbegrip van de achterstand, herhalingen, verhaalraad, en individuele verhalen bekijken. Alleen teamleden met [!UICONTROL Edit] toegang tot werk kunnen echter wijzigingen aanbrengen in het werk dat aan het team is toegewezen.

[!DNL Workfront] ondersteunt de volgende Google-methoden:

* **[!UICONTROL Scrum]**: Teams hebben een achterstand in hun werk. Wanneer het team klaar is om aan een specifiek stukje werk te werken, wordt het werk verplaatst van de achtergrond naar een herhaling. Voor meer gedetailleerde informatie over het leiden van een team van het Trommel, zie [ Scrum in een team van de Groot ](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]:** Teams verplaatsen werk in de Kanban-weergave over vooraf ingestelde statussen. Standaardstatus zijn: achterstand, in-process en gereed. Voor meer gedetailleerde informatie over het leiden van een team van Kanban, zie [ Kanban in een team van de Groot van de Agile ](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

## Toegangsvereisten

+++ Vouw uit om de toegangsvereisten voor de functionaliteit in dit artikel weer te geven.

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
   <p>Een nieuw Agile-team maken</p>
  <p>Werk of hoger om een team om te zetten in een Agile-team</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Beslissen over een Agile-methodologie

Je kunt een Scrum- of Kanban Agile-methodologie gebruiken voor je Agile-team. Elke methode levert verschillende voordelen op. De manier waarop je Agile-team werkt, bepaalt de Agile-methodologie die je kiest.

Met de methoden Scrum en Kanban Agile in [!DNL Workfront] kunt u artikelen over een artikelbord verplaatsen om een statuswijziging en de voortgang van het artikel aan te geven.

De methoden Scrum en Kanban Agile in [!DNL Workfront] verschillen op de volgende manieren:

### Voordelen van het gebruik van Kanban in [!DNL Workfront]

Met de [!DNL Kanban] Agile-methode in [!DNL Workfront] kunt u artikelen gemakkelijker over een artikel in een artikel verplaatsen en tegelijkertijd de hoeveelheid werk die wordt uitgevoerd, beperken. Er zijn geen begin- en einddatum wanneer u de [!DNL Kanban] gangbare methode gebruikt.

De volgende functionaliteit ondersteunt deze methode:

* Geef de achtergrond weer op het [!DNL Kanban] Agile story board.
Voor meer informatie, zie [ de backlog aan de [!UICONTROL Kanban] raad ](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md) toevoegen.

* Configureer items op de achtergrond die automatisch aan de [!UICONTROL Kanban] Agile story-board moeten worden toegevoegd wanneer andere items worden verplaatst naar een status die gelijk is aan Voltooien.
Voor meer informatie, zie sectie [ verhalen vormen die automatisch van de backlog ](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) in het artikel [ worden toegevoegd vormen Kanban ](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configureer een WIP-limiet (Work In Progress) die moet worden weergegeven op het [!UICONTROL Kanban] Agile story board.
Voor meer informatie, zie [ leiden het werk lopende (WIP) grens op het Kanbanboard ](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Voordelen van Scrum in [!DNL Workfront]

Met de Scrum Agile-methodologie in [!DNL Workfront] kunt u een set artikelen aan een Agile-iteratie toevoegen en een artikelbord voor die iteratie maken. De herhaling is gebaseerd op de begin- en einddatum die u opgeeft.

De volgende functionaliteit ondersteunt deze methode:

* Uitgaven opnemen op het [!UICONTROL Scrum] artikelbord
* Inclusief problemen op de achterstand van een Agile-team
* Subtaken kunnen worden weergegeven op het [!UICONTROL Scrum] artikelbord
* Bekijk een burndown grafiek om vooruitgang tegen verhalen tijdens de herhaling te zien
Voor meer informatie, zie [ Overzicht van de de burndown grafiek van de Gelijkheid ](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Een flexibel team maken

{{step1-to-team}}

1. Klik het **[!UICONTROL Switch Teams]** pictogram ![ het teampictogram van de Schakelaar ](assets/switch-team-icon.png), dan klik **[!UICONTROL Create new team]**.

   ![ Uitgezocht creeer nieuw team ](assets/create-new-team.png)

   Het vak Nieuw team wordt weergegeven.

1. Geef de volgende informatie op:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Name]</strong> </td> 
      <td>Typ een naam voor het nieuwe Agile-team.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL This is an Agile Team]</strong> </td> 
      <td>Selecteer deze optie als u dit nieuwe team wilt configureren voor een flexibel team.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>[!UICONTROL Is Active]</strong> </td> 
      <td>Selecteer deze optie om dit team te activeren. Inactieve teams zijn niet zichtbaar voor andere gebruikers om toe te wijzen aan het werk. </td> 
     </tr>


   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Group]</strong> </td> 
      <td> <p>Typ de naam van een groep die u aan het team wilt toevoegen en selecteer vervolgens de naam wanneer deze in de vervolgkeuzelijst staat.</p> <p><b>OPMERKING</b></p> <p> Wanneer een team aan een groep of een subgroep wordt toegewezen, kunnen om het even welke groepsbeheerders van die groep of subgroep het team leiden zonder een lid van het team te zijn. Groepsbeheerders kunnen vanuit [!UICONTROL Teams] naar het gebied [!UICONTROL Main Menu] gaan en op [!UICONTROL Switch Teams] pijl <img src="assets/switch-team-icon.png" alt="Pictogram voor wisselen van team"> klikken om alle teams weer te geven die zijn toegewezen aan de groepen die ze beheren.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Members]</strong> </td> 
      <td>Typ de naam van een gebruiker in het team en selecteer vervolgens de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.<br> herhaal dit proces om veelvoudige gebruikers aan het team toe te voegen.<br> omdat de gebruikers op meer dan één team kunnen zijn, kunnen zij op zowel de Gelijke als niet-Gelijke teams zijn.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Description]</strong> </td> 
      <td><p>Typ een beschrijving voor het team.</p> <p>De beschrijving wordt rechtsboven in het [!UICONTROL Teams] -gebied weergegeven wanneer het team wordt geselecteerd.</p>
      <p>Als de beschrijving lang is, kunt u erop klikken om de volledige beschrijving in een pop-up weer te geven. Als u toegang hebt om [!UICONTROL team settings] te bewerken, kunt u de beschrijving ook rechtstreeks in het pop-upvenster bewerken.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Klik op **[!UICONTROL Create]**.

   Raadpleeg de volgende artikelen voor informatie over het configureren van een Agile-team:

   * [Configureren [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configureren [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Een bestaand team converteren naar een Agile-team

U kunt een bestaand team converteren naar een Agile-team:

{{step1-to-team}}

1. Klik het **[!UICONTROL Switch team]** pictogram van het pictogram ![ team van de Schakelaar ](assets/switch-team-icon.png), dan of selecteer een nieuw team van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

1. Selecteer het team dat u naar een Agile-team wilt converteren.
1. Klik op het menu **[!UICONTROL More]** en selecteer vervolgens **[!UICONTROL Edit]** .

   Deze optie wordt alleen weergegeven voor teamleden met een [!UICONTROL Standard] -, [!UICONTROL Plan] - of [!UICONTROL Work] -licentie.
   ![ uitgezocht geef uit ](assets/edit-team-settings.png)

1. Selecteer **[!UICONTROL Agile]** in de sectie **[!UICONTROL This is an Agile Team]** .

1. Selecteer in de sectie **[!UICONTROL Methodology]** of het team een **[!UICONTROL Scrum]** - of **[!UICONTROL Kanban]** Agile-methodologie gebruikt.

1. Klik **sparen Veranderingen**.

   Het team wordt opgeslagen als een Agile-team. U kunt het nieuwe team als een Scrum of een Kanban-team configureren wanneer u het team bewerkt.

   Zie de volgende artikelen voor meer informatie:

   * [Configureren [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configureren [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
