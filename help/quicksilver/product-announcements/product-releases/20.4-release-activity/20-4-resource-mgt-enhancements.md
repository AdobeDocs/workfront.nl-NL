---
title: 20.4 Verbeteringen in het beheer van hulpbronnen
description: 20.4 Verbeteringen in het beheer van hulpbronnen
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9f660a38-4a59-4135-8178-0841088cc7d6
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 0%

---

# 20.4 Verbeteringen in het beheer van hulpbronnen

Op deze pagina worden alle verbeteringen in het beheer van bronnen beschreven die zijn aangebracht met de versie 20.4 voor de voorvertoningsomgeving. Deze verbeteringen worden beschikbaar gesteld in de productieomgeving in de week van 9 november 2020.

Voor een lijst van alle veranderingen beschikbaar met de versie 20.4, zie [&#x200B; overzicht van de versie 20.4 &#x200B;](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Werk plannen met werkinspanning in plaats van geplande uren

Om u flexibiliteit te geven wanneer u het werk aan uw projecten plant, hebben wij het nieuwe concept Werkinspanning voor taken geïntroduceerd. U kunt schatten of de Werkinspanning voor een taak klein, middelgroot, of groot is zonder manueel de Geplande Uren voor de taak te schatten. Elk inspanningsniveau wordt berekend gebaseerd op een percentage van tijd van de typische uren per dag zoals gevormd in uw instantie.

De volgende verbeteringen zijn nu beschikbaar met deze nieuwe functie:

* Schakel deze instelling voor projecten en sjablonen in om deze beschikbaar te maken voor taken en sjabloontaken
* Werk deze instelling voor elke taak bij met een eenvoudig type duur waarmee de geplande uren van de taak automatisch worden bijgewerkt
* Schakel deze instelling uit met een lay-outsjabloon voor gebruikers die de geplande uren liever zouden blijven gebruiken.
* Geef de waarde van dit nieuwe veld weer in een takenlijst of rapport.

Voor informatie over de inspanning van het Werk, zie [&#x200B; Overzicht van de Werkinspanning van het Werk &#x200B;](../../../manage-work/tasks/task-information/work-effort.md).

Deze eigenschap is nu inbegrepen in de [&#x200B; Grondbeginselen van de Planner, Deel 2 het leren weg &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront/using/home) op Workfront Één.

## Op projectstatus gebaseerde kleuren voor werkitems in werklastverdeling

Voor een betere zichtbaarheid en een betere aanpassing van uw ervaring in Workload Balancer kunt u nu de kleuren van de projecten en hun werkitems aanpassen aan de status van de projecten. De kleuren komen overeen met projectstatussen op groepsniveau of op systeemniveau. De weergegeven kleuren kunnen zowel overeenkomen met de status van het systeem als met die van het aangepaste project.

Voor informatie over het aanpassen van de mening in de Balancer van de Werklast, zie [&#x200B; de Balancer van de Werkbelasting &#x200B;](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) navigeren.

## De gebruikerstoewijzing aanpassen met behulp van percentagewaarden in Workload Balancer

U kunt nu de toewijzingen van uw gebruikers in Workload Balancer beheren met percentages in plaats van uren.

Voor informatie over het beheren van toewijzingen in de Balancer van de Werklast, zie [&#x200B; gebruikerstoewijzingen in de Balancer van de Werklast beheren &#x200B;](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Voltooid werk tonen of verbergen in werklastbalans

Met een nieuwe instelling kunt u nu voltooide werkitems weergeven of verbergen in Workload Balancer. De instelling wordt standaard ingeschakeld en voltooide werkitems die overeenkomen met de filtercriteria en het geselecteerde tijdkader in het werklastevenwicht.

Vóór deze verbetering, voltooide het werkpunten altijd getoond in de Balancer van de Werkbelasting.

Voor meer informatie over het aanpassen van montages in de Balancer van de Werkbelasting, zie [&#x200B; de Balancer van de Werkbelasting &#x200B;](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) navigeren.

## Verbeteringen van de bruikbaarheid van de werklastbalans

Voor een gestroomlijnde en gebruiksvriendelijke ervaring wanneer u uw bronnen beheert in Workload Balancer, zijn de volgende gebruiksverbeteringen nu beschikbaar:

* U kunt de Samenvatting voor kwesties en taken van het Summiere pictogram in plaats van het Meer menu nu openen. Deze ervaring is nu in overeenstemming met die van lijsten.

  >[!NOTE]
  >
  >Deze optie is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring.

* U hebt toegang tot het menu Meer links van een objectbalk in plaats van aan het einde van een objectbalk. Hierdoor is het gemakkelijker om te vinden wanneer objecten een lange periode beslaan.
* U kunt de toewijzingsfuncties openen met een sneltoets. Eerder was dit alleen beschikbaar in het menu Meer.
* U kunt alle resterende items onder de naam van een gebruiker laden in plaats van alleen de volgende 20 items door op Meer laden te klikken.

Voor meer informatie over het navigeren van de Balancer van de Werkbelasting, zie [&#x200B; de Balancer van de Werkbelasting &#x200B;](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) navigeren.

## Toewijzingsdiagram voor gebruikers in Workload Balancer

Om u toe te staan om een high-level visuele vertegenwoordiging van de toewijzing van gebruikers binnen een bepaald tijdkader te hebben, laat een nieuw plaatsen nu een grafiekmening voor toe hoe de toewijzingen in de Balancer van de Werklast worden getoond. Als u deze instelling inschakelt, wordt de toewijzing van de gebruikers weergegeven in een lijndiagram dat de overtoewijzingen in rode blokken en de ondertoewijzingen in blauw aangeeft.

Voor meer informatie over het vormen van montages in de Balancer van de Werkbelasting, zie [&#x200B; de Balancer van de Werkbelasting &#x200B;](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) navigeren.

## Voltooid werk visualiseren in Workload Balancer

Om u toe te staan om werk gemakkelijk te identificeren dat reeds is voltooid zodat u gebruikerstoewijzingen correct kunt beheren, hebben wij een visuele indicator in de Balancer van de Werkbelasting toegelaten die toont wanneer de punten voor een geselecteerd tijdkader zijn voltooid. U ziet nu een groen vinkje voor taken, problemen wanneer deze zijn voltooid. Het project toont ook het groene vinkje wanneer er het werkpunten tijdens het tijdkader worden voltooid dat op het scherm wordt getoond.

Voor informatie over het bekijken van informatie in de Balancer van de Werklast, zie [&#x200B; de Balancer van de Werkbelasting &#x200B;](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) navigeren.

## Nieuw standaardfilter voor het toegewezen werkgebied in het werklastverdelingsmechanisme

Het standaardfilter voor het Toegewezen gebied van het Werk in de Balancer van de Werklast toont nu slechts gebruikers die lid van alle teams zijn die u, als het programma geopende gebruiker, met wordt geassocieerd. Het nieuwe filter geeft u nu standaard de meest relevante informatie weer.

Voordat u deze upgrade uitvoert, worden alle gebruikers die toegang hadden tot de weergave in dit gebied weergegeven.

Voor informatie over het gebruiken van filters in de Balancer van de Werklast, zie [&#x200B; filters in de Balancer van de Werklast beheren &#x200B;](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Nieuw pictogram voor het schakelen tussen uren en percentagewaarden, of toegewezen en resterende tijd in de Balancer van de Werkbelasting

We hebben een nieuwe instelling toegevoegd waarmee u kunt schakelen tussen toegewezen uren en percentages wanneer u de werklastbalans weergeeft. Met dit nieuwe pictogram hebben we ook de sectie Gebruikerswerkbelasting in het deelvenster Instellingen verwijderd. De werklastbalans toont standaard toegewezen tijd en we hebben de resterende uren verplaatst naar het nieuwe pictogram Percentage of Uren.

Deze verbetering elimineert kliks en maakt het navigeren van de Balancer van de Werkbelasting gemakkelijker en efficiënter.

Voor informatie over het beheren van montages voor de Balancer van de Werklast, zie [&#x200B; de Balancer van de Werkbelasting &#x200B;](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) navigeren.

## Een nieuw ingebouwd filter voor het evenwicht van de Werklast: Gebruikers op projecten

Om uw filterervaring in de Balancer van de Werkbelasting efficiënter te maken, hebben wij een nieuw ingebouwd filter in het Toegewezen het gebied van het Werk toegevoegd. U kunt de Gebruikers op projectfilter nu toepassen die gebruikers toont die aan taken en kwesties in de projecten worden toegewezen u specificeert.

Voor informatie over het gebruiken van filters in de Balancer van de Werkbelasting, zie [&#x200B; informatie van de Filter in de Balancer van de Werkbelasting &#x200B;](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

