---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 Projectverbeteringen
description: Op deze pagina worden alle projectverbeteringen beschreven die zijn aangebracht met de release 2020.2 voor de productieomgeving. Deze verbeteringen zijn in de productieomgeving beschikbaar gesteld in de week van 11 mei 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 150bc838-d6a5-445a-af77-62c4ed74dd1b
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---

# 2020.2 Projectverbeteringen

Op deze pagina worden alle projectverbeteringen beschreven die zijn aangebracht met de release 2020.2 voor de productieomgeving. Deze verbeteringen zijn in de productieomgeving beschikbaar gesteld in de week van 11 mei 2020.

Voor een lijst van alle veranderingen beschikbaar met de versie 2020.2, zie [ overzicht van de versie 2020.2 ](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Voor Workfront-beheerders: Nieuwe failsafe wanneer de projectstatus voor nieuwe projecten verborgen of ontgrendeld is

In Opstelling, vormt u een voorkeur om ervoor te zorgen dat elk nieuw project een bepaalde status heeft wanneer het project wordt gecreeerd. Dit is belangrijk omdat een project altijd een status nodig heeft om goed te kunnen functioneren in Workfront, zelfs als het een gloednieuw project is.

Om ervoor te zorgen dat de nieuwe projecten altijd een status hebben, zelfs als een beheerder de status voor nieuwe projecten verbergt of ontgrendelt, wijst het systeem nu de eerste status in de lijst van de Status aan alle nieuwe projecten toe tot u de nieuwe status voor nieuwe projecten opnieuw vormt.

Voor informatie over het plaatsen van de voorkeur voor het statuut van alle nieuwe projecten, zie [ systeem-brede projectvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen (of als u Klassiek Adobe Workfront gebruikt, zie [ Plaatsende Voorkeur van het Project ](https://experienceleague.adobe.com/nl/docs/workfront/using/home)).

**Beschikbaar in deze milieu&#39;s:**

* Adobe Workfront Classic
* De nieuwe Adobe Workfront-ervaring

## Voor Workfront-beheerders: verbeterd ontwerp in projectvoorkeuren

De ervaring met het instellen van projectvoorkeuren is nu intuïtiever en gebruiksvriendelijker:

* Titels zijn groter dan optielabels, zodat u sneller kunt vinden wat u zoekt.
* Door lijnen en extra witruimte te splitsen, kunt u elke sectie afzonderlijk bekijken, zodat u zich gemakkelijker kunt richten op wat u aan het doen bent.
* Als u een ongeldig getal typt voor een optie zoals &quot;Normaal aantal uren per werkdag&quot;, wordt direct een waarschuwingsbericht weergegeven in plaats van dat het bericht wordt weergegeven nadat u op Opslaan hebt geklikt.
* Optie-labels komen overeen met de overeenkomende interfacetekst elders in Workfront, zoals in het gebied Details en rapporten.

Voor informatie over het gebied van de Voorkeur van het Project, zie [ systeem-brede projectvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen (of als u Klassiek Adobe Workfront gebruikt, zie [ Plaatsende Voorkeur van het Project ](https://experienceleague.adobe.com/nl/docs/workfront/using/home)).

**Beschikbaar in deze milieu&#39;s:**

* Adobe Workfront Classic
* De nieuwe Adobe Workfront-ervaring

## Geselecteerde Filter, Mening, en Groepering behouden in de lijsten van het Rapport

Nu wordt het laatste filter, de weergave of de groepering die op een specifiek rapport is toegepast, geselecteerd, zelfs als de gebruiker zich afmeldt bij Workfront.

Eerder, nadat een gebruiker een Filter, Mening, of Groepering op een lijst van het Rapport toepaste en dan vanaf die pagina navigeerde, verscheen de standaardFilter, Mening, of Groepering de volgende tijd de gebruiker aan dat zelfde rapport navigeerde.

**Beschikbaar in deze milieu&#39;s:**

* De nieuwe Adobe Workfront-ervaring
* Adobe Workfront Classic

## Het bewegen van en het kopiëren van taken aan een ander project houdt de taakbeperking wanneer de taken binnen de chronologie van het project kunnen passen

We hebben een verbetering aangebracht in de manier waarop Workfront de datum-specifieke taakbeperking van een taak afhandelt wanneer u de taak kopieert of verplaatst naar een ander project. De voorbeelden van datum-specifieke taakbeperkingen zijn moet beginnen, moet beëindigen, Vaste Data, Begin niet later dan, etc.

Bijvoorbeeld, wanneer u of kopieert een taak met moet Begin op beperking aan een ander project de waarvan Geplande Datum van het Begin vóór de Datum van het Begin van de taak is, houdt de taak de beperking nadat het wordt gekopieerd of bewogen. Wanneer u beweegt of een taak kopieert met moet op beperking aan een project beginnen de waarvan Geplande Datum van het Begin na de Datum van het Begin van de taak is, verandert de Beperking van de Taak in zo spoedig mogelijk.

Voorafgaand aan deze verandering, verandert de Beperking van de Taak altijd in zo spoedig mogelijk.

Voor informatie over het bewegen van taken zie, [ de taken van de Beweging ](../../../manage-work/tasks/manage-tasks/move-tasks.md) (of als u Classic Adobe Workfront gebruikt, zie [ Bewegende Taken ](https://experienceleague.adobe.com/nl/docs/workfront/using/home)).

Voor informatie over het kopiëren van taken, zie [ Kopiëren en dupliceren taken ](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (of als u de Klassieke van Adobe Workfront gebruikt, zie [ Taken ](https://experienceleague.adobe.com/nl/docs/workfront/using/home) Exemplaar en Dupliceren).

Voor een overzicht van alle Beperkingen van de Taak, zie [ Overzicht van de Beperking van de Taak ](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (of als u Klassiek Adobe Workfront gebruikt, zie [ Overzicht van de Restrictie van de Taak ](https://experienceleague.adobe.com/nl/docs/workfront/using/home)).

**Beschikbaar in deze milieu&#39;s:**

* Adobe Workfront Classic
* De nieuwe Adobe Workfront-ervaring

## Het voorkomen van gegevensverlies terwijl het aanbrengen van veranderingen op het lusje van Details of een taaklijst

Om gegevensverlies te verhinderen wanneer u informatie over de pagina van Details over een voorwerp of taken in een taaklijst op het projectniveau wanneer het opslaan van veranderingen manueel bijwerkt, toont een waarschuwingsbericht nu, om u op de hoogte te brengen dat u unsaved veranderingen hebt alvorens u probeert om informatie in de kopbal uit te geven. De enige handelingen die u hebt toegestaan voordat u uw wijzigingen opslaat, zijn het abonneren of het toevoegen van het object aan uw favorieten.

Voor informatie over het uitgeven van taken in een lijst, zie [ taken in een lijst ](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md) uitgeven

**Beschikbaar in deze milieu&#39;s:**

* De nieuwe Adobe Workfront-ervaring

