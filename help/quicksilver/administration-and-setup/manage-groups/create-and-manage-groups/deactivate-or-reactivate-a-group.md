---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Groep deactiveren of opnieuw activeren
description: U kunt een groep deactiveren die u beheert en die u niet meer gebruikt.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---

# Een groep deactiveren of opnieuw activeren

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

U kunt een groep deactiveren die u beheert en die u niet meer gebruikt.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <td> <p>Plan </p> <p>U moet een groepsbeheerder van de groep of een beheerder van Workfront zijn. Voor meer informatie, zie <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref"> de beheerders van de Groep </a> en <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> verlenen een gebruiker volledige administratieve toegang </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; als u moet weten welk plan of licentietype u hebt, contacteer uw beheerder van Workfront.

+++

## Een groep deactiveren of opnieuw activeren

>[!IMPORTANT]
>
>Wanneer u een groep deactiveert, worden ook de onderliggende subgroepen gedeactiveerd.
>
>Als u een van deze programma&#39;s opnieuw moet activeren, kunt u dit doen nadat u een van de volgende handelingen hebt uitgevoerd:
>
>* Verwijder het uit de bovenliggende groep. Voor meer informatie, zie de sectie [ een subgroep van zijn oudergroep verwijderen en het maken een top-level groep ](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) in het artikel [ beheren een subgroep ](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* Verplaats het onder een actieve groep. Voor meer informatie, zie de sectie [ creëren, bewegen, bekijken, uitgeven, exemplaar, anders noemen, uitvoeren of schrappen subgroup ](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) in artikel [ een subgroup ](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md) beheert.

{{step-1-to-setup}}

1. In het linkerpaneel, uitgezochte **Groepen**.

   In de lijst die wordt weergegeven, ziet u de groepen die u beheert, samen met eventuele subgroepen die u beheert. Adobe Workfront-beheerders kunnen alle groepen zien.

1. Klik op de naam van de groep om de pagina te openen.

1. Klik het Meer menu ![](assets/more-icon.png) naast de naam van de groep, dan klik **Deactivate** of **Reactivate**.

   >[!NOTE]
   >
   >De optie Is actief (optie Opnieuw activeren in Voorvertoning) is niet beschikbaar als de groep een subgroep van een gedeactiveerde groep is. Voordat u de toepassing opnieuw kunt activeren, moet u deze uit de bovenliggende groep verwijderen of verplaatsen naar een actieve groep, zoals in de notitie hierboven wordt beschreven.

1. (Voorwaardelijk) als u de groep deactiveert, klik **** deactivate in **** doos van de Deactiveer groep die toont.

## Overwegingen voor inactieve groepen

Overweeg het volgende over een groep die u door de Is Actieve optie onbruikbaar te maken die in de sectie [ wordt verklaard een groep ](#View) in dit artikel deactiveren of reactiveert.

* Als u een groep deactiveert, worden ook alle onderliggende subgroepen gedeactiveerd. Dit geldt ook voor subgroepen die u toevoegt nadat u de toepassing hebt gedeactiveerd.

  Voor informatie over het opnieuw activeren van een subgroep in deze situatie, zie [ Ongeveer het opnieuw activeren van een subgroep onder een inactieve oudergroep ](#about-reactivating-a-subgroup-below-an-inactive-parent-group) in dit artikel.

* Wanneer u naar het gebied Groepen in Opstelling gaat, kunt u slechts actieve groepen in de lijst zien omdat Actief het standaardfilter ![](assets/filter-nwepng.png) voor het is. Als u alle groepen wilt zien die u beheert, inclusief de niet-actieve groepen, kunt u het filter Alles gebruiken. U kunt ook het filter Inactief gebruiken om alleen de inactieve filters weer te geven.

  Voor meer informatie over filters in lijsten, zie [ Overzicht van Filters ](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Als u een groep deactiveert, verandert het volgende niet:

   * De groepskoppelingen naar objecten. Gekoppelde objecten blijven functioneren zoals voorheen, zonder wijzigingen.

     Als een project bijvoorbeeld is gekoppeld aan een groep die u deactiveert, blijft het project de voorkeuren en status van de groep gebruiken zonder wijzigingen.

   * Uw capaciteit om een nieuw voorwerp, zoals een goedkeuring, een team, of een bedrijf, van binnen de pagina van de groep in opstelling tot stand te brengen. Standaard is het nieuwe object gekoppeld aan de inactieve groep.
   * Uw capaciteit, als beheerder, om de groep in filters en rapportering te vinden.

     U kunt het in groepstype-vooruit gebieden ook vinden waar u de montages van de groep in het gebied van de Opstelling zou kunnen willen beheren. Dit zijn onder andere de gebieden Voorkeuren, Gebeurtenismeldingen en Systeemlicenties.

     Bijvoorbeeld, als u naar Opstelling > de Voorkeur van het Project > Projecten gaat en het type-vooruit gebied boven de opties daar ontruimt, kunt u nog een inactieve groep vinden en zijn projectvoorkeur vormen.

## Subgroepen opnieuw activeren onder een niet-actieve bovenliggende groep {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

Als u een groep deactiveert, worden ook alle onderliggende subgroepen gedeactiveerd. Als u een van de subgroepen opnieuw moet activeren onder een niet-actieve groep, kunt u een van de volgende twee handelingen uitvoeren:

* Verplaats de subgroep onder een actieve groep. Dan laat zijn Actieve optie voor de verplaatste groep toe, zoals die in de sectie [ wordt verklaard een groep ](#View) in dit artikel deactiveren of opnieuw activeren.

  Voor instructies bij het bewegen van een groep, zie [ een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md) bewegen.

* Verwijder de subgroep uit de bovenliggende groep (die van de subgroep een bovenste groep maakt). Dan laat zijn Actieve optie voor de verplaatste groep toe, zoals die in de sectie [ wordt verklaard een groep ](#View) in dit artikel deactiveren of opnieuw activeren.

  Voor instructies bij het verwijderen van een subgroep uit zijn oudergroep, zie de sectie [ een subgroep uit zijn oudergroep verwijderen en het maken een top-level groep ](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) in het artikel [ een subgroep ](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md) beheren.
