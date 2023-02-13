---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Een groep deactiveren of opnieuw activeren
description: U kunt een groep deactiveren die u beheert en die u niet meer gebruikt.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 0%

---

# Een groep deactiveren of opnieuw activeren

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

U kunt een groep deactiveren die u beheert en die u niet meer gebruikt.

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

## Een groep deactiveren of opnieuw activeren

>[!IMPORTANT]
>
>Wanneer u een groep deactiveert, worden ook de onderliggende subgroepen gedeactiveerd.
>
>Als u een van deze programma&#39;s opnieuw moet activeren, kunt u dit doen nadat u een van de volgende handelingen hebt uitgevoerd:
>
>* Verwijder het uit de bovenliggende groep. Zie de sectie voor meer informatie [Een subgroep verwijderen uit de bovenliggende groep en deze maken tot een groep op hoofdniveau](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) in het artikel [Een subgroep beheren](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* Verplaats het onder een actieve groep. Zie de sectie voor meer informatie [Een subgroep maken, verplaatsen, weergeven, bewerken, kopiëren, hernoemen, exporteren of verwijderen](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) in het artikel [Een subgroep beheren](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>


1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Selecteer in het linkerdeelvenster de optie **Groepen**.

   In de lijst die wordt weergegeven, ziet u de groepen die u beheert, samen met eventuele subgroepen die u beheert. Adobe Workfront-beheerders kunnen alle groepen zien.

1. Klik op de naam van de groep om de pagina te openen.

1. Klik op het menu Meer ![](assets/more-icon.png) naast de naam van de groep klikt u op **Deactiveren** of **Opnieuw activeren**.

   >[!NOTE]
   >
   >De optie Is actief (optie Opnieuw activeren in Voorvertoning) is niet beschikbaar als de groep een subgroep van een gedeactiveerde groep is. Voordat u de toepassing opnieuw kunt activeren, moet u deze uit de bovenliggende groep verwijderen of verplaatsen naar een actieve groep, zoals in de notitie hierboven wordt beschreven.

1. (Voorwaardelijk) Als u de groep deactiveert, klikt u op **Deactiveren** in de **Groep deactiveren** weergegeven.

## Overwegingen voor inactieve groepen

Overweeg het volgende over een groep die u door onbruikbaar te maken is Actieve optie in de sectie wordt verklaard die [Een groep deactiveren of opnieuw activeren](#View) in dit artikel.

* Als u een groep deactiveert, worden ook alle onderliggende subgroepen gedeactiveerd. Dit geldt ook voor subgroepen die u toevoegt nadat u de toepassing hebt gedeactiveerd.

   Voor informatie over het opnieuw activeren van een subgroep in deze situatie, zie [Subgroepen opnieuw activeren onder een niet-actieve bovenliggende groep](#about-reactivating-a-subgroup-below-an-inactive-parent-group) in dit artikel.

* Wanneer u naar het gebied van Groepen in Opstelling gaat, kunt u slechts actieve groepen in de lijst zien omdat Actief de standaardfilter is ![](assets/filter-nwepng.png) daarvoor. Als u alle groepen wilt zien die u beheert, inclusief de niet-actieve groepen, kunt u het filter Alles gebruiken. U kunt ook het filter Inactief gebruiken om alleen de inactieve filters weer te geven.

   Zie voor meer informatie over filters in lijsten [Overzicht van filters in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Als u een groep deactiveert, verandert het volgende niet:

   * De groepskoppelingen naar objecten. Gekoppelde objecten blijven functioneren zoals voorheen, zonder wijzigingen.

      Als een project bijvoorbeeld is gekoppeld aan een groep die u deactiveert, blijft het project de voorkeuren en status van de groep gebruiken zonder wijzigingen.

   * Uw capaciteit om een nieuw voorwerp, zoals een goedkeuring, een team, of een bedrijf, van binnen de pagina van de groep in opstelling tot stand te brengen. Standaard is het nieuwe object gekoppeld aan de inactieve groep.
   * Uw capaciteit, als beheerder, om de groep in filters en rapportering te vinden.

      U kunt het in groepstype-vooruit gebieden ook vinden waar u de montages van de groep in het gebied van de Opstelling zou kunnen willen beheren. Dit zijn onder andere de gebieden Voorkeuren, Gebeurtenismeldingen en Systeemlicenties.

      Bijvoorbeeld, als u naar Opstelling > de Voorkeur van het Project > Projecten gaat en het type-vooruit gebied boven de opties daar ontruimt, kunt u nog een inactieve groep vinden en zijn projectvoorkeur vormen.

## Subgroepen opnieuw activeren onder een niet-actieve bovenliggende groep {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

Als u een groep deactiveert, worden ook alle onderliggende subgroepen gedeactiveerd. Als u een van de subgroepen opnieuw moet activeren onder een niet-actieve groep, kunt u een van de volgende twee handelingen uitvoeren:

* Verplaats de subgroep onder een actieve groep. Schakel vervolgens de optie Is actief in voor de verplaatste groep, zoals in de sectie wordt uitgelegd [Een groep deactiveren of opnieuw activeren](#View) in dit artikel.

   Voor instructies over het verplaatsen van een groep raadpleegt u [Een groep verplaatsen](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* Verwijder de subgroep uit de bovenliggende groep (die van de subgroep een groep op hoofdniveau maakt). Schakel vervolgens de optie Is actief in voor de verplaatste groep, zoals in de sectie wordt uitgelegd [Een groep deactiveren of opnieuw activeren](#View) in dit artikel.

   Zie de sectie voor instructies over het verwijderen van een subgroep uit de bovenliggende groep [Een subgroep verwijderen uit de bovenliggende groep en deze maken tot een groep op hoofdniveau](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) in het artikel [Een subgroep beheren](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
