---
product-area: resource-management;projects
navigation-topic: resource-planning
title: Prioriteit geven aan projecten in de functie voor middelenplanner
description: De projecten zijn vermeld in orde van prioriteit in de Planner van het Middel met het belangrijkste project bij de bovenkant.
author: Lisa
feature: Resource Management
exl-id: fe9c8cf9-f1e0-4cd5-9299-0f04893d71a5
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1308'
ht-degree: 0%

---

# Prioriteit geven aan projecten in de functie Bronnen

De projecten zijn vermeld in orde van prioriteit in de Planner van het Middel met het belangrijkste project bij de bovenkant.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
    <td><p>Nieuw: alle</p>
       <p>of</p>
       <p>Huidig: Pro of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot resourcebeheer bewerken, inclusief toegang tot bewerkingsprioriteiten en begrotingstijden in de bronnenplanner</p> <p>Toegang tot financiële gegevens, projecten en gebruikers bewerken</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Beheer machtigingen voor de projecten waarvoor u begrotingsgegevens wilt maken met de mogelijkheid om financiën te beheren</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## De standaardorde van projecten in de Planner van het Middel

Door gebrek, zijn de projecten vermeld in de Mening van het Project van de Planner van het Middel door de hieronder criteria in overweging te nemen.

>[!IMPORTANT]
>
>De projecten worden vermeld volgens de drie hieronder criteria slechts de eerste keer u de Planner van het Middel opent. Nochtans, wordt deze standaardprioriteit automatisch uw douaneprioriteit en kan niet aan de originele prioriteit worden teruggekeerd om het even welke tijd u één van het volgende doet:
>
>* Wanneer u op Opslaan klikt.
>* Wanneer u manueel de project planningsprioriteit verandert. Voor informatie over het veranderen van de project planningsprioriteit manueel, zie de sectie [&#x200B; manueel de Prioriteit van de Planning van het Project &#x200B;](#manually-change-the-project-planning-priority) in dit artikel veranderen.
>
>Nadat de projectprioriteit uw douaneprioriteit wordt, beïnvloeden om het even welke veranderingen in de projectinformatie niet meer de orde van de projecten gebruikend deze criteria. Daarna, kunt u projecten slechts manueel voorrang geven.

De oorspronkelijke standaardcriteria voor het een lijst maken van de projecten in de Mening van het Project zijn als volgt, in deze orde:

1. Door de Score van de Uitlijning op het project.\
   Voor meer informatie over de Score van de Uitlijning van het project, zie [&#x200B; een scorecard op een project toepassen en een Score van de Uitlijning &#x200B;](../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md) produceren.

1. Door de Geplande Datum van het Begin van het project (als het gebied van de Uitlijning ongeldig is of het zelfde voor verscheidene projecten) is.
1. Alfabetisch (als het veld Uitlijning null is of hetzelfde is en de geplande begindatum voor verschillende projecten gelijk is).

Overweeg het volgende wanneer het werken met projectprioriteiten in de Planner van het Middel:

* U kunt de projectprioriteit manueel aanpassen slechts wanneer u de Mening van het Project toepast. Dit verandert ook de orde van de projecten in de Planner van het Middel.
* Wanneer u de Rol of de Mening van de Gebruiker in de Planner van het Middel toepast, verschijnen de projecten in de zelfde orde van prioriteit die in de Mening van het Project wordt gevestigd.
* De orde van de projecten in de Planner van het Middel is uniek aan u. Andere gebruikers kunnen de zelfde projecten in de Planner van het Middel, maar in een verschillende orde bekijken. U kunt niet op het gebied van de Prioriteit van de Planning van het Project melden. Dit is zichtbaar enkel in de Planner van het Middel en het dient als vlag voor het prioriteren van uw projecten.

Projecten die aan een portfolio zijn gekoppeld, kunnen een prioriteit op portfolioniveau hebben. U kunt het bekijken van de portfolioprioriteit van een project in de Planner van het Middel, naast de prioriteit van de Planner van het Middel toelaten. U kunt de projecten volgens hun portefeuilleprioriteit ook opdracht geven.

## De projectplanningsprioriteit handmatig wijzigen {#manually-change-the-project-planning-priority}

U moet Edit toegang tot het Beheer van het Middel hebben en toestemmingen beheren aan projecten, om projecten in de Planner van het Middel te herschikken.

Door projecten een nieuwe prioriteit te geven, kunt u ze in volgorde van belangrijkheid rangschikken.

De projectplanningsprioriteit bewerken:

1. Ga naar de **Planner van het Middel**.

1. Klik binnen het gebied links van de projectnaam die een aantal bevat, en ga een aantal in om de Prioriteit van de Planning te veranderen, dan te drukken binnengaan.\
   ![&#x200B; Prioriteit van de Planning van de Verandering &#x200B;](assets/mceclip4.png)\
   of\
   Houd de muisaanwijzer boven de naam van het project en klik op de indicator links van de naam van het project en sleep het project naar de juiste plaats om de prioriteit te wijzigen.

   ![&#x200B; drag_and_drop_projects_RP__1_.png &#x200B;](assets/drag-and-drop-projects-rp--1--350x184.png)

   Wanneer u aantallen selecteert om aan projecten voorrang te geven, selecteer lagere aantallen voor hogere (belangrijkere) prioriteiten, en hogere aantallen voor lagere (minder belangrijke) prioriteiten. Wanneer u het prioritaire aantal van een project in een lager aantal (hogere prioriteit) verandert, verschuiven alle andere projecten in de Planner van het Middel onderaan op de lijst (minder belangrijk worden).\
   Wanneer u het prioriteitsaantal van een project in een hoger aantal (lagere prioriteit) verandert, verschuiven alle andere projecten in de Planner van het Middel omhoog op de lijst (worden belangrijker).

1. Klik **sparen**.\
   De orde van de projecten verandert volgens uw selecties en dit wordt uw prioriteit van het douaneproject in de Planner van het Middel. Andere gebruikers kunnen uw orde van prioriteit voor de projecten in de Planner van het Middel niet zien, hoewel zij de zelfde projecten in hun Planners van het Middel zouden kunnen bekijken.

## Projecten bestellen volgens hun Portfolio-prioriteit in de functie voor middelenplanner

>[!IMPORTANT]
>
>Uw bedrijf moet een bedrijfs of hoger plan van Workfront hebben om projecten in Portfolio Optimizer voorrang te geven.
>
>Voor meer informatie over de plannen van Workfront, zie [&#x200B; Onze Abonnementen &#x200B;](https://business.adobe.com/nl/products/workfront/pricing.html).
>
>Voor informatie over het prioriteren van projecten in Portfolio optimaliseert, zie [&#x200B; projecten in de Optimizer van Portfolio &#x200B;](../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md) Prioritize.

1. Open de **Planner van het Middel** in de **Mening van het Project**.
1. Klik het **pictogram van Montages**.
1. Laat **het plaatsen van de Prioriteiten van Portfolio van de Vertoning** toe om de projectprioriteiten volgens Portfolio te tonen zij aan worden toegewezen. De prioriteit van de projecten volgens hun portefeuilles toont naast de prioriteit van de Planner van het Middel. Deze instelling is standaard uitgeschakeld.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: check screen shot to see if this is accurate still - should say Order, and not Sort:)</p>
   -->

   ![&#x200B; prioriteit van Portfolio &#x200B;](assets/rp-portfolio-priority-unordered-edit-350x180.png)

   De portefeuilleprioriteiten van de projecten worden alleen weergegeven in de projectweergave van de bronnenplanner.

1. Klik **Orde** om tot de projecten volgens de portefeuilleprioriteiten opdracht te geven.

   Als u projecten hebt die tot meer dan één portefeuille behoren, kon u veelvoudige projecten met de zelfde portfolioprioriteit in de Planner van het Middel zien. In dit geval worden de projecten met dezelfde portefeuilleprioriteit opgesomd aan de volgende criteria, in deze volgorde:

   1. Uitlijningsscore
   1. Geplande begindatum
   1. Projectnaam

   ![&#x200B; Portfolio prioriteit bevolen &#x200B;](assets/rp-portfolio-priority-ordered-350x198.png)

1. Klik **sparen**.

## Het effect van het veranderen van de Prioriteit van de Planning van het Project op Beschikbare Uren van de Gebruiker

De prioriteit van de Planning van het Project beïnvloedt de Beschikbare Uren van gebruikers. De gebruikers verbonden aan het project met de hoogste prioriteit tonen hun volledige beschikbaarheid voor de Beschikbare kolom van Uren (AVL) voor dit project, volgens hun programma&#39;s.

Dezelfde gebruikers die bij het tweede project in volgorde van prioriteit betrokken zijn, zullen een waarde van Beschikbare uren laten zien, die het verschil is tussen hun volledige bedrag van Beschikbare Uren en wat reeds voor het eerste project in de kolom Begrotingsuren is begroot, etc. Voor informatie over het opnemen van middelen in de Planner van het Middel, zie [&#x200B; middelen van de Begroting in de Planner van het Middel gebruikend de meningen van het Project en van de Rol &#x200B;](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

Als er geen uren zijn begroot voor het eerste project (in volgorde van prioriteit) voor een gebruiker, maar er uren zijn begroot voor het tweede project voor dezelfde gebruiker, zal de gebruiker het volledige aantal beschikbare uren voor beide projecten tonen.

Wij adviseren het bijwerken van de Begroeide kolom van Uren voor uw gebruikers in de orde van de projecten in de Planner van het Middel, om ervoor te zorgen dat u de Beschikbare Uren voor de gebruiker op elk ogenblik nauwkeurig kunt zien.

>[!NOTE]
>
>Omdat de Prioriteit van de Planning van het Project aan elke middelmanager uniek is, zou uw tweede prioritaire project een eerste prioritair project voor een andere gebruiker kunnen zijn die de zelfde projecten in hun Planner van het Middel bekijken. Als een andere middelmanager een middel voor hun eerste project budgetteert, zullen de Beschikbare Uren voor dat middel voor uw eerste project verminderen dat op die verandering wordt gebaseerd.
>
>De gebruiker die de uren begroot wijst eerst dat middel toe en vermindert het aantal Beschikbare Uren voor dat middel over het systeem. De hoeveelheid beschikbare uren moet voor alle gebruikers worden bijgewerkt zodra de begrote uren uren voor een resource in de Resource Planner zijn opgeslagen.
>
>Voor meer informatie over Beschikbare Uren, zie [&#x200B; Beschikbaarheid en toewijzing van middelen &#x200B;](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#availability-and-allocation-of-resources).
