---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: bovenliggende taken weergeven'
description: U kunt de onderstaande taakfilters toepassen om werktaken weer te geven. De werktaken zijn taken die onafhankelijk kunnen worden gewerkt en geen oudertaken aan andere taken zijn. In één voorbeeld identificeert een filter kindertaken die ouders zelf zouden kunnen zijn. In dit geval zijn zij geen werktaken.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Filter: bovenliggende taken weergeven

U kunt de onderstaande taakfilters toepassen om werktaken weer te geven. De werktaken zijn taken die onafhankelijk kunnen worden gewerkt en geen oudertaken aan andere taken zijn. In één voorbeeld identificeert een filter kindertaken die ouders zelf zouden kunnen zijn. In dit geval zijn zij geen werktaken.

>[!TIP]
>
>* Als u overweegt toevoegend meer dan één filter aan een rapport, adviseren wij dat u al uw filters gebruikend de interface van de rapportbouwer toevoegt, en het klikken van Schakelaar aan de Wijze van de Tekst nadat alle andere filterregels zijn toegevoegd. Vervolgens kunt u de code voor het bovenliggende taakfilter toevoegen, zoals hierboven is aangegeven. 
* Wij adviseren ook dat u een groepering voor de Naam van het Project toevoegt om het rapport gemakkelijker te maken te lezen. Zie het artikel voor meer informatie over het toevoegen van groepen aan uw rapporten [Overzicht van groepen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>


## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Verzoek om een filter te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Taken weergeven zonder onderliggende items (deze kunnen een bovenliggend item hebben)

U kunt het volgende filter op een taakrapport toepassen om taken zonder kinderen te tonen. Ze zouden zelf ouders kunnen hebben en kinderen kunnen zijn van andere taken.

1. Van de **Hoofdmenu** ![](assets/main-menu-icon.png), klikt u op **Rapporten.**

1. Klikken **Nieuw rapport**.
1. Selecteer een **Taakrapport**.
1. Klikken **Filters**.
1. Klikken **Filterregel toevoegen**.
1. In de **Veldnaam beginnen te typen...** regel, beginnen met typen **Aantal onderliggende elementen**.

1. Selecteren **Gelijk (hoofdlettergevoelig)** voor uw bepaling, dan ga binnen **0** voor het aantal kinderen.\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   of

   Klikken **Overschakelen naar tekstmodus** en kopieer en plak in het tekstbewerkingsvenster de volgende tekst: 

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Klikken **Opslaan + Sluiten**.

   Dit trekt een rapport voor alle taken die taken in uw systeem werken. Sommige van deze taken kunnen een bovenliggende taak hebben, maar zijn zelf geen bovenliggende taken.

## Taken weergeven met bovenliggende items (mogelijk onderliggende items)

U kunt het volgende filter op een taakrapport toepassen om taken met ouders te tonen, betekenend zijn zij kindtaken. Deze taken kunnen echter ook eigen onderliggende items hebben, omdat het filter de onderliggende items niet uitsluit. Kindertaken die ook ouders zijn voor andere taken worden niet beschouwd als werktaken.

1. Van de **Hoofdmenu** ![](assets/main-menu-icon.png), klikt u op **Rapporten.
1. Klikken **Nieuw rapport**.
1. Selecteer een **Taakrapport**.
1. Klikken **Filters**.
1. Klikken **Filterregel toevoegen**.
1. In de **Veldnaam beginnen te typen...** regel, beginnen met typen **Bovenliggende id**.
1. Selecteren **Is niet leeg** voor uw bepaling.

   ![](assets/filter-parent-id-not-blank-350x100.png)

   of

   Klikken **Overschakelen naar tekstmodus** en kopieer en plak in het tekstbewerkingsvenster de volgende tekst: 

   `parentID_Mod=notblank`

1. Klikken **Opslaan + Sluiten**.

   Hiermee wordt een rapport gepubliceerd voor alle taken in uw systeem die ouders hebben en kindertaken zijn van die ouders. Sommige van deze taken zouden een ouder zelf kunnen zijn.

## Taken weergeven zonder onderliggende items en zonder bovenliggende items (zelfstandige taken)

U kunt het volgende filter op een taakrapport toepassen om standalone werkende taken te tonen. Deze taken hebben geen ouder en ze hebben geen eigen kinderen.

1. Van de **Hoofdmenu** ![](assets/main-menu-icon.png), klikt u op **Rapporten.**
1. Klikken **Nieuw rapport**.
1. Selecteer een **Taakrapport**.
1. Klikken **Filters**.
1. Klikken **Filterregel toevoegen** en in de **Veldnaam beginnen te typen...** Regelbegin typen **Aantal onderliggende elementen** selecteren **Gelijk (hoofdlettergevoelig)** voor uw bepaling, dan ga binnen **0** voor het aantal kinderen.
1. Klikken **Een andere filterregel toevoegen** en in de **Veldnaam beginnen te typen...** Regelbegin typen **Bovenliggende id** selecteert u vervolgens **Is leeg**.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   of

   Klik in plaats van de stappen 6-7 op **Overschakelen naar tekstmodus** en kopieer en plak in het tekstbewerkingsvenster de volgende tekst: 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure steps above stay accurate)</p>
   -->

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Klikken **Opslaan + Sluiten**.

   Hiermee wordt een rapport gepubliceerd voor alle taken in uw systeem die geen ouders of kinderen hebben. Dit zijn zelfstandige werktaken.
