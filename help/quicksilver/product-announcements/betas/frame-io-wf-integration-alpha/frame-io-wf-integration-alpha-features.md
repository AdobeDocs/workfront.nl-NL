---
content-type: reference
navigation-topic: betas
title: 'Native integratie-alfa van Adobe Workfront en Frame.io: functies'
description: Geplande functies voor de native integratie-alfa van Adobe Workfront en Frame.io
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
source-git-commit: 0ad33f377086f71699c550e2300731056a834e72
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---


# Standaard Adobe Workfront- en Frame.io-integratie alfa: functies

## Gebruik hoofdletters en kleine letters en functie testen

Met deze integratie willen we creatieve mensen in staat stellen om in hun keuze (CC of Frame.io) te blijven voor het maken van inhoud en collegiale toetsingen, terwijl we tegelijkertijd projectmanagers hebben die het werk coördineren en het formele evaluatieproces vanuit Workfront initialiseren en controleren. Dit kan worden bereikt door de beste van beide oplossingen te gebruiken: Workfront-goedkeuringen voor nieuwe documenten voor het beheer van goedkeuringen van inhoud, in combinatie met de mogelijkheden voor inhoudsrevisie die Frame.io biedt. De nieuwe goedkeuringen voor documenten en Frame.io vormen samen onze nieuwe complete ervaring voor het beoordelen en goedkeuren van inhoud. 

Ga voor meer informatie over de werking van de alfa en de manier waarop u kunt deelnemen naar [Adobe Workfront- en Frame.io-integratie alfa: overzicht](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>Als u deze pagina&#39;s tegenkomt zonder dat uw bedrijf deelneemt aan dit alpha-programma, moet u de informatie hier zorgvuldig behandelen en contact opnemen met uw Workfront of Frame.io-beheerder voor meer informatie.

<!--Initial setup and basic test scenario 

As part of the alpha program, we've provisioned a new test Frame.io account for you and connected it to a new group "Frame.io alpha testing" in your existing Workfront Preview or Sandbox environment. To test the delivered functionality please log in to your Workfront Preview or Sandbox instance and  perform the following steps: 

Coordinators: Within Workfront, create a project with the "Frame.io alpha testing" group assigned as project group 

Coordinators: Within Workfront, assign your creatives to the project or Frame enabled tasks and change the project status to "Current" 

Creatives: Check your emails for an invite to the newly created Frame.io project 

Creatives: Click on the "Join project" button within the invitation email to join the Frame.io project, review the creative brief within the project and start your content creation within your CC tool of choice 

Creatives: Upload your created assets to Frame.io and add them to the linked Workfront project (or assigned Frame enabled tasks)  

Coordinators: Within Workfront, see the linked Frame.io assets in your project and assign reviewers / approvers (new document approvals: More help on this feature) 

Stakeholders: Withing Workfront, view your approval request in Workfront Home or Document Details and review the Frame connected document in the Frame.io Viewer. Leave a comment feedback 

Coordinators: Within Workfront, view the stakeholder created comments within the Updates section of the Frame.io connected document in Workfront 

Stakeholders: Make a decision from within the Frame.io Viewer 

Creatives: Within Frame.io, notice the overall approval decision made for your assets 

Creatives: Within Frame.io, Apply the requested changes by adding the updated version to the version stack of the connected asset 

Coordinators: Within Workfront, assign approvers / reviewers to the new version upload and monitor the progress until it reaches sign-off-->

## Functieplannen

Hieronder vindt u informatie over de gevallen van primair gebruik die we willen aanpakken en de kenmerken die we momenteel voor ogen hebben. <!--, along with documentation to get you started testing.-->


### Workfront-beheerders kunnen een verbinding instellen tussen Workfront-groepen en Frame.io-accounts

* _Binnen Workfront kunt u een Workfront-groep verbinden met een Frame.io-account_

* Er wordt een nieuw Frame.io-team gemaakt binnen Frame.io dat de verbonden Workfront-groep vertegenwoordigt

**Mogelijke verbeteringen in toekomstige versies:**

* Een Workfront-groep loskoppelen van een Frame.io-account

* Een Workfront-groep verbinden met een bestaand Frame.io-team

### Projectcoördinatoren kunnen bepalen welke Workfront-projecten naar Frame.io worden verzonden en de toegewezen Creatieven in Workfront eraan hebben toegevoegd in Frame.io

* Mogelijkheid om Workfront-projecten te markeren als Frame.io ingeschakeld door een Frame verbonden groep toe te wijzen

* _Verbetering: de mogelijkheid om taken binnen Workfront-projecten als frametaken in te schakelen die op hun beurt taakmappen binnen Frame.io maken_

* Wanneer een het projectstatus van Workfront aan Huidig wordt geplaatst, wordt een overeenkomstig verbonden project gecreeerd in Kader, worden de aan Workfront toegewezen gebruikers toegevoegd aan het project van het Kader, en een e-mailbericht wordt verzonden naar hen van Frame.io

   * Alle leden van het Project van Workfront (gebruikers en teams) zullen als Medewerkers aan het project Frame.io (bij projectverwezenlijking en later) worden toegevoegd

   * _Verandering: De gebruikers en de teams die aan Kader toegelaten taken van Workfront worden toegewezen zullen als Medewerkers aan het project Frame.io worden toegevoegd en (bij projectverwezenlijking en later) op de hoogte gebracht_

* De documenten (Creative Brief) die aan het project en Kader toegelaten taken worden toegevoegd zullen aan het project Frame.io (binnen respectieve het werkomslag) worden geduwd wanneer het project wordt gecreeerd (trekker: projectstatus die aan Huidig wordt geplaatst)

   * We raden u aan de hoeveelheid documenten die aan uw project wordt toegevoegd te beperken voordat u actief wordt aan uw creatieve instructies, om te voorkomen dat er meerdere onnodige documenten naar Frame.io worden verzonden

* _Verbetering: gebruikers / teams die expliciet niet zijn toegewezen aan een voor frames ingeschakelde Workfront-taak worden verwijderd uit het Frame.io-project_

**Mogelijke verbeteringen in toekomstige versies:**

* De kader toegelaten taken kunnen op projectmalplaatjes worden gevormd

* Nieuwe versie uploadt naar creatieve briefjes wordt naar Frame geduwd

* Geoptimaliseerde projectsynchronisatie (projecten loskoppelen, projecten en documenten opnieuw synchroniseren, enz.)

### In Frame.io kunnen Creative Cloud gemaakte middelen naar het Workfront-project sturen voor formele revisie

* Mogelijkheid om enig element Frame.io te verbinden met een WF-project of -taak. Er wordt een assetverwijzing gemaakt in Workfront

* Nieuwe versie die wordt geüpload in Frame.io, maakt automatisch een nieuwe documentversie in Workfront op verbonden elementen

* _Verbetering: mogelijkheid om de Workfront-taken waarnaar wordt verwezen, vanuit Frame.io als voltooid te markeren_

* _Verbetering: als het verbonden Workfront-document wordt verwijderd, blijft het binnen Frame.io en kan het opnieuw worden verbonden met dezelfde of een andere projecttaak_

**Mogelijke verbeteringen in toekomstige versies:**

* Mogelijkheid om meerdere Frame.io-elementen tegelijk naar Workfront te verzenden

* Tijd die tegen Workfront project/taak van binnen Frame.io registreren

### Projectcoördinatoren kunnen het formele goedkeuringsproces toewijzen aan documenten die zijn gekoppeld vanuit Frame.io

* Workfront-gebruikers en -teams kunnen worden toegevoegd aan nieuwe documentgoedkeuringen voor Frame.io-verbonden documenten

* _Verbetering: wanneer een gebruiker/team wordt losgekoppeld van een voor frames geschikt document, verliest hij/zij ook zijn toegang tot het element in Frame.io Viewer_

**Mogelijke verbeteringen in toekomstige versies:**

* Meerdere elementen verzenden als één revisie

* Ongelimiteerde toewijzing van fiatteurs/revisoren aan Workfront-documenten

### Belanghebbenden kunnen hun revisie en goedkeuring uitvoeren in Frame.io Viewer

* Belanghebbenden worden op de hoogte gesteld en kunnen het met het frame verbonden document weergeven in de Frame.io Viewer

* Frame.io Viewer kan worden geopend vanaf verschillende locaties in Workfront, bijvoorbeeld documentlijst, documentgegevens, Workfront Home

* Mogelijkheid om de bestaande revisie- en opmerkingsmogelijkheden van de Frame.io Viewer te benutten die worden gesynchroniseerd met de Workfront Update Stream

* _Mogelijkheid om een nieuw goedkeuringsbesluit voor een document te nemen vanuit de Frame.io Viewer_

### Binnen Frame.io worden Creative Suite op de hoogte gesteld van de algemene beslissing die is genomen met betrekking tot het gekoppelde Frame.io-element

* _Verbetering: de algehele status van documentgoedkeuring wordt weergegeven op het element in Frame.io_

### Projectcoördinatoren kunnen definitieve middelen naar AEM sturen

* _Verbetering: aan frames gekoppelde documenten, inclusief metagegevens, kunnen naar AEM worden verzonden met de bestaande Workfront + AEM Asset CS-connector_