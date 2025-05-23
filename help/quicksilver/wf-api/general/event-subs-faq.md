---
content-type: api;faq
navigation-topic: general-api
title: Veelgestelde vragen - Abonnementen voor gebeurtenissen
description: Veelgestelde vragen - Abonnementen voor gebeurtenissen
author: Becky
feature: Workfront API
role: Developer
exl-id: a6120939-5d76-4f46-a304-125de6b22502
source-git-commit: 074f78e27d2ab1cb1d1b8216f14557b91d9afd00
workflow-type: tm+mt
source-wordcount: '973'
ht-degree: 0%

---

# Veelgestelde vragen - Abonnementen voor gebeurtenissen

<!--
{{highlighted-preview}}
-->

Hier volgen vaak gestelde vragen over abonnementen op gebeurtenissen:

## Wat is een abonnement?

Een abonnement is een reeks gegevens die worden gebruikt om de gebeurtenissen van Adobe Workfront aan het eindpunt van HTTP van een klant aan te passen en te leveren. Deze bron bestaat uit vier primaire kenmerken:

* customer_id
* obj_code
* obj_id
* url

Een abonnement kan ook andere kenmerken hebben, zoals een eigen unieke id en de datum waarop het is gemaakt, maar de hierboven vermelde kenmerken worden vooral gebruikt om gebeurtenissen aan te passen en deze aan klanten te leveren.

## Kan ik selecteren welke gebeurtenissen naar een eindpunt worden verzonden dat op bepaalde criteria binnen een gebeurtenislading wordt gebaseerd?

Filters voor gebeurtenisabonnementen zijn een manier waarop subs van gebeurtenissen op opgegeven criteria kunnen worden gesorteerd. Men adviseert dat u filters op gebeurtenisabonnementen toepast aangezien het het aantal berichten kan beduidend verminderen dat een eindpunt moet verbruiken. Voor meer informatie zie [ het abonnement filtreren van de Gebeurtenis ](../../wf-api/general/event-subs-api.md#event).

## Waarom retourneert de API een 409-conflictreactiecode?

Als u een gebeurtenisabonnement probeert te maken en een antwoordcode ontvangt: 409-conflict, is het abonnement dat u probeerde te maken een duplicaat. Workfront staat het maken van dubbele abonnementen niet toe.

## Wat zou ik moeten doen als mijn berichten niet aan mijn eindpunt worden geleverd?

Zoek de volgende scenario&#39;s en gebruik de geadviseerde oplossing:

* Zorg ervoor dat uw abonnement eindpunt-bepaald door **url** gebied-een 2XX de reactiecode van HTTP terugkeert. Als het niet is, contacteer de Steun van Workfront of zie {de leveringsvereisten van het Abonnement van 0} Gebeurtenis [&#128279;](../../wf-api/general/setup-event-sub-endpoint.md).

* Het verzoek om gebeurtenislevering kan een time-out zijn voordat het is voltooid. Zorg ervoor dat uw eindpunt constant binnen 5 seconden antwoordt. Dit is de standaardonderbreking die voor de HTTP- aanvraag wordt geplaatst om een bericht van het Abonnement van de Gebeurtenis te leveren. Als uw eindpunt niet binnen 5 seconden antwoordt, contacteer de Steun van Workfront of zie {de leveringsvereisten van het Abonnement van 0} Gebeurtenis [&#128279;](../../wf-api/general/setup-event-sub-endpoint.md).
* De gebeurtenissen genereren mogelijk niet de manier waarop u denkt. Zorg ervoor dat u geen veronderstellingen maakt over hoe of wanneer gebeurtenissen moeten worden uitgevoerd en dat u niets doet. U zou bijvoorbeeld kunnen denken dat het bijwerken van een document op een taak een gebeurtenis van de taakupdate produceert, maar in plaats daarvan, creeert het een document tot stand brengen of gebeurtenis van de documentupdate.
* Uw abonnement is mogelijk niet geconfigureerd zoals u verwacht. U kunt gebeurtenissenabonnementen in verschillende omgevingen maken en verwachten dat deze op dezelfde manier worden overgedragen als hun andere Workfront-gegevens. Gebeurtenisabonnementsgegevens zijn echter niet geconfigureerd voor het kopiëren of promoten van gegevens naar andere omgevingen. Zorg ervoor dat u API-verzoeken naar de juiste omgeving verzendt en dat de abonnementen in die omgeving op de verwachte wijze zijn geconfigureerd.
* De lading werd niet ontvangen omdat het noodzakelijke adres van Workfront IP niet aan de lijst van gewenste personen op uw firewall is toegevoegd. Gebeurtenissen van het Abonnement van de gebeurtenis worden verzonden van slechts een paar IP adressen. Zorg ervoor dat het bestemmingsnetwerk alle IP uitzonderingen noodzakelijk heeft om ladingen van de Abonnementen van de Gebeurtenis van Workfront te ontvangen.
* De lading werd niet ontvangen omdat het meer dan 1 MB was. Abonnementsberichten of -objecten voor gebeurtenissen mogen niet groter zijn dan 1 MB.

## Waarom duurt het te lang voordat mijn berichten mijn eindpunt bereiken?

Sommige van de volgende scenario&#39;s kunnen verantwoordelijk zijn:

* Een grote verrichting-zulke als bulkupdate-in het systeem kan een groot volume van berichten veroorzaken om allen in één keer worden gevraagd, die wat tijd aan proces kan vergen.
* Lange berekeningen of tijdlijnberekeningen voor grote projecten kunnen leiden tot vertraging bij de publicatie van berichten voor abonnementen op gebeurtenissen.
* Het abonnement is mogelijk uitgeschakeld.

   * Na een periode van de 100 berichtrespijtperiode, als een bepaalde URL (die met één of meerdere abonnementen kon worden geassocieerd) meer dan 70% van de tijd ontbreekt of als URL er niet in slaagt om na 2000 opeenvolgende pogingen te leveren, worden alle berichten die abonnementen met dat zelfde URL aanpassen niet geprobeerd voor levering. In plaats daarvan worden deze berichten direct in de wachtrij geplaatst voor een nieuwe poging.

     Elke 10 minuten nadat een URL is uitgeschakeld, proberen we het volgende bericht te leveren dat wordt weergegeven voor verwerking. Als dat bericht slaagt, dan re-toelaten wij die URL en om het even welke passende abonnementen. Als dat bericht niet verzendt, dan stelt die tijdopnemer 10 minuten terug en wij proberen opnieuw nadat het verloopt.

     Dit gedrag kan worden gezien als inconsistente of vertraagde leveringen, maar het volgt eenvoudig ons beleid voor hoe de berichten van het Abonnement van de Gebeurtenis worden behandeld.

   * Een URL voor een abonnement op een gebeurtenis wordt hard uitgeschakeld als aan een van de volgende voorwaarden wordt voldaan:

      * De abonnements-URL is 7 dagen lang niet bezorgd en heeft in de afgelopen 72 uur ten minste 2000 opeenvolgende leveringspogingen mislukt.
      * De abonnements-URL heeft niet 50.000 opeenvolgende pogingen uitgevoerd.

## Wat zou ik moeten doen als ik een 500 reactiestatus ontvang wanneer ik probeer om het Abonnement API van de Gebeurtenis te roepen?

Neem contact op met Workfront Support. Leren hoe te om steun te contacteren, zie [ de Steun van de Klant van het Contact ](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## Welke verschillende verificatietypen kan ik gebruiken met Workfront Event Subscriptions?

U kunt om het even welke authentificatie gebruiken die een dragertoken gebruikt. Het **authToken** gebied van een abonnement is een koord dat een token vertegenwoordigt OAuth2 dat wordt gebruikt om met URL voor authentiek te verklaren die in het **wordt gespecificeerd url** gebied. In theorie, zou deze symbolische waarde om het even wat onder 255 karakters kunnen zijn zolang het bestemmingshindpunt zich van bewust is hoe te om zijn het coderen te behandelen, die **utf-8** is.

## Hoe lang moet het zijn voordat ik mijn gebeurtenislading van Workfront Event Abonnementen ontvang?

Over het algemeen kunt u verwachten dat u binnen minder dan 5 seconden na de gegevenswijziging die wordt geregistreerd, gebeurtenisleveringsverzoeken voor het abonnement op gebeurtenissen ontvangt. Gemiddeld worden webhaakmeldingen binnen 1 seconde ontvangen vanaf het moment dat de gegevens worden gewijzigd. Nochtans, kan de dienst berichten in zulke grote hoeveelheden ontvangen dat het ook langer zou kunnen duren.

## Aanvullende bronnen

* **API Documentatie**: [ Abonnement API van de Gebeurtenis ](../../wf-api/general/event-subs-api.md)

* **Beste praktijken**: [ beste praktijken van het abonnement van de Gebeurtenis ](../../wf-api/general/event-sub-best-practice.md)

* **Gebieden die de nuttige ladingen van het Abonnement van de Gebeurtenis** teweegbrengen: [ het middelgebieden van het abonnement van de Gebeurtenis ](../../wf-api/api/event-sub-resource-fields.md)

* **Begrijpend de Abonnementen van de Gebeurtenis** opnieuw: [ het abonnementsherangen van de Gebeurtenis ](../../wf-api/api/event-sub-retries.md)

* **Vormend uw firewall voor Workfront**: [ vorm de lijst van gewenste personen van uw firewall ](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)
