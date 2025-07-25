---
title: Het hoofdmenu aanpassen met behulp van een lay-outsjabloon
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Adobe Workfront-beheerder of groepsbeheerder kunt u een lay-outsjabloon gebruiken om de opties te configureren die gebruikers zien wanneer ze het Hoofdmenu in Workfront openen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: 00ec13dfb082ecd9b087d79b385a4eea677cf55d
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# Het hoofdmenu aanpassen met een lay-outsjabloon

<!--Audited: 01/2024-->

Als Adobe Workfront-beheerder of groepsbeheerder kunt u een lay-outsjabloon gebruiken om de opties te configureren die gebruikers zien wanneer ze het Hoofdmenu in Workfront openen.

>[!NOTE]
>
>De belangrijkste opties van het Menu die de gebruikers zien hangen van hun vergunningstype af en welke montages in hun toegangsniveau worden gevormd. Sommige gebruikers die deze lay-outsjabloon gebruiken, zien mogelijk niet alle opties die u hier kiest. Voor meer informatie zie [ hoe de toegangsniveaus en de toestemmingen samen ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) en [ Configureerbare toegang tot functionaliteit voor elk objecten type ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md) werken.
>
>U zou verschillende opties in het Belangrijkste Menu kunnen zien als uw organisatie op de Adobe Workfront Verenigde Ervaring is ingezien. Voor informatie, zie [ Adobe Verenigde Ervaring voor Workfront ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

Voor informatie over het creëren van lay-outmalplaatjes, zie [ lay-outmalplaatjes ](../use-layout-templates/create-and-manage-layout-templates.md) creëren en beheren.

Voor informatie over lay-outmalplaatjes voor groepen, zie [ tot stand brengen en wijzigen de lay-outmalplaatjes van een groep ](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nadat u een lay-outmalplaatje hebt gevormd, moet u het aan gebruikers voor veranderingen toewijzen u aanbracht om aan anderen zichtbaar te zijn. Voor informatie over het toewijzen van een lay-outmalplaatje aan gebruikers, zie [ gebruikers aan een lay-outmalplaatje ](../use-layout-templates/assign-users-to-layout-template.md) toewijzen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan</strong></td> 
   <td><p>Alle</p>

<p>Het toevoegen van aangepaste toepassingen aan het hoofdmenu is alleen beschikbaar voor organisaties die een licentie hebben voor Adobe App Builder.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie*</strong></td> 
   <td><p>Huidig: Plan</p>
   of
   <p>Nieuw: Standaard</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuratie op toegangsniveau</strong></td> 
   <td> <p>Om deze stappen op systeemniveau uit te voeren, hebt u het toegangsniveau van de Beheerder van het Systeem nodig.</p>
    <p>Om hen voor een groep uit te voeren, moet u een manager van die groep zijn.</p> 
     </td> 
  </tr> 
 </tbody> 
</table>

*Voor meer informatie over toegangsvereisten, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Het hoofdmenu aanpassen

1. Begin werkend aan een lay-outmalplaatje, zoals die in [ wordt beschreven creeer en beheer lay-outmalplaatjes ](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klik **Vastgestelde HoofdMenu** in de hoger-juiste hoek van het malplaatje.

   Het vak Hoofdmenu wordt geopend en u kunt de gebieden zien die momenteel worden weergegeven in het hoofdmenu voor de sjabloon, plus de items die beschikbaar zijn om toe te voegen. Hieronder vindt u alle mogelijke items die u kunt toevoegen:
   * Home

     >[!TIP]
     >
     >Door gebrek, toont het pictogram van het Huis in het Belangrijkste Menu het Mijn gebied van Updates voor revisie-vergunning gebruikers (in het huidige vergunningsplan), tenzij zij een lay-outmalplaatje verbonden aan hun profiel hebben dat het Mijn gebied van Updates in het Belangrijkste Menu, naast het gebied van het Huis omvat.

   * Portfolio&#39;s
   * Programma&#39;s
   * Projecten
   * Rapporten
   * Dashboards
   * Kalenders
   * Bronnen
   * Scenarios

     >[!NOTE]
     >
     >Voor de Scenario Planner is een aanvullende licentie vereist. Voor informatie over de Planner van het Scenario van Workfront, zie [ het overzicht van de Planner van het Scenario ](../../../scenario-planner/scenario-planner-overview.md).

   * Teams
   * Gebruikers

     >[!NOTE]
     >
     >Slechts kunnen de gebruikers met een vergunning van het Plan (in het huidige vergunningsmodel), of de gebruikers met een Standaardvergunning (in het nieuwe vergunningsmodel) het pictogram van Gebruikers van het gebied van Gebruikers ![ ](assets/users-icon-in-main-menu.png) in het Belangrijkste Menu zien.

   * Verzoeken
   * Timesheets
   * Documenten
   * Sjablonen
   * Proofing
   * Doelen

     >[!NOTE]
     >
     >Voor doelen is een extra licentie vereist. Voor informatie over de Doelen van Workfront, zie [ overzicht van de Doelen van Adobe Workfront ](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * Mijn updates
   * Borden
   * Blauwdrukken
   * Planning

     >[!NOTE]
     >
     >Voor planning is een aanvullende licentie vereist. Voor informatie over de Planning van Workfront, zie [ het Overzicht van de Planning van Adobe Workfront ](/help/quicksilver/planning/general/planning-overview.md).

   * Aangepaste toepassing

     >[!NOTE]
     >
     > Aangepaste toepassingen moeten afzonderlijk worden gemaakt voordat ze beschikbaar komen als opties in het hoofdmenu. Voor meer informatie, zie [ een douanetoepassing voor Workfront met Adobe App Builder ](/help/quicksilver/app-builder/app-builder.md) creëren.

1. Voer een van de volgende handelingen uit:

   * Verberg ![ pictogram van de Verbergen ](assets/remove-icon---x-in-circle.png) **Actieve punten** dat u niet wilt tonen
   * Toon ![ pictogram van de Show ](assets/add-icon-plus-in-circle.png) **Beschikbare punten** die u op het Belangrijkste Menu wilt tonen.
   * De belemmering ![ pictogram van de belemmering ](assets/move-icon---dots.png) **Actieve punten** om hun vertoningsorde op het Belangrijkste Menu te veranderen.

1. Klik **Gedaan**.

   U kunt **ook klikken annuleert** op elk ogenblik als u uw veranderingen wilt verwerpen.

1. Blijf het lay-outmalplaatje aanpassen.

   of

   Als u wordt gebeëindigd aanpassend, klik **sparen**.

   >[!TIP]
   >
   >U kunt **klikken sparen** op elk ogenblik om uw vooruitgang te bewaren, dan blijven het malplaatje later wijzigen.

Voor meer informatie over lay-outmalplaatjes, zie [ lay-outmalplaatjes ](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) creëren en beheren.
