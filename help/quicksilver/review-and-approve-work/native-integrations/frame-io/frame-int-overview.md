---
product-area: documents
navigation-topic: approvals
title: Overzicht van de integratie van Frame.io
description: Overzicht van de integratie van Frame.io
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: c4e1961092883f523d04adaacd58129a0379783d
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---


# Overzicht van de integratie van Frame.io

Dankzij de integratie van Workfront en Frame.io kunnen projectcoördinatoren projecten beheren en werken plannen in Workfront, terwijl creatieve personen, marketers en belanghebbenden hun middelen in Frame.io kunnen bekijken en goedkeuren.

## Gebaseerd op Adobe Enterprise Storage

De kern van deze integratie is Adobe Enterprise Storage - een op cloud gebaseerde opslagoplossing die fungeert als centrale opslagplaats voor bedrijfsmiddelen in Adobe, waaronder Workfront, Frame.io en Creative Cloud.

De belangrijkste voordelen van Adobe Enterprise Storage zijn:

* Geïntegreerde opslaglaag voor creatieve middelen en bedrijfsbeheermiddelen
* Gecentraliseerde machtigingen via Adobe IMS voor veilig toegangsbeheer
* End-to-end asset visibility voor Workfront-, Frame.io- en Creative Cloud-toepassingen <!--coming soon?-->
* Schaalbare opslag en quotabeheer voor bedrijfsbehoeften

Voor meer details, zie [ overzicht van de ondernemingsopslag van Adobe ](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Geïntegreerde revisie en goedkeuring

De integratie van Workfront en Frame.io maakt gebruik van de uniforme goedkeuringsfunctionaliteit van Workfront voor het beheer van revisies en goedkeuringen. Met uniforme goedkeuringen kunt u:

* Recensies en goedkeuringen rechtstreeks vanuit Workfront maken en beheren
* De status van revisies en goedkeuringen bijhouden in real-time
* Feedback en goedkeuringen op één plaats centraliseren
* Ervoor zorgen dat alle belanghebbenden toegang hebben tot de nieuwste versies van middelen
* AI Reviewers gebruiken om beoordelingen van naleving van merk te automatiseren
* en meer

Voor meer informatie, zie [ Verenigde documentgoedkeuringen: artikelindex ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md).


### De viewer Frame.io gebruiken

De integratie verbindt ook met de kijker Frame.io. De viewer Frame.io biedt

* Gereedschappen voor markeringen en opmerkingen
* Versiegeschiedenis en vergelijking
* Opmerkingen met tijdstempel voor videorevisies
* Mobiele toegang voor revisies en goedkeuringen onderweg

Voor meer informatie, zie [ begonnen worden met de integratie Frame.io ](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md).

#### Limieten voor videorevisie

Er is een jaarlijks plafond voor videoproefdrukken vastgesteld op 10% van de totale betaalde Workfront-gebruikerslicenties (Standard and Light) van een organisatie. Dit plafond wordt toegepast op het niveau van de organisatie.

Workfront-beheerders ontvangen meldingen wanneer het gebruik 80% en 100% van de limiet bereikt.

Deze limiet geldt niet voor Enterprise-klanten van Frame.io.

#### Ondersteunde bestandstypen in de viewer Frame.io

De viewer Frame.io ondersteunt alle gangbare typen video, afbeeldingen, audio, PDF en MS® Office. Voor een gedetailleerde lijst van gesteunde dossiers, zie [ Types op Frame.io ](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Toegang tot en licenties voor de Frame.io-viewer

De viewer Frame.io is beschikbaar voor alle Workfront-gebruikers met een betaalde licentie. Er is geen aanvullende Frame.io-licentie vereist als u de Frame.io-viewer wilt gebruiken voor revisies en goedkeuringen met deze integratie.

Als uw organisatie van extra functionaliteit Frame.io, zoals het uploaden van activa rechtstreeks aan projecten in Frame.io wil profiteren, kunt u een Frame.io ondernemingsvergunning kopen. Neem contact op met uw Adobe-accountvertegenwoordiger om een demo te plannen en de voordelen van de volledige Frame.io-oplossing te verkennen.

Bij deze integratie is Workfront-proefdrukfunctionaliteit niet beschikbaar.

## Krachtig projectbeheer in Workfront

Met de integratie van Workfront en Frame.io kunnen projectcoördinatoren Workfront gebruiken om krachtige projectbeheermogelijkheden te plannen, te volgen en te beheren.

Voor meer informatie over het beheren van projecten in Workfront, zie [ Projecten: artikelindex ](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

### Gedwongen conventies voor structuur en naamgeving

Omdat deze integratie gebruikend ESM wordt gebouwd, zijn er sommige gedwongen structuur en noemende overeenkomsten om zich van bewust te zijn wanneer het beheren van projecten en documenten.

* Objectnamen moeten uniek zijn en kunnen niet worden gedupliceerd
* ESM vereist unieke namen voor peer-objecten met hetzelfde bovenliggende item in de hiërarchiestructuur
* Documenten kunnen niet dezelfde naam hebben als ze tot hetzelfde project behoren

Met het oog op deze beperkingen wijzigt Workfront automatisch de naam van objecten of documenten om conflicten te voorkomen.

### Documentbeheer in Workfront

Documenten worden op projectniveau met deze integratie beheerd en kunnen op dit moment niet worden geüpload naar taken of problemen.

Documenttoegang wordt ook op projectniveau beheerd. Als een gebruiker toegang tot een project heeft, kunnen zij tot alle documenten toegang hebben verbonden aan dat project.

<!--Documents can't be dragged as full folders.-->

### Beperkingen voor ervaring met documenten

Omdat deze integratie met behulp van ESM is gemaakt, zijn er enkele beperkingen voor de ervaring met het originele document in Workfront:

#### Beperkingen

De volgende mogelijkheden worden niet opgenomen in deze integratie:

<!--* External document providers-->
* Toegang tot proefdrukken
* Documentviewer in Workfront
* Favoriete documenten
* Documenten aanvragen


<!--#### Temporary limitations

For now, the following capabilities are not available:

* Send documents to Adobe Experience Manager Assets
* Multi-stage approvals
* Upload documents to comments or updates in Workfront
* Upload documents to tasks or issues in Workfront-->



