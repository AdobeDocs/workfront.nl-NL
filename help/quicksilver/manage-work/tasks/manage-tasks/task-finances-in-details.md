---
product-area: projects
navigation-topic: manage-tasks
title: Taakfinanciën beheren in de sectie Taakdetails
description: Taakfinanciën beheren in de sectie Taakdetails
author: Alina
feature: Work Management
exl-id: 54ae48e5-bc8c-4e90-8fa1-0015523df4e6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 0%

---

# Taakfinanciën beheren in de sectie Taakdetails

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, to it in both articles)</p>
-->

U kunt de financiële informatie van een taak bekijken of uitgeven door tot het gebied van het Overzicht van de sectie van de Details van de Taak toegang te hebben. Er is een beperkt aantal velden dat u in dit gebied kunt weergeven of bewerken. Voor informatie over het bewerken van alle financiële informatie voor een taak raadpleegt u [Taken bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten en taken bewerken</p> <p>Toegang tot financiële gegevens of hoger weergeven</p> <p>U moet Edit toegang tot Financiële Gegevens hebben om financiële informatie over taken uit te geven</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven voor de taak die View Finance of hoger bevat</p> <p>U moet beheermachtigingen hebben voor de taak die onder meer Edit Finance bevat om financiële informatie over taken te bewerken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Taakfinanciën bewerken in de sectie Taakdetails

1. Ga naar een project waar u een taak wilt bekijken.

   >[!NOTE]
   >
   >Als u een taak wilt zoeken, kunt u er ook naar zoeken en op de naam klikken om de taak te openen. Ga voor meer informatie over het zoeken naar objecten in Workfront naar [Zoeken in Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

1. Klikken **Taken** in het linkerdeelvenster.
1. Klik op de naam van een taak die u wilt weergeven.
1. Klikken **Taakdetails**.
1. (Optioneel) Klik op de knop **Alles samenvouwen** in de rechterbovenhoek van de pagina Taakdetails.

   ![](assets/collapse-all-icon-on-details-page.png)

   >[!NOTE]
   >
   >Afhankelijk van hoe uw Workfront-beheerder of groepsbeheerder onze lay-outsjabloon instelt, kunnen de velden in de sectie Taakdetails opnieuw worden gerangschikt of niet worden weergegeven. Zie voor meer informatie [De weergave Details aanpassen met een lay-outsjabloon](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Klikken **Financiën** de financiële informatie voor de taak uit te breiden en te bekijken.

   Klik op de knop **Bewerken** pictogram ![](assets/edit-icon.png) in de rechterbovenhoek van de sectie Details klikt u op **Financiën**.

1. Bewerk een veld dat u kunt bewerken door één keer op het veld te klikken of klik op **+Toevoegen** om informatie toe te voegen aan een leeg veld.
1. Controleer of bewerk de volgende informatie in het dialoogvenster **Financiën** gebied:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Kostensoort</td> 
      <td> <p>Geef het type kosten voor de taak op. Dit gaat bepalen hoe de kosten van de taak, gebaseerd op het aantal uren op de taken worden berekend. </p> <p>Selecteer een van de volgende opties: </p> 
       <ul> 
        <li> <p>Geen kosten</p> </li> 
        <li> <p>Vaste uren </p> </li> 
        <li> <p> Uur gebruiker </p> </li> 
        <li> <p> Rol Uur</p> </li> 
       </ul> <p>Voor meer informatie over het volgen van kosten, zie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Trackkosten</a> . Uw Workfront-beheerder of groepsbeheerder selecteert de standaardinstelling Kostensoort voor de taken in uw systeem of groep. Voor informatie over het plaatsen van projectgebreken, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Projectvoorkeuren voor het hele systeem configureren</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type inkomsten</td> 
      <td> <p>Geef het type inkomsten voor de taak op. Dit gaat bepalen hoe de Inkomsten op de taak worden berekend, gebaseerd op het aantal uren op de taken. </p> <p>Selecteer een van de volgende opties: </p> 
       <ul> 
        <li> <p> Niet opteerbaar </p> </li> 
        <li> <p>Uur gebruiker </p> </li> 
        <li> <p>Rol Uur </p> </li> 
        <li> <p>Vaste uren </p> </li> 
        <li> <p>Uur gebruiker met lampvoet </p> </li> 
        <li> <p>Rol Uur met lampvoet </p> </li> 
        <li> <p>Uur plus vaste kosten gebruiker </p> </li> 
        <li> <p>Rol Uur plus vast </p> </li> 
        <li> <p>Vaste inkomsten </p> </li> 
       </ul> <p>Voor meer informatie over het volgen van opbrengst, zie<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overzicht van facturering en inkomsten</a> . </p> <p>Uw Workfront-beheerder of groepsbeheerder selecteert de standaardinstelling Inkooptype voor de taken in uw systeem of groep. Voor informatie over het plaatsen van projectgebreken, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Projectvoorkeuren voor het hele systeem configureren</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplande kosten</td> 
      <td> <p>Dit is een berekening die de kosten van de taak toont die op de geplande uren, het kostentype, en het uurtarief voor gebruikers of baanrollen wordt gebaseerd. Voor meer informatie over het volgen van kosten, zie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Trackkosten</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werkelijke kosten</td> 
      <td> <p> Dit is een berekening die de kosten van de taak toont die op de daadwerkelijke uren, het kostentype, en het uurtarief voor gebruikers of baanrollen wordt gebaseerd. Voor meer informatie over het volgen van kosten, zie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Trackkosten</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplande inkomsten</td> 
      <td> <p>Dit is een berekening die de opbrengst verbonden aan de taak toont die op de geplande uren, het opbrengsttype, en het uurtarief voor gebruikers of baanrollen wordt gebaseerd. Voor meer informatie over het volgen van kosten, zie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Trackkosten</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werkelijke ontvangsten</td> 
      <td> <p>Dit is een berekening die de opbrengst verbonden aan de taak toont die op de daadwerkelijke uren, het opbrengsttype, en het uurtarief voor gebruikers of baanrollen wordt gebaseerd. Voor meer informatie over het volgen van kosten, zie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Trackkosten</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>CPI/SPI/CSI</strong> </td> 
      <td> <p>Dit zijn de metriek van taakprestaties die tonen hoe uw taak, op een bepaald ogenblik uitvoert. Hun waarden worden berekend op basis van de methode van de Index van Prestaties van het project.<br>Zie de volgende artikelen voor meer informatie:</p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Kostenprestatie-index (CPI) berekenen</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Prestatie-index (SPI) voor planning berekenen </a> </p> </li> 
        <li> <p> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Prestatie-index (CSI) voor kostenplanning berekenen</a> </p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Raming bij voltooiing (EAC)</td> 
      <td> <p>Dit is een berekening die de totale kosten van uw taak, bij voltooiing toont. Voor meer informatie over de schatting bij voltooiing, zie <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Schatting berekenen bij voltooiing (EAC)</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Voorwaardelijk) Als u de velden in de sectie Financiën bewerkt, klikt u op **Opslaan***Wijzigingen**.
