---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: bovenliggende taken weergeven'
description: U kunt de onderstaande taakfilters toepassen om werktaken weer te geven. De werktaken zijn taken die onafhankelijk kunnen worden gewerkt en geen oudertaken aan andere taken zijn. In één voorbeeld identificeert een filter kindertaken die ouders zelf zouden kunnen zijn. In dit geval zijn zij geen werktaken.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 0%

---

# Filter: bovenliggende taken weergeven

<!--Audited: 10/2024-->

U kunt de onderstaande taakfilters toepassen om werktaken weer te geven. De werktaken zijn taken die onafhankelijk kunnen worden gewerkt en geen oudertaken aan andere taken zijn. In één voorbeeld identificeert een filter kindertaken die ouders zelf zouden kunnen zijn. In dit geval zijn zij geen werktaken.

>[!TIP]
>
>* Als u overweegt toevoegend meer dan één filter aan een rapport, adviseren wij dat u al uw filters gebruikend de interface van de rapportbouwer toevoegt, en het klikken van Schakelaar aan de Wijze van de Tekst nadat alle andere filterregels zijn toegevoegd. Vervolgens kunt u de code voor het bovenliggende taakfilter toevoegen, zoals hierboven is aangegeven. 
>* Wij adviseren ook dat u een groepering voor de Naam van het Project toevoegt om het rapport gemakkelijker te maken te lezen. Voor meer informatie over het toevoegen van groeperingen aan uw rapporten, zie het artikel [ overzicht van Groepen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Medewerker of verzoek om een filter te wijzigen </p>
   <p>Standaard of Plan om een rapport te wijzigen</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Taken weergeven zonder onderliggende items (deze kunnen een bovenliggend item hebben)

U kunt het volgende filter op een taakrapport toepassen om taken zonder kinderen te tonen. Ze zouden zelf ouders kunnen hebben en kinderen kunnen zijn van andere taken.

1. Van het **Belangrijkste Menu** ![ Belangrijkste pictogram van het Menu ](assets/main-menu-icon.png) in de hoger-juiste hoek, of de **HoofdMenu** ![ Belangrijkste lijnen van het Menu ](assets/lines-main-menu.png) in de upper-left hoek, als beschikbaar, klik **Rapporten**.

1. Klik **Nieuw Rapport**.
1. Selecteer het Rapport van de Taak van a ****.
1. Klik **Filters**.
1. Klik **toevoegen een Regel van de Filter**.
1. In het **Begin typend gebiedsnaam..** lijn, begin **Aantal Kinderen** te typen, dan klik **Taak >> Aantal Kinderen** wanneer het in de lijst toont.

1. Selecteer **Gelijk (Gevoelig van het Geval)** voor uw bepaling, dan ga **0** voor het aantal kinderen in.\
   ![ de taakfilter van de Ouder ](assets/parent-task-filter-from-the-ui-350x76.png)

   of

   Klik **Schakelaar aan de Wijze van de Tekst**, en in het tekst het uitgeven venster, kopieer en plak de volgende tekst

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Klik **sparen + Sluiten**.

   Dit trekt een rapport voor alle taken die taken in uw systeem werken. Sommige van deze taken kunnen een bovenliggende taak hebben, maar zijn zelf geen bovenliggende taken.

## Taken weergeven met bovenliggende items (mogelijk onderliggende items)

U kunt het volgende filter op een taakrapport toepassen om taken met ouders te tonen, betekenend zijn zij kindtaken. Deze taken kunnen echter ook eigen onderliggende items hebben, omdat het filter de onderliggende items niet uitsluit. Kindertaken die ook ouders zijn voor andere taken worden niet beschouwd als werktaken.

1. Van het **Belangrijkste Menu** ![ Belangrijkste pictogram van het Menu ](assets/main-menu-icon.png) in de hoger-juiste hoek, of de **HoofdMenu** ![ Belangrijkste lijnen van het Menu ](assets/lines-main-menu.png) in de upper-left hoek, als beschikbaar, klik **Rapporten**.

1. Klik **Nieuw Rapport**.
1. Selecteer het Rapport van de Taak van a ****.
1. Klik **Filters**.
1. Klik **toevoegen een Regel van de Filter**.
1. In het **Begin typend gebiedsnaam..** lijn, begin **identiteitskaart van de Ouder** te typen, dan uitgezochte **Taak >> identiteitskaart van de Ouder** wanneer het in de lijst toont.
1. Selecteer **is niet leeg** voor uw bepaling.

   ![ identiteitskaart van de Ouder is niet leeg ](assets/filter-parent-id-not-blank-350x100.png)

   of

   Klik **Schakelaar aan de Wijze van de Tekst**, en in het tekst het uitgeven venster, kopieer en kleef de volgende tekst: 

   `parentID_Mod=notblank`

1. Klik **sparen + Sluiten**.

   Hiermee wordt een rapport gepubliceerd voor alle taken in uw systeem die ouders hebben en kindertaken zijn van die ouders. Sommige van deze taken zouden een ouder zelf kunnen zijn.

## Taken weergeven zonder onderliggende items en zonder bovenliggende items (zelfstandige taken)

U kunt het volgende filter op een taakrapport toepassen om standalone het werken taken te tonen. Deze taken hebben geen ouder en ze hebben geen eigen kinderen.

1. Van het **Belangrijkste Menu** ![ Belangrijkste pictogram van het Menu ](assets/main-menu-icon.png) in de hoger-juiste hoek, of de **HoofdMenu** ![ Belangrijkste lijnen van het Menu ](assets/lines-main-menu.png) in de upper-left hoek, als beschikbaar, klik **Rapporten**.

1. Klik **Nieuw Rapport**.
1. Selecteer het Rapport van de Taak van a ****.
1. Klik **Filters**.
1. Klik **toevoegen een Regel van de Filter**.
1. In het **Begin typend gebiedsnaam..** lijn begint **Aantal Kinderen** te typen, dan uitgezochte **Taak >> Aantal Kinderen** van de lijst.
1. Selecteer **Gelijk (Gevoelig van het Geval)** voor uw bepaling, dan ga **0** voor het aantal kinderen in.
1. Klik **toevoegen een andere Regel van de Filter**.
1. In het **Begin typend gebiedsnaam..** lijn begint **identiteitskaart van de Ouder** te typen, dan uitgezochte **Taak >> identiteitskaart van de Ouder** van de lijst.
1. Selecteer **is leeg** voor de bepaling.

   ![ identiteitskaart van de Ouder is leeg en geen kinderen ](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   of

   In plaats van stappen 6-10 <!--ensure steps above stay accurate-->, klik **Schakelaar aan de Wijze van de Tekst** en in het tekst het uitgeven venster, kopieer en kleef de volgende tekst:

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Klik **sparen + Sluiten**.

   Hiermee wordt een rapport gepubliceerd voor alle taken in uw systeem die geen ouders of kinderen hebben. Dit zijn zelfstandige werktaken.
