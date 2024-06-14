---
title: Het hoofdmenu aanpassen met een lay-outsjabloon
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Adobe Workfront-beheerder of groepsbeheerder kunt u een lay-outsjabloon gebruiken om de opties te configureren die gebruikers zien wanneer ze het Hoofdmenu in Workfront openen.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# Het hoofdmenu aanpassen met een lay-outsjabloon

<!--Audited: 01/2024-->

Als Adobe Workfront-beheerder of groepsbeheerder kunt u een lay-outsjabloon gebruiken om de opties te configureren die gebruikers zien wanneer ze het Hoofdmenu in Workfront openen.

![Opties voor Hoofdmenu](assets/main-menu-with-blueprints-no-branding.png)

>[!NOTE]
>
>De belangrijkste opties van het Menu die de gebruikers zien hangen van hun vergunningstype af en welke montages in hun toegangsniveau worden gevormd. Sommige gebruikers die deze lay-outsjabloon gebruiken, zien mogelijk niet alle opties die u hier kiest. Zie voor meer informatie [Hoe de toegangsniveaus en de toestemmingen samenwerken](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) en [Configureerbare toegang tot functionaliteit voor elk objecttype](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

Voor informatie over het maken van lay-outsjablonen raadpleegt u [Lay-outsjablonen maken en beheren](../use-layout-templates/create-and-manage-layout-templates.md).

Voor informatie over lay-outsjablonen voor groepen raadpleegt u [De lay-outsjablonen van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nadat u een lay-outmalplaatje hebt gevormd, moet u het aan gebruikers voor veranderingen toewijzen u aanbracht om aan anderen zichtbaar te zijn. Voor informatie over het toewijzen van een lay-outsjabloon aan gebruikers raadpleegt u [Gebruikers toewijzen aan een lay-outsjabloon](../use-layout-templates/assign-users-to-layout-template.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan</strong></td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie*</strong></td> 
   <td><p>Huidig:Plan</p>
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

*Voor meer informatie over toegangsvereisten, zie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Het hoofdmenu aanpassen

1. Beginnen met het werken aan een lay-outsjabloon, zoals beschreven in [Lay-outsjablonen maken en beheren](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klikken **Hoofdmenu instellen** rechtsboven in de sjabloon.

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
     >Voor de Scenario Planner is een aanvullende licentie vereist. Voor informatie over de Workfront Scenario Planner raadpleegt u [Overzicht van de functie Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

   * Teams
   * Gebruikers

     >[!NOTE]
     >
     >Alleen gebruikers met een licentie voor het abonnement (in het huidige licentiemodel) of gebruikers met een standaardlicentie (in het nieuwe licentiemodel) kunnen het gebruikersgebied zien ![](assets/users-icon-in-main-menu.png) in het hoofdmenu.

   * Verzoeken
   * Timesheets
   * Documenten
   * Sjablonen
   * Analyse
   * Proofing
   * Doelen

     >[!NOTE]
     >
     >Voor doelen is een extra licentie vereist. Voor informatie over Workfront Goals raadpleegt u [Overzicht van Adobe Workfront-doelen](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * Mijn updates
   * Borden
   * Blauwdrukken

1. Voer een van de volgende handelingen uit:

   * Verbergen ![](assets/remove-icon---x-in-circle.png) **Actieve objecten** die u niet wilt weergeven
   * Tonen ![](assets/add-icon-plus-in-circle.png) **Beschikbare objecten** die u wel wilt weergeven in het hoofdmenu.
   * Slepen ![](assets/move-icon---dots.png) **Actieve objecten** om hun vertoningsorde op het Belangrijkste Menu te veranderen.

1. Klikken **Gereed**.

   U kunt ook op **Annuleren** als u uw wijzigingen wilt negeren.

1. Blijf het lay-outmalplaatje aanpassen.

   of

   Als u klaar bent met aanpassen, klikt u op **Opslaan**.

   >[!TIP]
   >
   >U kunt op elk gewenst moment op Opslaan klikken om de voortgang op te slaan en de sjabloon later blijven wijzigen.

Zie voor meer informatie over lay-outsjablonen [Lay-outsjablonen maken en beheren](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
