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
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# Een groep deactiveren of opnieuw activeren

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

U kunt een groep deactiveren die u beheert en die u niet meer gebruikt.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>U moet een groepsbeheerder van de groep of een systeembeheerder zijn.</td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een groep deactiveren of opnieuw activeren

>[!IMPORTANT]
>
>Wanneer u een groep deactiveert, worden ook de onderliggende subgroepen gedeactiveerd.
>
>Als u een van deze programma&#39;s opnieuw moet activeren, kunt u dit doen nadat u een van de volgende handelingen hebt uitgevoerd:
>
>* Verwijder het uit de bovenliggende groep. Voor meer informatie, zie de sectie [&#x200B; een subgroep van zijn oudergroep verwijderen en het maken een top-level groep &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) in het artikel [&#x200B; beheren een subgroep &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* Verplaats het onder een actieve groep. Voor meer informatie, zie de sectie [&#x200B; creëren, bewegen, bekijken, uitgeven, exemplaar, anders noemen, uitvoeren of schrappen subgroup &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) in artikel [&#x200B; een subgroup &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md) beheert.

{{step-1-to-setup}}

1. In het linkerpaneel, uitgezochte **Groepen**.

   In de lijst die wordt weergegeven, ziet u de groepen die u beheert, samen met eventuele subgroepen die u beheert. Adobe Workfront-beheerders kunnen alle groepen zien.

1. Klik op de naam van de groep om de pagina te openen.

1. Klik het Meer menu ![&#x200B; Meer pictogram &#x200B;](assets/more-icon.png) naast de naam van de groep, dan klik **Deactivate** of **Reactivate**.

   >[!NOTE]
   >
   >De optie Is actief (optie Opnieuw activeren in Voorvertoning) is niet beschikbaar als de groep een subgroep van een gedeactiveerde groep is. Voordat u de toepassing opnieuw kunt activeren, moet u deze uit de bovenliggende groep verwijderen of verplaatsen naar een actieve groep, zoals in de notitie hierboven wordt beschreven.

1. (Voorwaardelijk) als u de groep deactiveert, klik **&#x200B;**&#x200B;deactivate in **&#x200B;**&#x200B;doos van de Deactiveer groep die toont.

## Overwegingen voor inactieve groepen

Overweeg het volgende over een groep die u door de Is Actieve optie onbruikbaar te maken die in de sectie [&#x200B; wordt verklaard een groep &#x200B;](#View) in dit artikel deactiveren of reactiveert.

* Als u een groep deactiveert, worden ook alle onderliggende subgroepen gedeactiveerd. Dit geldt ook voor subgroepen die u toevoegt nadat u de toepassing hebt gedeactiveerd.

  Voor informatie over het opnieuw activeren van een subgroep in deze situatie, zie [&#x200B; Ongeveer het opnieuw activeren van een subgroep onder een inactieve oudergroep &#x200B;](#about-reactivating-a-subgroup-below-an-inactive-parent-group) in dit artikel.

* Wanneer u naar het gebied van Groepen in Opstelling gaat, kunt u slechts actieve groepen in de lijst zien omdat Actief het standaardfilter ![&#x200B; pictogram van de Filter &#x200B;](assets/filter-nwepng.png) voor het is. Als u alle groepen wilt zien die u beheert, inclusief de niet-actieve groepen, kunt u het filter Alles gebruiken. U kunt ook het filter Inactief gebruiken om alleen de inactieve filters weer te geven.

  Voor meer informatie over filters in lijsten, zie [&#x200B; Overzicht van Filters &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Als u een groep deactiveert, verandert het volgende niet:

   * De groepskoppelingen naar objecten. Gekoppelde objecten blijven functioneren zoals voorheen, zonder wijzigingen.

     Als een project bijvoorbeeld is gekoppeld aan een groep die u deactiveert, blijft het project de voorkeuren en status van de groep gebruiken zonder wijzigingen.

   * Uw capaciteit om een nieuw voorwerp, zoals een goedkeuring, een team, of een bedrijf, van binnen de pagina van de groep in opstelling tot stand te brengen. Standaard is het nieuwe object gekoppeld aan de inactieve groep.
   * Uw capaciteit, als beheerder, om de groep in filters en rapportering te vinden.

     U kunt het in groepstype-vooruit gebieden ook vinden waar u de montages van de groep in het gebied van de Opstelling zou kunnen willen beheren. Dit zijn onder andere de gebieden Voorkeuren, Gebeurtenismeldingen en Systeemlicenties.

     Bijvoorbeeld, als u naar Opstelling > de Voorkeur van het Project > Projecten gaat en het type-vooruit gebied boven de opties daar ontruimt, kunt u nog een inactieve groep vinden en zijn projectvoorkeur vormen.

## Subgroepen opnieuw activeren onder een niet-actieve bovenliggende groep {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

Als u een groep deactiveert, worden ook alle onderliggende subgroepen gedeactiveerd. Als u een van de subgroepen opnieuw moet activeren onder een niet-actieve groep, kunt u een van de volgende twee handelingen uitvoeren:

* Verplaats de subgroep onder een actieve groep. Dan laat zijn Actieve optie voor de verplaatste groep toe, zoals die in de sectie [&#x200B; wordt verklaard een groep &#x200B;](#View) in dit artikel deactiveren of opnieuw activeren.

  Voor instructies bij het bewegen van een groep, zie [&#x200B; een groep &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md) bewegen.

* Verwijder de subgroep uit de bovenliggende groep (die van de subgroep een bovenste groep maakt). Dan laat zijn Actieve optie voor de verplaatste groep toe, zoals die in de sectie [&#x200B; wordt verklaard een groep &#x200B;](#View) in dit artikel deactiveren of opnieuw activeren.

  Voor instructies bij het verwijderen van een subgroep uit zijn oudergroep, zie de sectie [&#x200B; een subgroep uit zijn oudergroep verwijderen en het maken een top-level groep &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) in het artikel [&#x200B; een subgroep &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md) beheren.
