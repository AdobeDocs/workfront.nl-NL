---
content-type: api
navigation-topic: general-api
title: Aanbevolen werkwijzen voor abonnementen op gebeurtenissen
description: Aanbevolen werkwijzen voor abonnementen op gebeurtenissen
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 19e0b792bc49ede0504af479952fdbdf384dc73c
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---


# Aanbevolen werkwijzen voor abonnementen op gebeurtenissen

Adobe Workfront Event Subscription messages worden automatisch verzonden vanuit Workfront nadat u de service op de juiste wijze hebt geconfigureerd en een Event Subscription hebt gemaakt om deze berichtleveringen te activeren. Meer over behoorlijk vestiging zien de Abonnementen van de Gebeurtenis, {de leveringsvereisten van het Abonnement van 0} Gebeurtenis [&#128279;](../../wf-api/general/setup-event-sub-endpoint.md).


Hieronder vindt u een aantal tips en trucs waarmee u op effectieve wijze gebeurtenisabonnementen kunt maken.

## Geef alle vereiste velden voor aanvraagbody op

Zorg ervoor dat alle vereiste velden voor de aanvraaghoofdtekst naar de API worden verzonden. Voor informatie over alle vereiste verzoekattributen, te zien gelieve [ Abonnement API van de Gebeurtenis ](../../wf-api/general/event-subs-api.md).

## Vermijd het gebruik van extra tekstvelden

Neem geen extra tekstvelden op in de aanvraag, omdat dit ertoe leidt dat de API er niet in slaagt om een abonnement te maken.

## Volledige tests binnen de respijtperiode

Probeer alle abonnementstests binnen de respijtperiode van 100 berichten uit te voeren. Meer over deze aflossingsperiode leren, zie [ FAQs - de Abonnementen van de Gebeurtenis ](../../wf-api/general/event-subs-faq.md).

## Voldoe aan de standaardvereisten voor levering van berichten voor abonnementen voor gebeurtenissen

Zorg ervoor uw abonnementseindpunt aan de StandaardVereisten van de Levering van het Bericht van het Abonnement van de Gebeurtenis voldoet. Om over deze vereisten te leren, zie {de leveringsvereisten van het Abonnement van 0} Gebeurtenis [&#128279;](../../wf-api/general/setup-event-sub-endpoint.md).

## IP van de Lijst van gewenste personen adressen door globaal gebied

Als u via uw firewall gebeurtenisabonnementen wilt ontvangen, moet u de IP-adressen per regio aan de lijst van gewenste personen toevoegen. Meer leren, zie [ Abonnement API van de Gebeurtenis ](../../wf-api/general/event-subs-api.md).

## Heb het juiste toegangsniveau en de authentificatie

Uw Workfront-gebruiker heeft het volgende nodig om een gebeurtenissenabonnement te maken, te vragen of te verwijderen:

* Een toegangsniveau van **Beheerder van het Systeem**
Meer leren, zie [ een gebruiker volledige administratieve toegang ](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) verlenen of [ gebruikers administratieve toegang verlenen tot bepaalde gebieden ](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Een header `sessionID` is vereist om de API voor abonnementen op gebeurtenissen te gebruiken

  Voor meer informatie, zie [ Authentificatie ](api-basics.md#authentication) in [ API Grondbeginselen ](api-basics.md).
