---
product-area: documents
navigation-topic: approvals
title: Algemeen overzicht van revisie en goedkeuring
description: Meer informatie over Unified Review en goedkeuringen van Workfront en Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: b5f0150b-40b5-4386-98bc-374e7ca65b74
source-git-commit: d35e6c33479ed051aaa87b07ddf38811fffc0cc0
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# Algemeen overzicht van revisie en goedkeuring

De verenigde overzicht en goedkeuringen die door Workfront en Frame.io worden aangedreven staan projectcoördinatoren toe om projecten te beheren en het werk in Workfront te plannen terwijl de creatieve personen, de verkopers, en de belanghebbenden activa in Frame.io kunnen herzien en goedkeuren.

## Integratievereisten

* Workfront en Frame.io moeten worden geïmplementeerd in dezelfde Identity Management System (IMS)-organisatie.

* Gebruikers kunnen binnen de IMS-organisatie slechts tot één Workfront-instantie behoren.

* De Workfront-instantie moet zijn ingeschakeld op de Adobe Unified Experience en Adobe Enterprise storage.

* De integratie moet door Adobe Professional Services worden gevormd.


## Gebaseerd op Adobe Enterprise Storage

De verenigde revisie en goedkeuringen zijn gebaseerd op Adobe Enterprise Storage — een cloudgebaseerde opslagoplossing die fungeert als centrale opslagplaats voor bedrijfsmiddelen in Adobe, waaronder Workfront en Frame.io. <!--, and Creative Cloud.-->

De belangrijkste voordelen van Adobe Enterprise Storage zijn:

* Geïntegreerde opslaglaag voor creatieve middelen en bedrijfsbeheermiddelen
* Gecentraliseerde machtigingen via het Adobe Identity Management-systeem (IMS) voor veilig toegangsbeheer
* De zichtbaarheid van end-to-end elementen in Workfront en Frame.io <!--, and Creative Cloud apps -->
* Schaalbare opslag en quotabeheer voor bedrijfsbehoeften

Voor meer details, zie [ overzicht van de ondernemingsopslag van Adobe ](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Geïntegreerde revisie en goedkeuring

Met verenigde revisie en goedkeuringen kunt u:

* Recensies en goedkeuringen rechtstreeks vanuit Workfront maken en beheren
* De status van revisies en goedkeuringen bijhouden in real-time
* Feedback en goedkeuringen op één plaats centraliseren
* Ervoor zorgen dat alle belanghebbenden toegang hebben tot de nieuwste versies van middelen
* AI Reviewers gebruiken om beoordelingen van naleving van merk te automatiseren
* en meer

Voor meer informatie, zie [ Verenigde documentgoedkeuringen: artikelindex ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md).


### De viewer Frame.io gebruiken

Met de viewer Frame.io kunt u elementen controleren en goedkeuren. De viewer Frame.io biedt

* Gereedschappen voor markeringen en opmerkingen
* Versiegeschiedenis en vergelijking
* Opmerkingen met tijdstempel voor videorevisies
* Mobiele toegang voor revisies en goedkeuringen onderweg

Voor meer informatie, zie [ begonnen worden met verenigde overzicht en goedkeuring ](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

#### Limieten voor videorevisie

Er is een jaarlijks maximum voor videoproefdrukaanvragen dat is ingesteld op 10% van de totale betaalde Workfront-gebruikerslicenties voor een organisatie: Standard en Light. Dit plafond wordt toegepast op het niveau van de organisatie.

Workfront-beheerders ontvangen meldingen wanneer het gebruik 80% en 100% van de limiet bereikt.

Deze limiet geldt niet voor Enterprise-klanten van Frame.io.

#### Ondersteunde bestandstypen in de viewer Frame.io

De viewer Frame.io ondersteunt alle gangbare typen video, afbeeldingen, audio, PDF en MS® Office. Voor een gedetailleerde lijst van gesteunde dossiers, zie [ Gesteunde Types van Dossier op Frame.io ](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Toegang tot en licenties voor de Frame.io-viewer

De viewer Frame.io is de standaardviewer voor alle Workfront-workflows voor revisie en goedkeuring. Deze wordt automatisch opgenomen voor alle Workfront-gebruikers met een betaalde licentie. Er is geen aanvullende Frame.io-licentie vereist als u de Frame.io-viewer wilt gebruiken voor revisies en goedkeuringen.

Als uw organisatie van extra functionaliteit Frame.io beschikbaar met deze integratie, zoals het uploaden van activa rechtstreeks aan projecten in Frame.io wil profiteren, kunt u een Frame.io ondernemingsvergunning kopen. Neem contact op met uw Adobe-accountvertegenwoordiger om een demo te plannen en de voordelen van de volledige Frame.io-oplossing te verkennen.

Workfront Proofing-functionaliteit is niet beschikbaar bij deze integratie.

## Krachtig projectbeheer in Workfront

Projectcoördinatoren kunnen gebruikmaken van de krachtige mogelijkheden voor projectbeheer van Workfront om werk te plannen, te volgen en te beheren.

Voor meer informatie over het beheren van projecten in Workfront, zie [ Projecten: artikelindex ](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

### Gedwongen conventies voor structuur en naamgeving

Omdat de verenigde overzicht en de goedkeuringen gebruikend de ondernemingsopslag van Adobe worden gebouwd, zijn er sommige gedwongen structuur en noemende overeenkomsten om zich van bewust te zijn wanneer het beheren van projecten en documenten.

* Objectnamen moeten uniek zijn en kunnen niet worden gedupliceerd
* Adobe Enterprise Storage vereist unieke namen voor peer-objecten met hetzelfde bovenliggende element in de hiërarchiestructuur
* Documenten kunnen niet dezelfde naam hebben als ze tot hetzelfde project behoren
* Namen van documenten mogen de volgende speciale tekens niet bevatten: \ / : * ? &quot; | &lt; >
* Documentnamen mogen maximaal 255 tekens bevatten

Met het oog op deze beperkingen wijzigt Workfront automatisch de naam van objecten of documenten om conflicten te voorkomen.

### Delen en machtigingen

Als onderdeel van de integratie, worden de gebruikerstoestemmingen gecontroleerd in Workfront en stroom neer aan Frame.io. Dit betekent u kunt geen gebruiker aan een project in Frame.io uitnodigen of gebruikerstoestemmingen in Frame.io wijzigen. Deze acties moeten worden uitgevoerd via het modaal project voor het delen van projecten in Workfront.

In de volgende tabel wordt aangegeven hoe Workfront-machtigingen worden toegewezen aan Frame.io-machtigingen:

<table>
<tr>
<th>Workfront-gebruikersrechten</th>
<th>Frame.io-gebruikersmachtigingen</th>
</tr>
<tr>
<td>Beheren</td>
<td>Bewerken en delen</td>
</tr>
<tr>
<td>Contribute</td>
<td>Bewerken en delen</td>
</tr>
<tr>
<td>Weergave</td>
<td>Alleen opmerkingen</td>
</tr>
</table>



### Documentbeheer in Workfront

Documenten die naar Workfront worden geüpload, worden opgeslagen in Adobe Enterprise Storage en zijn toegankelijk in zowel Workfront als Frame.io. Wanneer u een document uploadt naar een taak of uitgave in Workfront, wordt een door het systeem gegenereerde map gemaakt in Adobe Enterprise storage die de machtigingen van de taak of uitgave overneemt. Alle documenten die naar die taak of uitgave zijn geüpload, worden in die map opgeslagen en nemen er rechten van over. Voor meer informatie over documenten in Workfront, zie [ het nieuwe overzicht van het documentengebied ](/help/quicksilver/documents/managing-documents/documents-area.md) en [ de toestemmingen van Objecten en het overzicht van het toegangsniveau voor het model van de ondernemingsopslag van Adobe ](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

### Beperkingen voor ervaring met documenten

De volgende documentmogelijkheden worden niet opgenomen:

<!--* External document providers-->
* Toegang tot proefdrukken in Workfront
* Documentviewer in Workfront
* Favoriete documenten
* Documenten aanvragen