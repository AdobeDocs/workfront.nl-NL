---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Verbeteringen in het beheer van hulpbronnen
description: Deze pagina beschrijft alle verbeteringen in het beheer van hulpbronnen die zijn aangebracht met de versie 20.3 in de productieomgeving. Deze verbeteringen zijn beschikbaar gesteld in de productieomgeving in de week van 10 augustus 2020.
author: Luke
feature: Product Announcements
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 0%

---

# 20.3 Verbeteringen in het beheer van hulpbronnen

Deze pagina beschrijft alle verbeteringen in het beheer van hulpbronnen die zijn aangebracht met de versie 20.3 in de productieomgeving. Deze verbeteringen zijn beschikbaar gesteld in de productieomgeving in de week van 10 augustus 2020.

Voor een lijst van alle veranderingen beschikbaar met versie 20.3, zie [20.3 - releaseoverzicht](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## Uren opnemen uit uitgaven in het werkgebied Toegewezen werklastbalans

Om u een volledig beeld van al uw werklasten van mensen te laten zien, hebben wij een het plaatsen geïntroduceerd die u toestaat om uren van kwesties in het Toegewezen Werkgebied van de Balancer van de Werkbelasting te omvatten.

Voor informatie over het werken in de Balancer van de Werkbelasting, zie [Navigeren door werklastbalans](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Toewijzingen aanpassen voor niet-werkdagen in werklastbalans

U kunt toewijzingen voor uw bronnen voor niet-werkdagen aanpassen met behulp van Workload Balancer.

Voor informatie over het beheren van toewijzingen in het werklastevenwicht raadpleegt u [Toewijzingen van gebruikers beheren in Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Variabele filters beschikbaar in Workload Balancer

Om uw ervaring te verbeteren en u meer flexibiliteit te geven wanneer u informatie deelt, hebben wij nu veranderlijke filters voor de Balancer van de Werkbelasting uitgevoerd. De volgende filters zijn toegevoegd aan Workload Balancer:

* &quot;Me&quot; (bij het filtreren door gebruikers)
* &quot;Mijn primaire rol&quot; (bij het filteren op rollen)
* &quot;Mijn Team van het Huis&quot;of &quot;Al Mijn Teams&quot; (wanneer het filtreren door teams).

Deze filters vervangen de jokertekenfiltervariabelen $$USER.ID, $$USER.roleID, $$USER.homeTeamID en $$USER.teamID&#39;s

Wanneer u een van deze filters toepast en vervolgens de werklastbalans deelt of op een dashboard plaatst, zien alle andere gebruikers hun eigen gegevens.

Zie voor informatie over het toepassen van filters op de werklastbalans [Gegevens in de werklastbalans filteren](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Nieuwe sortering voor projecten in het werklastevenwicht

De werklastbalans sorteert nu de projecten op basis van de vroegste geplande begindatum en op basis van de laatste geplande einddatum van de taken in het project die plaatsvinden tijdens het tijdsbestek dat de gebruiker op het scherm weergeeft. Hierdoor kunt u het werk ordenen in een boomachtige hiërarchie, zodat u het werk voor een dag gemakkelijker kunt identificeren.

Voor informatie over het bekijken van projecten en het werkpunten in de Balancer van de Werkbelasting, zie [Navigeren door werklastbalans](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Werklastbalans weergeven

Om u een nauwkeurig perspectief van de vooruitgang van uw werkbelasting te geven, hebben wij een nieuwe het plaatsen in de Balancer van de Werkbelasting geïntroduceerd die de chronologie van taken en kwesties volgens hun Geprojecteerde Datums toont. U kunt de instelling Geprojecteerde datums weergeven inschakelen om naast de geplande tijdlijn de geprojecteerde tijdlijn van het werkitem weer te geven.

Als met deze verbetering een taak of een kwestie eerder wordt voltooid dan de geplande Voltooiingsdatum, worden de toegewezen uren van de resterende dagen doorgehaald om aan te geven dat zij niet meetellen voor de totale toewijzing van de gebruiker.

Voor informatie over het navigeren door de werklastverdeler en het inschakelen van instellingen raadpleegt u [Navigeren door werklastbalans](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Functies voor werklastverdeling die eerder werden meegedeeld als releasing met de release van 20.2

* [De dagelijkse en wekelijkse toewijzing in de werklastbalans aanpassen](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [Taak geplande uren bijwerken in werklastbalans](#update-task-planned-hours-in-the-workload-balancer)
* [Een handigere manier om toewijzingen bij te werken in het werklastevenwicht](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### De dagelijkse en wekelijkse toewijzing in de werklastbalans aanpassen {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

U kunt de dagelijkse en wekelijkse toewijzing van uw gebruikers nu aanpassen aan uw werklastbalans om te voorkomen dat uw bronnen worden gebrand.

Voorafgaand aan deze verhoging, was dit slechts mogelijk gebruikend het Middel dat hulpmiddelen plant.

Voor informatie over het beheren van toewijzingen in het werklastevenwicht raadpleegt u [Toewijzingen van gebruikers beheren in Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

**Beschikbaar in deze omgevingen:**

* Adobe Workfront Classic
* De nieuwe Adobe Workfront-ervaring

### Taak geplande uren bijwerken in werklastbalans {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>Deze verbetering zal in Productie kort na de versie van 2020.2 beschikbaar zijn.

Een nieuwe optie in het gebied van het Beheer van het Middel van het toegangsniveau staat nu gebruikers met deze toegang toe om Geplande Uren van de Balancer van de Werkbelasting uit te geven. Wanneer u toewijzingen aanpast in het werklastevenwicht, hoeft het totaal van de dagelijkse toewijzingen niet overeen te komen met het aantal geplande uren van de taken. Als u uw toewijzingen hebt opgeslagen, wordt het totaal van de toewijzingstijden de geplande uren van de taak. Dit is alleen mogelijk voor taken met een eenvoudig type duur.

Voor informatie over het beheren van toewijzingen in het werklastevenwicht raadpleegt u [Toewijzingen van gebruikers beheren in Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Voor informatie over het verlenen van toegang tot het Beheer van het Middel, zie [Toegang verlenen tot beheer van hulpbronnen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

### Een handigere manier om toewijzingen bij te werken in het werklastevenwicht {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

Om het gemakkelijker te maken om de toewijzingen van een gebruiker aan een het werkpunt in de Balancer van de Werkbelasting te beheren, kunt u het het werkpunt nu tweemaal klikken. U kunt ook nog steeds de bestaande menuoptie Toewijzingen bewerken gebruiken. Bovendien hoeft u de weergave van toewijzingen niet meer in te schakelen om deze bij te werken.

Voor informatie over het beheren van toewijzingen in het werklastevenwicht raadpleegt u [Toewijzingen van gebruikers beheren in Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
