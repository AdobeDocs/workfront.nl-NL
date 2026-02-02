---
product-area: projects
navigation-topic: manage-tasks
title: Taakfinanciën beheren in de sectie Taakdetails
description: U kunt de financiële informatie van een taak bekijken of uitgeven door tot het gebied van het Overzicht van de sectie van de Details van de Taak toegang te hebben. Er is een beperkt aantal velden dat u kunt weergeven of bewerken in de sectie Taakdetails.
author: Alina
feature: Work Management
exl-id: 54ae48e5-bc8c-4e90-8fa1-0015523df4e6
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# Taakfinanciën beheren in de sectie Taakdetails

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, to it in both articles)</p>
-->

U kunt de financiële informatie van een taak bekijken of uitgeven door tot het gebied van het Overzicht van de sectie van de Details van de Taak toegang te hebben. Er is een beperkt aantal velden dat u in dit gebied kunt weergeven of bewerken.

Voor informatie over het uitgeven van alle financiële informatie voor een taak zie [ taken ](../../../manage-work/tasks/manage-tasks/edit-tasks.md) uitgeven.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard</p> 
   <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten en taken bewerken</p> <p>Toegang tot financiële gegevens of hoger weergeven</p> <p>U moet Edit toegang tot Financiële Gegevens hebben om financiële informatie over taken uit te geven</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven voor de taak die View Finance of hoger bevat</p> <p>U moet beheermachtigingen hebben voor de taak die onder meer Edit Finance bevat om financiële informatie over taken te bewerken</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Tasks</p> <p>View access to Financial Data or higher</p> <p>You must have Edit access to Financial Data to edit financial information on tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the task that include View Finance or higher</p> <p>You must have Manage permissions on the task that include Edit Finance to edit financial information on tasks</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Taakfinanciën bewerken in de sectie Taakdetails

1. Ga naar een project waar u een taak wilt bekijken.

   >[!NOTE]
   >
   >Als u een taak wilt zoeken, kunt u er ook naar zoeken en op de naam klikken om de taak te openen. Voor meer informatie bij het zoeken naar voorwerpen in Workfront, zie [ Onderzoek Adobe Workfront ](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

1. Klik **Taken** in het linkerpaneel.
1. Klik op de naam van een taak die u wilt weergeven.
1. Klik **Details van de Taak**.
1. (Facultatief) klik **Vouw al** pictogram in het hoogste recht van de pagina van de Details van de Taak samen.

   ![ Vouw al pictogram op de pagina van Details samen ](assets/collapse-all-icon-on-details-page.png)

   >[!NOTE]
   >
   >Afhankelijk van hoe uw Workfront-beheerder of groepsbeheerder onze lay-outsjabloon instelt, kunnen de velden in de sectie Taakdetails opnieuw worden gerangschikt of niet worden weergegeven. Voor informatie, zie [ de mening van Details aanpassen gebruikend een lay-outmalplaatje ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Klik **Financiën** om de financiële informatie voor de taak uit te breiden en te bekijken.

   Klik **uitgeven** pictogram ![ geeft pictogram ](assets/edit-icon.png) in de hoger-juiste hoek van de sectie van Details uit, dan klik **Financiën**.

1. Bewerk elk veld dat u kunt bewerken door één keer op het veld te klikken of klik op **+Toevoegen** om informatie toe te voegen aan een leeg veld.
1. Herzie of geef de volgende informatie in het **Financiën** gebied uit:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Kostensoort</td> 
      <td> <p>Geef het type kosten voor de taak op. Dit gaat bepalen hoe de kosten van de taak, gebaseerd op het aantal uren op de taken worden berekend. </p> <p>Selecteer een van de volgende opties: </p> 
       <ul> 
        <li> <p>Geen kosten</p> </li> 
        <li> <p>Vast uurwerk </p> </li> 
        <li> <p> Uur gebruiker </p> </li> 
        <li> <p> Rol Uur</p> </li> 
       </ul> <p>Voor meer informatie over het volgen van kosten, zie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref"> Kosten van het Spoor </a>. Uw Workfront-beheerder of groepsbeheerder selecteert de standaardinstelling Kostensoort voor de taken in uw systeem of groep. Voor informatie over het plaatsen van projectgebreken, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref"> systeem-brede projectvoorkeur </a> vormen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type inkomsten</td> 
      <td> <p>Geef het type inkomsten voor de taak op. Dit gaat bepalen hoe de Inkomsten op de taak worden berekend, gebaseerd op het aantal uren op de taken. </p> <p>Selecteer een van de volgende opties: </p> 
       <ul> 
        <li> <p> Niet opblaasbaar </p> </li> 
        <li> <p>Uur gebruiker </p> </li> 
        <li> <p>Rol Uur </p> </li> 
        <li> <p>Vast uurwerk </p> </li> 
        <li> <p>Uur gebruiker met lampvoet </p> </li> 
        <li> <p>Rol Uur met lampvoet </p> </li> 
        <li> <p>Uur plus vaste kosten gebruiker </p> </li> 
        <li> <p>Rol Uur plus vast </p> </li> 
        <li> <p>Vaste inkomsten </p> </li> 
       </ul> <p>Voor meer informatie over het volgen van opbrengst, zie <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref"> Overzicht van Facturering en Ontvangsten </a>. </p> <p>Uw Workfront-beheerder of groepsbeheerder selecteert de standaardinstelling Inkooptype voor de taken in uw systeem of groep. Voor informatie over het plaatsen van projectgebreken, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref"> systeem-brede projectvoorkeur </a> vormen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplande kosten</td> 
      <td> <p>Dit is een berekening die de kosten van de taak toont die op de geplande uren, het kostentype, en het uurtarief voor gebruikers of baanrollen wordt gebaseerd. Voor meer informatie over het volgen van kosten, zie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref"> Kosten van het Spoor </a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werkelijke kosten</td> 
      <td> <p> Dit is een berekening die de kosten van de taak toont die op de daadwerkelijke uren, het kostentype, en het uurtarief voor gebruikers of baanrollen wordt gebaseerd. Voor meer informatie over het volgen van kosten, zie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref"> Kosten van het Spoor </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplande inkomsten</td> 
      <td> <p>Dit is een berekening die de opbrengst verbonden aan de taak toont die op de geplande uren, het opbrengsttype, en het uurtarief voor gebruikers of baanrollen wordt gebaseerd. Voor meer informatie over het volgen van kosten, zie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref"> Kosten van het Spoor </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werkelijke ontvangsten</td> 
      <td> <p>Dit is een berekening die de opbrengst verbonden aan de taak toont die op de daadwerkelijke uren, het opbrengsttype, en het uurtarief voor gebruikers of baanrollen wordt gebaseerd. Voor meer informatie over het volgen van kosten, zie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref"> Kosten van het Spoor </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> CPI/SPI/CSI </strong> </td> 
      <td> <p>Dit zijn de metriek van taakprestaties die tonen hoe uw taak, op een bepaald ogenblik uitvoert. Hun waarden worden berekend op basis van de methode van de Index van Prestaties van het project.<br> voor meer informatie zie de volgende artikelen:</p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref"> berekent de Index van de Prestaties van Kosten (CPI) </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref"> de Index van de Prestaties van het Programma berekenen (SPI) </a> </p> </li> 
        <li> <p> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref"> berekent de Index van de Prestaties van het Programma van Kosten (CSI) </a> </p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Raming bij voltooiing (EAC)</td> 
      <td> <p>Dit is een berekening die de totale kosten van uw taak, bij voltooiing toont. Voor meer informatie over raming bij voltooiing, zie <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref"> Schatting bij Voltooiing (EAC) berekenen </a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Voorwaardelijk) als u de gebieden in de sectie van de Financiën uitgeeft, klik **sparen***Veranderingen**.
