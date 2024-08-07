---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1 Verbeteringen voor proefdrukken
description: Op deze pagina worden alle verbeteringen op het gebied van proefdrukken beschreven die zijn opgenomen in de release 2019.1. De functionaliteit is nu beschikbaar in de productieomgeving.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 6b9b847c-dfb5-4285-b8fc-72f33c6a54d0
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# 2019.1 Verbeteringen voor proefdrukken

Op deze pagina worden alle verbeteringen op het gebied van proefdrukken beschreven die zijn opgenomen in de release 2019.1. De functionaliteit is nu beschikbaar in de productieomgeving.

Voor een lijst van alle veranderingen die in 2019.1 worden aangebracht, zie [ 2019.1 overzicht van de versieactiviteit ](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## Voor beheerders

* [Standaardproefdrukrol configureren voor niet-ontvangers die een proefdrukproef openen](#configure-default-proofing-role-for-non-recipients-who-open-a-proof)

## Voor alle gebruikers

* [ Proef Interactieve Inhoud in de Kijker van het Bewijs van het Web ](#proof-interactive-content-in-the-web-proofing-viewer)
* [Standaardsorteervolgorde voor opmerkingen in de Proofingviewer is nu oudst naar nieuwste](#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest)
* [ Verbeterde Recensent voor Commentaren in de Beproefende Kijker verbonden aan een Waaier van Video ](#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video)
* [ Verbinding aan de Details van het Document van een Bericht van het Bewijs of de Beproefende Kijker ](#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer)
* [ verander uw e-mailberichten in de het Proofing Kijker ](#change-your-email-notifications-in-the-proofing-viewer)
* [De achtergrondkleur in de Desktop Proofing Viewer wijzigen](#change-the-background-color-in-the-desktop-proofing-viewer)
* [Browsergegevens in cache wissen met een proefdruk in de Desktop Proofing Viewer](#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer)

## Standaardproefdrukrol configureren voor niet-ontvangers die een proefdrukproef openen {#configure-default-proofing-role-for-non-recipients-who-open-a-proof}

Workfront-beheerders kunnen nu de standaardproefdrukrol configureren voor gebruikers die geen ontvangers zijn in de workflow van de proefdrukproef, maar wel toegang hebben tot de proefdrukproef via het Workfront-object (zoals project, taak of uitgave).

Eerder, toen gebruikers en gasten toegang tot een proef hadden zonder aan zijn werkschema te worden toegevoegd, hun standaard het proefdrukken rol was Reviewer.

Deze functionaliteit is alleen van toepassing op proefdrukken die zijn gemaakt in Workfront, niet in Workfront Proof.

## Interactieve inhoud proefdrukken in de webproefdrukviewer {#proof-interactive-content-in-the-web-proofing-viewer}

Als het beveiligingsbeleid van uw organisatie het gebruik van de standalone Desktop Proofing Viewer-app niet toestaat, kan uw Workfront-beheerder nu interactieve inhoud inschakelen in de Web Proofing Viewer. De inhoud moet in een ZIP-bestand worden gebundeld voordat u de proefdruk maakt.

Zie het artikel voor meer informatie.

VIDEO

## Standaardsorteervolgorde voor opmerkingen in de Proofingviewer is nu oudst naar nieuwste  {#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest}

In de Proofing Viewer is de standaardsorteervolgorde voor opmerkingen op een proefdruk nu Oudst tot Nieuwst, zoals in een verbaal gesprek.

Eerder was de standaardsorteervolgorde Nieuwst naar Oudst.

U kunt een andere sorteeroptie selecteren en deze optie wordt onthouden voor alle andere proefdrukken die u opent.

Zie de sectie in het artikel voor meer informatie.

## Verbeterde revisie voor opmerkingen in de Proofing Viewer gekoppeld aan een videobereik {#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video}

Wanneer u een opmerking reviseert die is gekoppeld aan een bereik met videobeelden in de Proofing Viewer, kunt u nu op Afspelen klikken om het volledige bereik met beeldmateriaal weer te geven. Het afspelen wordt onderbroken wanneer het einde van het bereik is bereikt. De opmerking blijft open, zodat u niet uit het oog verliest waar u zich bevindt.

Eerder, toen u een commentaar voor een waaier van videolengte opende moest u het begin van de waaier manueel vinden door de kaderaantallen te bekijken die op de commentaar worden getoond alvorens Spel te klikken. Anders is de Proofing Viewer begonnen met afspelen op de locatie waar u het laatst in de videotijdlijn hebt geklikt en is de viewer aan het einde van het bereik niet gepauzeerd. De opmerking is samengevouwen wanneer u op Afspelen hebt geklikt. Het is dus niet langer duidelijk welke opmerking u aan het bekijken was.

Zie voor informatie over het bekijken van videoproefdrukken.

VIDEO

## Koppeling maken naar documentdetails via een proefdrukmelding of de proefdrukweergave {#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer}

Wanneer u een e-mail ontvangt waarin u wordt gevraagd een proefdruk te controleren of wanneer u een proefdruk bekijkt in de Proofing Viewer, hebt u nu snel toegang tot de pagina Documentdetails voor de proefdruk. Op deze pagina ziet u het Workfront-object (zoals een taak, project of uitgave) dat aan de proefdruk is gekoppeld. Dit verstrekt context om u te helpen het werk begrijpen u op het bewijs moet doen.

Deze functionaliteit werkt mogelijk alleen voor nieuwe gebruikers die u aan uw systeem toevoegt. Dit is een tijdelijk probleem.

Zie het artikel voor meer informatie.

VIDEO

## Uw e-mailmeldingen wijzigen in de Proofingviewer {#change-your-email-notifications-in-the-proofing-viewer}

Nu kunnen alle revisoren die de proef uitvoeren, opgeven welke proefdrukberichten ze voor een proefdruk willen ontvangen. Dit is met name van belang wanneer wordt samengewerkt met externe belanghebbenden.

Eerder kon alleen de eigenaar van de proefdruk of de verkeersmanager de e-mailwaarschuwingen van een proefdruk configureren voor de controleurs die ze aan de proefdruk hebben toegevoegd. Externe medewerkers konden niet controleren welke e-mailwaarschuwingen ze over de bewijsmiddelen hadden ontvangen omdat ze niet de vereiste toegang tot Workfront hadden, noch het juiste machtigingsniveau.

Deze instellingen staan los van de instellingen voor e-mailwaarschuwingen die u kunt configureren in Workfront.

Voor meer informatie, zie [ berichten voor proefdrukcommentaren en besluiten beheren ](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md)

VIDEO

## De achtergrondkleur in de Desktop Proofing Viewer wijzigen {#change-the-background-color-in-the-desktop-proofing-viewer}

Nu kunt u de achtergrondkleur van de Desktop Proofing Viewer wijzigen van de standaard bijna-zwarte kleur in wit. Hierdoor is het gemakkelijker om inhoud met een transparante achtergrond te controleren.

Voor meer informatie, zie [ het proefdrukken van kijkersmontages ](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md) vormen.

VIDEO

## Browsergegevens in cache wissen met een proefdruk in de Desktop Proofing Viewer {#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer}

Wanneer de cookie- en cacheinstellingen van uw browser zo zijn ingesteld dat inhoud zoals pop-ups wordt geblokkeerd, kan dit blokkeringsgedrag ook optreden in de Desktop Proofing Viewer. Hierdoor kunnen controleurs de pop-upinhoud in uw proefdruk niet zien en er opmerkingen over maken.

Nu kunt u de cachegegevens van de browser wissen die met een proefdruk worden opgeslagen, zodat alle inhoud in de Desktop Proofing Viewer wordt weergegeven en revisoren er opmerkingen over kunnen zien en opmerkingen over kunnen maken.

Voor meer informatie, zie [ het proefdrukken van kijkersmontages ](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md) vormen.

VIDEO
