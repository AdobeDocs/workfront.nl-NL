---
content-type: api
navigation-topic: general-api
title: Aanbevolen werkwijzen voor abonnementen op gebeurtenissen
description: Aanbevolen werkwijzen voor abonnementen op gebeurtenissen
author: John
feature: Workfront API
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 50675b7af3fcd2188a18391732a93a7b67454db9
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Aanbevolen werkwijzen voor abonnementen op gebeurtenissen

Adobe Workfront Event Subscription messages worden automatisch verzonden vanuit Workfront nadat u de service correct hebt geconfigureerd en een Event Subscription hebt gemaakt om deze berichtleveringen te activeren. Ga voor meer informatie over het correct instellen van gebeurtenisabonnementen naar [Vereisten voor levering van abonnementen](../../wf-api/general/setup-event-sub-endpoint.md).


Hieronder vindt u een aantal tips en trucs waarmee u op effectieve wijze gebeurtenisabonnementen kunt maken.

## Geef alle vereiste velden voor aanvraagbody op

Zorg ervoor dat alle vereiste velden voor de aanvraaghoofdtekst naar de API worden verzonden. Voor informatie over alle vereiste aanvraagkenmerken raadpleegt u [Event Subscription API](../../wf-api/general/event-subs-api.md).

## Vermijd het gebruik van extra tekstvelden

Neem geen extra tekstvelden op in de aanvraag, omdat dit ertoe leidt dat de API er niet in slaagt om een abonnement te maken.

## Volledige tests binnen de respijtperiode

Probeer alle abonnementstests binnen de respijtperiode van 100 berichten uit te voeren. Voor meer informatie over deze respijtperiode raadpleegt u [Veelgestelde vragen - Abonnementen voor gebeurtenissen](../../wf-api/general/event-subs-faq.md).

## Voldoe aan de standaardvereisten voor levering van berichten voor abonnementen voor gebeurtenissen

Zorg ervoor uw abonnementseindpunt aan de StandaardVereisten van de Levering van het Bericht van het Abonnement van de Gebeurtenis voldoet. Zie voor meer informatie over deze vereisten [Vereisten voor levering van abonnementen](../../wf-api/general/setup-event-sub-endpoint.md).

## IP van de Lijst van gewenste personen adressen door globaal gebied

Als u via uw firewall gebeurtenisabonnementen wilt ontvangen, moet u de IP-adressen per regio aan de lijst van gewenste personen toevoegen. Zie voor meer informatie [Event Subscription API](../../wf-api/general/event-subs-api.md).

## Beschikken over het juiste toegangsniveau en een API-sleutel

Uw Workfront-gebruiker heeft het volgende nodig om een gebeurtenissenabonnement te maken, te vragen of te verwijderen:

* Een toegangsniveau van **Systeembeheerder**
Zie voor meer informatie [Volledige administratieve toegang verlenen aan een gebruiker](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) of [Gebruikers administratieve toegang verlenen tot bepaalde gebieden](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Een API-sleutel

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more, see .</p>
  -->
