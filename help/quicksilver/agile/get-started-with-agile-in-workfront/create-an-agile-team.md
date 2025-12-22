---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Een flexibel team maken
description: Adobe Workfront stelt Agile-teams in staat hun werk op een incrementele, georganiseerde manier te voltooien.
author: Jenny
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# Een flexibel team maken

<!--Audited: 01/2024-->

Met [!DNL Adobe Workfront] kunnen mobiele teams hun werk op een incrementele, georganiseerde manier voltooien.

Om het even welke gebruiker in de organisatie kan het team van Agile zien en alle componenten van Agile voor het team, met inbegrip van de achterstand, herhalingen, verhaalraad, en individuele verhalen bekijken. Alleen teamleden met [!UICONTROL Edit] toegang tot het werk kunnen echter wijzigingen aanbrengen in het werk dat aan het team is toegewezen.

[!DNL Workfront] biedt ondersteuning voor de volgende Google-methoden:

* **[!UICONTROL Scrum]**: Teams hebben een achterstand in hun werk die moet worden uitgevoerd. Wanneer het team aan een specifiek segment van het werk klaar is te werken, wordt het werk verplaatst van de achterstand naar een herhaling. Voor meer gedetailleerde informatie over het beheren van een team van het Trommel, zie [ Trommel in een team van de Groep van de Stijl ](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]:** de teams bewegen het werk in de mening Kanban over vooraf bepaalde statussen. De standaardstatussen zijn: achterstand, in-proces, en gedaan. Voor meer gedetailleerde informatie over het beheren van een team Kanban, zie [ Kanban in een team van de Gelijkheid ](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

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
   <p>Een nieuw Agile-team maken</p>
  <p>Werk of hoger om een team om te zetten in een Agile-team</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Beslissen over een Agile-methode

U kunt een methode voor Scrum of Kanban Agile gebruiken voor uw Agile-team. Elke methode biedt verschillende voordelen. De manier waarop uw Agile-team werkt, bepaalt de Agile-methode die u kiest.

Met de methoden Scrum en Kanban Agile in [!DNL Workfront] kunt u artikelen over een artikelbord verplaatsen om een statuswijziging en de voortgang van het artikel aan te geven.

De methoden Scrum en Kanban Agile in [!DNL Workfront] verschillen op de volgende manieren:

### Voordelen van het gebruik van Kanban in [!DNL Workfront]

Met de [!DNL Kanban] Agile-methode in [!DNL Workfront] kunt u artikelen gemakkelijker over een artikel in een artikel verplaatsen en tegelijkertijd de hoeveelheid werk die wordt uitgevoerd, beperken. Er zijn geen begin- en einddatum wanneer u de [!DNL Kanban] gangbare methode gebruikt.

Deze methode wordt ondersteund door de volgende functionaliteit:

* Geef de achterstand weer op de [!DNL Kanban] Agile story board.
Voor meer informatie, zie [ de achterstand aan de [!UICONTROL Kanban] raad ](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md) toevoegen.

* Configureer de items op de achtergrond die automatisch aan de [!UICONTROL Kanban] artikel-board voor een mobiel artikel moeten worden toegevoegd wanneer andere items naar een status worden verplaatst die gelijk is aan Voltooid.
Voor meer informatie, zie de sectie [ verhalen vormen die automatisch van de achterstand ](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) in het artikel [ worden toegevoegd Kanban ](../../agile/get-started-with-agile-in-workfront/configure-kanban.md) vormen.

* Configureer een WIP-limiet (Work In Progress) die moet worden weergegeven op de [!UICONTROL Kanban] Agile story board.
Voor meer informatie, zie [ leiden het werk lopend (WIP) grens op de raad Kanban ](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Voordelen van het gebruik van Scrum in [!DNL Workfront]

Met de methode Scrum Agile in [!DNL Workfront] kunt u een set artikelen toevoegen aan een Agile-herhaling en een artikelbord voor die herhaling maken. De herhaling is gebaseerd op de begin- en einddatum die u definieert.

Deze methode wordt ondersteund door de volgende functionaliteit:

* Inclusief problemen op de whiteboard van [!UICONTROL Scrum]
* Inclusief problemen op de achterstand van een Agile-team
* Subtaken kunnen worden weergegeven op het [!UICONTROL Scrum] artikelbord
* Een uitvouwdiagram weergeven om de voortgang tegen artikelen tijdens de herhaling te bekijken
Voor meer informatie, zie [ Overzicht van de de burndown grafiek van de Gelijkheid ](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Een flexibel team maken

{{step1-to-team}}

1. Klik het **[!UICONTROL Switch Teams]** pictogram van het pictogram ![ team van de Schakelaar ](assets/switch-team-icon.png), dan klik **[!UICONTROL Create new team]**.

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
      <td> <p>Typ de naam van een groep die u aan het team wilt toevoegen en selecteer vervolgens de naam wanneer deze in de vervolgkeuzelijst wordt weergegeven.</p> <p><b>OPMERKING</b></p> <p> Wanneer een team aan een groep of subgroep wordt toegewezen, kunnen om het even welke groepsbeheerders van die groep of subgroep het team beheren zonder een lid van het team te zijn. Groepbeheerders kunnen vanuit [!UICONTROL Teams] naar het gebied [!UICONTROL Main Menu] gaan en op [!UICONTROL Switch Teams] pijl <img src="assets/switch-team-icon.png" alt="Teampictogram wisselen"> klikken om alle teams weer te geven die zijn toegewezen aan de groepen die ze beheren.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Members]</strong> </td> 
      <td>Typ de naam van een gebruiker die zich in het team moet bevinden en selecteer vervolgens de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.<br> herhaal dit proces om veelvoudige gebruikers aan het team toe te voegen.<br> omdat de gebruikers op meer dan één team kunnen zijn, kunnen zij op zowel de Gelijke als niet-Gelijke teams zijn.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Description]</strong> </td> 
      <td><p>Typ een beschrijving voor het team.</p> <p>De beschrijving wordt rechtsboven in het [!UICONTROL Teams] -gebied weergegeven wanneer het team is geselecteerd.</p>
      <p>Als de beschrijving lang is, kunt u erop klikken om de volledige beschrijving in een pop-up te tonen. Als u toegang hebt om de [!UICONTROL team settings] te bewerken, kunt u de beschrijving ook rechtstreeks in het pop-upvenster bewerken.</p></td>
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

1. Selecteer het team dat u wilt omzetten in een team van Agile.
1. Klik op het menu **[!UICONTROL More]** en selecteer vervolgens **[!UICONTROL Edit]** .

   Deze optie wordt alleen weergegeven voor teamleden met een licentie [!UICONTROL Standard] , [!UICONTROL Plan] of [!UICONTROL Work] .
   ![ Uitgezochte geeft uit ](assets/edit-team-settings.png)

1. Selecteer **[!UICONTROL Agile]** in de sectie **[!UICONTROL This is an Agile Team]** .

1. Selecteer in de sectie **[!UICONTROL Methodology]** of het team een **[!UICONTROL Scrum]** - of **[!UICONTROL Kanban]** Agile-methode gebruikt.

1. Klik **sparen Veranderingen**.

   Het team wordt opgeslagen als een Agile-team. U kunt het nieuwe team als Trommel of een team vormen Kanban wanneer u het team uitgeeft.

   Raadpleeg de volgende artikelen voor meer informatie:

   * [Configureren [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configureren [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
