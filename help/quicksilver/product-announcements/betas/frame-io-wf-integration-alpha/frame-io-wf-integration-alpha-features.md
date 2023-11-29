---
content-type: reference
navigation-topic: betas
title: 'Native integratie-alfa van Adobe Workfront en Frame.io: functies'
description: Geplande functies voor de native integratie-alfa van Adobe Workfront en Frame.io
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
exl-id: a1603a06-957b-4d52-89f3-f0cec1a4e02c
source-git-commit: 02e55be36d3b649aeb5b81d185538f77ac3d4ec7
workflow-type: tm+mt
source-wordcount: '1183'
ht-degree: 0%

---

# Standaard Adobe Workfront- en Frame.io-integratie alfa: functies en testen

Met deze integratie willen we creatieve mensen in staat stellen om in hun keuze (CC of Frame.io) te blijven voor het maken van inhoud en collegiale toetsingen, terwijl we tegelijkertijd projectmanagers hebben die het werk coördineren en het formele evaluatieproces vanuit Workfront initialiseren en controleren. Dit kan worden bereikt door de beste van beide oplossingen te gebruiken: Workfront-goedkeuringen voor nieuwe documenten voor het beheer van goedkeuringen van inhoud, in combinatie met de mogelijkheden voor inhoudsrevisie die Frame.io biedt. De nieuwe goedkeuringen voor documenten en Frame.io vormen samen onze nieuwe complete ervaring voor het beoordelen en goedkeuren van inhoud. 

Ga voor meer informatie over de werking van de alfa en de manier waarop u kunt deelnemen naar [Adobe Workfront- en Frame.io-integratie alfa: overzicht](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>Als u deze pagina&#39;s tegenkomt zonder dat uw bedrijf deelneemt aan dit alpha-programma, moet u de informatie hier zorgvuldig behandelen en contact opnemen met uw Workfront of Frame.io-beheerder voor meer informatie.

## Basis testscenario

Om u toe te staan om de nieuwe eigenschappen van het alpha- programma gemakkelijk te testen, hebben wij een nieuw testrekening Frame.io gecreeerd en het verbonden met een nieuwe groep genoemd `Frame.io alpha testing` in uw bestaande Workfront Preview- of Sandbox-omgeving.

Meld u aan bij de Workfront Preview- of Sandbox-instantie en voer de volgende stappen uit om de functionaliteit te testen:

1. **Coördinatoren:** Maak in Workfront een project met de `Frame.io alpha testing` groep die als projectgroep wordt toegewezen.

1. **Coördinatoren:** Wijs binnen Workfront uw creatieve items toe aan de taken waarvoor het project of frame is ingeschakeld en wijzig de projectstatus in &quot;Current&quot; (Huidig).

1. **Creatieve producten:** Controleer uw e-mails voor een uitnodiging tot het zojuist gemaakte Frame.io-project

1. **Creatieve producten:** Klik op de knop &quot;Deelnemen aan project&quot; in de uitnodigings-e-mail om deel te nemen aan het Frame.io-project, bekijk de creatieve samenvatting in het project en start het maken van uw inhoud met het gereedschap Creative Cloud van keuze.

1. **Creatieve producten:** Upload uw gemaakte elementen naar Frame.io en voeg deze toe aan het gekoppelde Workfront-project (of aan toegewezen taken waarvoor Frame is ingeschakeld).

1. **Coördinatoren:** Zoek in Workfront naar de gekoppelde Frame.io-elementen in uw project en wijs revisoren/fiatteurs toe (voor meer informatie over het toewijzen van revisies/fiatteurs raadpleegt u [Extra fiatteurs of revisoren toevoegen aan een document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md)).

1. **Belanghebbenden:** Bekijk in Workfront uw goedkeuringsaanvraag in Home- of Document Details en bekijk het document met Frame-verbinding in de Frame.io Viewer. Laat vervolgens een opmerking met feedback achter.

1. **Coördinatoren:** In Workfront kunt u de door de belanghebbende gemaakte opmerkingen weergeven in de sectie Updates van het document Frame.io.

1. **Belanghebbenden:** Maak een beslissing vanuit de Frame.io Viewer.

1. **Creatieve producten:** Merk in Frame.io het algemene goedkeuringsbesluit op dat voor uw elementen is genomen.

1. **Creatieve producten:** Pas in Frame.io de gewenste wijzigingen toe door de bijgewerkte versie toe te voegen aan de versiestapel van het gekoppelde element.

1. **Coördinatoren:** Wijs in Workfront fiatteurs/revisoren toe aan de geüploade versie en controleer de voortgang totdat deze afmelding bereikt.

## Functieplannen

Hieronder vindt u informatie over de gevallen van primair gebruik die we willen aanpakken en de kenmerken die we momenteel voor ogen hebben. <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
><span class="preview">Gemarkeerde tekst</span> Hieronder wordt verwezen naar functies die nog niet zijn geïmplementeerd, maar die in een latere versie worden opgenomen.
>
>Opsommingstekens onder een **&quot;Mogelijke verbeteringen in toekomstige versies&quot;** header kan al dan niet worden opgenomen in een toekomstige release , afhankelijk van alfafeedback en onze ontwikkelingsplannen .
>


### Workfront-beheerders kunnen een verbinding instellen tussen Workfront-groepen en Frame.io-accounts

* <span class="preview">Binnen Workfront kunt u een Workfront-groep verbinden met een Frame.io-account</span>

* Er wordt een nieuw Frame.io-team gemaakt binnen Frame.io dat de verbonden Workfront-groep vertegenwoordigt

**Mogelijke verbeteringen in toekomstige versies:**

* Een Workfront-groep loskoppelen van een Frame.io-account

* Een Workfront-groep verbinden met een bestaand Frame.io-team

### Projectcoördinatoren kunnen bepalen welke Workfront-projecten naar Frame.io worden verzonden en de toegewezen Creatieven in Workfront eraan hebben toegevoegd in Frame.io

* Mogelijkheid om Workfront-projecten te markeren als Frame.io ingeschakeld door een Frame verbonden groep toe te wijzen

* <span class="preview">Verbetering: de mogelijkheid om taken binnen Workfront-projecten als frametaken in te schakelen die op hun beurt taakmappen binnen Frame.io maken</span>

* Wanneer een het projectstatus van Workfront aan Huidig wordt geplaatst, wordt een overeenkomstig verbonden project gecreeerd in Kader, worden de aan Workfront toegewezen gebruikers toegevoegd aan het project van het Kader, en een e-mailbericht wordt verzonden naar hen van Frame.io

   * Alle leden van het Project van Workfront (gebruikers en teams) zullen als Medewerkers aan het project Frame.io (bij projectverwezenlijking en later) worden toegevoegd

   * <span class="preview">Verandering: De gebruikers en de teams die aan Kader toegelaten taken van Workfront worden toegewezen zullen als Medewerkers aan het project Frame.io worden toegevoegd en (bij projectverwezenlijking en later) op de hoogte gebracht</span>

* De documenten (Creative Brief) die aan het project en Kader toegelaten taken worden toegevoegd zullen aan het project Frame.io (binnen respectieve het werkomslag) worden geduwd wanneer het project wordt gecreeerd (trekker: projectstatus die aan Huidig wordt geplaatst)

   * We raden u aan de hoeveelheid documenten die aan uw project wordt toegevoegd te beperken voordat u actief wordt aan uw creatieve instructies, om te voorkomen dat er meerdere onnodige documenten naar Frame.io worden verzonden

* <span class="preview">Verbetering: gebruikers / teams die expliciet niet zijn toegewezen aan een voor frames ingeschakelde Workfront-taak worden verwijderd uit het Frame.io-project</span>

**Mogelijke verbeteringen in toekomstige versies:**

* De kader toegelaten taken kunnen op projectmalplaatjes worden gevormd

* Nieuwe versie uploadt naar creatieve briefjes wordt naar Frame geduwd

* Geoptimaliseerde projectsynchronisatie (projecten loskoppelen, projecten en documenten opnieuw synchroniseren, enz.)

### In Frame.io kunnen Creative Cloud gemaakte middelen naar het Workfront-project sturen voor formele revisie

* Mogelijkheid om enig element Frame.io te verbinden met een WF-project of -taak. Er wordt een assetverwijzing gemaakt in Workfront

* Nieuwe versie die wordt geüpload in Frame.io, maakt automatisch een nieuwe documentversie in Workfront op verbonden elementen

* <span class="preview">Verbetering: mogelijkheid om de Workfront-taken waarnaar wordt verwezen, vanuit Frame.io als voltooid te markeren</span>

* <span class="preview">Verbetering: als het verbonden Workfront-document wordt verwijderd, blijft het binnen Frame.io en kan het opnieuw worden verbonden met dezelfde of een andere projecttaak</span>

**Mogelijke verbeteringen in toekomstige versies:**

* Mogelijkheid om meerdere Frame.io-elementen tegelijk naar Workfront te verzenden

* Tijd die tegen Workfront project/taak van binnen Frame.io registreren

### Projectcoördinatoren kunnen het formele goedkeuringsproces toewijzen aan documenten die zijn gekoppeld vanuit Frame.io

* Workfront-gebruikers en -teams kunnen worden toegevoegd aan nieuwe documentgoedkeuringen voor Frame.io-verbonden documenten

* <span class="preview">Verbetering: wanneer een gebruiker/team wordt losgekoppeld van een voor frames geschikt document, verliest hij/zij ook zijn toegang tot het element in Frame.io Viewer</span>

**Mogelijke verbeteringen in toekomstige versies:**

* Meerdere elementen verzenden als één revisie

* Ongelimiteerde toewijzing van fiatteurs/revisoren aan Workfront-documenten

### Belanghebbenden kunnen hun revisie en goedkeuring uitvoeren in Frame.io Viewer

* Belanghebbenden worden op de hoogte gesteld en kunnen het met het frame verbonden document weergeven in de Frame.io Viewer

* Frame.io Viewer kan worden geopend vanaf verschillende locaties in Workfront, bijvoorbeeld documentlijst, documentgegevens, Workfront Home

* Mogelijkheid om de bestaande revisie- en opmerkingsmogelijkheden van de Frame.io Viewer te benutten die worden gesynchroniseerd met de Workfront Update Stream

* <span class="preview">Mogelijkheid om een nieuw goedkeuringsbesluit voor een document te nemen vanuit de Frame.io Viewer</span>

### Binnen Frame.io worden Creative Suite op de hoogte gesteld van de algemene beslissing die is genomen met betrekking tot het gekoppelde Frame.io-element

* <span class="preview">Verbetering: de algehele status van documentgoedkeuring wordt weergegeven op het element in Frame.io</span>

### Projectcoördinatoren kunnen definitieve middelen naar AEM sturen

* <span class="preview">Verbetering: aan frames gekoppelde documenten, inclusief metagegevens, kunnen naar AEM worden verzonden met de bestaande Workfront + AEM Asset CS-connector</span>
