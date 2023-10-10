---
navigation-topic: business-case-and-scorecards
title: Een bedrijfscase goedkeuren
description: Nadat u de Business Case voor een projectverzoek hebt voltooid en ingediend, moet de Business Case zijn goedgekeurd. Dit hangt van het werkschema in uw organisatie af. Een project kan zonder de BedrijfsGeval beginnen die moet worden goedgekeurd, maar uw beheerder van Adobe Workfront en projecteigenaars zouden het niet ideaal kunnen vinden om dit te doen.
author: Alina
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
source-git-commit: f4ef463ebdc9a4a7a0802e5394d7820ebc447aa9
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 0%

---

# Een bedrijfscase goedkeuren

Nadat u de Business Case voor een projectverzoek hebt voltooid en ingediend, moet de Business Case zijn goedgekeurd. Dit hangt van het werkschema in uw organisatie af. Een project kan zonder de BedrijfsGeval beginnen die moet worden goedgekeurd, maar uw beheerder van Adobe Workfront en projecteigenaars zouden het niet ideaal kunnen vinden om dit te doen. 

Raadpleeg het artikel voor meer informatie over het voltooien en verzenden van een Business Case [Een bedrijfscase maken voor een project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Pro of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een project beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Overzicht van goedkeuring van bedrijfscase

Overweeg het volgende wanneer het goedkeuren van een BedrijfsGeval van een project:

* U moet over beheerdersmachtigingen voor een project beschikken om de Business Case voor het project goed te keuren. 
* U zult niet de projecten kunnen zien die op de BedrijfsGeval wachten om onder uw Goedkeuringen in Huis worden goedgekeurd.
* U moet manueel naar de individuele projecten gaan die goedkeuring van het BedrijfsGeval nodig hebben om te zien dat zij in afwachting van goedkeuring zijn. Er is geen Workfront-meldingsmechanisme waarmee iemand wordt gewaarschuwd dat hij of zij de Business Case van een project moet goedkeuren.
* U kunt de projecten vinden die op de goedkeuring van het BedrijfsGeval wachten of door een projectrapport te bouwen, of door tot de portefeuille toegang te hebben zij met worden geassocieerd. 

  Raadpleeg het artikel voor meer informatie over Portfolio&#39;s [Overzicht van Portfolio&#39;s in Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

## De bedrijfscase goedkeuren door een projectrapport op te stellen

U kunt een rapport voor projecten bouwen om te zien welke projecten hun goedgekeurd BedrijfsGeval nodig hebben. 

Een rapport opstellen voor projecten die in afwachting zijn van de goedkeuring van hun zaken:

1. Maak een rapport voor projecten.

   Zie het artikel voor meer informatie over het maken van rapporten [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Selecteer de **Weergave** tabblad van het rapport en klik vervolgens op **Kolom toevoegen**.

1. Typ &quot;Status&quot; in het dialoogvenster **Tonen in deze kolom** en selecteer dit veld wanneer het in de lijst wordt weergegeven.

    Deze kolom zal de status van de projecten tonen.

1. Selecteer de **Filters** tabblad van het rapport en klik vervolgens op **Filterregel toevoegen**.

1. Typ &quot;Status&quot; in het dialoogvenster **Alleen projecten tonen waarin ...** en selecteert u deze wanneer deze in de lijst wordt weergegeven.
1. Selecteren **Gelijk** voor de filteroptie.
1. Typ &quot;Gevraagd&quot; in het beschikbare veld. 

   Dit zorgt ervoor dat het rapport slechts projecten omvat die in de Gevraagde status zijn.

     ![requested_projects_filter.png](assets/requested-projects-filter-350x14.png)

1. (Optioneel) Klik op **Een andere filterregel toevoegen**.

   U kunt extra filters toevoegen om alleen projecten te tonen waar u de eigenaar van het project bent, of de sponsor van het project of de eigenaar van het Portfolio.

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

   om te tonen waar u als Manager van het Portfolio wordt aangewezen. 

1. Klikken **Opslaan en sluiten**.

   Bericht dat alle projecten in het rapport in de status verkeren **Gevraagd**.

1. Klik op de naam van een project in het rapport om het te openen.
1. Klikken **Bedrijfs-case** in het linkerdeelvenster.
1. Klikken **Goedkeuren** of **Afwijzen** in het gebied Overzicht van bedrijfscase om de Business Case goed te keuren of af te wijzen.

   ![](assets/business-case-summary-with-rp-information--1-.png)

   De projectstatus wordt gewijzigd in **Goedgekeurd** als de Business Case is goedgekeurd.

   De projectstatus wordt gewijzigd in **Geweigerd** als de zaak-Business wordt afgewezen.

   >[!NOTE]
   >
   >Er zijn geen meldingen die de gebruiker die de goedkeuring van de bedrijfscase heeft ingediend, waarschuwen of zijn projectaanvraag is goedgekeurd of afgewezen.

## Goedkeuren van de bedrijfscase door toegang te krijgen tot aangevraagde projecten in een portfolio

Raadpleeg het artikel voor meer informatie over het evalueren van aangevraagde projecten [Gevraagde projecten controleren](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).
