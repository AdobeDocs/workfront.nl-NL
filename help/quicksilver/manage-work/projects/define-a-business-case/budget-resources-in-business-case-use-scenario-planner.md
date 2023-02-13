---
navigation-topic: business-case-and-scorecards
title: De middelen van de begroting in BedrijfsGeval die Scenario Planner gebruiken
description: Als deel van middelplanning, kunt u de Planner van het Scenario van Adobe Workfront gebruiken om de baanrollen noodzakelijk voor de voltooiing van het werk in een project te voorzien wanneer u het bedrijfscase bouwt.
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: ffd7a588c0c9449b7a6aa18e6df7baa7c9872926
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 0%

---

# De middelen van de begroting in BedrijfsGeval die Scenario Planner gebruiken

Als deel van middelplanning, kunt u de Planner van het Scenario van Adobe Workfront gebruiken om de baanrollen noodzakelijk voor de voltooiing van het werk in een project te voorzien wanneer u het bedrijfscase bouwt.

Ga voor meer informatie over het maken van een business case naar [Een bedrijfscase maken voor een project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>De informatie van de baanrol voor het initiatief verbonden aan het project dat u in de systeem-vlakke Planner van het Scenario ingaat is zichtbaar in het het budgetteren van het Middel gebied van het bedrijfscase van het project wanneer u het initiatief publiceert. De Scenario Planner is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring en vereist een aanvullende licentie. Voor informatie over de Workfront Scenario Planner raadpleegt u [Overzicht van de functie Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

U kunt middelen in het bedrijfsgeval ook begroten gebruikend de Planner van het Middel. Raadpleeg de volgende secties voor meer informatie:

* [Begrotingsmiddelen in het bedrijfscase](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)

<!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>Wij adviseren dat u het besluit neemt of om de Planner van het Middel of de Planner van het Scenario te gebruiken wanneer u begint werkend aan een project. Het vaak schakelen tussen beide tijdens de levensduur van het project kan tot inconsistenties in de manier leiden u uw middelen voor het project begroot.

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
   <td> <p>U moet een extra licentie voor de Adobe Workfront Scenario Planner aanschaffen om toegang te krijgen tot de functionaliteit die in dit artikel wordt beschreven.</p> <p>Ga voor informatie over het verkrijgen van de Workfront Scenario Planner naar <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Toegang nodig om de Planner van het Scenario te gebruiken</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot het volgende bewerken: </p> 
    <ul> 
     <li> <p>Projecten</p> </li> 
     <li> <p>Financiële gegevens</p> </li> 
     <li> <p>Scenario Planner </p> </li> 
    </ul> <p>Voor informatie over de toegang tot begrotingsmiddelen, zie ook <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Toegang tot begrotingsmiddelen in Adobe Workfront</a>.</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Adobe Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het project beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

Voordat u begint, moet u het volgende doen:

* Creeer een plan gebruikend de Planner van het Scenario.

   Zie voor meer informatie [Abonnementen maken en bewerken in Scenario Planner](../../../scenario-planner/create-and-edit-plans.md).

* Maak een initiatief over het plan en koppel het aan een project.

   Zorg ervoor dat u de vereiste informatie voor de taakrollen voor het initiatief opgeeft en werk het gekoppelde project bij met deze informatie.

   Raadpleeg de volgende artikelen voor meer informatie:

   * [Initiatieven maken en bewerken in de functie Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md)
   * [Projecten importeren naar plannen in het scenario Scenario Planner](../../../scenario-planner/import-projects-to-plans.md)
   * [Werk of creeer projecten bij door initiatieven in de Planner van het Scenario te publiceren](../../../scenario-planner/publish-scenarios-update-projects.md).

* Hoewel dit geen eerste vereisten zijn, adviseren wij ook het volgende:

   * Wijs taken op het project aan de baanrollen toe die in de Planner van het Scenario worden begroot.
   * Vermeld het aantal geplande uren voor de taken van het project.

      Dit helpt u begrijpen hoeveel werk een taak zou kunnen moeten voltooien, die met het besluit helpt hoeveel tijd de middelen voor de voltooiing van de taak zouden moeten worden begroot.

      Voor informatie over het associëren van taken met Geplande Uren, zie [Taken bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Begrotingsmiddelen in het geval van de Zaken die de Planner van het Scenario gebruiken voor projecten met betrekking tot initiatieven

>[!IMPORTANT]
U kunt uw middelen voor een periode van 15 jaar begroten. Als u middelen begroot voor een project met een looptijd van meer dan 15 jaar, is de begrotingsinformatie misschien niet correct.
<!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->


1. Ga naar het project waarvoor u middelen wilt begroten.

   >[!TIP]
   Het gaat om een project dat verband houdt met een initiatief in het Scenario Planner, waarvan het gekoppelde initiatief minstens één keer is gepubliceerd.

1. Klikken **Bedrijfs-case** in het linkerdeelvenster.
1. (Voorwaardelijk) In de **Bronnen begroten** voert u een van de volgende handelingen uit:

   * Als u net informatie van de Planner van het Scenario hebt gepubliceerd, selecteer de Planner van het Scenario in **Kies welke uren u wilt gebruiken om de begrote arbeidskosten van het project te berekenen** veld in het gebied Resource Budgeting en klik vervolgens op **Kies**.

      ![](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * Als de functie voor middelenplanning eerder is geselecteerd voor budgettering van bronnen voor het project, klikt u op **Wijzigen** > **Scenario Planner** > **Kies**.

      ![](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

      Workfront maakt gebruik van de vereiste arbeidstijden van het gekoppelde initiatief om de begrote arbeidskosten van het project te berekenen. Dit is de aanbevolen optie. Kostendenvertoningen in het BedrijfsGeval in de valuta van het project.

      >[!IMPORTANT]
      Wanneer u de Planner van het Scenario aan begrotingsmiddelen voor het project gebruikt, tonen de Begrotende Kosten van de Arbeid in de volgende gebieden van Workfront:
      * Bronbudgettair gebied van de Business Case
      * De Scenario-planner op systeemniveau als de Personeelskosten van het initiatief in verband met het project. Zie voor meer informatie [Initiatieven maken en bewerken in de functie Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md).


1. (Optioneel) Klik op **Weergeven in Scenario Planner** het plan te openen dat het met het project samenhangende initiatief bevat. Hiermee opent u het deelvenster Scenario in een nieuw browsertabblad.
1. (Optioneel) Informatie over het initiatief bijwerken. Zie voor meer informatie [Initiatieven maken en bewerken in de functie Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md).

   >[!NOTE]
   U moet het initiatief na elke verandering voor het het Leiden gebied van het Middel op het project publiceren om bij te werken.
