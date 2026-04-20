---
product-area: documents
navigation-topic: approvals
title: Aan de slag met de Workfront Content Reviewer
description: Gebruik de Workfront Content Reviewer AI Collaborator om inhoud te beoordelen op basis van richtlijnen van het merk tijdens workflows voor revisie en goedkeuring.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 72fa86e6dc653905181603e0111f65eb0ca5965b
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 0%

---

# Aan de slag met de Workfront Content Reviewer

Content Reviewer is een AI Collaborator (een type AI-agent dat kan worden toegevoegd aan uw projecten, taken en documenten). AI de Medewerkers kunnen in het gebied van de Opstelling worden gevormd en enkel als gebruikers worden toegewezen.

In Workfront helpt Content Reviewer de snelheid van de inhoud te verhogen en de naleving van het merk tijdens het beoordelings- en goedkeuringsproces te verbeteren. U kunt Content Reviewers toevoegen aan goedkeuringssjablonen of deze opnemen in afzonderlijke revisie- en goedkeuringsaanvragen.

## Toegangsvereisten

Als u Content Reviewers wilt instellen in Workfront, moet u systeembeheerder zijn.

Elke gebruiker kan de Content Reviewer toevoegen aan een revisie- en goedkeuringsaanvraag.

## Vereisten

* Uw instantie van Workfront moet Verenigde Goedkeuringen hebben toegelaten.
* Uw organisatie moet GenStudio Foundation hebben.
   * Content Reviewer in Workfront biedt de functionaliteit die in GenStudio Foundation beschikbaar is voor workflows voor het beoordelen en goedkeuren van bedrijfsmiddelen. U hoeft GenStudio Foundation niet rechtstreeks te openen om uw werk te voltooien. Je toegang tot GenStudio Foundation-functionaliteit via Content Reviewer valt onder de voorwaarden van je Workfront-contract.
* Adobe moet een ondertekende Adobe Gen AI-overeenkomst in het bestand hebben.
Voor meer informatie bij het ondertekenen van de overeenkomst, zie [ Ondertekenen de overeenkomst van Adobe Gen AI ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).
* Content Reviewer is niet beschikbaar in Sandbox-omgevingen.


## Ondersteunde bestandstypen {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="Niet-ondersteund bestandstype"
>abstract="Deze Content Reviewer biedt geen ondersteuning voor het geselecteerde bestandstype. Upload een ondersteund bestandstype of verwijder de Content Reviewer om de aanvraag te verzenden."

De Content Reviewer kan de volgende bestandstypen controleren:

* PNG (.png)
* JPEG (.jpeg, .jpg)
* WEBP (.webp)
* GIF zonder animatie (.gif)
* PDF (.pdf)
* PPT (.ppt, .pptx)
* DOC (.doc, .docx)

Als u een niet-ondersteund bestandstype uploadt, is de optie Content Reviewer niet beschikbaar wanneer u een goedkeuringswerkstroom maakt.

## Richtlijnen voor merken instellen

De Workfront Content Reviewer gebruikt de merkrichtlijnen bij het beoordelen van uw inhoud. Workfront-beheerders kunnen richtlijnen voor het merk instellen in het gedeelte Workfront Setup. In GenStudio Foundation gemaakte merken zijn ook beschikbaar in Workfront.

Systeembeheerders moeten de volgende merkrichtlijnen instellen:

1. [Toegang tot merkrechten verlenen](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)
1. [ creeer en beheer merken voor de Recensent van de Inhoud ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).


## Content Reviewers maken

Als ten minste één merk is ingesteld, kunnen Workfront-beheerders beginnen met het maken van Content Reviewers in het gedeelte Setup. U kunt meerdere Content Reviewers maken die zich richten op verschillende richtlijnen:

* **Beeld**: Deze Recensent van Inhoud zal de activa tegen de richtlijnen van het beeldmerk herzien u opstelling in Workfront. [!BADGE Bèta]{type=Positive tooltip="Deze functie is momenteel in bèta."}
   * Systeembeheerders moeten de bètaovereenkomst ondertekenen om deze functie in te schakelen.
* **stem van de Merk**: De recensent van de Inhoud zal de activa tegen de richtlijnen van de merkstem herzien u opstelling in Workfront.

De revisoren van de inhoud kunnen vervolgens worden toegewezen aan goedkeuringssjablonen en individuele revisie- en goedkeuringsaanvragen.

Voor meer informatie, zie [ AI Medewerkers ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md) vormen.

## Inhoudsrevisoren toevoegen aan revisie- en goedkeuringsverzoeken

Gebruikers kunnen Content Reviewers toevoegen aan bestaande goedkeuringssjablonen of aan individuele revisie- en goedkeuringsaanvragen.

### Goedkeuringssjablonen

Als uw organisatie vaak dezelfde personen toevoegt om aanvragen te controleren en goed te keuren, kunnen gebruikers met een standaardlicentie goedkeuringssjablonen maken in het gedeelte Workfront Setup.

Gebruikers kunnen Content Reviewers toevoegen aan goedkeuringssjablonen om automatisch te controleren of er sprake is van naleving van het merk wanneer een sjabloon wordt gebruikt om een aanvraag te maken.

Zodra gecreeerd, kunnen de goedkeuringsmalplaatjes op activa in het gebied van Documenten van een project, een taak, of een kwestie worden toegepast.

Voor meer informatie, zie [ een malplaatje van het goedkeuringswerkschema voor documenten ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) creëren.

![ malplaatjelijst die AI recensenten ](assets/ai-review-templates.png) toont

### Individuele beoordeling en goedkeuringsaanvraag

Wanneer gebruikers individuele revisie- en goedkeuringsverzoeken maken, kunnen ze een Content Reviewer toevoegen met andere deelnemers of kunnen ze één aanvraag maken met alleen de Content Reviewer om te controleren of de producten voldoen aan de merken.

Voor meer informatie, zie [ een werkschema van de documentgoedkeuring ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) creëren.


![ de recensent van de Inhoud die aan individueel goedkeuringsverzoek wordt toegevoegd ](assets/new-stage.png)

## score en feedback van Content Reviewer weergeven

Seconden nadat de revisie- en goedkeuringsaanvraag met een Content Reviewer is verzonden, zijn de score en feedback van de Content Reviewer beschikbaar in het deelvenster Documentoverzicht, zelfs als andere deelnemers nog bezig zijn met het reviseren en nemen van beslissingen.

Erkenningseigenaars ontvangen ook een e-mail met de kennisgeving dat een revisie op het middel is voltooid. Van e-mail, klik **gaan aan overzicht** en de score en terugkoppelen in Workfront zien.

De Content Reviewer is niet ontworpen als besluitvormer in de revisie- en goedkeuringswerkstroom. Het biedt alleen een score en aanbevelingen om het element in overeenstemming te brengen met de opgegeven merkvereisten.

Als het middel niet voldoet aan de richtlijnen voor het merk, kan de ontwerper een nieuwe versie uploaden en kan de eigenaar van de goedkeuring een tweede revisie- en goedkeuringsaanvraag maken met de Content Reviewer.

Voor meer informatie bij het bekijken van scores en koppel terug, zie [ de score en terugkoppelen van de Recensent van de Inhoud van de Mening ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md).

