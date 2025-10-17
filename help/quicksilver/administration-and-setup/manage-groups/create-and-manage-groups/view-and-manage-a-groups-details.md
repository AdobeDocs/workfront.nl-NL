---
title: De details van een groep weergeven en beheren
description: U kunt de pagina Groepdetails weergeven en bewerken voor een groep of subgroep die u beheert.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: edd2c58a-f912-4638-b6a3-ff3b1b622f48
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# De details van een groep weergeven en beheren

U kunt de pagina Groepdetails weergeven en bewerken voor een groep of subgroep die u beheert. Deze pagina bevat:

* Een beschrijving van de groep
* De namen van de bedrijfsleider en groepsbeheerders
* Een optie waarmee u de groep en de subgroepen ervan openbaar of privé kunt maken

Voor informatie over andere manieren kunt u een groep beheren, zie [ een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) creëren.

Voor informatie over hoe u een groep kunt deactiveren of reactiveren, zie [ een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md) deactiveren of reactiveren.

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
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>U moet een groepsbeheerder van de groep of een systeembeheerder zijn.</td>
  </tr>
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## De details van een groep weergeven en beheren

{{step-1-to-setup}}

1. Klik **Groepen**.

   In de lijst die wordt weergegeven, ziet u de groepen die u beheert, samen met eventuele subgroepen die u beheert. Adobe Workfront-beheerders kunnen alle groepen zien.

1. Klik op de naam van de bovenste groep die u wilt bewerken.
1. Als u de groep wilt deactiveren of opnieuw activeren,
1. In het linkermenu, klik **Details van de Groep**, dan doe om het even welke volgend:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Beschrijving</td> 
      <td> <p>U kunt maximaal 512 tekens typen.</p> <p>Als het gebied leeg is, voegt de klik <strong> </strong> toe om een beschrijving te typen.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Is actief</td> 
      <td> <p>(Wordt standaard ingeschakeld) Hiermee maakt u de groep actief in uw Workfront-instantie.</p> <p>In typevelden zoals hieronder weergegeven, worden alleen actieve groepen weergegeven in de lijst wanneer gewone gebruikers naar een groep zoeken om deze aan een object te koppelen of om er een object mee te delen.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Om dit voor uw gebruikers te stroomlijnen, kunt u de optie Is Actief voor groepen onbruikbaar maken die momenteel niet in gebruik zijn.</p> <p>Met dit veld kunt u de lijst Groepen op basis van de actieve of inactieve status eenvoudig weergeven, filteren en groeperen. Voor informatie over het gebruiken van meningen, filters, en groeperingen in lijsten, zie <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref"> Meldend elementen: filters, meningen, en groeperingen </a>.</p> <p>Voor informatie over inactieve groepen, zie de sectie <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md#inactive" class="MCXref xref"> Overwegingen voor inactieve groepen </a> in het artikel <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md" class="MCXref xref"> Schrapping of deactiveer een douanevorm </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Groepstoegankelijkheid</td> 
      <td> <p>(Alleen beschikbaar als u Details voor een groep bekijkt, niet voor een subgroep.) Laat of maak de optie <strong> toe onbruikbaar maken deze groep en subgroepen privé </strong>.</p> <p>Voor een openbare groep kan elke gebruiker (in of uit de groep) die toegang heeft tot een gebruiker met bewerkingen de groep toevoegen aan het profiel van andere gebruikers. Ze kunnen dit niet doen voor een privégroep.</p> <p>U kunt deze optie alleen bewerken in de bovenste bovenliggende groep in een hiërarchie van groepen met meer dan één niveau. Alle subgroepen van de bovenliggende groep nemen de instelling over.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Groepbelanghebbenden</td> 
      <td> 
       <ul> 
        <li><strong> Beheerders van de Groep </strong>: Voeg of verwijder gebruikers met een vergunning van de Planner als groepsbeheerders voor de groep toe. Typ de naam van een gebruiker en klik vervolgens op de naam wanneer deze wordt weergegeven in het keuzemenu.</li> 
        <li><strong> BedrijfsLeader </strong>: Voer één van het volgende te doen:
         <ul>
          <li>Als u nog geen BedrijfsLeader voor de groep hebt toegewezen, <strong> voegt toe </strong>, begint de naam van de gebruiker te typen u wilt toewijzen, dan de naam van de persoon klikken wanneer het verschijnt.</li>
          <li>Als de groep al een Business Leader heeft en u deze wilt wijzigen, dubbelklikt u op de naam van de bestaande Business Leader. Verwijder de naam, typ de naam van de gebruiker die u wilt toewijzen en klik vervolgens op de naam van de persoon wanneer deze wordt weergegeven.</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aangepast formulier toevoegen</td> 
      <td>Als u met uw toegangsniveau aangepaste formulieren kunt beheren, voegt u een aangepast formulier toe aan de groep. Voor meer informatie, zie <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref"> de vormen van de Douane </a>.</td> 
     </tr> 
    </tbody> 
   </table>
