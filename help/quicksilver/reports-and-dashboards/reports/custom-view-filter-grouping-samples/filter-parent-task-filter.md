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
source-wordcount: '760'
ht-degree: 0%

---

# Filter: bovenliggende taken weergeven

U kunt de onderstaande taakfilters toepassen om werktaken weer te geven. De werktaken zijn taken die onafhankelijk kunnen worden gewerkt en geen oudertaken aan andere taken zijn. In één voorbeeld identificeert een filter kindertaken die ouders zelf zouden kunnen zijn. In dit geval zijn zij geen werktaken.

>[!TIP]
>
>* Als u overweegt toevoegend meer dan één filter aan een rapport, adviseren wij dat u al uw filters gebruikend de interface van de rapportbouwer toevoegt, en het klikken van Schakelaar aan de Wijze van de Tekst nadat alle andere filterregels zijn toegevoegd. Vervolgens kunt u de code voor het bovenliggende taakfilter toevoegen, zoals hierboven is aangegeven. 
>* Wij adviseren ook dat u een groepering voor de Naam van het Project toevoegt om het rapport gemakkelijker te maken te lezen. Voor meer informatie over het toevoegen van groeperingen aan uw rapporten, zie het artikel [ overzicht van Groepen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
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

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Taken weergeven zonder onderliggende items (deze kunnen een bovenliggend item hebben)

U kunt het volgende filter op een taakrapport toepassen om taken zonder kinderen te tonen. Ze zouden zelf ouders kunnen hebben en kinderen kunnen zijn van andere taken.

1. Van het **Belangrijkste Menu** ![](assets/main-menu-icon.png), klik **Rapporten.**

1. Klik **Nieuw Rapport**.
1. Selecteer het Rapport van de Taak van a ****.
1. Klik **Filters**.
1. Klik **toevoegen een Regel van de Filter**.
1. In het **Begin typend gebiedsnaam..** lijn, begin **Aantal Kinderen** te typen.

1. Selecteer **Gelijk (Gevoelig van het Geval)** voor uw bepaling, dan ga **0** voor het aantal kinderen in.\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   of

   Klik **Schakelaar aan de Wijze van de Tekst**, en in het tekst het uitgeven venster, kopieer en kleef de volgende tekst: 

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Klik **sparen + Sluiten**.

   Dit trekt een rapport voor alle taken die taken in uw systeem werken. Sommige van deze taken kunnen een bovenliggende taak hebben, maar zijn zelf geen bovenliggende taken.

## Taken weergeven met bovenliggende items (mogelijk onderliggende items)

U kunt het volgende filter op een taakrapport toepassen om taken met ouders te tonen, betekenend zijn zij kindtaken. Deze taken kunnen echter ook eigen onderliggende items hebben, omdat het filter de onderliggende items niet uitsluit. Kindertaken die ook ouders zijn voor andere taken worden niet beschouwd als werktaken.

1. Van het **Belangrijkste Menu** ![](assets/main-menu-icon.png), klik **Rapporten.
1. Klik **Nieuw Rapport**.
1. Selecteer het Rapport van de Taak van a ****.
1. Klik **Filters**.
1. Klik **toevoegen een Regel van de Filter**.
1. In het **Begin typend gebiedsnaam..** lijn, begin **Identiteitskaart van de Ouder** te typen.
1. Selecteer **is niet leeg** voor uw bepaling.

   ![](assets/filter-parent-id-not-blank-350x100.png)

   of

   Klik **Schakelaar aan de Wijze van de Tekst**, en in het tekst het uitgeven venster, kopieer en kleef de volgende tekst: 

   `parentID_Mod=notblank`

1. Klik **sparen + Sluiten**.

   Hiermee wordt een rapport gepubliceerd voor alle taken in uw systeem die ouders hebben en kindertaken zijn van die ouders. Sommige van deze taken zouden een ouder zelf kunnen zijn.

## Taken weergeven zonder onderliggende items en zonder bovenliggende items (zelfstandige taken)

U kunt het volgende filter op een taakrapport toepassen om standalone het werken taken te tonen. Deze taken hebben geen ouder en ze hebben geen eigen kinderen.

1. Van het **Belangrijkste Menu** ![](assets/main-menu-icon.png), klik **Rapporten.**
1. Klik **Nieuw Rapport**.
1. Selecteer het Rapport van de Taak van a ****.
1. Klik **Filters**.
1. Klik **toevoegen een Regel van de Filter** en in het **Begin typend gebiedsnaam..** lijnbegin typend **Aantal van Kinderen** uitgezochte **Gelijk (Gevoelig van het Geval)** voor uw bepaling, dan ga **0** voor het aantal kinderen in.
1. Klik **toevoegen een andere Regel van de Filter** en in het **Begin typend gebiedsnaam..** lijnbegin typend **identiteitskaart van de Ouder**, dan uitgezocht **is Lege**.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   of

   In plaats van stappen 6-7, klik **Schakelaar aan de Wijze van de Tekst** en in het tekst het uitgeven venster, kopieer en kleef de volgende tekst: 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure steps above stay accurate)</p>
   -->

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Klik **sparen + Sluiten**.

   Hiermee wordt een rapport gepubliceerd voor alle taken in uw systeem die geen ouders of kinderen hebben. Dit zijn zelfstandige werktaken.
