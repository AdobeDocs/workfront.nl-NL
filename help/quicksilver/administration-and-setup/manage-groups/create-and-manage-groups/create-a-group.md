---
user-type: administrator
product-area: system-administration;user-management
keywords: maken,groep,subgroep,nieuw
navigation-topic: create-and-manage-groups
title: Een groep maken
description: Als Adobe Workfront-beheerder kunt u groepen maken om gebruikers en projecten te organiseren en toegangsrechten toe te wijzen in Workfront.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4a039619-0943-4b5b-ba7a-1ad9b5c11df0
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 0%

---

# Een groep maken

<!--
DON'T DELETE, DRAFT, OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT-SENSITIVE HELP LINKS.
-->

Als Adobe Workfront-beheerder kunt u groepen maken om gebruikers en projecten te organiseren en toegangsrechten toe te wijzen in Workfront. Zie voor meer informatie [Overzicht van groepen](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Elke subgroep heeft minstens één groepsbeheerder nodig. Groepbeheerders kunnen de pagina Groepen gebruiken om hun groepen op één locatie te beheren.

Als u een groepsbeheerder of een Workfront-beheerder bent, kunt u ook subgroepen maken onder een groep. Zie voor instructies [Een subgroep maken](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

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

## Een geheel nieuwe groep op hoofdniveau maken

In deze stappen wordt uitgelegd hoe u een nieuwe groep helemaal zelf kunt maken. Voor informatie over het creëren van een groep of een subgroep door bestaande te kopiëren, zie [Een groep op hoofdniveau maken door een bestaande groep of subgroep te kopiëren](#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) in dit artikel.

U moet een beheerder van Workfront zijn om een top-level groep tot stand te brengen.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Groepen** ![](assets/groups-icon.png).

1. Klik boven de lijst met groepen op **Nieuwe groep**.

   >[!TIP]
   >
   >Onder aan de lijst met groepen kunt u ook op **Meer groepen toevoegen** om een groep online toe te voegen, dan klik **Enter** wanneer u klaar bent met het toevoegen van de groepsgegevens.

1. In de **Nieuwe groep** Typ een naam voor de groep.
1. Geef de volgende informatie op:

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
      <td>Typ een beschrijving voor de groep. U kunt maximaal 512 tekens typen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Is actief</td> 
      <td> <p>(Wordt standaard ingeschakeld) Hiermee maakt u de groep actief in uw Workfront-instantie.</p> <p>In typevelden zoals hieronder weergegeven, worden alleen actieve groepen weergegeven in de lijst wanneer gewone gebruikers naar een groep zoeken om deze aan een object te koppelen of om er een object mee te delen.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Om dit voor uw gebruikers te stroomlijnen, kunt u de optie Is Actief voor groepen onbruikbaar maken die momenteel niet in gebruik zijn.</p> <p>Met dit veld kunt u de lijst Groepen op basis van de actieve of inactieve status eenvoudig weergeven, filteren en groeperen. Voor informatie over het gebruik van weergaven, filters en groepen in lijsten raadpleegt u <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementen rapporteren: filters, weergaven en groepen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Deze groep en de bijbehorende subgroepen openbaar maken</td> 
      <td> <p>(Alleen beschikbaar als u Details bekijkt voor een groep op hoofdniveau, niet voor een subgroep.) Schakel deze optie in als u wilt dat gebruikers in de groep met bewerkingsgebruikerstoegang (die geen beheerders van de groep zijn) deze groep en de subgroepen ervan kunnen toevoegen aan het gebruikersprofiel van andere gebruikers.</p> <p>Voor een openbare groep kan elke gebruiker (in of uit de groep) die toegang heeft tot een gebruiker met bewerkingen de groep toevoegen aan het profiel van andere gebruikers. Ze kunnen dit niet doen voor een privégroep.</p> <p>U kunt deze optie alleen bewerken in de bovenste bovenliggende groep in een hiërarchie van groepen met meer dan één niveau. Alle subgroepen van de bovenliggende groep nemen de instelling over.</p> <p><b>OPMERKING</b>:  
        <ul> 
         <li>U kunt een subgroep niet openbaar maken op zich, maar u kunt het de oudergroep op hoofdniveau openbaar maken, die ook alle subgroepen van de ouder openbaar maakt.</li> 
         <li>Een subgroep die tot een openbare groep behoort is door gebrek openbaar, zodat om het even welke gebruiker met uitgeven-gebruiker toegang de subgroep aan andere gebruikers kan toevoegen, eveneens.</li> 
        </ul> </p> <p>Als u informatie nodig hebt over de toegang die nodig is om gebruikers te bewerken, raadpleegt u <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Toegang verlenen aan gebruikers</a>. Voor informatie over het bewerken van gebruikers raadpleegt u <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Gebruikersprofiel bewerken</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bedrijfsleider </td> 
      <td> <p>U kunt één gebruiker toewijzen als bedrijfsleider voor een groep die u beheert. Een bedrijfsleider is iemand die bedrijfsbesluiten voor de groep neemt. Zie voor meer informatie <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Overzicht van Business Leader</a><span>.</span></p> <p>Als de persoon nog geen lid is van de groep en de naam aan dit veld toevoegt, worden de personen ook aan de groep toegevoegd.</p> <p><b>OPMERKING</b>:  
        <ul> 
         <li>Voordat u de Business Leader uit een groep kunt verwijderen, moet u de naam ervan uit het veld Business Leader verwijderen.</li> 
         <li>Als u de naam uit het veld Bedrijfsleider verwijdert, blijft die gebruiker lid van de groep, tenzij u deze uit de groep verwijdert. Zie de sectie voor instructies over het verwijderen van iemand uit een groep <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">De groepslidmaatschappen beheren</a> in het artikel <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">Een groep beheren</a>.</li> 
        </ul> </p> <p>Zie voor meer informatie <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Overzicht van Business Leader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Groepsleden en groepbeheerders</td> 
      <td> 
       <ul> 
        <p>Als u groepsleden wilt toevoegen, typt u de naam van een bestaande gebruiker of groep die u wilt toevoegen en selecteert u vervolgens de naam wanneer deze wordt weergegeven.</p> 
        <p>Gebruikers en groepen die u toevoegt, hebben toegang tot alle objecten die met de groep worden gedeeld.</p>
        <p>Een top-level groep moet minstens één groepsbeheerder hebben. </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Personen en groepen in de lijst zoeken</td> 
      <td> Als u een gebruiker of groep wilt zoeken die al aan deze groep is toegewezen, kunt u hier hun naam typen en deze selecteren wanneer deze wordt weergegeven.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Groep maken**.

## Een groep op hoofdniveau maken door een bestaande groep of subgroep te kopiëren {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

Als beheerder van Workfront, kunt u een nieuwe top-level groep tot stand brengen door een bestaande groep of subgroep te kopiëren.

Denk aan het volgende wanneer u dit wilt doen:

* Alle leden en alle subgroepen die tot de bestaande groep behoren, worden gekopieerd naar de nieuwe bovenste groep.
* De leden van de gekopieerde groep behouden de toewijzingen die ze in de oorspronkelijke groep hadden. Daarom worden de groepsbeheerders van de originele groep ook aangewezen als groepsbeheerders in de gekopieerde groep.

Een nieuwe bovenste groep maken door een groep of subgroep te kopiëren:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Groepen** ![](assets/groups-icon.png).

   In de lijst die wordt weergegeven, ziet u de groepen die u beheert, samen met eventuele subgroepen die u beheert. Adobe Workfront-beheerders kunnen alle groepen zien.

1. Selecteer de groep die u wilt kopiëren en klik op het pictogram Kopiëren ![](assets/copy-icon.png).
1. In de **Groep kopiëren** vak dat wordt weergegeven, typt u een **Groepsnaam** voor de gekopieerde groep.

1. Geef de volgende informatie op:

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
      <td>Typ een beschrijving voor de groep. U kunt maximaal 512 tekens typen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Is actief</td> 
      <td> <p>(Wordt standaard ingeschakeld) Hiermee maakt u de groep actief in uw Workfront-instantie.</p> <p>In typevelden zoals hieronder weergegeven, worden alleen actieve groepen weergegeven in de lijst wanneer gewone gebruikers naar een groep zoeken om deze aan een object te koppelen of om er een object mee te delen.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Om dit voor uw gebruikers te stroomlijnen, kunt u de optie Is Actief voor groepen onbruikbaar maken die momenteel niet in gebruik zijn.</p> <p>Met dit veld kunt u de lijst Groepen op basis van de actieve of inactieve status eenvoudig weergeven, filteren en groeperen. Voor informatie over het gebruik van weergaven, filters en groepen in lijsten raadpleegt u <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Elementen rapporteren: filters, weergaven en groepen</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Deze groep en de bijbehorende subgroepen openbaar maken</td> 
      <td> <p>(Alleen beschikbaar als u Details bekijkt voor een groep op hoofdniveau, niet voor een subgroep.) Schakel deze optie in als u wilt dat gebruikers in de groep met bewerkingsgebruikerstoegang (die geen beheerders van de groep zijn) deze groep en de subgroepen ervan kunnen toevoegen aan het gebruikersprofiel van andere gebruikers.</p> <p>Voor een openbare groep kan elke gebruiker (in of uit de groep) die toegang heeft tot een gebruiker met bewerkingen de groep toevoegen aan het profiel van andere gebruikers. Ze kunnen dit niet doen voor een privégroep.</p> <p>U kunt deze optie alleen bewerken in de bovenste bovenliggende groep in een hiërarchie van groepen met meer dan één niveau. Alle subgroepen van de bovenliggende groep nemen de instelling over.</p> <p><b>OPMERKING</b>:  
        <ul> 
         <li>U kunt een subgroep niet openbaar maken op zich, maar u kunt het de oudergroep op hoofdniveau openbaar maken, die ook alle subgroepen van de ouder openbaar maakt.</li> 
         <li>Een subgroep die tot een openbare groep behoort is door gebrek openbaar, zodat om het even welke gebruiker met uitgeven-gebruiker toegang de subgroep aan andere gebruikers kan toevoegen, eveneens.</li> 
        </ul> </p> <p>Als u informatie nodig hebt over de toegang die nodig is om gebruikers te bewerken, raadpleegt u <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Toegang verlenen aan gebruikers</a>. Voor informatie over het bewerken van gebruikers raadpleegt u <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Gebruikersprofiel bewerken</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bedrijfsleider </td> 
      <td> <p>U kunt één gebruiker toewijzen als bedrijfsleider voor een groep die u beheert. Een bedrijfsleider is iemand die bedrijfsbesluiten voor de groep neemt. Zie voor meer informatie <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Overzicht van Business Leader</a><span>.</span></p> <p>Als de persoon nog geen lid is van de groep en de naam aan dit veld toevoegt, worden de personen ook aan de groep toegevoegd.</p> <p><b>OPMERKING</b>:  
        <ul> 
         <li>Voordat u de Business Leader uit een groep kunt verwijderen, moet u de naam ervan uit het veld Business Leader verwijderen.</li> 
         <li>Als u de naam uit het veld Bedrijfsleider verwijdert, blijft die gebruiker lid van de groep, tenzij u deze uit de groep verwijdert. Zie de sectie voor instructies over het verwijderen van iemand uit een groep <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">De groepslidmaatschappen beheren</a> in het artikel <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Een groep beheren</a>.</li> 
        </ul> </p> <p>Zie voor meer informatie <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Overzicht van Business Leader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Groepsleden en groepbeheerders</td> 
      <td> 
       <ul> 
        <li> <p>Groepsleden: Als u gebruikers en groepen aan de groep wilt toevoegen, typt u de naam van een bestaande gebruiker of groep die u wilt toevoegen en selecteert u de naam wanneer deze wordt weergegeven.</p> <p>De gebruikers en groepen die u toevoegt, hebben toegang tot alle objecten die met de groep worden gedeeld.</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.copied groups">Groepbeheerders: Om het even welke groepsbeheerders van de originele groep worden ook aangewezen als groepsbeheerders in de gekopieerde groep. U kunt een groepslid als beheerder voor de groep toewijzen gebruikend het drop-down menu rechts van de naam van de gebruiker.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Een top-level groep moet minstens 1 groepsbeheerder hebben.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Personen en groepen in de lijst zoeken</td> 
      <td> Als u een gebruiker of groep wilt zoeken die al aan deze groep is toegewezen, kunt u hier hun naam typen en deze selecteren wanneer deze wordt weergegeven.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >* Als de originele groep subgroepen heeft, worden de subgroepen toegevoegd aan de nieuwe groep, en hun namen, door gebrek, &quot;de originele subgroepnaam (Exemplaar)&quot; zijn.
   >* U kunt elke gebruiker of subgroep uit de oorspronkelijke groep verwijderen door op de X rechts van de naam van de gebruiker of subgroep te klikken.


1. Klikken **Groep maken**.
