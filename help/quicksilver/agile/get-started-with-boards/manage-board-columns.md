---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Bordkolommen beheren
description: Een nieuwe board bevat standaard drie kolommen. U kunt meer kolommen toevoegen, de orde van de kolommen veranderen, kolommen anders noemen, en om het even welke kolommen schrappen die u niet nodig hebt. U kunt ook kolombeleid definiëren.
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 040dd446ff2b347dabf8a139feb17fd1a7d50e4e
workflow-type: tm+mt
source-wordcount: '1092'
ht-degree: 0%

---

# Bordkolommen beheren

<!-- Audited: 05/2024 -->

Een nieuwe board bevat standaard drie kolommen. U kunt meer kolommen toevoegen, de orde van de kolommen veranderen, kolommen anders noemen, en om het even welke kolommen schrappen die u niet nodig hebt.

De montages van de kolom omvatten beleid, dat u toestaat om opties te bepalen voor wat met een kaart gebeurt wanneer het in die kolom wordt bewogen.

Voor informatie over het sorteren van de kaarten in kolommen, zie [Filteren en zoeken in een board](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> <p>Nieuw: Medewerker of hoger </p>
        <p>of</p> 
        <p>Huidige: [!UICONTROL Request] of hoger </p></td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Een kolom aan een board toevoegen

{{step1-to-boards}}

1. Toegang tot een bord. Zie voor meer informatie [Een board maken of bewerken](../../agile/get-started-with-boards/create-edit-board.md).
1. Klikken **[!UICONTROL Add Column]** rechts van de bestaande kolommen.
1. Typ een naam in de nieuwe kolom en klik op **[!UICONTROL Add Column]**.

   ![Nieuwe kolom toevoegen](assets/boards-add-column.png)

>[!TIP]
>
>Als u een inlaatkolom wilt toevoegen, raadpleegt u [Een inlaatkolom aan een bord toevoegen](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Kolommen opnieuw ordenen aan boord

1. Toegang tot het bord.
1. Sleep de kolommen in de juiste volgorde. Selecteer de bovenkant van de kolom voordat u deze naar een andere locatie sleept.

   ![Kolom slepen en neerzetten](assets/boards-dragdropcolumn.png)

## De naam van een boardkolom wijzigen

1. Toegang tot het bord.
1. Klik op de kolomnaam, typ de nieuwe naam en druk op Enter.

   of

   Klik op de knop **[!UICONTROL More]** menu ![Het menu Meer](assets/more-icon-spectrum.png) in de kolom en selecteer **[!UICONTROL Edit]**. Typ in het gedeelte Instellingen de nieuwe naam in het dialoogvenster **[!UICONTROL Column name]** en klik op **[!UICONTROL Close]**.

## Een boardkolom verwijderen

Wanneer u een kolom van een board schrapt, kan het niet worden teruggekregen.

1. Toegang tot het bord.
1. Klik op de knop **[!UICONTROL More]** menu ![Het menu Meer](assets/more-icon-spectrum.png) in de kolom en selecteer **[!UICONTROL Delete]**.

   >[!NOTE]
   >
   >Kolommen die kaarten bevatten, inclusief gearchiveerde kaarten, kunnen niet worden verwijderd. Als u een kolom probeert te schrappen die kaarten bevat, moet u een andere kolom voor die kaarten kiezen.

## Aantal kaarten weergeven

U kunt een configuratie het plaatsen gebruiken om het aantal kaarten in elke kolom te tonen.

Als u de grens van het KLOOFJE op een kolom gebruikt, wordt een afzonderlijke kaartteller niet toegevoegd. Voor meer informatie over de grenzen van het WIP, zie [De [!UICONTROL Work in Progress] (WIP)-limiet aan boord](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Toegang tot het bord.
1. Klikken **[!UICONTROL Configure]** rechts van de board om het Configure paneel te openen.
1. Uitbreiden **[!UICONTROL Column]**.
1. Inschakelen **[!UICONTROL Display a column card count]**.

   ![Kaartteller inschakelen](assets/display-card-count.png)

   De kaartteller wordt boven aan elke kolom weergegeven.

1. Klikken **[!UICONTROL Hide configure]** om de [!UICONTROL Configure] deelvenster.

## Kolominstellingen en -beleid definiëren

Kolombeleid omvat het automatisch bijwerken van veldwaarden en het instellen van een limiet voor werkzaamheden in uitvoering.

Het beleid voor het bijwerken van de status werkt automatisch voor zowel de kaart als de kolom:

* Wanneer een kaart naar een kolom met een beleid wordt verplaatst, wordt de kaartstatus bijgewerkt aan de status die in het beleid wordt bepaald. Dit geldt zowel voor ad hoc als voor aangesloten kaarten.
* Wanneer een ad hoc of verbonden kaartstatus op de kaart wordt bijgewerkt om de kolomstatus in het beleid aan te passen, of een verbonden kaartstatus elders in Workfront wordt bijgewerkt, wordt de kaart automatisch naar die kolom verplaatst. Als een aangepaste status op een kaart overeenkomt met de systeemstatus die aan de kolom is toegewezen, wordt de kaart ook naar die kolom verplaatst.

Een kaart blijft in een kolom waar deze wordt geplaatst als de kaartstatus niet overeenkomt met een status die is ingesteld in een bestaand kolombeleid.

>[!NOTE]
>
>Dynamische borden plaatsen altijd kaarten in de kolom die hun status aanpast, ongeacht of het kolombeleid wordt toegelaten of onbruikbaar gemaakt. De kaarten zullen aan hun toegewezen kolommen terugkeren wanneer u de raad vernieuwt.
> 
>Als u voor alle typen kaarten een kaart verplaatst van de ene kolom naar een andere kolom met dezelfde status, wordt de kaart teruggezet naar de oorspronkelijke kolom wanneer u de kaart vernieuwt.

1. Toegang tot het bord.
1. Klik op de knop **[!UICONTROL More]** menu ![Het menu Meer](assets/more-icon-spectrum.png) in de kolom en selecteer **[!UICONTROL Edit]**.

   De [!UICONTROL Settings] wordt weergegeven. De **[!UICONTROL Column name]** Hiermee weet u voor welke kolom u instellingen definieert.

1. De optie **[!UICONTROL Update field values automatically]** beleid om bepaalde veldwaarden automatisch te wijzigen wanneer een kaart naar deze kolom wordt verplaatst.

   ![Kolominstellingen en -beleid](assets/boards-column-policies-enabled.png)

1. (Optioneel) Stel een waarde in voor de kaartstatus:

   1. Selecteer de **[!UICONTROL Status]** selectievakje.

   1. Selecteer de status die u wilt toepassen op een kaart wanneer deze naar deze kolom wordt verplaatst.

      ![Status voor kolommen](assets/boards-column-status.png)

      De statusvertaalopties voor verbonden kaarten worden ook weergegeven. (De statusvertaling is niet van toepassing op ad-hockaarten.) Deze opties bepalen de aangepaste status die wordt toegepast op de taak of uitgave in [!DNL Workfront] wanneer een aangesloten kaart naar deze kolom wordt verplaatst.

   1. Selecteer een [!UICONTROL **Aangepast**] status die op de kaart moet worden toegepast voor taken en voor problemen.

      Wanneer een kaart naar deze kolom wordt verplaatst, [!DNL Workfront] probeert eerst de aangepaste status toe te passen (bijvoorbeeld Opgelost). Als de geselecteerde aangepaste status niet beschikbaar is voor die kaart, wordt u gevraagd een andere status te kiezen die overeenkomt met de systeemstatus (in stap b hierboven). Zie voor meer informatie over statussen [Overzicht van statussen](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

      Als de status van de verbonden taak of uitgave wordt gewijzigd in de aangepaste of systeemstatus die is ingesteld in het kolombeleid, wordt de kaart automatisch naar de kolom verplaatst.

1. (Optioneel) Stel een waarde in voor de kaarttoewijzingen:

   1. Selecteer de **[!UICONTROL Assignees]** selectievakje.
   1. Selecteer een handeling.

      * **[!UICONTROL Add on assignees]:** De geselecteerde toewijzingen worden toegevoegd aan de bestaande lijst met toewijzingen op een kaart wanneer deze naar deze kolom wordt verplaatst.
      * **[!UICONTROL Override assignees]:** De geselecteerde toewijzingen overschrijven alle andere toewijzingen en worden de enige toewijzingen op een kaart wanneer deze naar deze kolom wordt verplaatst.

   1. Klikken [!UICONTROL **Toewijzing toevoegen**] en zoek naar een gebruiker. Selecteer de toewijzingen in de zoekresultaten. Alle Workfront-gebruikers en -teams kunnen kiezen uit.

      ![Toewijzingen voor kolom](assets/boards-column-assignees.png)

1. (Optioneel) Stel een waarde in voor de kaartcodes:

   1. Selecteer de **[!UICONTROL Cards]** selectievakje.
   1. Selecteer een handeling.

      * **[!UICONTROL Add on tags]:** De tags die u selecteert, worden toegevoegd aan de bestaande lijst met codes op een kaart wanneer deze naar deze kolom wordt verplaatst.
      * **[!UICONTROL Override tags]:** De tags die u selecteert, overschrijven alle andere tags en worden de enige tags op een kaart wanneer deze naar deze kolom wordt verplaatst.

   1. Selecteer de labels in de vervolgkeuzelijst. Alleen tags die al in het dialoogvenster [!UICONTROL Tag Manager] zijn beschikbaar waaruit u kunt kiezen. Zie voor informatie over het toevoegen van nieuwe tags [Tags toevoegen](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![Codes voor kolom](assets/boards-column-tags.png)

1. De optie **[!UICONTROL Work in progress limit]** beleid om het aantal kaarten te beperken dat aan de kolom kan worden toegevoegd. Typ vervolgens het limietnummer in het dialoogvenster **[!UICONTROL Set limit]** veld.

   ![WIP-limiet voor kolom](assets/boards-wip-limit-in-column.png)

   Zie voor meer informatie [De WIP-limiet (Work in progress) op een bord beheren](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Klikken **[!UICONTROL Close]** om het gebied van Montages weg te gaan en de kolom en zijn kaarten te bekijken.
