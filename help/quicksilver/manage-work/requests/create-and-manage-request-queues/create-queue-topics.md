---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Werkvoorraadonderwerpen maken
description: De Onderwerpen van de rij werken samen met het Verpletteren van Regels om het inkomende werk aan een gebruiker, baanrol, team automatisch toe te wijzen, of het op een project te plaatsen. De Onderwerpen van de rij bepalen de voorwaarden die voor de Verpletterende Regel moeten bestaan worden uitgevoerd.
author: Becky
feature: Work Management, Requests
role: User, Admin
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
source-git-commit: 4a0cb96f5888819747f63472712f91c685621cf1
workflow-type: tm+mt
source-wordcount: '1013'
ht-degree: 0%

---

# Werkvoorraadonderwerpen maken

<!-- Audited: 12/2023 -->

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Het is beschikbaar slechts in het milieu van de Sandbox van de Voorproef.</span>

De Onderwerpen van de rij werken samen met het Verpletteren van Regels om het inkomende werk aan een gebruiker, baanrol, team automatisch toe te wijzen, of het op een project te plaatsen. De Onderwerpen van de rij bepalen de voorwaarden die voor de Verpletterende Regel moeten bestaan worden uitgevoerd.

Er is geen grens aan het aantal Onderwerpen van de Rij die aan een Groep van het Onderwerp of aan een project kunnen worden toegewezen. De Onderwerpen van de rij zijn een te melden objecten type.

U kunt de Onderwerpen van de Rij voor individuele projecten, of voor projectmalplaatjes tot stand brengen.

Zodra gecreeerd, kunt u rijonderwerpen van één project of malplaatje aan een andere niet bewegen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<!--drafted - replace table with P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
    <p>Standard</p>
    <p>Plan</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p> Rechten voor het project beheren</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een onderwerp in de wachtrij maken

1. Creeer een Verpletterende Regel, een Groep van het Onderwerp, en een douaneformulier, als u van plan bent om hen met uw Onderwerp van de Rij te associëren.\
   Voor meer informatie over hoe te om het Verpletteren van Regels, de Groepen van het Onderwerp of douanevormen tot stand te brengen, verwijs naar de volgende artikelen:

   * [&#x200B; creeer Verpletterend Regels &#x200B;](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)
   * [&#x200B; creeer de Groepen van het Onderwerp &#x200B;](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [Een aangepast formulier maken](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)

1. Ga naar het project of het malplaatje u verkoos om als Rij van het Verzoek van de Hulp toe te laten en waar u een nieuw rijonderwerp wilt creëren.\
   Voor meer informatie over hoe te om een project als Rij van het Verzoek van de Hulp aan te wijzen, zie [&#x200B; een Rij van het Verzoek van de Vraag &#x200B;](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren.

   U kunt verwante Onderwerpen van de Rij onder een Groep van het Onderwerp organiseren. De aanvrager krijgt dan een aantal vervolgkeuzemenu&#39;s bij het indienen van een aanvraag.

   of

   U kunt de Onderwerpen van de Rij onder het project direct nesten dat als Rij van het Verzoek van de Hulp, zonder een Groep van het Onderwerp wordt aangewezen.

   Voor informatie over het creëren van de Groepen van het Onderwerp, zie [&#x200B; de Groepen van het Onderwerp &#x200B;](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md) creëren.

1. Klik **de Onderwerpen van de Rij** in het linkerpaneel.
1. Klik **Nieuw Onderwerp van de Rij**.
1. Op de **Nieuwe vorm van het Onderwerp van de Rij**, ga het volgende in:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong> Naam </strong> </td> 
      <td> Naam van het Onderwerp van de Rij.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Beschrijving </strong> </td> 
      <td>Beschrijf de verzoekwachtrij. De beschrijving toont wanneer de gebruikers het rijonderwerp in het proces selecteren om een nieuw verzoek voor te leggen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> voeg aan de Groep van het Onderwerp toe </strong> </td> 
      <td> Als er geen Groepen van het Onderwerp op het project zijn, blijft de naam van het project als Groep van het Onderwerp in gebreke.<br> als u de extra Groepen van het Onderwerp van hier wilt tot stand brengen, <strong> creeer Nieuwe Groep van het Onderwerp </strong> van het drop-down menu.<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_within_queue_topic.png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Aangepaste Forms </strong> </td> 
      <td>Selecteer de aangepaste formulieren die u aan het onderwerp van de wachtrij wilt koppelen. U moet aangepaste formulieren maken voor problemen voordat u deze kunt koppelen aan onderwerpen in de wachtrij. Voor informatie over het creëren van douaneformulieren, zie <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md"> een douaneformulier </a> creëren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standaardgoedkeuring</strong></td> 
      <td> <p>Koppel een goedkeuringsproces aan dit rijonderwerp. In dit keuzemenu worden alleen processen voor goedkeuring van uitgaven weergegeven. Alle problemen die naar deze wachtrij worden verzonden, worden gekoppeld aan dit goedkeuringsproces. Uw beheerder van Adobe Workfront moet de processen van de Goedkeuring op systeemniveau bepalen alvorens u hen met rijonderwerpen kunt associëren. <span> de gebruiker van A met administratieve toegang tot de Processen van de Goedkeuring kan tot groep-specifieke goedkeuringsprocessen ook leiden.</span> voor meer informatie over het creëren van de Processen van de Goedkeuring, zie <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref"> een goedkeuringsproces voor het werkpunten </a> creëren.<br></p> 
       <div> 
        <p>Belangrijk: als de groep van het project verandert, wordt het groepsspecifieke goedkeuringsproces verbonden aan bestaande kwesties een goedkeuringsproces voor eenmalig gebruik. Voor meer informatie over hoe de veranderingen in de groep van het project of de veranderingen in het goedkeuringsproces goedkeuringsmontages beïnvloeden, zie <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref"> hoe de groep en de veranderingen van het goedkeuringsproces aangewezen goedkeuringsprocessen </a> beïnvloeden.</p> 
        <p>Overweeg het volgende wanneer het toevoegen van goedkeuringsprocessen aan rijonderwerpen: </p> 
        <ul style="list-style-type: circle;"> 
         <li>Alleen actieve goedkeuringsprocessen worden in de lijst weergegeven. </li> 
         <li> <p>Systeemspecifieke en groepsspecifieke goedkeuringsprocessen worden in de lijst weergegeven. Een goedkeuringsproces verbonden aan een groep buiten die van het project toont niet in de lijst.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> StandaardDuur </strong> </td> 
      <td>Dit is de standaardduur van het verzoek, en de Geplande Datum van Voltooiing van het verzoek wordt berekend gebaseerd op deze waarde.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> StandaardRoute </strong> </td> 
      <td>Specificeer de verpletterende regel u met het Onderwerp van de Rij wilt associëren. U moet de verpletterende regel tot stand brengen alvorens u het aan een Onderwerp van de Rij kunt vastmaken. Voor informatie, zie <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md"> het Verpletteren van Regels </a> creëren. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Types van Verzoek </strong> </td> 
      <td> <p>Kies welk soort verzoeken dit rijonderwerp opslaat. De zichtbare opties worden geplaatst op het <strong> lusje van de Details van de Rij </strong> van het project. Dit is een verplicht veld. </p> 
       <p><b> NOTA </b>:</p>
      <p>De types tonen als selectie op het gebied van Verzoeken slechts als het Type van Verzoek in zowel de Details van de Rij als de pagina's van het Onderwerp van de Rij wordt geselecteerd. Voor informatie over vestiging het gebied van de Details van de Rij van een project, zie <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref"> een Rij van het Verzoek </a> creëren. </p> <p>Selecteer een van de volgende typen:</p> 
       <ul> 
        <li>Foutrapport</li> 
        <li>Volgorde wijzigen</li> 
        <li>Probleem</li> 
        <li>Verzoek</li> 
       </ul> <p>Mogelijk is de naam van uw Workfront-beheerder gewijzigd in een aantal van deze opties. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![&#x200B; Nieuwe doos van het Onderwerp van de Rij &#x200B;](assets/new-queue-topic-box.png)

1. Klik **sparen**.\
   Het onderwerp van de Rij is nu beschikbaar aan gebruik en is zichtbaar in het gebied van Verzoeken van Workfront, nadat een Rij van het Verzoek en een Groep van het Onderwerp worden geselecteerd.

## Een onderwerp in de wachtrij bewerken

Een bestaand onderwerp van de Rij uitgeven:

1. Ga naar het project of het malplaatje dat het Onderwerp van de Rij bevat u wilt uitgeven.
1. Klik **de Onderwerpen van de Rij** in het linkerpaneel.
1. In het milieu van de Productie, selecteer het Onderwerp van de Rij dat u wilt uitgeven. Voor de pagina van Details die opent, geeft de klik **het Onderwerp van de Rij** uit.
1. <span class="preview"> in het milieu van de Voorproef, klik het rijonderwerp dat u wilt uitgeven.

Voor informatie over beschikbare geef opties uit, zie [&#x200B; tot een Onderwerp van de Rij &#x200B;](#create-a-queue-topic) in dit artikel leiden.

## Een onderwerp uit de wachtrij verwijderen

U kunt één of meerdere rijonderwerpen tezelfdertijd schrappen.

1. Ga naar het project of het malplaatje dat het Onderwerp van de Rij bevat u wilt schrappen.
1. Klik **de Onderwerpen van de Rij** in het linkerpaneel.
1. Klik de doos naast de naam van elk Onderwerp van de Rij dat u wilt schrappen. Er verschijnt een vinkje in het vak.
1. Klik het **pictogram van de Schrapping** ![&#x200B; bij de bovenkant van de pagina.](assets/delete-icon.png)

