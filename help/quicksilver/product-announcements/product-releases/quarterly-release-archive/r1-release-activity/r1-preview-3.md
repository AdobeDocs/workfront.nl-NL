---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Voorvertoning 3
description: Deze pagina beschrijft alle veranderingen beschikbaar in het milieu van de Voorproef met R1.3 versie. De functionaliteit op deze pagina is op 1 februari 2017 beschikbaar gesteld in de voorvertoningsomgeving.
author: Luke
feature: Product Announcements
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1343'
ht-degree: 0%

---

# R1 Voorvertoning 3

Deze pagina beschrijft alle veranderingen beschikbaar in het milieu van de Voorproef met R1.3 versie. De functionaliteit op deze pagina is op 1 februari 2017 beschikbaar gesteld in de voorvertoningsomgeving.

Voor een lijst van alle veranderingen die in R1 worden aangebracht, zie [Overzicht van de release van R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Verbeterde methode voor het koppelen van externe bestanden

De optie voor het koppelen van documenten van een externe bron (zoals Google Drive, Box, Dropbox enzovoort) bevindt zich nu op een prominentere locatie in het gebied Documenten. 

Bovendien is het nu intuïtiever om een documentleverancier toe te staan voordat bestanden van die leverancier voor het eerst worden gekoppeld (het is gewoon een extra stap wanneer bestanden van een externe provider worden gekoppeld).

Vóór deze wijzigingen bevindt de optie voor het koppelen van bestanden uit een externe bron zich in het dialoogvenster Documenten toevoegen in het gebied Documenten. Voordat een document voor het eerst vanuit een externe bron wordt gekoppeld, moest de gebruiker die het document koppelt, de documentprovider autoriseren in het gedeelte Instellen.

Zie voor meer informatie  [Documenten van externe toepassingen koppelen](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Bijgewerkt team dat aan Kalender werkt

>[!NOTE]
>
>De hulpmiddelen van de Planning van het Middel zijn afgekeurd en uit Workfront met versie 23.1 verwijderd. Voor informatie over het plannen van middelen die de Balancer van de Werkbelasting gebruiken, zie [Overzicht van de werklastbalans](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

De kalender Werken aan die beschikbaar is voor teams bevat nu extra functionaliteit en een bijgewerkte look en feel. Het team dat aan kalender werkt functioneert nu gelijkend op het middel die hulpmiddel voor projecten plannen.

Het bijgewerkte team dat aan kalender werkt omvat de volgende verbeteringen:

* Gebruikers alfabetisch weergeven of gegroepeerd op rol.
* Filter de planning chronologie door projectprioriteiten, status, en individuele projecten. U kunt de plantijdlijn ook filteren op rollen en gebruikers. (Het gebied Filter bevat minder opties dan wanneer u bronnen voor projecten instelt.)
* Neem problemen op in de tijdlijn van de planning.
* De gebruikerstoewijzingen van de vertoning en wijzigen het aantal uren dat de gebruikers aan bepaalde taken en kwesties voor elke dag worden toegewezen.
* De indicatoren van de mening die tonen wanneer de gebruikers over-toegewezen op om het even welke bepaalde dag zijn.
* Vorm of het voltooide werk op de het plannen chronologie wordt getoond.

Verschillen van het middel dat hulpmiddel plant wanneer het plannen van middelen voor projecten:

* Alle teamleden worden getoond in het team dat aan kalender werkt.\
  Wanneer het plannen van middelen voor projecten, slechts worden de gebruikers die een rol verbonden aan hen hebben die een rol van één of meerdere taken in Unassigned gebied aanpast getoond.
* Het gereedschap Wisselen is niet beschikbaar in de werkkalender van het team.
* Om het even welk teamlid kan veranderingen aanbrengen op het team dat aan kalender werkt.\
  Wanneer het plannen van middelen voor projecten, slechts kunnen de Managers van het Middel resourcing besluiten voor het project nemen.
* De kwesties worden door gebrek getoond op het team dat aan kalender werkt.\
  Wanneer het plannen van middelen voor projecten, worden de kwesties niet getoond door gebrek.

Voor meer informatie over het gebruiken van het bijgewerkte team dat aan kalender werkt, zie &quot;het Plannen van het Middel&quot;.

## Verbeteringen op gebied van middelenplanning

De tijdlijn voor planning bevat de volgende verbeteringen:

* &quot;Gebruik het filter om te bepalen welke gebruikers op de geplande tijdlijn worden getoond&quot;
* &quot;Gebruikers blijven op de tijdlijn staan nadat een taak is toegewezen&quot;

### Gebruik het filter om te bepalen welke gebruikers op de geplande tijdlijn worden weergegeven {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

>[!NOTE]
>
>De hulpmiddelen van de Planning van het Middel zijn afgekeurd en uit Workfront met versie 23.1 verwijderd. Voor informatie over het plannen van middelen die de Balancer van de Werkbelasting gebruiken, zie [Overzicht van de werklastbalans](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Het filter kan nu worden gebruikt om te bepalen welke gebruikers worden weergegeven op de planningstijdlijn, naast welke taken en problemen worden weergegeven in het gebied Niet toegewezen. Wanneer gebruikers in het filter worden geselecteerd, worden alleen de gebruikers weergegeven die u selecteert, ongeacht of ze een roltoewijzing hebben die overeenkomt met de roltoewijzing van taken in het niet-toegewezen gebied. Alle taken die momenteel aan die gebruiker zijn toegewezen, worden ook weergegeven.

Voorafgaand aan deze verandering, controleerde de filter slechts welke taken en kwesties in het Unassigned gebied werden getoond. De gebruikers werden getoond in de het plannen chronologie slechts als de gebruiker de roltoewijzing van een taak in het Niet toegewezen gebied aanpaste.

Voor meer informatie over het gebruiken van de filter om te controleren wat op de het plannen chronologie wordt getoond, zie &quot;informatie van de Filter in het Plannende gebied&quot;, en &quot;toewijzen manueel niet toegewezen taken en kwesties in de Plannende gebieden&quot;.

### Gebruikers blijven op de tijdlijn staan nadat een taak is toegewezen {#users-remain-on-the-timeline-after-being-assigned-a-task}

De gebruikers blijven op de het plannen chronologie nadat zij een taak of een kwestie worden toegewezen, zelfs als er geen resterende taken of kwesties zijn die een passende roltoewijzing hebben. Zo kunt u de benodigde wijzigingen aanbrengen nadat gebruikers zijn toegewezen.

Voorafgaand aan deze verandering, zouden de gebruikers van de het plannen chronologie onmiddellijk na worden toegewezen een taak of kwestie verdwijnen als er geen resterende taken of kwestie in het Niet toegewezen gebied met een passende roltoewijzing waren.

Zie &quot;Niet-toegewezen taken en problemen in de planningsgebieden handmatig toewijzen&quot; voor meer informatie.

## Workfront-terminologie aanpassen door objectnamen te wijzigen

U kunt de Workfront-terminologie nu aanpassen door de namen van bepaalde objecten te wijzigen.\
Met behulp van een lay-outsjabloon kunt u nu de namen van de volgende werkobjecten aanpassen aan de behoeften in uw organisatie:

* Portfolio
* Programma
* Project
* Taak
* Probleem

Als u bijvoorbeeld in uw organisatie met campagnes werkt in plaats van projecten, kunt u de naam van het object Project vervangen door Campagne.

Wanneer u deze vervanging aanbrengt, wordt in de volgende gebieden van de toepassing de bijgewerkte naam van de objecten weergegeven:

* Algemene navigatiebalk
* Alle tabbladen
* Alle menu&#39;s 
* Rapportbuilder en rapportelementen (weergaven, filters en groepen)
* Knoppen opslaan
* Geëxporteerde bestanden
* E-mails

In de volgende gebieden wordt de bijgewerkte naam van de objecten niet weergegeven:

* Bronschattingen
* Resource Budget Manager
* Capaciteitsplanner
* Bronraster
* Teamontwerper
* Portfolio optimaliseren 
* Mobiele apps
* Outlook Add-in

Voor meer informatie over hoe te om de terminologie van Workfront aan te passen gebruikend een Malplaatje van de Lay-out, zie de &quot;Aangepaste sectie van Terminologie&quot;in &quot;het Creëren en het Leiden de Malplaatjes van de Lay-out&quot;en de &quot;Begrip van de Gevolgen van het Aanpassen van de Namen van Objecten&quot;sectie in [Objecten in Adobe Workfront begrijpen](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Begin- en einddatum van goedkeuring opnemen in rapporten

U kunt nu de volgende velden opnemen wanneer u rapporten maakt of wijzigt:

* Begindatum goedkeuringspad
* Voltooiingsdatum goedkeuringspad

Met deze velden kunt u inzicht krijgen in het moment waarop het huidige of meest recente goedkeuringspad is gestart en het moment waarop het is gemarkeerd als Voltooid.

Zie voor meer informatie over deze velden [Woordenlijst met Adobe Workfront-terminologie](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Voor meer informatie over goedkeuringspaden, hoe deze worden gemaakt en geactiveerd en de functie die ze in goedkeuringsprocessen gebruiken, raadpleegt u [Een goedkeuringsproces voor werkitems maken](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

De volgende velden zijn uit Workfront verwijderd en kunnen niet langer in de rapporten worden opgenomen (deze velden bevatten informatie over het project in plaats van informatie over de goedkeuringen zelf, en werden vaak misbruikt):

* Geplande begindatum voor goedkeuring
* Begindatum goedkeuring verwacht
* Geschatte begindatum goedkeuring

## Nieuwe e-mailsamenvattingsopties voor &quot;Aanvragen die ik heb gemaakt&quot;

De leveringsoptie Dagelijkse samenvatting is toegevoegd aan het gedeelte &quot;Verzoeken die ik heb gemaakt&quot; van uw meldingsinstellingen.

Zie voor meer informatie [Uw eigen e-mailmeldingen wijzigen](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Vergeet niet het e-mailadres bij te werken dat aan uw account is gekoppeld om deze functionaliteit te kunnen testen. Dit is vereist omdat de voorvertoningssandbox de e-mailadressen van alle gebruikers wist.

## Bijgewerkte e-mailmeldingen voor het bekijken en bekijken van goedkeuring van documenten

De vormgeving van het bericht voor &quot;Documentgoedkeuring&quot; is bijgewerkt met een nieuwe interface:

Zie voor meer informatie over e-mailmeldingen [Adobe Workfront-berichten](../../../../workfront-basics/using-notifications/wf-notifications.md).

Vergeet niet het e-mailadres bij te werken dat aan uw account is gekoppeld om deze functionaliteit te kunnen testen. Dit is vereist omdat de voorvertoningssandbox de e-mailadressen van alle gebruikers wist.

## Verbeteringen in de milestone-weergave

De milestone-weergave die beschikbaar is wanneer u een projectlijst of projectrapport bekijkt, bevat nu de volgende verbeteringen:

* Geplande datums kunnen worden bewerkt
* Percentage voltooid voor projecten en taken wordt weergegeven

Voordat deze wijziging werd doorgevoerd, moest u naar de individuele taak gaan om de datums of het weergavepercentage te kunnen bewerken.

Zie voor meer informatie [De milestone-weergave gebruiken](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).
