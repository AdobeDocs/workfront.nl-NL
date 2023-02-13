---
content-type: api
navigation-topic: api-navigation-topic
title: Abonnementspogingen voor gebeurtenissen opnieuw proberen
description: Abonnementspogingen voor gebeurtenissen opnieuw proberen
author: John
feature: Workfront API
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 606d19b8a83b833aba6d6b15231a8683aa2cee40
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Abonnementspogingen voor gebeurtenissen opnieuw proberen

Wanneer het uitvoeren van een systeem van de berichtlevering is er een paar bedenkingen die moeten worden gericht om stabiliteit, consistentie, en goede gebruikerservaring te verzekeren. Één van de tekortkomingen van een systeem van de berichtlevering zorgt ervoor dat de berichten hun bestemming met succes bereiken en weten wat te doen wanneer de berichten niet aankomen.

Sommige integraties kunnen mislukking van levering goedkeuren, en dan het bericht laten vallen en naar het volgende bericht bewegen.  In andere integraties kan het niet leveren van een bericht niet worden genegeerd. Bijvoorbeeld, zou een financiële integratie kunnen proberen om een bericht te leveren, maar in plaats daarvan ontvangt een de statuscode van HTTP van 404, die erop wijst de server niet het eindpunt kon vinden waaraan het bericht moest worden geleverd. In dergelijke gevallen zou een ontbrekende boodschap kunnen betekenen dat iemand niet voor zijn tijd wordt betaald of dat een organisatie de begroting overdraagt met gecontracteerde middelen.

## Adobe Workfront-strategie voor abonnementstrips voor gebeurtenissen

Omdat klanten het Workfront-platform gebruiken als een essentieel onderdeel van hun dagelijkse kennisactiviteiten, biedt het Workfront Event Subscription Framework een mechanisme om ervoor te zorgen dat de levering van elk bericht zoveel mogelijk wordt geprobeerd.

Gebeurtenis-teweeggebrachte uitgaande berichten die er niet in slagen om aan klanteneindpunten te worden geleverd zijn opnieuw aanwezig tot de levering voor een periode van 48 uren succesvol is. Tijdens deze tijd, komen de pogingen met een incrementeel verminderde frequentie voor tot de levering succesvol is of tot 48 uur is verstreken.

De klanten moeten ervoor zorgen dat om het even welke eindpunten die uitgaande berichten van de Abonnementen van de Gebeurtenis van Workfront verbruiken opstelling zijn om een 200-niveau antwoordbericht terug naar Workfront terug te keren wanneer de levering succesvol is.

## Afhandeling mislukte gebeurtenisgestuurde uitgaande berichten

In het volgende stroomschema ziet u de strategie voor het genereren van berichtleveringen met Workfront Event-abonnementen:

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

De volgende uitleg komt overeen met de stappen in het stroomschema:

1. Bericht kan niet worden afgeleverd.
1. Foutgegevens voor berichtlevering worden geregistreerd.

   Alle ontbroken pogingen om een bericht te leveren worden geregistreerd zodat het zuiveren kan worden uitgevoerd om de worteloorzaak van een bepaalde mislukking of een reeks mislukkingen te bepalen.

1. URL-fouten zijn verhoogd.
1. Het aantal pogingen van het bericht wordt verhoogd.
1. Bereken de vertraging tot de levering van dit bericht opnieuw wordt geprobeerd.
1. Het bericht wordt geplaatst op de rij van het bericht opnieuw probeert.

   Zoals aangetoond in het voorafgaande stroomschema, is de berichtrij die voor de herpogingen van de verwerkingsberichtlevering wordt gebruikt een afzonderlijke rij van die wordt gebruikt die de aanvankelijke leveringspoging voor elk bericht verwerkt. Dit staat de dichtbij stroom in real time van berichten toe om onbelemmerd door de mislukking van om het even welke ondergroep van berichten verder te gaan.

1. De status van de URL-circuit wordt geëvalueerd. Een van de volgende situaties doet zich voor:

   * Als de kring open is en levering op dit ogenblik niet toestaat, begin het proces bij stap 5 opnieuw.
   * Als de kring half-open is, impliceert dit dat onze kring momenteel open is, maar genoeg tijd is overgegaan om het testen van URL toe te staan om te zien of is het probleem met het leveren aan het opgelost.
   * Als de limieten voor de poging tot het verzenden van berichten zijn bereikt (48 uur na het opnieuw proberen), wordt het bericht verwijderd

1. Als de kring URL wordt gesloten en leveringen toestaat, probeer om het bericht te leveren. Als deze levering ontbreekt, zal het bericht bij stap 1 opnieuw beginnen

1. Als de kring URL wordt gesloten en leveringen toestaat, probeer om het bericht te leveren. Als deze levering ontbreekt, zal het bericht bij stap 1 opnieuw beginnen.

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront disables Event Subscriptions when both of the following criteria are met:
   <ul>
   <!--
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The Event Subscription has failed 1000 delivery attempts consecutively</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">48 hours have passed since the last successful delivery</li>
   </ul></li>
   -->
