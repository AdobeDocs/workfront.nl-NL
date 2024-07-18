---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: Een statische proefdruk voor websites maken met  [!DNL Workfront Proof]
description: U kunt statische proefdrukken maken van uw webpagina's. Daarnaast kunt u verschillende apparaten simuleren door de schermresolutie van de vastgelegde beelden te definiëren.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# Proefexemplaar statische website maken met [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [ het Bewijzen ](../../../review-and-approve-work/proofing/proofing.md).

U kunt statische proefdrukken maken van uw webpagina&#39;s. Daarnaast kunt u verschillende apparaten simuleren door de schermresolutie van de vastgelegde beelden te definiëren.

## Proef van statische website maken

1. Open de [!UICONTROL New proof] pagina, zoals die in [ wordt beschreven produceer Proofs in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).
1. Plak of typ uw URL in het **www.shareyourlink.com** vakje.
1. U kunt deze stap herhalen om meerdere URL&#39;s toe te voegen.
1. Klik net onder dit vak op de resolutie (de standaardwaarde is 1366 x 768) en selecteer de gewenste resoluties in het vak **[!UICONTROL Screensot resolution]** .
Selecteer een lagere resolutie als u ontwerpen voor mobiele apparaten wilt proefdrukken. In het algemeen worden ontwerpen geladen volgens de resolutie van het scherm-/browservenster.

1. Klik op **[!UICONTROL Look for subpages]** als u verbonden pagina&#39;s wilt opnemen die zich in hetzelfde domein of subdomein bevinden als de ingevoerde URL.
   [!DNL Workfront Proof] scant de verbonden pagina&#39;s en geeft ze weer onder de optie **[!UICONTROL Look for subpages]** . U kunt de pagina&#39;s selecteren die u wilt opnemen.

1. Met de functie [!UICONTROL Combine proofs] kunt u alle webpagina&#39;s verzenden als één proefdruk van meerdere pagina&#39;s.
1. Klik **[!UICONTROL Done]**, dan klaar met het vormen van uw proef zoals die in [ wordt verklaard produceer Proofs in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Over met een wachtwoord beveiligde pagina&#39;s en pagina&#39;s waarvoor toestemming is vereist

[!DNL Workfront Proof] kan geen met een wachtwoord beveiligde website vastleggen als een statische proefdruk.

Als u proefdrukken wilt maken van pagina&#39;s waarvoor toestemming is vereist, moet uw IT-team een van de volgende URL&#39;s toevoegen aan de Lijst van gewenste personen van uw bedrijf waarmee het hulpprogramma voor het vastleggen van webpagina&#39;s verbinding maakt:

**clusters van AWS in de V.S.**: webcapture.proofhq.com

**GCP clusters in de V.S.**: webcapture.gcp.proofhq.com

**EMEA clusters**: webcapture.proofhq.eu

>[!NOTE]
>
>We raden interactieve proefdrukken aan in plaats van statische proefdrukken voor interne pagina&#39;s waarvoor verificatie en websites met wachtwoordbeveiliging vereist zijn. Voor meer informatie, zie [ Interactieve inhoudsproeven overzicht ](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

## Informatie over het verwerken van statische websiteproefdrukken

* Animaties, ingesloten video&#39;s, scripts en interacties kunnen niet worden opgenomen in statische websiteproefdrukken. Als u interactieve inhoud wilt proefdrukken, zie [ Proefdrukken in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) in [ produceren Proefdrukken in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

* Proefpagina&#39;s worden over het algemeen voorbereid met een snelheid van ongeveer 20 seconden per pagina. De algemene voorbereidingstijd is echter ook afhankelijk van de servers waarop de pagina&#39;s worden gehost. Het gereedschap wacht 60 seconden op elke verzonden URL die moet worden geladen. Als deze wachttijd wordt overschreden, mislukt het bewijs.
* Als een van de URL&#39;s bij gecombineerde proefdrukken niet reageert op het vastleggereedschap, mislukt de proefdruk.
* [!DNL Workfront Proof] legt webpagina&#39;s vast tot 195 inch lang na het rasteren. Als de webpagina langer is dan deze, mislukt de proefdruk.
* Tekst extraheren is beschikbaar voor alle tekstelementen, maar tekst die als afbeeldingen is geplaatst, wordt niet geëxtraheerd.
* Op de proefdrukken kan op teksthyperlinks worden geklikt en de gekoppelde pagina&#39;s worden geopend op de nieuwe tabbladen van de browser.
* Er kan niet op hyperlinks in de afbeeldingen worden geklikt als de elementen style=&quot;display:block&quot; binnen de tags `<a>` worden gebruikt. We raden u aan deze onderdelen van het paginaontwerp aan te passen.
* Voor de beste resultaten raden we u aan de pagina&#39;s te maken met de beste coderingspraktijken en erkende standaarden.
