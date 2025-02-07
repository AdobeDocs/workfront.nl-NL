---
content-type: api
navigation-topic: api-navigation-topic
title: Abonnementspogingen voor gebeurtenissen opnieuw proberen
description: Abonnementspogingen voor gebeurtenissen opnieuw proberen
author: Becky
feature: Workfront API
role: Developer
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Abonnementspogingen voor gebeurtenissen opnieuw proberen

Wanneer het uitvoeren van een systeem van de berichtlevering is er een paar bedenkingen die moeten worden gericht om stabiliteit, consistentie, en goede gebruikerservaring te verzekeren. Één van de tekortkomingen van een systeem van de berichtlevering zorgt ervoor dat de berichten hun bestemming met succes bereiken en weten wat te doen wanneer de berichten niet aankomen.

Sommige integraties kunnen mislukking van levering goedkeuren, en dan het bericht laten vallen en naar het volgende bericht bewegen.  In andere integraties kan het niet leveren van een bericht niet worden genegeerd. Bijvoorbeeld, zou een financiële integratie kunnen proberen om een bericht te leveren, maar in plaats daarvan ontvangt een de statuscode van HTTP van 404, die erop wijst de server niet het eindpunt kon vinden waaraan het bericht moest worden geleverd. In dergelijke gevallen zou een ontbrekende boodschap kunnen betekenen dat iemand niet voor zijn tijd wordt betaald of dat een organisatie de begroting overdraagt met gecontracteerde middelen.

## Adobe Workfront-strategie voor abonnementstrips voor gebeurtenissen

Omdat klanten het Workfront-platform gebruiken als een essentieel onderdeel van hun dagelijkse kennisactiviteiten, biedt het Workfront Event Subscription Framework een mechanisme om ervoor te zorgen dat de levering van elk bericht zoveel mogelijk wordt geprobeerd.

Gebeurtenis-teweeggebrachte uitgaande berichten die er niet in slagen om aan klanteneindpunten te worden geleverd zijn opnieuw aanwezig tot de levering voor een periode van 48 uren succesvol is. Tijdens deze tijd, komen opnieuw proberen met een incrementele verhoogde frequentie voor tot de levering succesvol is of tot 11 pogingen zijn gedaan.

De formule voor deze pogingen is:

`((2^attempt) - 1) * 84800ms`

De eerste poging wordt na 1,5 minuten opnieuw uitgevoerd, de tweede na bijna 5 minuten en de 11e na ongeveer 48 uur.

De klanten moeten ervoor zorgen dat om het even welke eindpunten die uitgaande berichten van de Abonnementen van de Gebeurtenis van Workfront verbruiken opstelling zijn om een 200-niveau antwoordbericht terug naar Workfront terug te keren wanneer de levering succesvol is.

## Uitgeschakelde en bevroren abonnementsregels

* Een abonnement URL wordt onbruikbaar gemaakt **als het een mislukkingstarief meer dan 70% met meer dan 100 pogingen heeft OF als het 2.000 opeenvolgende mislukkingen heeft**
* Een abonnement URL wordt bevroren **als het meer dan 2.000 opeenvolgende mislukkingen heeft en het laatste succes meer dan 72 uur geleden OF als het 50.000 opeenvolgende mislukkingen in om het even welk tijdkader heeft.**
* A **gehandicapte** abonnement URL zal blijven levering proberen om de 10 minuten en zal met een succesvolle levering opnieuw worden toegelaten.
* A **bevroren** abonnement URL zal nooit levering proberen tenzij het manueel door een API verzoek te maken wordt toegelaten.




<!--

## Handling Failed Event-Triggered Outbound Messages

The following flowchart shows the strategy for reattempting message deliveries with Workfront Event Subscriptions:

![Event sub retries](assets/event-subscription-circuit-breaker-retries-350x234.png)

The following explanations correspond with the steps depicted in the flowchart:

1. Message fails to be delivered. 
1. Message delivery failure information is logged.

   All failed attempts to deliver a message are logged so that debugging may be performed to determine the root cause of a given failure or series of failures. 

1. URL failures incremented. 
1. Message attempt count is incremented. 
1. Calculate the delay until this message's delivery will be attempted again. 
1. Message is placed onto the message retry queue.

   As shown in the preceding flowchart, the message queue used for processing message delivery retries is a separate queue from the one that processes the initial delivery attempt for each message. This allows the near real-time flow of messages to continue unimpeded by the failure of any subset of messages. 

1. URL circuit status is evaluated. One of the following occurs:

   * If the circuit is open and not allowing deliveries at this time, restart the process at step 5.
   * If the circuit is half-open, this implies that our circuit is currently open, but enough time has passed to allow testing of the URL to see if the problem with delivering to it has been resolved.
   * If the message delivery attempt limits have been reached (48 hours of retrying) then the message is dropped

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1 

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1.
   -->
