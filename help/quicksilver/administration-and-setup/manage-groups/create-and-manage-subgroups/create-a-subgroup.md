---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: Een subgroep maken
description: U kunt een subgroep maken onder een groep die u beheert om gebruikers en projecten te organiseren en toegangsrechten toe te wijzen in Adobe Workfront. Groepbeheerders beheren doorgaans groepen en subgroepen. Ze kunnen de pagina Groepen gebruiken om hun groepen en subgroepen op één locatie te beheren.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# Een subgroep maken

U kunt een subgroep maken onder een groep die u beheert om gebruikers en projecten te organiseren en toegangsrechten toe te wijzen in Adobe Workfront.

Als er groepen zijn boven de groep die u beheert, kunnen hun beheerders dit ook voor uw groep doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

Groepbeheerders beheren doorgaans echter groepen en subgroepen. Ze kunnen de pagina Groepen gebruiken om hun groepen en subgroepen op één locatie te beheren. Voor informatie over hoe groepen en subgroepen binnen Workfront werken, raadpleegt u [Overzicht van groepen](../../../administration-and-setup/manage-groups/groups-overview/groups.md) en [Overzicht subgroepen](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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

## Een subgroep toevoegen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Groepen**.

   In de lijst die wordt weergegeven, ziet u de groepen die u beheert, samen met eventuele subgroepen die u beheert. Adobe Workfront-beheerders kunnen alle groepen zien.

1. Selecteer de bestaande groep of subgroep waaraan u een nieuwe subgroep wilt toevoegen.
1. Klikken **Nieuwe subgroep**.
1. In de **Nieuwe subgroep** vak dat wordt weergegeven, typt u een **Groepsnaam** voor de subgroep.
1. (Optioneel) Geef een of meer van de volgende gegevens op:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Groepsnaam</td> 
      <td>Wijzig de naam van de groep.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschrijving</td> 
      <td>Typ een beschrijving voor de subgroep. U kunt maximaal 512 tekens typen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Is actief</td> 
      <td> <p>(Wordt standaard ingeschakeld) Hiermee maakt u de groep actief in uw Workfront-instantie.</p> <p>In typevelden zoals hieronder weergegeven, worden alleen actieve groepen weergegeven in de lijst wanneer gewone gebruikers naar een groep zoeken om deze aan een object te koppelen of om er een object mee te delen.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Om dit voor uw gebruikers te stroomlijnen, kunt u de optie Is Actief voor groepen onbruikbaar maken die momenteel niet in gebruik zijn.</p> <p>Met dit veld kunt u de lijst Groepen op basis van de actieve of inactieve status eenvoudig weergeven, filteren en groeperen. Voor informatie over het gebruik van weergaven, filters en groepen in lijsten raadpleegt u <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Elementen rapporteren: filters, weergaven en groepen</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Deze groep en de bijbehorende subgroepen openbaar maken</td> 
      <td> <p>(Alleen beschikbaar als u Details bekijkt voor een groep op hoofdniveau, niet voor een subgroep.) Schakel deze optie in als u wilt dat gebruikers in de subgroep met bewerkingsgebruikerstoegang (die geen beheerders van de groep zijn) deze groep en de subgroepen ervan kunnen toevoegen aan het gebruikersprofiel van andere gebruikers.</p> <p>Voor een openbare groep kan elke gebruiker (in of uit de groep) die toegang heeft tot een gebruiker met bewerkingen de groep toevoegen aan het profiel van andere gebruikers. Ze kunnen dit niet doen voor een privégroep.</p> <p>U kunt deze optie alleen bewerken in de bovenste bovenliggende groep in een hiërarchie van groepen met meer dan één niveau. Alle subgroepen van de bovenliggende groep nemen de instelling over.</p> <p><b>OPMERKING</b>:  
        <ul> 
         <li>U kunt een subgroep niet openbaar maken op zich, maar u kunt het de oudergroep op hoofdniveau openbaar maken, die ook alle subgroepen van de ouder openbaar maakt.</li> 
         <li>Een subgroep die tot een openbare groep behoort is door gebrek openbaar, zodat om het even welke gebruiker met uitgeven-gebruiker toegang de subgroep aan andere gebruikers kan toevoegen, eveneens.</li> 
        </ul> </p> <p>Als u informatie nodig hebt over de toegang die nodig is om gebruikers te bewerken, raadpleegt u <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Toegang verlenen aan gebruikers</a>. Voor informatie over het bewerken van gebruikers raadpleegt u <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Gebruikersprofiel bewerken</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bedrijfsleider </td> 
      <td> <p>U kunt één gebruiker toewijzen als bedrijfsleider voor een subgroep die u beheert. Een bedrijfsleider is iemand die bedrijfsbesluiten voor subgroup neemt. Zie voor meer informatie <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Overzicht van Business Leader</a><span>.</span></p> <p>Als de persoon nog geen lid is van de subgroep en de naam aan dit veld toevoegt, worden de personen ook aan de groep toegevoegd.</p> <p><b>OPMERKING</b>:  
        <ul> 
         <li>Voordat u de Business Leader uit een subgroep kunt verwijderen, moet u de naam uit het veld Business Leader verwijderen.</li> 
         <li>Als u de naam uit het veld Bedrijfsleider verwijdert, blijft die gebruiker lid van de subgroep, tenzij u deze verwijdert. Zie de sectie voor instructies over het verwijderen van iemand uit een groep <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">De groepslidmaatschappen beheren</a> in het artikel <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Een groep beheren</a>.</li> 
        </ul> </p> <p>Zie voor meer informatie <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Overzicht van Business Leader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Groepsleden en groepbeheerders</td> 
      <td> 
       <ul> 
        <li> <p>Groepsleden: Als u gebruikers en groepen aan de subgroep wilt toevoegen, typt u de naam van een bestaande gebruiker of groep die u wilt toevoegen en selecteert u de naam wanneer deze wordt weergegeven.</p> <p>De gebruikers en groepen die u toevoegt, hebben toegang tot alle objecten die met de groep worden gedeeld.</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.subgroups">Groepbeheerders: Een subgroep erft de groepsbeheerders van de groep erboven, zodat is het specificeren van een gebruiker als groepsbeheerder voor een subgroep facultatief. U kunt een groepslid als beheerder voor de groep toewijzen gebruikend het drop-down menu rechts van de naam van de gebruiker.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Personen en groepen in de lijst zoeken</td> 
      <td> Als u een gebruiker of een groep moet vinden die reeds aan deze subgroep wordt toegewezen, kunt u hun naam hier typen en het selecteren wanneer het verschijnt.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Opslaan.**
