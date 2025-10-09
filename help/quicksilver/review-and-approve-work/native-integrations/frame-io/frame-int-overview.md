---
product-area: documents
navigation-topic: approvals
title: Overzicht van de integratie van Frame.io
description: Overzicht van de integratie van Frame.io
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b5f0150b-40b5-4386-98bc-374e7ca65b74
source-git-commit: 07fa7207960f424cc8580eb46fe13bd5af4e56a8
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Overzicht van de integratie van Frame.io

Dankzij de integratie van Workfront en Frame.io kunnen projectcoördinatoren projecten beheren en werken plannen in Workfront, terwijl creatieve personen, marketers en belanghebbenden hun middelen in Frame.io kunnen bekijken en goedkeuren.

## Integratievereisten

* Workfront en Frame.io moeten worden geïmplementeerd in dezelfde Identity Management System (IMS)-organisatie.

* Gebruikers kunnen binnen de IMS-organisatie slechts tot één Workfront-instantie behoren.

* De Workfront-instantie moet zijn ingeschakeld op de Adobe Unified Experience en Adobe Enterprise storage.

* De integratie moet door Adobe Professional Services worden gevormd.


## Gebaseerd op Adobe Enterprise Storage

De kern van deze integratie is Adobe Enterprise Storage — een op cloud gebaseerde opslagoplossing die fungeert als centrale opslagplaats voor bedrijfsmiddelen in Adobe, waaronder Workfront en Frame.io. <!--, and Creative Cloud.-->

De belangrijkste voordelen van Adobe Enterprise Storage zijn:

* Geïntegreerde opslaglaag voor creatieve middelen en bedrijfsbeheermiddelen
* Gecentraliseerde machtigingen via het Adobe Identity Management-systeem (IMS) voor veilig toegangsbeheer
* De zichtbaarheid van end-to-end elementen in Workfront en Frame.io <!--, and Creative Cloud apps -->
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

Met de integratie van Workfront en Frame.io kunnen projectcoördinatoren Workfront gebruiken om krachtige projectbeheermogelijkheden te plannen, te volgen en te beheren.

Voor meer informatie over het beheren van projecten in Workfront, zie [ Projecten: artikelindex ](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

### Gedwongen conventies voor structuur en naamgeving

Omdat deze integratie is opgebouwd met behulp van Adobe Enterprise Storage, zijn er bepaalde gedwongen structuren en naamgevingsconventies die u bekend moeten maken bij het beheren van projecten en documenten.

* Objectnamen moeten uniek zijn en kunnen niet worden gedupliceerd
* Adobe Enterprise Storage vereist unieke namen voor peer-objecten met hetzelfde bovenliggende item in de hiërarchiestructuur
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

Documenten worden op projectniveau met deze integratie beheerd en kunnen op dit moment niet worden geüpload naar taken of problemen.

Documenttoegang wordt ook op projectniveau beheerd. Als een gebruiker toegang tot een project heeft, kunnen zij tot alle documenten toegang hebben verbonden aan dat project.

### Beperkingen voor ervaring met documenten

Omdat deze integratie is gebouwd met behulp van Adobe Enterprise Storage, zijn er enkele beperkingen aan de ervaring met het originele document in Workfront:

#### Beperkingen

De volgende mogelijkheden worden niet opgenomen in deze integratie:

<!--* External document providers-->
* Toegang tot proefdrukken in Workfront
* Documentviewer in Workfront
* Favoriete documenten
* Documenten aanvragen


<!--#### Temporary limitations

For now, the following capabilities are not available:

* Send documents to Adobe Experience Manager Assets
* Multi-stage approvals
* Upload documents to comments or updates in Workfront
* Upload documents to tasks or issues in Workfront-->
