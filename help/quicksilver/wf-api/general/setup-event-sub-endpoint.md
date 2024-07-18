---
content-type: api
navigation-topic: general-api
title: Vereisten voor levering van abonnementen
description: Vereisten voor levering van abonnementen
author: Becky
feature: Workfront API
role: Developer
exl-id: 1b621b35-6c8b-4f6a-bcba-ed6cbfe83a8c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---


# Vereisten voor levering van abonnementen

Abonnementsberichten voor gebeurtenissen zijn meldingen die kunnen worden ingesteld om gebruikers op de hoogte te stellen wanneer bepaalde gebeurtenissen zich voordoen. Meer over leren welke Abonnementen van de Gebeurtenis [ FAQs - de Abonnementen van de Gebeurtenis ](../../wf-api/general/event-subs-faq.md) zien.

## Normen voor de berichtlevering van het Event Subscription

De eindpunten van de dienst die de berichten van het de gebeurtenisabonnement van Adobe Workfront gebruiken moeten aan de volgende basisvereisten voldoen, om ervoor te zorgen dat de berichten correct worden verzonden en ontvangen:

* Het de diensteindpunt moet de verzoeken van de POST van HTTP goedkeuren. De POST van HTTP is de verzoekmethode die in alle leveringen van de berichten van het gebeurtenisabonnement, met inbegrip van bevestigingsberichten wordt gebruikt.

* Opdat het systeem van de levering van het gebeurtenisabonnement bevestigt het bericht met succes werd ontvangen, moet het eindpunt een 200 niveauHTTP- status (bijvoorbeeld, 200 O.K. of 202) voor alle inkomende berichten terugkeren.

* Als een status op 200-niveau niet wordt geretourneerd, gaat het abonnementssysteem van de gebeurtenis ervan uit dat het bericht niet met succes is bezorgd en wordt het juiste hertestbeleid toegepast. Meer over Workfront leren herprobeert beleid, zie [ het abonnementsherpogingen van de Gebeurtenis ](../../wf-api/api/event-sub-retries.md).

* In combinatie met het terugkeren van een 200-niveaustatus als reactiestatus, moet de reactie van HTTP binnen vijf seconden na de leveringspoging worden ontvangen.Deze beperking zorgt ervoor dat de de bedrijfsprocessen van de consument of infrastructuurbeperkingen de levering van andere berichten in afwachting van levering niet vertragen.

* Als een langdurig bedrijfsproces wordt geactiveerd via een gebeurtenisabonnementbericht, raadt Workfront aan  dat

   1. het eindpunt bewaart de berichtinformatie op ontvangstbewijs en antwoordt onmiddellijk met een 200 niveaustatus.
   1. Nadat een eindpunt op een verzoek van de gebeurtenisabonnementlevering heeft gereageerd, kunnen de bewaarde berichten worden verwerkt.
