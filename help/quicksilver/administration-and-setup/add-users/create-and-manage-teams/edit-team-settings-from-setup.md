---
title: De montages van een Team van het Gebied van de Opstelling uitgeven
description: Als beheerder van Adobe Workfront, kunt u de montages van een team van het gebied van de Opstelling uitgeven. U kunt gebruikers aan een team toevoegen, het lay-outmalplaatje van een team plaatsen, en plaatsen hoe de status wordt geregistreerd wanneer de het werkpunten door een team worden voltooid.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# De instellingen van een team bewerken in het gedeelte Instellen

Als beheerder van Adobe Workfront, kunt u de montages van een team van het gebied van de Opstelling uitgeven. U kunt gebruikers aan een team toevoegen, het lay-outmalplaatje van een team plaatsen, en plaatsen hoe de status wordt geregistreerd wanneer de het werkpunten door een team worden voltooid.

Voor informatie over teams, zie [&#x200B; Overzicht van Teams &#x200B;](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Een groepsbeheerder kan de instellingen van een team bewerken voor een groep die hij of zij beheert. Voor meer informatie, zie [&#x200B; de teams van een groep &#x200B;](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md) creëren en wijzigen.
>* Een gebruiker met een Standard- of Plan-licentie kan de instellingen van een team bewerken in het gedeelte Teams. Voor meer informatie, zie [&#x200B; teammontages &#x200B;](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md) uitgeven.

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
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## De instellingen van een team bewerken

{{step-1-to-setup}}

1. Klik **Teams** in het linkerpaneel.
1. Selecteer een team, dan klik **uitgeven** ![&#x200B; pictogram &#x200B;](assets/edit-icon.png) uitgeeft.

1. Breng een van de volgende wijzigingen aan:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Teamnaam</td> 
      <td>Typ een naam voor het team.</td> 
     </tr>
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Is actief </td> 
       <td>Deze optie is standaard ingeschakeld voor nieuwe en bestaande teams. Schakel het uit om het team te deactiveren. Voor meer informatie, zie <a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref"> een team </a> deactiveren </td> 
      </tr>
     <tr> 
      <td role="rowheader">Groep</td> 
      <td> <p>Associeer het team met een groep. Typ de naam van de groep en selecteer vervolgens de naam wanneer deze wordt weergegeven.</p> <p><b> NOTA </b>: Wanneer een team aan een groep of een subgroep wordt toegewezen, kunnen om het even welke groepsbeheerders van die groep of subgroep het team beheren zonder een lid van het te zijn. De beheerders van de groep kunnen naar het gebied van Teams van het Belangrijkste Menu gaan en de pijl van de Teams van de Schakelaar <img src="assets/switch-team-icon.png" alt="Teampictogram wisselen"> klikken om van alle teams een lijst te maken die aan de groepen worden toegewezen die zij beheren.</p> <p>U kunt ervoor zorgen dat u de juiste groep aan het team koppelt door de muisaanwijzer boven de groep te plaatsen en op het informatiepictogram <img src="assets/info-icon.png"> te klikken dat naast de groep wordt weergegeven. Hier wordt knopinfo weergegeven met informatie over de groep, zoals de hiërarchie van de bovenliggende groepen en de bijbehorende beheerders.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eigenaar</td> 
      <td>Selecteer een eigenaar voor het team.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Teamleden</td> 
      <td> <p>Toevoegen en teamleden. Typ de naam van een gebruiker en selecteer vervolgens de naam wanneer deze wordt weergegeven. Herhaal dit proces om meerdere gebruikers aan het team toe te voegen.</p> 
      <p><b> TIP </b>: U kunt om het even welk aantal gebruikers aan een team toevoegen. Wij raden u echter aan om geen buitensporig groot aantal toe te voegen aan één team, omdat het werkbeheer van het team te complex kan worden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschrijving</td> 
      <td>Typ een beschrijving voor het team.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lay-outsjabloon</td> 
      <td> <p>Typ de naam van de lay-outsjabloon die het team moet gebruiken en klik vervolgens op de naam wanneer deze wordt weergegeven.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Agile</td> 
      <td>Geef op of dit een Agile-team is. Voor informatie over de teams van de Gelijkheid en hoe te om hun werk te beheren, zie <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref"> een team van de Gelijkheid </a> creëren.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">eraan werken</td> 
      <td> <p>Wijzig de knop Aan de werkbalk in een knop Start. Wanneer een gebruiker op Start klikt, wordt de status van het item automatisch bijgewerkt.</p> <p>Voor meer informatie over hoe te om de knoop van het Begin te vormen, zie <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref"> het Werk op het knoop met een knoop van het Begin vervangen </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gereed, knop</td> 
      <td> <p>Pas de knop Gereed aan. Zie voor meer informatie:</p> 
       <ul> 
        <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref"> vorm de Done knoop voor taken </a> </li> 
        <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref"> vorm de Done knoop voor kwesties </a> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **sparen Veranderingen**.
