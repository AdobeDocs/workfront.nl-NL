---
content-type: reference
navigation-topic: betas
title: 'Geïntegreerde bèta van Adobe Workfront en Frame.io: functies'
description: Geplande functies voor de geïntegreerde bètaversie van Adobe Workfront en Frame.io
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
exl-id: a1603a06-957b-4d52-89f3-f0cec1a4e02c
source-git-commit: b7a0fe333f0d8f17bc2d6c612d8cff6ee484c935
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 0%

---

# Geïntegreerde bèta van Adobe Workfront en Frame.io: functies en tests

Met deze integratie willen we creatieve mensen in staat stellen om in hun keuze (CC of Frame.io) te blijven voor het maken van inhoud en collegiale toetsingen, terwijl we tegelijkertijd projectmanagers hebben die het werk coördineren en het formele evaluatieproces vanuit Workfront initialiseren en controleren. Dit kan worden bereikt door de beste van beide oplossingen te gebruiken: Workfront-goedkeuringen voor nieuwe documenten voor het beheer van goedkeuringen van inhoud, in combinatie met de mogelijkheden voor inhoudsrevisie die Frame.io biedt. De nieuwe goedkeuringen voor documenten en Frame.io vormen samen onze nieuwe complete ervaring voor het beoordelen en goedkeuren van inhoud. 

Ga voor meer informatie over de werking van de bètaversie en de manier waarop u kunt deelnemen naar [Adobe Workfront en Frame.io integratiebèta: overzicht](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md).

>[!NOTE]
>
>Als u deze pagina&#39;s tegenkomt zonder dat uw bedrijf deelneemt aan dit bètaprogramma, moet u de informatie hier zorgvuldig behandelen en contact opnemen met uw Workfront of Frame.io-beheerder voor meer informatie.
>

## Video demo

>[!VIDEO](https://video.tv.adobe.com/v/3426406/)

## Basis testscenario

Om u toe te staan om de nieuwe eigenschappen van het bètaprogramma gemakkelijk te testen, hebben wij een nieuwe testrekening Frame.io gecreeerd en het verbonden met een nieuwe groep genoemd `Frame.io testing` in uw bestaande Workfront Preview- of Sandbox-omgeving.

Meld u aan bij de Workfront Preview- of Sandbox-instantie en voer de volgende stappen uit om de functionaliteit te testen:

1. **Coördinatoren:** Maak in Workfront een project met de `Frame.io testing` groep die als projectgroep wordt toegewezen.

1. **Coördinatoren:** Markeer in Workfront de taken waarvoor creatief werk nodig is als &#39;frame-enabled&#39; (in taakdetails) en wijs uw creatieve projecten hieraan toe (wijs uzelf ook toe als u de hele workflow wilt testen).

>[!NOTE]
>
>Subtaken kunnen niet worden gemarkeerd als Frame ingeschakeld.
>

1. **Coördinatoren:** Upload uw creatieve opdracht en verander de projectstatus in &quot;Huidige&quot;.

1. **Creatieve producten:** Controleer uw e-mails voor een uitnodiging tot het zojuist gemaakte Frame.io-project

1. **Creatieve producten:** Klik op de knop &quot;Deelnemen aan project&quot; in de uitnodigings-e-mail om deel te nemen aan het Frame.io-project, bekijk de creatieve samenvatting in het project en start het maken van uw inhoud met het gereedschap Creative Cloud van keuze.

1. **Creatieve producten:** Upload uw gecreeerde activa aan Frame.io en voeg hen aan het verbonden project van Workfront toe door één van de toegewezen Kader-Toegelaten taken te selecteren. Selecteer de optie om de taak als voltooid te markeren.

1. **Coördinatoren:** Zoek in Workfront de gekoppelde Frame.io-elementen in de voor frames ingeschakelde taak en controleer of de status van de taak is gewijzigd in &quot;complete&quot;.

1. **Coördinatoren:** Wijs revisoren/fiatteurs toe aan het gekoppelde Frame.io-element. Wijs uzelf ook als fiatteur toe als u de volledige workflow wilt testen. (Voor meer informatie over het toewijzen van beoordelingen/fiatteurs raadpleegt u [Extra fiatteurs of revisoren toevoegen aan een document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md)).

1. **Belanghebbenden:** Bekijk uw goedkeuringsaanvraag in Workfront in Home, Document Details of in het ontvangen e-mailbericht. Open de middelen in de Kijker Frame.io, geef een commentaar met terugkoppelen, en maak een besluit.

1. **Coördinatoren:** In Workfront bekijkt u de opmerkingen die door de belanghebbende zijn gemaakt in de sectie Updates van het document dat is verbonden met Frame.io, en de beslissing in de sectie Goedkeuring of het samenvattingsvenster van het document.

1. **Creatieve producten:** Merk in Frame.io het algemene goedkeuringsbesluit op dat voor uw elementen is genomen.

1. **Creatieve producten:** Pas in Frame.io de gewenste wijzigingen toe door de bijgewerkte versie toe te voegen aan de versiestapel van het gekoppelde element.

1. **Coördinatoren:** Wijs in Workfront fiatteurs/revisoren toe aan de geüploade versie en controleer de voortgang totdat deze afmelding bereikt.

## Gedetailleerd testscenario

Voor deelnemers die extra functionaliteit willen testen, hebben wij een meer betrokken testscenario gecreeerd. Hier kunt u een handleiding voor dit gedetailleerde testscenario downloaden: [WF + Frame.io Gedetailleerde Analyse van het Scenario van de Test](/help/quicksilver/product-announcements/betas/assets/MVP-WF-Frame-Detailed-Walk-Through.pdf).



## Functieplannen

Hieronder vindt u informatie over de gevallen van primair gebruik die we willen aanpakken en de kenmerken die we momenteel voor ogen hebben. <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
>Opsommingstekens onder een **&quot;Mogelijke verbeteringen in toekomstige versies&quot;** header kan al dan niet worden opgenomen in een toekomstige release, afhankelijk van bètafeedback en onze ontwikkelingsplannen die zich ontwikkelen.
>

### Workfront-beheerders kunnen een verbinding instellen tussen Workfront-groepen en Frame.io-accounts

* Binnen Workfront kunt u een Workfront-groep verbinden met een Frame.io-account

* Er wordt een nieuw Frame.io-team gemaakt binnen Frame.io dat de verbonden Workfront-groep vertegenwoordigt (let er op dat deze functie alleen is ingeschakeld voor klanten die de integratie op Production gebruiken. Klanten die nog op Sandbox of Voorproef testen zullen de verbinding hebben die door het team van de Adobe wordt gevormd.)

**Mogelijke verbeteringen in toekomstige versies:**

* Een Workfront-groep loskoppelen van een Frame.io-account

* Een Workfront-groep verbinden met een bestaand Frame.io-team

### Projectcoördinatoren kunnen bepalen welke Workfront-projecten naar Frame.io worden verzonden en de toegewezen Creatieven in Workfront eraan hebben toegevoegd in Frame.io

* Mogelijkheid om Workfront-projecten te markeren als Frame.io ingeschakeld door een Frame verbonden groep toe te wijzen

* Mogelijkheid om taken binnen Workfront-projecten als frametaken in te schakelen die op hun beurt weer taakmappen binnen Frame.io maken

* Op basis van een Workfront-project is een aan het kader gekoppelde groep toegewezen en minstens één aan het kader ingeschakelde taak, wanneer de status van het Workfront-project is ingesteld op Huidig, wordt een bijbehorend verbonden project gemaakt in Frame, worden aan Workfront toegewezen gebruikers toegevoegd aan het Frame-project en wordt een e-mailbericht verzonden naar hen van Frame.io

   * De gebruikers en de teams die aan Kader toegelaten taken van Workfront worden toegewezen zullen als Medewerkers aan het project Frame.io worden toegevoegd en (op projectverwezenlijking en later) worden meegedeeld

* De documenten (Creative Brief) die aan het project en Kader toegelaten taken worden toegevoegd zullen aan het project Frame.io (binnen respectieve het werkomslag) worden geduwd wanneer het project wordt gecreeerd (trekker: projectstatus die aan Huidig wordt geplaatst)

   * We raden u aan de hoeveelheid documenten die aan uw project wordt toegevoegd te beperken voordat u actief wordt aan uw creatieve instructies, om te voorkomen dat er meerdere onnodige documenten naar Frame.io worden verzonden

   * Documenten/taken die na de aanvankelijke projectsynchronisatie worden toegevoegd zullen niet aan Frame.io worden geduwd, slechts gebruikers/teams

**Mogelijke verbeteringen in toekomstige versies:**

* De kader toegelaten taken kunnen op projectmalplaatjes worden gevormd

* Nieuwe versie uploadt naar creatieve briefjes wordt naar Frame geduwd

* Geoptimaliseerde projectsynchronisatie (projecten loskoppelen, projecten en documenten opnieuw synchroniseren, enz.)

### In Frame.io kunnen Creative Cloud gemaakte middelen naar het Workfront-project sturen voor formele revisie

* Mogelijkheid om enig element Frame.io te verbinden met een WF-project of -taak. Er wordt een assetverwijzing gemaakt in Workfront

* Nieuwe versie die wordt geüpload in Frame.io, maakt automatisch een nieuwe documentversie in Workfront op verbonden elementen

* Mogelijkheid om de Workfront-taken waarnaar wordt verwezen vanuit Frame.io als voltooid te markeren

* Als het verbonden Workfront-document wordt verwijderd, blijft het binnen Frame.io en kan het opnieuw worden verbonden met dezelfde of een andere projecttaak

**Mogelijke verbeteringen in toekomstige versies:**

* Mogelijkheid om meerdere Frame.io-elementen tegelijk naar Workfront te verzenden

* Tijd die tegen Workfront project/taak van binnen Frame.io registreren

### Projectcoördinatoren kunnen het formele goedkeuringsproces toewijzen aan documenten die zijn gekoppeld vanuit Frame.io

* Workfront-gebruikers en -teams kunnen worden toegevoegd aan nieuwe documentgoedkeuringen voor Frame.io-verbonden documenten

* Wanneer een gebruiker/team niet wordt gedeeld vanuit een voor frames geschikt document, verliest hij/zij ook zijn toegang tot het element in Frame.io Viewer

**Mogelijke verbeteringen in toekomstige versies:**

* Meerdere elementen verzenden als één revisie

* Ongelimiteerde toewijzing van fiatteurs/revisoren aan Workfront-documenten

### Belanghebbenden kunnen hun revisie en goedkeuring uitvoeren in Frame.io Viewer

* Belanghebbenden worden op de hoogte gesteld en kunnen het met het frame verbonden document weergeven in de Frame.io Viewer

* Frame.io Viewer kan worden geopend vanaf verschillende locaties in Workfront, bijvoorbeeld documentlijst, documentgegevens, Workfront Home

* Mogelijkheid om de bestaande revisie- en opmerkingsmogelijkheden van de Frame.io Viewer te benutten die worden gesynchroniseerd met de Workfront Update Stream

* Mogelijkheid om een nieuw goedkeuringsbesluit voor een document te nemen vanuit de Frame.io Viewer
