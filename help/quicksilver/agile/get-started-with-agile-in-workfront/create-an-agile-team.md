---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Een bestandsteam maken
description: Met Adobe Workfront kunnen mobiele teams hun werk op een incrementele, georganiseerde manier voltooien.
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '892'
ht-degree: 0%

---

# Een bestandsteam maken

[!DNL Adobe Workfront] stelt flexibele teams in staat hun werk op een incrementele, georganiseerde manier te voltooien.

Om het even welke gebruiker in de organisatie kan het agile team zien en alle agile componenten voor het team, met inbegrip van de achterstand, herhalingen, verhaalraad, en individuele verhalen bekijken. Alleen leden van het team met [!UICONTROL Edit] de toegang tot het werk kan veranderingen aanbrengen aan het werk dat aan het team wordt toegewezen.

[!DNL Workfront] ondersteunt de volgende werkmethoden:

* **[!UICONTROL Scrum]**: Teams hebben een achterstand op het werk die moet worden gedaan. Wanneer het team aan een specifiek segment van het werk klaar is te werken, wordt het werk verplaatst van de achterstand naar een herhaling. Voor meer gedetailleerde informatie over het beheren van een team van de Trommel, zie [Scrum in een mobiel team](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]:** Teams verplaatsen het werk in de Kanban-weergave naar een vooraf bepaalde status. De standaardstatussen zijn: achterstand, in-proces, en gedaan. Voor meer gedetailleerde informatie over het beheren van een Kanban-team raadpleegt u [Kanban in een team](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

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
   <td> <p>[!UICONTROL Plan] een nieuw elegante team op te richten ; [!UICONTROL Work] of hoger om een team om te zetten in een flexibel team</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Beslissen over een flexibele methode

U kunt voor uw mobiele team een methode gebruiken voor Scrum of Kanban. Elke methode biedt verschillende voordelen. De manier waarop uw mobiele team werkt, bepaalt de flexibele methode die u kiest.

Zowel Scrum als Kanban agile methodologieën in [!DNL Workfront] Hiermee kunt u artikelen over een artikelbord verplaatsen om een statuswijziging en de voortgang van het artikel aan te geven.

Scrum en Kanban agile, methodologieën op het gebied van [!DNL Workfront] verschillen op de volgende manieren:

### Voordelen van Kanban in [!DNL Workfront]

De [!DNL Kanban] flexibele methodologie in [!DNL Workfront] kunt u artikelen gemakkelijker over een &#39;agile story&#39;-bord verplaatsen en de hoeveelheid werk die wordt uitgevoerd, beperken. Er zijn geen begin- en einddatums wanneer u de opdracht [!DNL Kanban] flexibele methodologie.

Deze methode wordt ondersteund door de volgende functionaliteit:

* De achterstand weergeven op het tabblad [!DNL Kanban] agile verhaalbord.\
   Zie voor meer informatie [De achterstand toevoegen aan de [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Configureer items op de achtergrond die automatisch moeten worden toegevoegd aan de [!UICONTROL Kanban] Een artikel opnieuw labelen wanneer andere items worden verplaatst naar een status die gelijk is aan Voltooien.\
   Zie de sectie voor meer informatie [Artikelen configureren die automatisch worden toegevoegd vanaf de achtergrond](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) in het artikel [Kanban configureren](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configureer een WIP-limiet (Work In Progress) die moet worden weergegeven op het tabblad [!UICONTROL Kanban] agile verhaalbord.\
   Zie voor meer informatie [De WIP-limiet (work in progress) op de Kanban-board beheren](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Voordelen van het gebruik van Scrum in [!DNL Workfront]

De methode voor de rol van de trommel [!DNL Workfront] kunt u een set artikelen toevoegen aan een flexibele herhaling en een artikelbord voor die herhaling maken. De herhaling is gebaseerd op de begin- en einddatum die u definieert.

Deze methode wordt ondersteund door de volgende functionaliteit:

* Inclusief problemen op het tabblad [!UICONTROL Scrum] artikelenlijst
* Inclusief problemen op de achtergrond van een bestandsteam
* Subtaken kunnen worden weergegeven op de [!UICONTROL Scrum] artikelenlijst
* Een uitvouwdiagram weergeven om de voortgang tegen artikelen tijdens de herhaling te bekijken\
   Zie voor meer informatie [Overzicht van gile burndown-diagram](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Een bestandsteam maken

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Teams]**.
1. Klik op de knop **[!UICONTROL Switch Teams]** pictogram ![Teampictogram wisselen](assets/switch-team-icon.png)en klik vervolgens op **[!UICONTROL Create New Team]**.

   ![Selecteer Nieuw team maken.](assets/create-new-team-350x198.png)

1. Geef de volgende informatie op over de [!UICONTROL New Team] dialoogvenster:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Name]</strong> </td> 
      <td>Typ een naam voor het nieuwe bestandsteam.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL This is an Agile Team]</strong> </td> 
      <td>Selecteer deze optie om dit nieuwe team te vormen om een flexibel team te worden.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Group]</strong> </td> 
      <td> <p>Typ de naam van een groep die u aan het team wilt toevoegen en selecteer vervolgens de naam wanneer deze in de vervolgkeuzelijst wordt weergegeven.</p> <p>Nota: Wanneer een team aan een groep of een subgroep wordt toegewezen, kunnen om het even welke groepsbeheerders van die groep of subgroep het team beheren zonder een lid van het te zijn. Groepbeheerders kunnen naar [!UICONTROL Teams] gebied van de [!UICONTROL Main Menu] en klik op de knop [!UICONTROL Switch Teams] pijl <img src="assets/switch-team-icon.png" alt="Teampictogram wisselen"> om van alle teams een lijst te maken die aan de groepen worden toegewezen die zij leiden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Members]</strong> </td> 
      <td>Typ de naam van een gebruiker die zich in het team moet bevinden en selecteer vervolgens de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.<br>Herhaal dit proces om meerdere gebruikers aan het team toe te voegen.<br>Omdat de gebruikers op meer dan één team kunnen zijn, kunnen zij op zowel flexibele als niet-flexibele teams zijn.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Description]</strong> </td> 
      <td><p>Typ een beschrijving voor het team.</p> <p>De beschrijving wordt rechtsboven in het dialoogvenster [!UICONTROL Teams] gebied wanneer het team wordt geselecteerd.</p>
      <p>Als de beschrijving lang is, kunt u erop klikken om de volledige beschrijving in een pop-up te tonen. Als u toegang hebt om de [!UICONTROL team settings]kunt u de beschrijving ook rechtstreeks in het pop-upvenster bewerken.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Klik op **[!UICONTROL Create]**.

   Raadpleeg de volgende artikelen voor informatie over het configureren van een Agile-team:

   * [Configureren [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configureren [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Een bestaand team converteren naar een flexibel team

U kunt een bestaand team omzetten in een flexibel team:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Teams]**.
1. Klik op de knop **[!UICONTROL Switch team]** pictogram ![Teampictogram wisselen](assets/switch-team-icon.png)Selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team op de zoekbalk.

1. Selecteer het team dat u in een flexibel team wilt omzetten.
1. Klik op de knop **[!UICONTROL More]** menu, selecteert u vervolgens **[!UICONTROL Edit]**.\
   Alleen teamleden met een van beide [!UICONTROL Plan] of [!UICONTROL Work] Deze optie ziet u voor een licentie.\
   ![](assets/edit-team-settings-350x205.png)

1. In de **[!UICONTROL Agile]** sectie, selecteert u **[!UICONTROL This is an Agile Team]**.

1. In de **[!UICONTROL Methodology]** selecteert u of het team een **[!UICONTROL Scrum]** of **[!UICONTROL Kanban]** flexibele methodologie.

1. Klikken **Wijzigingen opslaan.**

   Raadpleeg de volgende artikelen voor informatie over het configureren van een Agile-team:

   * [Configureren [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configureren [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
