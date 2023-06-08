---
content-type: reference
navigation-topic: betas
title: 'Bezig met rapporteren van canvasbèta: overzicht'
description: Informatie over het bètaprogramma voor het aanstaande hulpmiddel van het Canvas van de Rapportering voor Adobe Workfront
author: Nolan
feature: Product Announcements
hidefromtoc: true
source-git-commit: 2fa10260b54e4ba2e9ab661ac5a4985a91e69191
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Canvasbèta melden: overzicht

## Canvas melden

Een volledige herbezinning van rapportering in Workfront, is het nieuwe hulpmiddel van het Canvas van de Rapportering momenteel in ontwikkeling. Bij het ontwerpen van het Rapporterende Canvas, hebben wij hard gewerkt om een ervaring te verstrekken die maximalistische flexibiliteit in combinatie met een intuïtief, modulair ontwerp-zodat de gebruikers als u het meest effectief hefboomwerking uw eigen gegevens in het maken van en het delen van rapporten aanbiedt. Door een nieuw, verenigd rapporttype dat u toestaat om bijna elk element op een onbegrensd canvas te slepen-en-daling, zal het creëren van een visuele gegevensmeesterwerk spoedig gemakkelijker zijn dan ooit voordien.

Dit artikel bevat informatie over de huidige persoonlijke bètaversie, die beperkt is tot specifieke klanten. De nieuwe eigenschappen van het Canvas van de Rapportering worden nu opgesteld door de Dashboards van het Canvas. Zie **Ontwikkelingsplan** hieronder voor meer informatie .

### Ontwikkelingsplan

We bevinden ons in de laatste fase van het oplossen van een probleem op het gebied van gegevenskwaliteit dat we al eerder in de bètaversie van Reporting Canvas hebben gezien. Binnenkort zullen we opnieuw werken aan nieuwe visualisaties, de selectie van te rapporteren Workfront-objecten uitbreiden en de ervaringen met het maken en verspreiden van rapporten verbeteren. Deze zijn allemaal van wezenlijk belang voor het realiseren van onze doelstellingen voor het rapporteren van Canvas.

We bieden deze nieuwe ervaringen incrementeel, te beginnen met de release 23.2, via de nieuwe pagina Canvas-dashboards die nu beschikbaar is in uw voorvertoningsomgeving. De Dashboards van het canvas staan u toe om bestaande rapporten naast de nieuwe rapporteringsmogelijkheden te tonen wij bouwen, en zullen als onze primaire milieu voor het opstellen van en het testen van nieuwe eigenschappen voor het Melden van Canvas dienen. Ga voor meer informatie over het inschakelen en gebruiken van Canvasdashboards naar [Overzicht van canvasdashboards](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/canvas-dashboards-overview.md).

## Deelnemen aan de bètaversie

>[!IMPORTANT]
>
>De bètainformatie hieronder is voor beheerders die reeds in de bètaversie van het Canvas van de Rapportering zijn inbegrepen, die nieuwe deelnemers niet meer goedkeurt. Als u nieuwe eigenschappen van het Melden van Canvas zou willen testen aangezien zij worden toegevoegd, zie **Ontwikkelingsplan** hierboven voor informatie over het inschakelen van Canvasdashboards.

### Beschikbaarheid

De bèta van het Canvas van de Rapportering is beschikbaar aan alle organisaties die op AWS, ongeacht regio zijn.

### Deelnemen aan de bètaversie

De bèta van het Canvas van de Rapportering is volledig facultatief, maar kan slechts door een beheerder van Workfront worden gekozen. Als u zich wilt aanmelden als systeembeheerder:

1. Selecteer **Rapportage (bèta)** in het hoofdmenu van uw Workfront-instantie.
1. Klikken **Accepteren** om de voorwaarden te aanvaarden.
1. Toestaan dat de gegevens van uw organisatie worden toegevoegd aan het rapportcanvas (dit kan een paar uur duren).
1. Begin met het melden van canvas.

Nadat de gegevens van uw organisatie aan het Melden van Canvas worden toegevoegd, kunnen andere systeembeheerders verkiezen om zich op een individuele basis op de zelfde manier aan te sluiten (zonder het wachten op gegevens om opnieuw worden toegevoegd).

Andere gebruikers die geen Workfront-beheerders zijn, aanmelden:

1. Selecteer **Rapportage (bèta)** in het hoofdmenu van uw Workfront-instantie.
1. Klikken op **Canvasmachtigingen rapporteren**.
1. Zoek naar en selecteer de specifieke gebruikers u wilt deelnemen.

   >[!IMPORTANT]
   >
   >De gebruikers die u toegang tot het Melden van Canvas verleent zullen toegang hebben tot **alles** gegevens in het systeem in een read-only capaciteit, ongeacht hun standaardtoestemmingen om deze gegevens te bekijken.

1. Klikken **Opslaan**.
1. Voeg de **Rapportage (bèta)** in de hoofdlay-outsjabloon van elke gebruiker die is geselecteerd. Zie voor meer informatie [Het hoofdmenu aanpassen met een lay-outsjabloon](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).
1. Elke gebruiker moet dan afzonderlijk naar de **Rapportage (bèta)** in het hoofdmenu en accepteert de voorwaarden.

### Feedback verzenden

Feedback over de bètaversie verzenden:

1. Klik tijdens het rapporteren van canvas in Workfront op de knop **Feedback verzenden** knop.
1. Vul het formulier in en klik op **Verzenden**.

## Veelgestelde vragen over bèta

+++Kan ik mijn erfenisrapporten migreren naar het Rapporteren van Canvas?

Kortom, migrerende rapporten uit oudere versies zijn niet beschikbaar tijdens de bètaversie. Het is echter een gepland onderdeel (met een aantal punten die hieronder worden beschreven) voor de officiële lancering.

Hoewel de barrière om nieuwe rapporten te bouwen beduidend is verminderd met Reporting Canvas, begrijpen wij dat het overbrengen van sommige van uw bestaande rapporten en dashboards het goedkeuringsproces zal helpen versnellen. Als dusdanig, willen wij de hulpmiddelen en de middelen noodzakelijk verstrekken om ervoor te zorgen u om het even welke relevante erfenispunten kunt overbrengen om ervoor te zorgen dat u op de juiste voet in het Melden van Canvas begint. Aangezien de Rapportering van Canvas zo&#39;n radicale verandering in de manier is waarop de huidige rapportering werkt, zou het echter onmogelijk zijn om elk rapport of dashboard precies zo te migreren als nu het is.

Onze huidige strategie voor migratie in de officiële release moet u in staat stellen het volgende te doen:

1. Identificeer de rapporten en de dashboards die relevant zijn

   1. Geef u de capaciteit om een CSV van alle rapporten en dashboards in het systeem samen met om het even welke relevante het volgen informatie (aantal meningen, wanneer, en door wie) uit te voeren.
   1. Geef een exportbestand op van rapporten die samen met de ontvangers zijn ingesteld op geplande leveringen.

1. Selecteer de rapporten en dashboards die u wilt migreren, dan klik **Migreren**

   Dit is een eenrichtingsmigratie. Het leidt tot een exemplaar van de geselecteerde rapporten en dashboards aan het Melden van Canvas, verlatend het erfenisrapport of dashboard intact in het huidige rapporteringshulpmiddel.

   U kunt hetzelfde rapport of dashboard zo vaak migreren als u wilt.

1. Bij het Melden van Canvas, zorg ervoor dat alle rapporten en dashboards u selecteerde werden gemigreerd.
+++

+++Waarom kan ik niet alle voorwerpen zien ik normaal doe?

Om de bètaversie zo snel mogelijk aan onze klanten te kunnen leveren, hebben we er slechts een subset van de vele objecttypen beschikbaar in Workfront beschikbaar gesteld. Hieronder ziet u de objecttypen die momenteel in de bètaversie worden ondersteund:

* Toewijzing
* Document
* Documentgoedkeuring
* Kosten
* Uur
* Probleem
* Opmerking
* Portfolio
* Project
* Programma
* Taak
* Tijdschema
* Werkitem
+++

+++Als iets in het Melden van Canvas tijdens bèta verkeerd gaat, zullen de gegevens van mijn organisatie worden beïnvloed?

Nee. De bètaversie gebruikt een kopie van de gegevens van uw organisatie die in het rapportcanvas zijn ingevuld. Hoewel dit betekent dat u veilig kunt experimenteren tijdens de bètaversie zonder het risico te lopen belangrijke gegevens te beïnvloeden, betekent dit ook dat inline bewerken van gegevens in Reporting Canvas niet beschikbaar zal zijn tot de officiële start.
+++

+++Kan ik opteren voor de bètaversie als ik eenmaal ben toegetreden?

Een Workfront-beheerder kan zich niet afmelden voor de bètaversie. niet-systeembeheerders kunnen echter als volgt worden verwijderd:

1. Meld u aan als systeembeheerder.
1. Navigeer naar het rapportcanvas.
1. Klik op Canvas melden **machtigingen**.
1. Verwijder de gebruikers die u wilt uitschakelen uit de bètalijst die u hebt geselecteerd.
1. Klikken **Opslaan**.
+++
