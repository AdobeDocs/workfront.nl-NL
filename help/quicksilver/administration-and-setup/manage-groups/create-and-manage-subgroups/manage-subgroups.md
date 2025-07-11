---
user-type: administrator
product-area: system-administration;user-management
keywords: beheren,subgroep,bewerken
navigation-topic: create-and-manage-subgroups
title: Een subgroep beheren
description: Als groepsbeheerder van een subgroep kunt u de subgroep maken, verplaatsen, weergeven, bewerken, kopiëren, hernoemen, exporteren en verwijderen. U kunt een subgroep ook tot een groep op hoofdniveau maken door deze uit de bovenliggende groep te verwijderen.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: 6c3f5ee43040f81dac734c5e0b4def9021a0d737
workflow-type: tm+mt
source-wordcount: '1409'
ht-degree: 0%

---

# Een subgroep beheren

Als groepsbeheerder van een subgroep kunt u de subgroep maken, verplaatsen, weergeven, bewerken, kopiëren, hernoemen, exporteren en verwijderen.

U kunt een subgroep ook tot een groep op hoofdniveau maken door deze uit de bovenliggende groep te verwijderen.

Als er om het even welke groepen boven uw groep zijn, kunnen hun beheerders deze dingen voor uw groep ook doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

Voor meer informatie over subgroepen, zie [ Overzicht Subgroups ](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

>[!TIP]
>
>Wanneer u een groep beheert die subgroepen bevat, is het nuttig om gegevens over de gehele groep en alle subgroepen te kunnen identificeren en filteren. U kunt dit doen door het Bovenste gebied van identiteitskaart van de Ouder in een rapport of een lijst te gebruiken.
>
>Bijvoorbeeld, veronderstel dat u een grote afdeling van de Marketing beheert en u een lijst van alle projecten wilt die de volledige afdeling aan werkt.
>
>In Workfront, wordt deze afdeling van de Marketing vertegenwoordigd door een groep genoemd Marketing, met 3 subgroepen genoemd de Marketing van het Gebied, de Marketing van het Product, en Digitale Marketing. Om van de projecten een lijst te maken die tot de volledige afdeling van de Marketing (alle 4 groepen) behoren, kon u een filter voor het gebied van Projecten met de volgende filterregel tot stand brengen:
>
>`Group: Top Parent ID > Equal > Marketing`
>
>U kunt het Bovenste gebied van de Naam van de Ouder ook gebruiken om gegevens te identificeren verbonden aan een top-level groep, maar slechts in meningen, niet in filters of groepen.

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

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een subgroep maken

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen** ![ Groepen ](assets/groups-icon.png).

   In de lijst die wordt weergegeven, ziet u de groepen die u beheert, samen met eventuele subgroepen die u beheert. Adobe Workfront-beheerders kunnen alle groepen zien.

1. Klik op de naam van de groep waaraan u een subgroep wilt toevoegen.
1. In het linkermenu, klik **Subgroups**.
1. Om nieuwe subgroup één niveau neer van de groep tot stand te brengen u bekijkt, klik **subgroup** toevoegen.

   Of, als u nieuwe subgroep onder een andere subgroep in de lijst wilt tot stand brengen, selecteer die subgroep, dan klik **subgroep** toevoegen.

   Voor informatie over de opties kunt u gebruiken om subgroup te vormen, zie [ een subgroep ](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md) creëren.

   Een groepshiërarchie kan niet meer dan 15 niveaus zijn, maar één niveau kan een onbeperkt aantal parallelle groepen hebben.

## Een subgroep verplaatsen

U kunt bestaande subgroepen verplaatsen onder een andere groep die u beheert.

Een groepshiërarchie kan niet meer dan 15 niveaus zijn, maar één niveau kan een onbeperkt aantal parallelle groepen hebben.

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen** ![ Groepen ](assets/groups-icon.png).

   In de lijst die wordt weergegeven, ziet u de groepen die u beheert, samen met eventuele subgroepen die u beheert. Adobe Workfront-beheerders kunnen alle groepen zien.

1. Klik op de naam van de doelgroep (u geeft in een latere stap op welke subgroepen u wilt verplaatsen).
1. In het linkermenu, klik **Subgroups**.
1. (Optioneel) Selecteer een subgroep om deze tot de doelgroep te maken.

   Als u deze stap overslaat, is de groep die u in stap 3 hebt geselecteerd de doelgroep.

1. Klik **toevoegen Subgroep > Bestaande Groep**.
1. In het **Bestaande vakje van de Groep** dat verschijnt, begin het typen van de naam van een subgroep u wilt bewegen.

   De resultaten die worden weergegeven, bevatten geen groepen boven de doelgroep.

   U kunt ervoor zorgen u de juiste groep selecteert door over het te hangen en het informatiepictogram ![ informatiepictogram ](assets/info-icon.png) te klikken dat naast het toont. Hier wordt knopinfo weergegeven met informatie over de groep, zoals de hiërarchie van de bovenliggende groepen en de bijbehorende beheerders.

1. Selecteer de naam van de subgroep die u wilt verplaatsen wanneer u deze in de lijst opzoekt.
1. Herhaal stap 7-8 voor alle andere subgroepen die u naar de doelgroep wilt verplaatsen.
1. Klik **sparen**.

## Een subgroep bewerken

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen** ![ Groepen ](assets/groups-icon.png).

   In de lijst die wordt weergegeven, ziet u de groepen die u beheert, samen met eventuele subgroepen die u beheert. Adobe Workfront-beheerders kunnen alle groepen zien.

1. Klik op de naam van de groep die de subgroep bevat die u wilt bewerken.
1. In het linkermenu, klik **Subgroups**.
1. Selecteer subgroup u wilt uitgeven, dan **uitgeven** pictogram ![ uitgeven pictogram ](assets/edit-icon.png).

   Voor informatie over de opties kunt u gebruiken om subgroup te vormen, zie [ een subgroep ](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md) creëren.

## Een subgroep kopiëren

>[!NOTE]
>
>Alleen een systeembeheerder kan een subgroep kopiëren.

Wanneer u een subgroep kopieert, wordt deze een bovenliggende groep. Alle groepsleden en subgroepen worden ermee gekopieerd. De leden van de groep behouden hun taken in de oorspronkelijke groep.

Houd rekening met het volgende wanneer u een subgroep kopieert:

* Als een subgroep die u kopieert, zijn eigen subgroepen heeft, worden deze opgenomen in de kopie en krijgen hun namen de volgende notatie:

  `Original subgroup name (Copy)`

* Om het even welke subgroep die tot een openbare groep behoort is ook openbaar, zodat om het even welke gebruiker met toegang om gebruikers, in of uit de groep uit te geven, gebruikers aan subgroup kan toevoegen.

Een subgroep kopiëren:

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen** ![ Groepen ](assets/groups-icon.png).

   In de lijst die wordt weergegeven, ziet u de groepen die u beheert, samen met eventuele subgroepen die u beheert. Adobe Workfront-beheerders kunnen alle groepen zien.

1. Klik op de naam van de groep die de subgroep bevat die u wilt kopiëren.
1. In het linkermenu, klik **Subgroups**.
1. Selecteer een subgroep, dan klik het **pictogram van het Exemplaar** ![ om een nieuwe top-level groep tot stand te brengen die op de geselecteerde groep wordt gebaseerd.](assets/copy-icon.png)
1. Configureer de instellingen van de nieuwe groep.

   Voor hulp met deze montages, zie [ een top-level groep door een bestaande groep of subgroep ](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) in het artikel [ tot stand te brengen creëren een groep ](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

1. Klik **creëren groep**.

## Een subgroep exporteren

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen** ![ Groepen ](assets/groups-icon.png).

   In de lijst die wordt weergegeven, ziet u de groepen die u beheert, samen met eventuele subgroepen die u beheert. Adobe Workfront-beheerders kunnen alle groepen zien.

1. Klik op de naam van de groep die de subgroep bevat die u wilt exporteren.
1. In het linkermenu, klik **Subgroups**.
1. Selecteer de subgroep of subgroepen die u wilt exporteren.
1. Klik het **pictogram van de Uitvoer** het pictogram van de Uitvoer ![, dan selecteer het dossierformaat u wilt.](assets/export.png)

## Een subgroep verwijderen uit de bovenliggende groep en deze maken tot een groep op hoofdniveau

U kunt van een subgroep een groep op hoofdniveau maken door deze uit de bovenliggende groep te verwijderen.

>[!TIP]
>
>Wanneer u een groep deactiveert die onderliggende subgroepen heeft, worden deze subgroepen ook inactief. Als u wilt dat een van deze besturingselementen actief is, kunt u deze instructies gebruiken om het onderdeel uit de bovenliggende groep te verwijderen en vervolgens opnieuw te activeren.
>&#x200B;>Voor instructies bij het deactiveren en het opnieuw activeren van groepen, zie [ een groep ](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md) deactiveren of reactiveren.

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen** ![ Groepen ](assets/groups-icon.png).
1. Selecteer de oudergroep van subgroep u een top-level groep wilt maken, dan klik **uitgeven** pictogram ![ uitgeven pictogram ](assets/edit-icon.png).
1. In **geef groep** doos uit die verschijnt, begin de naam van subgroup die u een top-level groep in het **3&rbrace; gebied van het Onderzoek &lbrace;onder** Groep leden en de beheerders van de Groep **wilt maken, dan klik X aan het recht van zijn naam het wanneer het verschijnt.**
1. Klik **sparen**.

## Een subgroep verwijderen

>[!IMPORTANT]
>
>Wanneer u een groep of subgroep verwijdert, moet u de gebruikers, de werkitems en alle subgroepen die momenteel aan de groep of subgroep zijn toegewezen, behouden. Om ervoor te zorgen dat deze behouden blijven, moet u de objecten van de groep opnieuw toewijzen aan een andere groep.

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen** ![ Groepen ](assets/groups-icon.png).

   In de lijst die wordt weergegeven, ziet u de groepen die u beheert, samen met eventuele subgroepen die u beheert. Adobe Workfront-beheerders kunnen alle groepen zien.

1. Klik op de naam van de groep die de subgroep bevat die u wilt verwijderen.
1. In het linkermenu, klik **Subgroups**.
1. Selecteer subgroup, dan klik het **pictogram van de Schrapping** pictogram van de Schrapping ![.](assets/delete.png)

   In het **vakje van de Groep van de Schrapping** dat verschijnt, begin en selecteer dan de naam van de groep waar u de leden, de werkpunten, en de subgroepen van de groep wilt bewegen u schrapt.

1. Klik **Schrapping het**.

## De subgroepsleden van een groep weergeven en beheren

Wanneer u de hoofdpagina bekijkt van een groep die u beheert, kunt u alle gebruikers in de subgroepen van de groep weergeven en beheren. Voor instructies, zie [ Mening en beheer subgroepsleden ](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

