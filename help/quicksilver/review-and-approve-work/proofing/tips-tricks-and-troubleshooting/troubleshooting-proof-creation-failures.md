---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: Problemen met het maken van proefdrukken oplossen
description: Het proefdrukproces omvat zowel importeren als het genereren van proefdrukken. Wanneer u een proefdruk maakt, kan het gebeuren dat een bestand niet wordt geïmporteerd of dat de proefdruk niet wordt gegenereerd nadat het bestand is geïmporteerd.
author: Courtney
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---


# Problemen met het maken van proefdrukken oplossen

Het proefdrukproces omvat zowel importeren als het genereren van proefdrukken. Wanneer u een proefdruk maakt, kan het gebeuren dat een bestand niet wordt geïmporteerd of dat de proefdruk niet wordt gegenereerd nadat het bestand is geïmporteerd.

>[!NOTE]
>
> Als het document dat u probeert aan te tonen, niet aan een van de criteria voldoet die in deze sectie worden vermeld, kunt u contact opnemen met de Technische Ondersteuning van Adobe Workfront voor verder onderzoek.

## Redenen voor mislukte import

* U hebt een gecombineerde proefdruk gemaakt die meer dan 50 bestanden bevat.

## Redenen voor het aantonen van defecte productie

* Het bestandstype wordt niet ondersteund.\
  Voor een lijst van gesteunde dossiertypes, zie [&#x200B; Ondersteunde het proef dossiertypes en het overzicht van groottegrenzen &#x200B;](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

* De bestandsstructuur is een niet-standaardstructuur voor het bestandstype.
* Het bestand is beveiligd met een wachtwoord of het kopiëren van inhoud is uitgeschakeld.

  In tegenstelling tot andere bestandstypen kunnen PDF-bestanden worden gegenereerd in proefdrukken als de beveiligingsinstelling voor het kopiëren van inhoud is ingesteld op Toestaan op de PDF.

* De paginalengte of het aantal pagina&#39;s overschrijdt de limiet.

  De maximaal toegestane paginalengte is 195 duim na het rasteren; het maximum toegestane paginanummer is 1.000 pagina&#39;s voor één enkel bewijs.

* Het bestand is beschadigd of beschadigd.
* De deadline van de workflow voor een nieuwe proefversie is in het verleden.

  Dit komt voor wanneer u een nieuwe proefdrukversie gebruikend een snelle proefdrukmethode creeert en **produceert automatisch proeven wanneer het uploaden van documenten** wordt geselecteerd. De nieuwe proefdrukversie probeert de werkschemarijdtermijnen van de eerder geproduceerde proef te nemen. Het genereren van het bewijs mislukt als deze deadline in het verleden ligt. Om dit te verhelpen, kunt u de werkschematermijnen op de vorige versie in de toekomst plaatsen, of een nieuwe proefdrukversie produceren. Als u een nieuwe versie produceert, gebruik **Meer > Nieuwe Versie > Bewijs** en selecteer **deadlines van het Werkschema in de toekomst**.

* Bij het testen van PDF-bestanden zijn de volgende redenen voor het genereren van de proef:

   * Lettertypen en afbeeldingen zijn gekoppeld vanuit externe bronnen (bijvoorbeeld van uw lokale bestandssysteem)

     Lettertypen en afbeeldingen moeten in het PDF-bestand zijn ingesloten om op een andere computer of in Workfront Proof te kunnen worden weergegeven.

   * Het PDF-bestand bevat lege lagen of transparante of overlappende velden.

     Als u niet kunt bepalen welke laag of voorwerp dit veroorzaakt, voer het ontwerp/document als geoptimaliseerde PDF (dit verwijdert alle ongewenste elementen).

