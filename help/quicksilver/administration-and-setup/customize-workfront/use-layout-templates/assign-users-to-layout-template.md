---
title: Gebruikers toewijzen aan een lay-outsjabloon
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Als beheerder van Adobe Workfront, kunt u een lay-outmalplaatje toewijzen u aan om het even welke gebruiker, baanrol, team, of groep hebt gecreeerd die het moet gebruiken.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# Gebruikers toewijzen aan een lay-outsjabloon

U kunt een lay-outmalplaatje toewijzen u aan om het even welke gebruiker, baanrol, team, of groep creeerde die het moet gebruiken.

Voor gebruikers waaraan geen lay-outsjabloon is toegewezen, wordt de standaardlay-out gebruikt. Zie voor meer informatie over de standaardlay-out [De standaard Adobe Workfront-lay-out](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Gebruikers kunnen ook een lay-outsjabloon aan zichzelf toewijzen, zoals wordt beschreven in de gebieden Mijn werk en Werkverzoeken wijzigen met lay-outsjablonen.

U kunt meerdere verschillende lay-outsjablonen aan dezelfde naam toewijzen. Voor meer informatie waarover lay-outmalplaatje voor een gebruiker, een rol, een groep, of een team van kracht is, zie [Toewijzingsprioriteit lay-outsjabloon](#layout-template-assignment-priority) later in dit artikel.

Voor meer informatie over lay-outsjablonen raadpleegt u [Lay-outsjablonen](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

Voor informatie over lay-outsjablonen voor groepen raadpleegt u [De lay-outsjablonen van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Om deze stappen op systeemniveau uit te voeren, hebt u het toegangsniveau van de Beheerder van het Systeem nodig.
Om hen voor een groep uit te voeren, moet u een manager van die groep zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Een lay-outsjabloon toewijzen aan gebruikers

1. Beginnen met het werken aan een lay-outsjabloon, zoals beschreven in [Lay-outsjablonen maken en beheren](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

   >[!TIP]
   >
   >Als u tevreden bent met de lay-outsjabloon, raden we u aan deze te testen, zoals beschreven in [Een nieuwe lay-outsjabloon testen](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md).

1. Klikken **Deze toewijzen aan** in de bovenste sectie van de pagina.
1. Klik in het vak dat wordt weergegeven op **Een gebruiker, taakrol, team of groep toevoegen**, begint de naam van een gebruiker, baanrol, team, of groep te typen, dan klik de naam wanneer het in drop-down verschijnt.

   Onlangs toegevoegde namen worden weergegeven met een blauwe achtergrond. Dit is handig wanneer u een bestaande lay-outsjabloon bewerkt, omdat u de namen die u zojuist hebt toegevoegd kunt onderscheiden van de namen die al in de lijst stonden.

   Een pictogram Info ![](assets/info-icon.png) wordt rechts van de naam van een gebruiker, taakrol, team of groep weergegeven die al is toegewezen aan een andere lay-outsjabloon. Als u de muisaanwijzer op het pictogram plaatst, ziet u de naam van de lay-outsjabloon en bepaalt u of u de bestaande toewijzing wilt overschrijven.

1. Herhaal de twee vorige stappen om de lay-outsjabloon desgewenst toe te wijzen aan andere gebruikers, taakrollen, teams of groepen.

   U kunt maximaal 100 gebruikers tegelijk toewijzen.

1. Klikken **Gereed** en klik vervolgens op **Opslaan** in de linkerbenedenhoek.

   Met deze stap voltooit u het proces voor het maken en toewijzen van een lay-outsjabloon.

## Toewijzingsprioriteit lay-outsjabloon {#layout-template-assignment-priority}

U en andere Workfront-beheerders kunnen op de volgende vier verschillende manieren meerdere verschillende lay-outsjablonen aan dezelfde gebruiker toewijzen:

* Aan de individuele gebruiker
* Voor een bepaalde taakrol heeft de gebruiker
* Voor een bepaald team is de gebruiker ingeschakeld
* Aan een bepaalde groep bevindt de gebruiker zich in

Er is echter maar één lay-outsjabloon zichtbaar voor de gebruiker op een bepaald moment. De sjabloon die zichtbaar is, wordt bepaald door de volgende prioriteitshiërarchie:

* **Individuele gebruiker**: De lay-outmalplaatje dat aan de persoon als individuele gebruiker wordt toegewezen treedt alle anderen met voeten. U kunt een vorige toewijzing die tot een individuele gebruiker is gemaakt, overschrijven door een nieuwe toewijzing te maken; de meest recente heeft voorrang .
* **Primaire functie**: Als de persoon geen lay-outmalplaatje als één enkele gebruiker wordt toegewezen, zien zij het malplaatje dat voor hun primaire baanrol wordt toegewezen.

  Alleen de lay-outsjabloon die aan de primaire taakrol van een gebruiker is toegewezen, is zichtbaar voor de gebruiker. De malplaatjes die aan om het even welke secundaire baanrollen worden toegewezen die door de gebruiker worden gehouden zijn niet zichtbaar.

* **Thuisteam**: Als de persoon geen lay-outmalplaatje als individuele gebruiker, noch als gebruiker met een primaire baanrol wordt toegewezen, zien zij het malplaatje dat aan hun team van het Huis wordt toegewezen.

  Alleen de sjabloon die is toegewezen aan het Home-team van een gebruiker is zichtbaar voor de gebruiker. De malplaatjes die aan andere teams worden toegewezen waar een gebruiker een lid is zijn niet zichtbaar.

* **Thuisgroep**: Als de persoon geen lay-outmalplaatje als individuele gebruiker, noch als gebruiker met een primaire baanrol, noch als lid van een team van het Huis wordt toegewezen, zien zij het malplaatje dat aan hun groep van het Huis wordt toegewezen.

  Alleen de sjabloon die is toegewezen aan de groep Home van een gebruiker is zichtbaar voor de gebruiker. Sjablonen die aan een van de andere groepen zijn toegewezen, zijn niet zichtbaar.

## Grote aantallen gebruikers die zijn toegewezen aan een lay-outsjabloon

Als u een lay-outmalplaatje uitgeeft dat aan meer dan 2000 gebruikers wordt toegewezen en veranderingen in het aanbrengt, slechts zullen de eerste 2000 gebruikers op het lay-outmalplaatje worden behouden en zullen de veranderingen zien u aanbracht. De lay-outsjabloon wordt van alle andere sjablonen verwijderd.

Als u meer dan 2000 gebruikers aan een lay-outmalplaatje hebt toe te wijzen, adviseren wij dat u één van het volgende doet:

* Organiseer de gebruikers in groepen of teams en wijs het lay-outmalplaatje aan die groepen of teams toe. Zie voor meer informatie [Een groep maken](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) en [Teams maken en beheren](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

* Wijs baanrollen aan de gebruikers toe en wijs het lay-outmalplaatje aan hun primaire baanrol toe. Zie voor meer informatie [Taakrollen maken en beheren](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
