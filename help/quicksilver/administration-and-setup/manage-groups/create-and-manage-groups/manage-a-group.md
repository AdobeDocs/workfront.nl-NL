---
user-type: administrator
product-area: system-administration;user-management
keywords: beheren,groeperen,bewerken,
navigation-topic: create-and-manage-groups
title: Een groep beheren
description: Als groepsbeheerder, kunt u een groep beheren die u van het gebied van Groepen in Opstelling beheert. Als er groepen zijn boven de groep die u beheert, kunnen hun beheerders dit ook voor uw groep doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1321'
ht-degree: 0%

---

# Een groep beheren

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

Als groepsbeheerder, kunt u een groep beheren die u van het gebied van Groepen in Opstelling beheert. Als er groepen zijn boven de groep die u beheert, kunnen hun beheerders dit ook voor uw groep doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

>[!NOTE]
>
>Wanneer u als beheerder voor een groep wordt toegewezen, erft u de rol van de groepsbeheerder voor om het even welke subgroepen die onder het zijn. De enige gebruikers die een subgroep kunnen beheren zijn de groepbeheerders voor de bovenste groep erboven en groepbeheerders die aan de subgroep zijn toegewezen.

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-abonnement*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> <p>U moet een groepsbeheerder van de groep of een beheerder van Workfront zijn. Zie voor meer informatie <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Groepbeheerders</a> en <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de Workfront-beheerder als u wilt weten welk abonnement- of licentietype u hebt.

## De groepslidmaatschappen beheren

U kunt gebruikers en andere groepen toevoegen aan en verwijderen uit een groep die u beheert. U kunt ook groepsleden toewijzen als beheerders voor de groep en de gebruikersprofielgegevens van groepsleden beheren.

Zie voor instructies [De groepslidmaatschappen weergeven en beheren](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

## De details van een groep beheren

U kunt de pagina Groepdetails weergeven en bewerken voor een groep of subgroep die u beheert. Deze pagina bevat een beschrijving van de groep, de namen van de bedrijfsleider en groepsbeheerders en een optie waarmee u de groep en alle subgroepen van de groep openbaar of privé kunt maken. En als u met uw toegangsniveau aangepaste formulieren kunt beheren, kunt u een aangepast formulier aan een groep koppelen.

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

Zie voor instructies [De details van een groep weergeven en beheren](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

## Een groep bewerken, kopiëren of verwijderen

Zonder de hoofdpagina te verlaten van een groep u bekijkt, kunt u, snel uitgeven, kopiëren of schrappen

<!--
DRAFTED IN FLARE:
or deactivate

-->

de groep.

<!--
DRAFTED IN FLARE:
Make this change when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Groepen**.

   In de lijst die wordt weergegeven, ziet u de groepen die u beheert, samen met eventuele subgroepen die u beheert. Adobe Workfront-beheerders kunnen alle groepen zien.

1. Selecteer de groep en klik op Bewerken ![](assets/edit-icon.png), Kopiëren ![](assets/copy-icon.png), of Verwijderen ![](assets/delete.png) pictogram.

   Raadpleeg een van de volgende opties als u informatie nodig hebt over het gebruik van het vak dat wordt weergegeven:

   * **Bewerken**: [De details van een groep weergeven en beheren](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **Kopiëren**: [Een groep op hoofdniveau maken door een bestaande groep of subgroep te kopiëren](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group) in het artikel [Een groep maken](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)

   * **Verwijderen**: [Een groep verwijderen](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## Project-, taak- en probleemvoorkeuren voor een groep configureren

Als u een groepsbeheerder bent en uw groep andere project, taak, en geef voorkeurmontages uit van die die op het systeemniveau worden geplaatst, kunt u de beheerder van Workfront vragen om een voorkeur voor alle groepen door de organisatie te ontgrendelen. Nadat het wordt ontgrendeld, kunt u (en groepsbeheerders voor alle andere groepen) het voor de groepen vormen u beheert.

Zie voor instructies [Projectvoorkeuren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) en  [Taak- en uitgavevoorkeuren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Subgroepen weergeven, toevoegen en configureren

U kunt subgroepen maken, weergeven, bewerken, kopiëren, hernoemen, exporteren en verwijderen onder een groep die u beheert.

## Gebeurtenismeldingen voor een groep configureren

Als een beheerder van Workfront de capaciteit ontgrendelt om gebeurtenisberichten voor de groepen in uw organisatie te vormen, kunt u hen voor een groep vormen u beheert. Zie voor instructies [Gebeurtenismeldingen voor een groep weergeven en configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Statussen maken en aanpassen voor een groep

Als groepsbeheerder, kunt u douanestatus voor een top-level groep tot stand brengen die u beheert. Dit geeft uw groepsautonomie en helpt de behoefte aan tientallen bedrijfs-brede douanestatus te elimineren. (Een Workfront-beheerder kan dit ook voor elke groep doen.)

U kunt de systeemstatus voor een top-level groep ook aanpassen als een beheerder van Workfront hen heeft gevormd om aanpassing toe te staan.

Zie voor instructies [Een groepsstatus maken of bewerken](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Werken met projecten van een groep

In het gebied van Groepen in Opstelling, wanneer u de belangrijkste pagina van een groep bekijkt u beheert, kunt u het volgende met projecten doen:

* Maak een lijst van en werk met (geef uit, kopieer, schrap, en de uitvoer) de projecten die met de groep en zijn subgroepen worden geassocieerd en die met u zijn gedeeld
* Een nieuw project voor de groep maken

Zie voor instructies [Projecten van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

## De goedkeuringsprocessen van een groep weergeven en beheren

Wanneer u een groep bekijkt die u in het gebied van Groepen beheert, kunt u de goedkeuringsprocessen bekijken en werken waarvoor de beheerders van de groep, of één van zijn subgroepen, administratieve toegang hebben.

Zie voor instructies [Goedkeuringsprocessen op groepsniveau](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## De lay-outsjablonen van een groep weergeven en beheren

Wanneer u een groep bekijkt die u in het gebied Groepen beheert, kunt u het Malplaatje van de Lay-out bekijken en werken waarvoor de beheerders van de groep, of één van zijn subgroepen, administratieve toegang hebben.

Zie voor instructies [De lay-outsjablonen van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## De schema&#39;s van groepsleden weergeven en beheren

Een groepsbeheerder die een programma voor een groep maakt, moet de groep specificeren waarvan de beheerders het schema zullen beheren. Typisch, is dit de groep waarvoor het programma wordt gecreeerd, maar het zou een verschillende groep kunnen zijn als de groepsbeheerder veelvoudige groepen beheert en één van andere specificeert in plaats daarvan.

Wanneer u de hoofdpagina van een groep bekijkt u, als de groep als wordt aangewezen waarvan de beheerders een programma kunnen uitgeven, kunt u het programma van de pagina van de groep bekijken en beheren.

Zie voor instructies [De schema&#39;s van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

## Gebruikersprofielen van groepsleden weergeven en beheren

Wanneer u de hoofdpagina van een groep bekijkt u beheert, kunt u de timesheet profielen beheren die u en andere beheerders van groep-of één van zijn subgroups-toestemming hebben om uit te geven. Zie voor instructies [De profielen van een groep maken en beheren](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md).

## De subgroepsleden van een groep weergeven en beheren

Wanneer u de hoofdpagina bekijkt van een groep die u beheert, kunt u alle gebruikers in de subgroepen van de groep weergeven en beheren. Zie voor instructies [Subgroepleden weergeven en beheren](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## De teams van een groep weergeven en beheren

Wanneer u een groep bekijkt die u in het gebied Groepen beheert, kunt u met teams bekijken en werken verbonden aan de groep of om het even welk van zijn subgroepen.

Zie voor instructies [De teams van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).

## De bedrijven van een groep bekijken en beheren

Wanneer u een groep bekijkt die u in het gebied van Groepen beheert, kunt u met bedrijven bekijken en werken verbonden aan de groep of om het even welk van zijn subgroepen. Zie voor instructies [Bedrijven van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md).

## De portfolio&#39;s en programma&#39;s van een groep weergeven en beheren

Wanneer u een groep bekijkt die u in het gebied Groepen beheert, kunt u portefeuilles en programma&#39;s bekijken en werken wanneer allebei van het volgende waar is:

* Ze zijn gekoppeld aan de groep die u bekijkt of een van de subgroepen ervan
* U hebt machtigingen om deze weer te geven omdat u ze hebt gemaakt of omdat ze met u zijn gedeeld

Zie voor instructies [Projecten van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md) en [De programma&#39;s van een groep maken, wijzigen en weergeven](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md).

## Een groep deactiveren of opnieuw activeren

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

U kunt een groep in zijn standaard actieve staat houden of het deactiveren.

Het deactiveren van een groep kan handig zijn wanneer deze momenteel niet wordt gebruikt, omdat gebruikers deze niet meer zien in &#39;type-ahead&#39;-velden wanneer ze zoeken naar een groep die ze aan een ander object willen koppelen.

Voor instructies over het inactief of actief maken van een groep raadpleegt u [Een groep deactiveren of opnieuw activeren](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).
