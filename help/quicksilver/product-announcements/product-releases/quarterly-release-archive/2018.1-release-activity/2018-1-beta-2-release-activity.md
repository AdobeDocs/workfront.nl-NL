---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 2-releaseactiviteit
description: Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de Voorvertoningsomgeving met de Beta 2-release van 2018.1. De functionaliteit op deze pagina is op 14 december 2017 beschikbaar gesteld in de voorvertoningsomgeving. Het zal in maart 2018 beschikbaar worden gesteld in de productieomgeving.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 22e3836c-c41e-48a6-9926-e832af91e616
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1327'
ht-degree: 0%

---

# 2018.1 Beta 2-releaseactiviteit

Op deze pagina worden alle wijzigingen beschreven die het laatst beschikbaar zijn in de Voorvertoningsomgeving met de Beta 2-release van 2018.1. De functionaliteit op deze pagina is op 14 december 2017 beschikbaar gesteld in de voorvertoningsomgeving. Het zal in maart 2018 beschikbaar worden gesteld in de productieomgeving.

>[!IMPORTANT]
>
> De op deze pagina beschreven functionaliteit kan worden gewijzigd voordat deze beschikbaar is in de productieomgeving.

Voor een lijst met alle wijzigingen die in 2018.1 zijn aangebracht, raadpleegt u  [ 2018.1 overzicht van de versieactiviteit ](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

De Beta 2-release van 2018.1 bevat verbeteringen voor zowel Workfront-beheerders als andere gebruikers:

**voor Beheerders**

* [Groepsbeheer voor gebruikers en lay-outsjablonen](#group-administration-for-users-and-layout-templates)

**voor Alle Gebruikers**

* [ systeem-brede Vertoning van Breedbeeld ](#system-wide-widescreen-display)
* [ Resize de Momentopname van de Chronologie op de Grafiek van Gantt ](#resize-timeline-snapshot-on-the-gantt-chart)
* [ Interactieve Planner van het Middel in het BedrijfsGeval ](#interactive-resource-planner-in-the-business-case)
* [ Visualisatie in de Planner van het Middel - de Grafiek van de Toewijzing van de Gebruiker ](#visualization-in-the-resource-planner-user-allocation-chart)
* [ Verbeteringen in het Gebied van het Huis ](#improvements-in-the-home-area)
* [ Nieuwe het proefKijker Verbeteringen ](#new-proofing-viewer-improvements) 

## Groepsbeheer voor gebruikers en lay-outsjablonen {#group-administration-for-users-and-layout-templates}

U kunt nu groepsbeheerders aanwijzen in Workfront. Het veld Groepseigenaar is hernoemd naar groepsbeheerder en gebruikers die zijn aangewezen als groepsbeheerders, hebben aanvullende machtigingen om gebruikers en lay-outsjablonen te beheren voor de groepen die zij beheren.

* [ Beheer van de Gebruiker door groepsbeheerder ](#user-management-by-group-administrator)
* [Lay-outsjabloonbeheer door groepsbeheerders](#layout-template-management-by-group-administrators)

### Gebruikersbeheer per groepsbeheerder {#user-management-by-group-administrator}

Wij introduceren het nieuwe concept **groepsbeheerder**. Om dit te steunen, is het **gebied van de Eigenaar van de Groep 1} anders genoemd aan** groepsbeheerder **en de gebruikers die als groepsbeheerders worden aangewezen hebben extra toestemmingen om gebruikers en de groepen te beheren.**

Naast de toestemmingen die de Eigenaar van de Groep eerder gebruikers moest beheren, heeft de groepsbeheerder nu de volgende extra toegang wanneer het beheren van gebruikers binnen de groepen waar zij als groepsbeheerder worden geplaatst:

* Meld u aan als een andere gebruiker die tot een groep behoort die zij beheren.
* Stel het wachtwoord opnieuw in voor een andere gebruiker die behoort tot een groep die hij of zij beheert.
* Lay-outsjablonen maken die door hun groep worden beheerd. 

Vóór deze wijziging kon alleen de Workfront-beheerder deze functies uitvoeren.

Voor meer informatie over groepsbeheerders, zie de sectie van het &quot;Begrip van groepsbeheerders&quot;in [ een groep ](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) creëren.

### Lay-outsjabloonbeheer door groepsbeheerders {#layout-template-management-by-group-administrators}

Wij introduceren het nieuwe concept van **Groep met de Toegang van het Beleid** die u met een Malplaatje van de Lay-out kunt associëren.

De gebruiker die als groepsbeheerder voor deze groep is aangewezen, heeft toegang om dat Lay-outsjabloon te beheren en nieuwe Lay-outsjablonen te maken waarin de groepen die hij of zij beheert de beheergroepen van de sjablonen zijn. 

Vóór deze wijziging kon alleen de Workfront-beheerder lay-outsjablonen maken.

Zie &quot;Lay-outsjablonen maken en beheren&quot; voor meer informatie over het maken van lay-outsjablonen.

## Breedbeeld voor het hele systeem {#system-wide-widescreen-display}

Wanneer u een pagina in Workfront weergeeft, wordt het volledige browservenster nu automatisch gevuld en aangepast aan de schermgrootte.

Vóór deze wijziging werden alleen de pagina&#39;s die aan de volgende objecten waren gekoppeld, op breedbeeld weergegeven:

* Projecten
* Taken
* Problemen
* Rapporten
* Dashboards
* Kalenders

## De grootte van de tijdlijnopname wijzigen in de Gantt-grafiek {#resize-timeline-snapshot-on-the-gantt-chart}

U kunt de tijdlijnmomentopname nu uitbreiden om het volledige project in de grafiek van Gantt te tonen.

Voorafgaand aan deze verbetering, kon u een specifiek punt op de chronologiemomentopname selecteren om aan het in de grafiek van Gantt te navigeren.

Voor meer informatie over het vormen hoe de informatievertoningen op de grafiek van Gantt, zie [ vormen hoe de informatievertoningen op de Grafiek van Gantt ](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Interactive Resource Planner in de Business Case {#interactive-resource-planner-in-the-business-case}

Als Manager van het Middel, kunt u de Pools van het Middel in de sectie van de Begroting van het Middel van het BedrijfsGeval nu toevoegen. U kunt uw projectmiddelen ook begroten gebruikend de project-vlakke Planner van het Middel. Het begroten van uw middelen voor een project leidt tot de begrote arbeidskosten van het project.

Voorafgaand aan deze verandering, kon u de informatie van de Begroting van het Middel in het BedrijfsGeval bekijken als het project voor middelen in de globale Planner van het Middel in de begroting was opgenomen.

Voor meer informatie over de voltooiing van het in de begroting opnemen van projectmiddelen in het BedrijfsGeval, zie {de middelen van de Begroting in het BedrijfsGeval ](../../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).[

## Visualisatie in de functie Resourceplanner - Toewijzingsdiagram voor gebruikers {#visualization-in-the-resource-planner-user-allocation-chart}

U kunt de algemene Geplande Toewijzing van alle gebruikers tegen hun beschikbaarheid nu tonen in een grafiek in de Planner van het Middel. De grafiek is beschikbaar wanneer u **Mening door Gebruiker** in de Planner van het Middel selecteert.

De grafiek geeft de volgende informatie weer:

* Beschikbaarheid % zonder overtoewijzing voor alle gebruikers
* Overtoewijzing % voor alle gebruikers
* Onderbenutting % voor alle gebruikers
* Er is een overtoewijzing voor ten minste één gebruiker gedurende deze periode

Voorafgaand aan deze wijziging kon u de toewijzing en beschikbaarheid van afzonderlijke gebruikers alleen in tabelindeling bekijken.

Voor meer informatie over de grafiek van de gebruikerstoewijzing in de Planner van het Middel, zie [ overzicht van de Planner van het Middel ](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Verbeteringen in het thuisgebied {#improvements-in-the-home-area}

Er zijn nu diverse verbeteringen beschikbaar in het gebied van de startpagina, waaronder:

* Verbeteringen bekijken en voelen

   * Het juiste paneel is nu groter, zodat er meer ruimte is voor taak- en uitgiftegegevens.
   * Achterstallige items worden nu in een lichtere rode kleur weergegeven wanneer u deze optie selecteert in het linkerdeelvenster.
   * U ziet nu gemakkelijker de relatie tussen het linkerdeelvenster en het rechterdeelvenster. Het geselecteerde document in het linkerpaneel wijst naar het rechterpaneel.

* Standaardvelden worden weergegeven voor geselecteerde items. 

  Zie &quot;Lay-outsjablonen maken en beheren&quot; voor meer informatie over de standaardvelden.

* Nadat u op &quot;Werken met&quot; op een verzoek hebt geklikt, worden de velden die aan de uitgave zijn gekoppeld, weergegeven in het rechterdeelvenster.

  Voor meer informatie over het werken aan verzoeken van het gebied van het Huis, zie [ werk en teamverzoeken in het gebied van het Huis ](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md) in [ leiden werk en teamverzoeken in het gebied van het Huis ](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md).

* Wijs een gebruikersavatar op een het werkpunt in het linkerpaneel aan om de naam van de gebruiker te bekijken.
* Vouw het gebied &#39;Te laat&#39; in het linkerdeelvenster uit om alle late items weer te geven (als dit gebied is samengevouwen, worden alleen de eerste 5 items weergegeven).
* Nadat u een item hebt gemarkeerd als Voltooid, blijft het item in het linkerdeelvenster staan totdat u een ander item selecteert.\
  Voor informatie over het tonen van voltooide punten, zie [ de punten van de Vertoning in de Lijst van het Werk in het gebied van het Huis ](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) in [ punten van de Vertoning in de Lijst van het Werk in het gebied van het Huis ](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

Voor meer informatie over het gebruiken van het nieuwe gebied van het Huis, evenals informatie beschrijvend verschillen in functionaliteit tussen Mijn Werk en Huis, zie [ Gebruik het gebied van het Huis ](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Nieuwe verbeteringen in de proefdrukviewer  {#new-proofing-viewer-improvements}

* [ Verbeterde Lay-out en Ontwerp ](#improved-layout-and-design)
* [ de Commentaren van het Onderzoek door Aantal van de Commentaar ](#search-comments-by-comment-number)
* [ Optie om Commentaar naast de Indicator van de Prijsverhoging uit te geven ](#option-to-edit-comment-next-to-the-markup-indicator)
* [ Teken Alle Commentaren als Gelezen ](#mark-all-comments-as-read)
* [Verbeteringen linkermenu](#left-menu-improvements)

### Verbeterde layout en ontwerp {#improved-layout-and-design}

De kijker van het proef heeft een bijgewerkte blik en een gevoel. De  de volgende gebieden van de proefdrukviewer zijn bijgewerkt:

* Miniatuurgebied

  Zie in voor meer informatie over het gebruik van het gebied met miniaturen.

* Opmerkingen, gebied\
  Zie voor meer informatie over het gebied met opmerkingen.
* Linkermenugebied

### Opmerkingen zoeken op nummer van opmerking {#search-comments-by-comment-number}

Wanneer u nu de lijst met opmerkingen doorzoekt in de proefdrukviewer, kunt u het nummer van de opmerking invoeren in het zoekveld. De lijst met opmerkingen wordt vervolgens gefilterd om de opmerking weer te geven waarnaar u hebt gezocht. 

Zie voor meer informatie in .

### Optie voor het bewerken van opmerkingen naast de markeringen-indicator {#option-to-edit-comment-next-to-the-markup-indicator}

U kunt een bestaande opmerking nu gemakkelijker bewerken. Nadat u op een opmerking-indicator op de proefdruk hebt geklikt, wordt het pictogram Bewerken weergegeven naast de ballon. 

Voordat u deze wijziging aanbrengt, moest u op het pictogram Bewerken in het gebied Opmerking klikken.  

Zie voor meer informatie.

### Alle opmerkingen markeren als gelezen {#mark-all-comments-as-read}

Wanneer u een document weergeeft in de proefdrukviewer, kunt u alle opmerkingen nu markeren als Lezen.

### Verbeteringen linkermenu {#left-menu-improvements}

Het menu aan de linkerkant van de testviewer bevat de volgende verbeteringen:

* Bijgewerkt uiterlijk
* Pictogram boven aan het menu om het menu weer te geven of te verbergen

  ![ proof_viewer_menu_hide.png ](assets/proof-viewer-menu-hide.png)

* Plaats de muis boven het menu om het menu automatisch uit te vouwen om naast pictogrammen ook labels weer te geven. (Of schakel de optie in om het menu altijd in de samengevouwen weergave te houden.)
