---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: Een subgroep maken
description: U kunt een subgroep maken onder een groep die u beheert om gebruikers en projecten te organiseren en toegangsrechten toe te wijzen in Adobe Workfront. Groepbeheerders beheren doorgaans groepen en subgroepen. Ze kunnen de pagina Groepen gebruiken om hun groepen en subgroepen op één locatie te beheren.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: 008f96d52632f5f05554d63ae1c38cc37d21544b
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 0%

---

# Een subgroep maken

U kunt een subgroep maken onder een groep die u beheert om gebruikers en projecten te organiseren en toegangsrechten toe te wijzen in Adobe Workfront.

Als er groepen zijn boven de groep die u beheert, kunnen hun beheerders dit ook voor uw groep doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

Groepbeheerders beheren doorgaans echter groepen en subgroepen. Ze kunnen de pagina Groepen gebruiken om hun groepen en subgroepen op één locatie te beheren. Voor informatie over hoe de groepen en de subgroepen binnen Workfront werken, zie [ Overzicht van Groepen ](../../../administration-and-setup/manage-groups/groups-overview/groups.md) en [ Subgroups overzicht ](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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

## Een subgroep toevoegen

{{step-1-to-setup}}

1. Klik **Groepen**.

   In de lijst die wordt weergegeven, ziet u de groepen die u beheert, samen met eventuele subgroepen die u beheert. Adobe Workfront-beheerders kunnen alle groepen zien.

1. Selecteer de bestaande groep of subgroep waaraan u een nieuwe subgroep wilt toevoegen.
1. Klik **Nieuwe Subgroup**.
1. In **Nieuwe Subgroup** doos die verschijnt, typ de naam van de a **Groep** voor subgroup.
1. (Optioneel) Voer een van de volgende gegevens in:

   * **Beschrijving**: Type een beschrijving voor subgroup. U kunt maximaal 512 tekens typen.
   * **is Actief**: Deze optie wordt toegelaten door gebrek en maakt de groep actief in uw instantie van Workfront.

     In tekstkopvelden zoals de hieronder weergegeven velden, worden alleen actieve groepen weergegeven in de lijst als gewone gebruikers naar een groep zoeken om deze aan een object te koppelen of om er een object mee te delen.

     ![ gebied Typeahead voor een groep ](assets/typeahead-for-group.png)

     Om dit voor uw gebruikers te stroomlijnen, kunt u **onbruikbaar maken is Actieve** optie voor groepen die momenteel niet in gebruik zijn.

     Met dit veld kunt u de lijst Groepen op basis van de actieve of inactieve status eenvoudig weergeven, filteren en groeperen. Voor informatie over het gebruiken van meningen, filters, en groeperingen in lijsten, zie [ Meldend elementen: filters, meningen, en groeperingen ](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   * **BedrijfsLeader**: U kunt één gebruiker als BedrijfsLeader voor een subgroep toewijzen die u beheert. Een bedrijfsleider is iemand die bedrijfsbesluiten voor subgroup neemt. Voor meer informatie, zie [ Overzicht BedrijfsLeader ](/help/quicksilver/administration-and-setup/manage-groups/group-roles/business-leader-overview.md).

     Als de persoon nog geen lid is van de subgroep en de naam aan dit veld toevoegt, worden de personen ook aan de groep toegevoegd.

     >[!NOTE]
     >
     >* Voordat u de Business Leader uit een subgroep kunt verwijderen, moet u de naam uit het veld Business Leader verwijderen.
     >* Als u de naam uit het veld Bedrijfsleider verwijdert, blijft die gebruiker lid van de subgroep, tenzij u deze verwijdert. Voor instructies bij het verwijderen van iemand uit een groep, zie [ Mening en beheer het lidmaatschap van een groep ](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

   * **de leden van de Groep en de beheerders van de Groep**: Om gebruikers en groepen als leden van subgroup toe te voegen, begin de naam van een bestaande gebruiker of een groep te typen u, dan de naam wilt toevoegen wanneer het verschijnt.

     De gebruikers en groepen die u toevoegt, hebben toegang tot alle objecten die met de groep worden gedeeld.

     Een subgroep erft de groepsbeheerders van de groep erboven, zodat is het specificeren van een gebruiker als groepsbeheerder voor een subgroep facultatief. U kunt een groepslid als beheerder voor de groep toewijzen gebruikend het drop-down menu rechts van de naam van de gebruiker.

   * **de mensen en de groepen van het Onderzoek in de lijst**: Als u een gebruiker of een groep moet vinden die reeds aan deze subgroep wordt toegewezen, kunt u hun naam hier typen en het selecteren wanneer het verschijnt.

1. Klik **sparen.**
