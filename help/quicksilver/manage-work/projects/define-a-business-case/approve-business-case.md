---
navigation-topic: business-case-and-scorecards
title: Een bedrijfscase goedkeuren
description: Nadat u de Business Case voor een projectverzoek hebt voltooid en ingediend, moet de Business Case zijn goedgekeurd. Dit hangt van het werkschema in uw organisatie af. Een project kan zonder de BedrijfsGeval beginnen die moet worden goedgekeurd, maar uw beheerder van Adobe Workfront en projecteigenaars zouden het niet ideaal kunnen vinden om dit te doen.
author: Alina
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
source-git-commit: 9cfb67f627c06a5926e820860d52ba9f1ab58bcf
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 0%

---

# Een bedrijfscase goedkeuren

Nadat u de Business Case voor een projectverzoek hebt voltooid en ingediend, moet de Business Case zijn goedgekeurd. Dit hangt van het werkschema in uw organisatie af. Een project kan zonder de BedrijfsGeval beginnen die moet worden goedgekeurd, maar uw beheerder van Adobe Workfront en projecteigenaars zouden het niet ideaal kunnen vinden om dit te doen.

Voor meer informatie over de voltooiing van en het voorleggen van een BedrijfsGeval, zie het artikel [ een BedrijfsGeval voor een project ](../../../manage-work/projects/define-a-business-case/create-business-case.md) creëren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> 
   <p>Huidig: Prime of hoger</p> 
   <p>Verouderd: Pro of hoger</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Huidig: Standaard </p> 
   <p>Verouderd: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een project beheren</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overzicht van goedkeuring van bedrijfscase

Overweeg het volgende wanneer het goedkeuren van een BedrijfsGeval van een project:

* U moet over beheerdersmachtigingen voor een project beschikken om de Business Case voor het project goed te keuren.
* U zult niet de projecten kunnen zien die op het BedrijfsGeval wachten om onder Mijn Goedkeuringen widget in Huis worden goedgekeurd.
* U moet manueel naar de individuele projecten gaan die goedkeuring van het BedrijfsGeval nodig hebben om te zien dat zij in afwachting van goedkeuring zijn. Er is geen Workfront-meldingsmechanisme waarmee iemand wordt gewaarschuwd dat hij of zij de Business Case van een project moet goedkeuren.
* U kunt de projecten vinden die op de goedkeuring van het BedrijfsGeval wachten of door een projectrapport te bouwen, of door tot de portefeuille toegang te hebben zij met worden geassocieerd.

  Voor meer informatie over Portfolio&#39;s, zie het artikel [ overzicht van Portfolio in Adobe Workfront ](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

## De bedrijfscase goedkeuren door een projectrapport op te stellen

U kunt een rapport voor projecten bouwen om te zien welke projecten hun goedgekeurd BedrijfsGeval nodig hebben.

Een rapport opstellen voor projecten die in afwachting zijn van de goedkeuring van hun zaken:

1. Maak een rapport voor projecten.

   Voor meer informatie over het creëren van rapporten, zie het artikel [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

1. Selecteer het **lusje van de Mening** van het rapport, dan klik **toevoegen Kolom**.

1. Begin typend &quot;Status&quot;in **tonen in dit kolom** gebied, en selecteer dit gebied wanneer het in de lijst verschijnt.

   Deze kolom zal de status van de projecten tonen.

1. Selecteer het **lusje van Filters** van het rapport, dan klik **voeg een Regel van de Filter** toe.

1. Begin typend &quot;Status&quot;in **toont me slechts Projecten waarin het...** gebied, en selecteert het wanneer het in de lijst verschijnt.
1. Selecteer **Gelijk** voor de filterbepaling.
1. Typ &quot;Gevraagd&quot; in het beschikbare veld.

   Dit zorgt ervoor dat het rapport slechts projecten omvat die in de Gevraagde status zijn.

   ![ requested_projects_filter.png ](assets/requested-projects-filter-350x14.png)

1. (Facultatief) klik **voeg een andere Regel van de Filter toe**.

   U kunt extra filters toevoegen om alleen projecten weer te geven waar u de eigenaar van het project bent, of de sponsor van het project of de eigenaar van Portfolio.

   U kunt bijvoorbeeld de volgende filterinstructies gebruiken:

   ```
   Project Sponsor ID Equals $$USER.ID
   ```

   om projecten weer te geven waar u als projectsponsor bent aangewezen

   ```
   Project Owner ID Equals $$USER.ID
   ```

   om projecten te tonen waar u als eigenaar van het Project wordt aangewezen

   ```
   Project Portfolio Owner ID Equals $$USER. ID
   ```

   om te tonen waar u als Manager van Portfolio wordt aangewezen.

1. Klik **sparen+Sluiten**.

   Bericht dat alle projecten in het rapport in het statuut van **Gevraagde** zijn.

1. Klik op de naam van een project in het rapport om het te openen.
1. Klik **Bedrijfs Geval** in het linkerpaneel.
1. Klik **goedkeuren** of **verwerping** in het BedrijfsGeval Summiere gebied om het BedrijfsGeval goed te keuren of te verwerpen.

   ![ Bedrijfs geval ](assets/business-case-summary-with-rp-information--1-.png)

   De projectstatus wordt veranderd in **Goedgekeurd** als het BedrijfsGeval wordt goedgekeurd.

   De projectstatus wordt veranderd in **Verworpen** als het Bedrijfs geval wordt verworpen.

   >[!NOTE]
   >
   >Er zijn geen meldingen die de gebruiker die de goedkeuring van de bedrijfscase heeft ingediend, waarschuwen of zijn projectaanvraag is goedgekeurd of afgewezen.

## Goedkeuren van de bedrijfscase door toegang te krijgen tot aangevraagde projecten in een portfolio

Voor meer informatie over het herzien van Gevraagde projecten, zie het artikel [ Overzicht Gevraagde Projecten ](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).
