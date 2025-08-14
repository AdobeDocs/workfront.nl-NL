---
product-area: documents
navigation-topic: approvals
title: Aan de slag met de Workfront AI Reviewer
description: Workfront AI Reviewer
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
source-git-commit: bcf9e3eb987bf4c33b994d68276cb04b817c484d
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# Aan de slag met de Workfront AI Reviewer

>[!NOTE]
>
>Deze functie is momenteel in bèta.

Met de Workfront AI Reviewer kunt u de snelheid van de inhoud verhogen en de naleving van het merk optimaliseren in de revisie- en goedkeuringswerkstroom. U kunt AI-revisoren toevoegen aan goedkeuringssjablonen of aan afzonderlijke controle- en goedkeuringsaanvragen in Workfront.

## Toegangsvereisten

Als u AI Reviewers wilt instellen in Workfront, moet u systeembeheerder zijn.

Elke gebruiker kan de AI Reviewer toevoegen aan een revisie- en goedkeuringsaanvraag.


## Vereisten

* Uw organisatie moet zijn gemigreerd naar Adobe IMS (Identity Management System).
* Uw instantie van Workfront moet Verenigde Goedkeuringen hebben toegelaten.
* Adobe moet een ondertekende Adobe Gen AI-overeenkomst in het bestand hebben.
Voor meer informatie bij het ondertekenen van de overeenkomst, zie [ Ondertekenen de overeenkomst van Adobe Gen AI ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).


## Ondersteunde bestandstypen {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="Niet-ondersteund bestandstype"
>abstract="Deze AI Reviewer biedt geen ondersteuning voor het geselecteerde bestandstype. Upload een ondersteund bestandstype of verwijder de AI-revisor om de aanvraag in te dienen."

De AI Reviewer kan de volgende bestandstypen controleren:

* PNG (.png)
* JPEG (.jpeg, .jpg)
* WEBP (.webp)
* GIF zonder animatie (.gif)

## Richtlijnen voor merken instellen

De Workfront AI Reviewer gebruikt de merkrichtlijnen die in Genstudio zijn ingesteld voor Performance Marketing bij het beoordelen van uw inhoud. Momenteel kunt u alleen richtlijnen voor het merk van afbeeldingen instellen. Voor meer informatie, zie [ begonnen worden met Adobe GenStudio for Performance Marketing ](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started).


## AI-revisoren maken

Als er ten minste één merk is ingesteld in GenStudio Foundations, kunnen Workfront-beheerders beginnen met het maken van AI Reviewers in het gedeelte Setup. Die AI-revisoren kunnen vervolgens worden toegewezen aan goedkeuringssjablonen en aan individuele controle- en goedkeuringsaanvragen. Op dit moment kunnen AI-revisoren alleen controleren aan de hand van richtlijnen voor afbeeldingsmerken.

Voor meer informatie, zie [ AI Reviewers ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/set-up-ai-reviewer.md) creëren.

## AI-revisoren toevoegen aan aanvraag voor beoordeling en goedkeuring

Gebruikers kunnen AI-revisoren toevoegen aan bestaande goedkeuringssjablonen of aan afzonderlijke controle- en goedkeuringsaanvragen.

### Goedkeuringssjablonen

Als uw organisatie vaak dezelfde personen toevoegt om aanvragen te controleren en goed te keuren, kunnen gebruikers met een standaardlicentie goedkeuringssjablonen maken in het gedeelte Workfront Setup.

Gebruikers kunnen AI-revisoren toevoegen aan goedkeuringssjablonen om automatisch te controleren of er sprake is van brandcompatibiliteit wanneer een sjabloon wordt gebruikt om een aanvraag te maken.

Zodra gecreeerd, kunnen de goedkeuringsmalplaatjes op activa in het gebied van Documenten van een project, een taak, of een kwestie worden toegepast.

Voor meer informatie, zie [ een Malplaatje van de Goedkeuring voor activa en documenten ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) creëren.

![ malplaatjelijst die AI recensenten toont ](assets/ai-review-templates.png)

### Individuele beoordeling en goedkeuringsaanvraag

Wanneer gebruikers individuele revisie- en goedkeuringsverzoeken maken, kunnen ze een AI Reviewer toevoegen in samenwerking met andere deelnemers of kunnen ze één aanvraag maken met alleen de AI Reviewer om te controleren of de producten voldoen aan het merk.

Voor meer informatie, zie [ een documentoverzicht of goedkeuringsverzoek ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) creëren.


![ AI recensent die aan individueel goedkeuringsverzoek wordt toegevoegd ](assets/ad-ai-reviewer-to-request.png)

## Bekijk de score en feedback van AI Reviewer

Seconden nadat de aanvraag voor een revisie en goedkeuring bij een AI Reviewer is ingediend, zijn de score en feedback van de AI Reviewer beschikbaar in het deelvenster Documentoverzicht, zelfs als andere deelnemers nog bezig zijn met het evalueren en nemen van beslissingen.

Erkenningseigenaars ontvangen ook een e-mail met de kennisgeving dat een revisie op het middel is voltooid. Van e-mail, klik **gaan aan overzicht** en de score en terugkoppelen in Workfront zien.

De AI Reviewer is niet ontworpen als besluitvormer in de beoordelings- en goedkeuringswerkstroom. Het biedt alleen een score en aanbevelingen om het element in overeenstemming te brengen met de opgegeven merkvereisten.

Als de afbeelding lang voldoet aan de richtlijnen voor het merk, kan de ontwerper een nieuwe versie uploaden en kan de eigenaar van de goedkeuring een tweede revisie- en goedkeuringsaanvraag maken met de AI Reviewer, zodat u tussen de versies kunt schakelen en feedback kunt vergelijken.

Voor meer informatie bij het bekijken van scores en koppel terug, zie [ de score en terugkoppelen van de Revisor van de Mening AI ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md).


![ AI recensent terugkoppelt ](assets/ai-reviewer-feedback.png)


## Video doorloopt

>[!VIDEO](https://video.tv.adobe.com/v/3470847/)