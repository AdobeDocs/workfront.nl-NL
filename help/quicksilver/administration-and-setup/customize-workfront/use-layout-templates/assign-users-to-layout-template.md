---
title: Gebruikers toewijzen aan een lay-outsjabloon
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Als beheerder van Adobe Workfront, kunt u een lay-outmalplaatje toewijzen u aan om het even welke gebruiker, baanrol, team, of groep hebt gecreeerd die het moet gebruiken.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
source-git-commit: c037b4f9e5530d8dd796bed25021f7073f16061f
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---

# Gebruikers toewijzen aan een lay-outsjabloon

U kunt een lay-outmalplaatje toewijzen u aan om het even welke gebruiker, baanrol, team, of groep creeerde die het moet gebruiken.

Voor gebruikers waaraan geen lay-outsjabloon is toegewezen, wordt de standaardlay-out gebruikt. Om over de standaardlay-out te leren, zie [ Ongeveer de standaard lay-out van Adobe Workfront ](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Gebruikers kunnen ook een lay-outsjabloon aan zichzelf toewijzen, zoals wordt beschreven in de gebieden Mijn werk en Werkverzoeken wijzigen met lay-outsjablonen.

U kunt meerdere verschillende lay-outsjablonen aan dezelfde naam toewijzen. Voor meer informatie waarover lay-outmalplaatje in feite voor een gebruiker, een rol, een groep, of een team is, zie {de prioriteit van de het malplaatjetoewijzing van 0} Lay-out [ later in dit artikel.](#layout-template-assignment-priority)

Voor meer informatie over lay-outmalplaatjes, zie [ malplaatjes van de Lay-out ](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

Voor informatie over lay-outmalplaatjes voor groepen, zie [ tot stand brengen en wijzigen de lay-outmalplaatjes van een groep ](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>Om deze stappen op systeemniveau uit te voeren, hebt u het toegangsniveau van de Beheerder van het Systeem nodig.</p>
        <p>Om hen voor een groep uit te voeren, moet u een manager van die groep zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een lay-outsjabloon toewijzen aan gebruikers

1. Begin werkend aan een lay-outmalplaatje, zoals die in [ wordt beschreven creeer en beheer lay-outmalplaatjes ](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

   >[!TIP]
   >
   >Wanneer u met uw lay-outmalplaatje wordt tevreden, adviseren wij dat u het test, zoals die in [ wordt beschreven Test een nieuw lay-outmalplaatje ](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md).

1. Klik **toewijzen dit aan** in de hoogste sectie van de pagina.
1. In de doos die verschijnt, **voeg een Gebruiker, de Rol van de Baan, Team, of Groep** toe, begin de naam van een gebruiker, baanrol, team, of groep te typen, dan de naam te klikken wanneer het in drop-down verschijnt.

   Onlangs toegevoegde namen worden weergegeven met een blauwe achtergrond. Dit is handig wanneer u een bestaande lay-outsjabloon bewerkt, omdat u de namen die u zojuist hebt toegevoegd kunt onderscheiden van de namen die al in de lijst stonden.

   Een pictogram van Info ![ pictogram van Info ](assets/info-icon.png) toont rechts van de naam van om het even welke gebruiker, baanrol, team, of groep die reeds aan een ander lay-outmalplaatje wordt toegewezen. Als u de muisaanwijzer op het pictogram plaatst, ziet u de naam van de lay-outsjabloon en bepaalt u of u de bestaande toewijzing wilt overschrijven.

1. Herhaal de twee vorige stappen om de lay-outsjabloon desgewenst toe te wijzen aan andere gebruikers, taakrollen, teams of groepen.

   U kunt maximaal 100 gebruikers tegelijk toewijzen.

1. Klik **Gedaan**, dan klik **sparen en sluit** in de laag-linkerhoek.

   Met deze stap voltooit u het proces voor het maken en toewijzen van een lay-outsjabloon.

## Toewijzingsprioriteit lay-outsjabloon {#layout-template-assignment-priority}

U en andere Workfront-beheerders kunnen op de volgende vier verschillende manieren meerdere verschillende lay-outsjablonen aan dezelfde gebruiker toewijzen:

* Aan de individuele gebruiker
* Voor een bepaalde taakrol heeft de gebruiker
* Voor een bepaald team is de gebruiker ingeschakeld
* Aan een bepaalde groep bevindt de gebruiker zich in

Er is echter maar één lay-outsjabloon zichtbaar voor de gebruiker op een bepaald moment. De sjabloon die zichtbaar is, wordt bepaald door de volgende prioriteitshiërarchie:

* **Individuele gebruiker**: Het lay-outmalplaatje dat aan de persoon als individuele gebruiker wordt toegewezen treedt alle anderen met voeten. U kunt een vorige toewijzing negeren die is gemaakt als een individuele gebruiker door een nieuwe toewijzing te maken; de meest recente krijgt voorrang.
* **Primaire baanrol**: Als de persoon geen lay-outmalplaatje als één enkele gebruiker wordt toegewezen, zien zij het malplaatje dat voor hun primaire baanrol wordt toegewezen.

  Alleen de lay-outsjabloon die aan de primaire taakrol van een gebruiker is toegewezen, is zichtbaar voor de gebruiker. De malplaatjes die aan om het even welke secundaire baanrollen worden toegewezen die door de gebruiker worden gehouden zijn niet zichtbaar.

* **team van het Huis**: Als de persoon geen lay-outmalplaatje als individuele gebruiker, noch als gebruiker met een primaire baanrol wordt toegewezen, zien zij het malplaatje dat aan hun team van het Huis wordt toegewezen.

  Alleen de sjabloon die is toegewezen aan het Home-team van een gebruiker is zichtbaar voor de gebruiker. De malplaatjes die aan andere teams worden toegewezen waar een gebruiker een lid is zijn niet zichtbaar.

* **Groep van het Huis**: Als de persoon geen lay-outmalplaatje als individuele gebruiker, noch als gebruiker met een primaire baanrol, noch als lid van een team van het Huis wordt toegewezen, zien zij het malplaatje dat aan hun Groep van het Huis wordt toegewezen.

  Alleen de sjabloon die is toegewezen aan de groep Home van een gebruiker is zichtbaar voor de gebruiker. Sjablonen die aan een van de andere groepen zijn toegewezen, zijn niet zichtbaar.

## Grote aantallen gebruikers die zijn toegewezen aan een lay-outsjabloon

<!--If you edit a layout template which is assigned to more than 2000 users and make changes to it, only the first 2000 users will be retained on the layout template and will see the changes you made. The layout template is removed from all others.
-->
Als u meer dan 2000 gebruikers aan een lay-outmalplaatje hebt toe te wijzen, adviseren wij dat u één van het volgende doet:

* Organiseer de gebruikers in groepen of teams en wijs het lay-outmalplaatje aan die groepen of teams toe. Voor meer informatie, zie [ een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) creëren en [ teams ](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md) creëren en beheren.

* Wijs baanrollen aan de gebruikers toe en wijs het lay-outmalplaatje aan hun primaire baanrol toe. Voor meer informatie, zie [ baanrollen ](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md) creëren en beheren.
