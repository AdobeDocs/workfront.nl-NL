---
navigation-topic: business-case-and-scorecards
title: De middelen van de begroting in BedrijfsGeval die de Planner van het Middel gebruiken
description: Als deel van middelplanning, kunt u de project-vlakke Planner van het Middel gebruiken om de baanrollen noodzakelijk voor de voltooiing van het werk in een project te voorzien wanneer u het bedrijfscase bouwt.
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1249'
ht-degree: 0%

---

# De middelen van de begroting in BedrijfsGeval die de Planner van het Middel gebruiken

Als deel van middelplanning, kunt u de project-vlakke Planner van het Middel gebruiken om de baanrollen noodzakelijk voor de voltooiing van het werk in een project te voorzien wanneer u het bedrijfscase bouwt.

Ga voor meer informatie over het maken van een business case naar [Een bedrijfscase maken voor een project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>De informatie u in de project-vlakke Planner van het Middel ingaat is ook zichtbaar in de systeem-vlakke Planner van het Middel. Het omgekeerde geldt ook. Voor informatie over de Planner van het Middel, zie [Overzicht van de bronnenplanner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

U kunt middelen in de bedrijfscase ook begroten gebruikend de Planner van het Scenario van Adobe Workfront. Zie voor meer informatie [De middelen van de begroting in BedrijfsGeval die Scenario Planner gebruiken](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront-plan</a>*</td> 
   <td> <p>Pro of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Overzicht van Adobe Workfront-licenties</a>*</td> 
   <td> <p>Controleren of hoger</p> <p>Belangrijk: U moet een licentie voor het abonnement hebben om de informatie over het budgetteren van bronnen te wijzigen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot het volgende bewerken: </p> 
    <ul> 
     <li> <p>Projecten</p> </li> 
     <li> <p>Bronbeheer</p> </li> 
     <li> <p>Financiële gegevens</p> </li> 
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

* Voldoe aan alle voorwaarden voor middelplanning in Adobe Workfront. Zie voor meer informatie [Overzicht van de bronnenplanner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Brongroepen koppelen aan het project.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

   >[!NOTE]
   U kunt geen middelen begroten die aan kwesties in de BedrijfsGeval worden toegewezen. U kunt ze begroten in de bronnenplanner op systeemniveau. Voor meer informatie over de Planner van het Middel, zie [Overzicht van de bronnenplanner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Hoewel dit geen voorwaarde is, adviseren wij ook dat u op Geplande Uren voor de taken op het project wijst. Dit helpt u begrijpen hoeveel werk een taak zou kunnen moeten voltooien die met het besluit van veel tijd de middelen voor de voltooiing van de taak zou moeten worden begroot. Voor informatie over het associëren van taken met Geplande Uren, zie [Taken bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Bronnenpools toepassen op een project en budgetbronnen in de bedrijfscase

>[!IMPORTANT]
U kunt uw middelen voor een periode van 15 jaar begroten. Als u middelen begroot voor een project met een looptijd van meer dan 15 jaar, is de begrotingsinformatie misschien niet correct.

Om de Pools van het Middel en de middelen van het begrotingsproject in het BedrijfsGeval voor een project zonder Groep van het Middel toe te passen:

1. Ga naar het project waarvoor u middelen wilt begroten.
1. Klikken **Bedrijfs-case** in het linkerdeelvenster.
1. (Voorwaardelijk) Als uw bedrijf geen licentie voor de Workfront Scenario Planner heeft, klikt u op **Resource Budgeting bewerken** in de **Bronnen begroten** en gaat u verder met stap 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. (Facultatief en voorwaardelijk) als de projectinformatie uit een initiatief op de Planner Scenario is gepubliceerd, doe één van het volgende:

   * Bronnen selecteren in het dialoogvenster **Kies welke uren u wilt gebruiken om de begrote arbeidskosten van het project te berekenen** veld, klik vervolgens op **Kies > Bronbudgettering bewerken**.

      ![](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * Als Scenario Planner voor het opnemen van middelen voor het project werd geselecteerd, klik **Wijzigen** > **Resource Budgeting bewerken**.

      ![](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)
   Dit gebruikt de begrotingsuren van het project om de begrote arbeidskosten voor het project te berekenen.

   De Scenario Planner is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring en vereist een aanvullende licentie. Voor informatie over de Workfront Scenario Planner raadpleegt u [Overzicht van de functie Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   Wij adviseren dat u het besluit neemt of om de Planner van het Middel of de Planner van het Scenario te gebruiken wanneer u begint werkend aan een project. Het vaak schakelen tussen beide tijdens de levensduur van het project kan tot inconsistenties in de manier leiden u uw middelen voor het project begroot.

1. In de **Brongroep selecteren** veld, geef een of meerdere **Brongroepen**.

   U moet alleen bronnenpools opgeven die zijn gevuld met actieve gebruikers.

   >[!TIP]
   Als het project reeds met de Pools van het Middel wordt geassocieerd, toont de Planner van het Middel door gebrek. Om meer Pools van het Middel aan het project toe te voegen, geef het project uit. Voor informatie over het bewerken van een project raadpleegt u [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Klikken **Toepassen**.

   De Planner van het Middel wordt getoond, voor het geselecteerde project.

   Door gebrek, zijn de eerste 20 baanrollen verbonden aan dit project vermeld in de sectie van de Begroting van het Middel in alfabetische orde. 

   Voor meer informatie over de Planner van het Middel, zie [Overzicht van de bronnenplanner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![BC_resource_budgeting_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. (Optioneel en voorwaardelijk) Vergroot de taakrollen om de gebruikers te zien die aan deze rollen zijn gekoppeld.

   >[!NOTE]
   De actieve gebruikers worden getoond onder de baanrollen verbonden aan hen slechts als zij aan de volgende criteria voldoen:
   * Zij behoren tot één van de Groepen van Middel van het project.
   * Ze hebben de toegewezen uren begroot.
   * Zij worden geassocieerd met één van de baanrollen van het project.


    

1. Klikken **Vandaag** om terug te keren naar het huidige tijdpad.
1. (Optioneel) Klik op **Week**, **Maand** of **Kwart** om informatie voor het project in verschillende tijdkaders te tonen.
1. (Optioneel) Klik op de knop **Uren** en selecteert u **Uren**,**FTE**, of **Kosten** om te veranderen hoe de informatie in de Planner van het Middel toont. Standaardweergave in uren.

1. (Optioneel) Klik op **Exporteren** om de Planner van het Middel naar een dossier van Excel uit te voeren.

   >[!NOTE]
   U kunt gegevens gedurende maximaal twaalf tijdsperioden tegelijk exporteren.

1. (Optioneel) Klik op de knop **Volledig scherm** pictogram ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png) om de functie Bronnen op volledig scherm weer te geven.

1. Werk de **BDG** (Budgeted Hours) gebied met Uur, FTE, of de waarden van Kosten voor de gebruikers, de rollen, of het project door één van het volgende te doen:

   * Geef handmatig een schatting van de hoeveelheid uren, FTE of Kostenwaarden voor rollen, gebruikers of het project.

      of

   * Klik op de knop **Opties** pictogram voor het project of de baanrollen en selecteer een optie om de uren voor rollen, gebruikers, of het project automatisch te begroten.
   Voor meer informatie over het in de begroting opnemen in de Mening van het Project van de Planner van het Middel, zie [De middelen van de begroting in de Planner van het Middel gebruikend de meningen van het Project en van de Rol](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   U kunt uren, FTEs, of kosten voor uw middelen voor om het even welk tijdkader begroten dat in het het Begrotinggebied van het Middel wordt getoond, onafhankelijk van de chronologie van het project. Als u bijvoorbeeld wilt aangeven dat uw bronnen mogelijk niet beschikbaar zijn tijdens de tijdlijn van het project (waar ze zijn gekoppeld aan geplande uren), maar wel op een ander tijdstip beschikbaar zijn, kunt u dit doen door de bronnen in te voegen voor tijdframes waarin de geplande uren nul zijn, als dat het moment is waarop ze beschikbaar zijn om te werken.

1. (Optioneel) Als u wilt weten of u de begrote uren uren, VTE&#39;s of kosten naar een ander tijdpad kunt verplaatsen, klikt u op de knop **Opties** pictogram, dan **Bochtingsdatums aanpassen**.

   Zie voor meer informatie over het aanpassen van gebudgetteerde datums [Datums voor budgettering aanpassen in de functie voor middelenplanning](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. Klikken **Opslaan**.

   Als u Kosten per uren verbonden aan uw baanrollen hebt, berekent het in de begroting opnemen van de middelen op het gebied van de Begroting van het Middel het **begrote arbeidskosten** van het project. De begrote arbeidskosten worden getoond in het gebied van de Begroting van het Middel van het BedrijfsGeval en in het BedrijfsGevallenoverzicht.

   >[!TIP]
   Kostendenvertoningen in het BedrijfsGeval in de valuta van het project.

   De informatie over budgettering die in het bedrijfscase wordt gespecificeerd, wordt ook getoond in de Planner van het Middel.
