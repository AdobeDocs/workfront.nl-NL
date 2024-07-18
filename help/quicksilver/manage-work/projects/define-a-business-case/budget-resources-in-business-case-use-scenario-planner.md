---
navigation-topic: business-case-and-scorecards
title: De middelen van de begroting in BedrijfsGeval gebruikend de Planner van het Scenario
description: Als deel van middelplanning, kunt u de Planner van het Scenario van Adobe Workfront gebruiken om de baanrollen noodzakelijk voor de voltooiing van het werk in een project te voorzien wanneer u het bedrijfscase bouwt.
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# De middelen van de begroting in BedrijfsGeval gebruikend de Planner van het Scenario

Als deel van middelplanning, kunt u de Planner van het Scenario van Adobe Workfront gebruiken om de baanrollen noodzakelijk voor de voltooiing van het werk in een project te voorzien wanneer u het bedrijfscase bouwt.

Voor meer informatie over het creëren van een bedrijfsgeval, zie [ een BedrijfsGeval voor een project ](../../../manage-work/projects/define-a-business-case/create-business-case.md) creëren.

>[!TIP]
>
>De informatie van de baanrol voor het initiatief verbonden aan het project dat u in de systeem-vlakke Planner van het Scenario ingaat is zichtbaar in het het budgetteren van het Middel gebied van het bedrijfscase van het project wanneer u het initiatief publiceert. De Scenario Planner is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring en vereist een aanvullende licentie. Voor informatie over de Planner van het Scenario van Workfront, zie [ het overzicht van de Planner van het Scenario ](../../../scenario-planner/scenario-planner-overview.md).

U kunt middelen in het bedrijfsgeval ook begroten gebruikend de Planner van het Middel. Raadpleeg de volgende secties voor meer informatie:

* [ middelen van de Begroting in het BedrijfsGeval ](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)
  <!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>Wij adviseren dat u het besluit neemt of om de Planner van het Middel of de Planner van het Scenario te gebruiken wanneer u begint werkend aan een project. Het vaak schakelen tussen beide tijdens de duur van het project kan tot inconsistenties in de manier leiden u uw middelen voor het project begroot.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Zakelijk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>U moet een extra licentie voor de Adobe Workfront Scenario Planner aanschaffen om toegang te krijgen tot de functionaliteit die in dit artikel wordt beschreven.</p> <p>Voor informatie over het verkrijgen van de Planner van het Scenario van Workfront, zie <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref"> Toegang nodig om de Planner van het Scenario te gebruiken </a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot het volgende bewerken: </p> 
    <ul> 
     <li> <p>Projecten</p> </li> 
     <li> <p>Financiële gegevens</p> </li> 
     <li> <p>Scenario Planner </p> </li> 
    </ul> <p>Voor informatie over de toegang nodig aan begrotingsmiddelen, zie ook <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref"> Toegang nodig aan begrotingsmiddelen in Adobe Workfront </a>.</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Adobe Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het project beheren</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Vereisten

Voordat u begint, moet u het volgende doen:

* Maak een plan met de functie Scenario.

  Voor informatie, zie [ plannen in de Planner van het Scenario creëren en uitgeven ](../../../scenario-planner/create-and-edit-plans.md).

* Maak een initiatief over het plan en koppel het aan een project.

  Zorg ervoor dat u de vereiste informatie voor de taakrollen voor het initiatief opgeeft en werk het gekoppelde project bij met deze informatie.

  Raadpleeg de volgende artikelen voor meer informatie:

   * [ creeer en geef initiatieven in de Planner van het Scenario uit ](../../../scenario-planner/create-and-edit-initiatives.md)
   * [ de projecten van de Invoer aan plannen in de Planner van het Scenario ](../../../scenario-planner/import-projects-to-plans.md)
   * [ werk of creeer projecten door initiatieven in de Planner van het Scenario ](../../../scenario-planner/publish-scenarios-update-projects.md) te publiceren bij.

* Hoewel dit geen eerste vereisten zijn, adviseren wij ook het volgende:

   * Wijs taken op het project aan de baanrollen toe die in de Planner van het Scenario worden begroot.
   * Vermeld het aantal geplande uren voor de taken van het project.

     Dit helpt u begrijpen hoeveel werk een taak zou kunnen moeten voltooien, die met het besluit helpt hoeveel tijd de middelen voor de voltooiing van de taak zouden moeten worden begroot.

     Voor informatie over het associëren van taken met Geplande Uren, zie [ taken ](../../../manage-work/tasks/manage-tasks/edit-tasks.md) uitgeven.

## Begrotingsmiddelen in het geval van de Zaken die de Planner van het Scenario gebruiken voor projecten met betrekking tot initiatieven

>[!IMPORTANT]
>
>U kunt uw middelen voor een periode van 15 jaar begroten. Als u middelen begroot voor een project met een looptijd van meer dan 15 jaar, is de begrotingsinformatie misschien niet correct.
><!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->

1. Ga naar het project waarvoor u middelen wilt begroten.

   >[!TIP]
   >
   >Het gaat om een project dat verband houdt met een initiatief in het Scenario Planner, waarvan het gekoppelde initiatief minstens één keer is gepubliceerd.

1. Klik **Bedrijfs Geval** in het linkerpaneel.
1. (Voorwaardelijk) in de **Bron die** sectie in de begroting brengen, doe één van het volgende:

   * Als u enkel informatie van de Planner van het Scenario publiceerde, de uitgezochte Planner van het Scenario in **verkies welke uren om de Begrotende Kosten van de Arbeid van het project** gebied op het het Voorwerpen van het Middel te berekenen, dan **kiezen**.

     ![](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * Als de Planner van het Middel eerder voor het opnemen van middelen voor het project werd geselecteerd, klik **Verandering** > **de Planner van het Scenario** > **kiezen**.

     ![](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

     Workfront maakt gebruik van de vereiste arbeidstijden van het gekoppelde initiatief om de begrote arbeidskosten en de begrote uren uren uren te berekenen. Dit is de aanbevolen optie. Kostendenvertoningen in het BedrijfsGeval in de valuta van het project.

     Wanneer u een project kopieert, en u uitgezocht om de Begroeide Uren aan het nieuwe project te kopiëren, worden de uren die in de begroting worden opgenomen gebruikend de Planner van het Scenario niet gekopieerd aan het nieuwe project. Alleen uren die in de bronnenplanner zijn opgenomen, worden gekopieerd. Voor meer informatie, zie [ een project ](../manage-projects/copy-project.md) kopiëren.

     >[!IMPORTANT]
     >
     >Wanneer u de Planner van het Scenario aan begrotingsmiddelen voor het project gebruikt, tonen de Begrotende Kosten van de Arbeid in de volgende gebieden van Workfront:
     >
     >   
     >   
     >   * Bronbudgettair gebied van de Business Case
     >   * De Scenario-planner op systeemniveau als de Personeelskosten van het initiatief in verband met het project. Voor meer informatie, zie [ initiatieven in de Planner van het Scenario creëren en uitgeven ](../../../scenario-planner/create-and-edit-initiatives.md).
     >   
     >

1. (Facultatief) klik **Mening in de Planner van het Scenario** om het plan te openen dat het initiatief verbonden aan het project bevat. Hiermee opent u het deelvenster Scenario in een nieuw browsertabblad.
1. (Optioneel) Informatie over het initiatief bijwerken. Voor meer informatie, zie [ initiatieven in de Planner van het Scenario creëren en uitgeven ](../../../scenario-planner/create-and-edit-initiatives.md).

   >[!NOTE]
   >
   >U moet het initiatief na elke verandering voor het het Leiden gebied van het Middel op het project publiceren om bij te werken.
