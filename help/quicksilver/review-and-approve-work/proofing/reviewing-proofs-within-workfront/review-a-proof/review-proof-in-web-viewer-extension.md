---
product-area: documents
navigation-topic: proofing-overview
title: Interactieve inhoud controleren in de webproefdrukviewerextensie
description: Het Adobe Workfront-revisieprogramma is een browserextensie waarmee u interactieve inhoud in een ZIP-bestand of met een URL kunt controleren.
author: Courtney
feature: Digital Content and Documents
exl-id: 4fea13cc-2d56-466e-8851-6134782e7e80
source-git-commit: 78d9e8e47f8f6777f9211d8f85a3dfbc9405d798
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# Interactieve inhoud reviseren met het Adobe Workfront-revisieprogramma


>[!IMPORTANT]
>
> We raden u aan de Desktop Proofing-viewer te gebruiken voor interactieve inhoud die wordt gehost op een website die SSO-verificatie vereist of die het openen van de site in iFrames, zoals Figma, verhindert.

Het Adobe Workfront-revisieprogramma is een webbrowserextensie waarmee u interactieve inhoud in een ZIP-bestand of met een URL kunt markeren. Het Adobe Workfront-revisieprogramma is beschikbaar in de volgende browsers:

* Firefox
* Chrome
* Edge
* Safari

## De extensie installeren

### Vereisten

* U moet de uitbreiding van de verouderde webviewer verwijderen als u het gereedschap Adobe Workfront Review wilt gebruiken.

### De extensie installeren

Revisoren en fiatteurs moeten het Adobe Workfront-revisieprogramma installeren. in een van de volgende browsers:

* [&#x200B; uitbreiding Firefox &#x200B;](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [&#x200B; de uitbreiding van Chrome &#x200B;](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [&#x200B; Edge &#x200B;](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)

* [&#x200B; uitbreiding Safari &#x200B;](https://apps.apple.com/us/app/adobe-workfront-review-tool/id6741517062?mt=12)



Als u wilt dat interactieve proefdrukken automatisch worden geopend in het Adobe Workfront-revisieprogramma, moet een Workfront-beheerder de proefdrukinstellingen vooraf bijwerken, zoals in de onderstaande secties wordt beschreven.

## Adobe Workfront-revisieprogramma gebruiken in GenStudio for Performance Marketing en Creative Cloud Express

Deze extensie is vereist voor het reviseren van inhoud in GenStudio for Performance Marketing en Creative Cloud Express. Assets wordt automatisch geopend in de webviewer. U hoeft geen accountinstellingen bij te werken.


## Standaardinstellingen voor Workfront-proefdrukken bijwerken

Als u het Workfront-revisieprogramma wilt gebruiken als de standaardviewer voor interactieve inhoud, moet u de standaardwaarden voor proefdrukken in Workfront bijwerken.

>[!IMPORTANT]
>
>We raden u aan de Desktop Proofing Viewer te gebruiken als de inhoud die u wilt controleren zich op een website bevindt die
>
>* SSO-verificatie vereist
>* Hiermee voorkomt u dat de site wordt geopend in iFrames, zoals Figma

### Adobe Workfront-revisieprogramma instellen als standaardviewer voor URL- en ZIP-proefdrukken

Als u het gereedschap Webrevisie wilt gebruiken voor URL- en ZIP-proefdrukken, moet een Workfront-beheerder de standaardinstelling voor interactieve proefdrukken aanpassen.

1. In het Belangrijkste Menu van Workfront, klik **het Bewijzen**.
1. Klik **montages van de Rekening**, dan klik de **Montages** tabel.
1. In de **sectie van de Gebreken van de Bewijs**, vind **Desktop het Bewijzen van Kijker voor Interactieve het proef** en klik **Opstelling**.
1. In het drop-down menu, kies **Gehandicapten**. Interactieve proefdrukken die zijn gemaakt op basis van een URL- of ZIP-bestand, worden nu automatisch geopend in Adobe Workfront Review Tool, een webbrowser.
1. Klik **sparen**.

>[!NOTE]
>
>Deze wijziging is van toepassing op alle interactieve proefdrukken in uw Workfront-exemplaar. We raden u aan de nieuwe ervaring in uw voorvertoningsomgeving te testen voordat u deze inschakelt in Productie. U kunt gemakkelijk terug naar de Kijker van de Desktop schakelen door de **Desktop Proofing Kijker voor Interactieve het proef** rekening te veranderen die terug aan **wordt toegelaten voor alle interactieve proeven**.

### Adobe Workfront-revisieprogramma instellen als standaardviewer voor alleen ZIP-proefdrukken

Als u het gereedschap Webrevisie alleen wilt gebruiken voor ZIP-proefdrukken, moet een Workfront-beheerder de standaardinstelling voor interactieve proefdrukken aanpassen.

1. In het Belangrijkste Menu van Workfront, klik **het Bewijzen**.
1. Klik **montages van de Rekening**, dan klik de **Montages** tabel.
1. In de **sectie van de Gebreken van de Bewijs**, vind **Desktop het Bewijzen van Kijker voor Interactieve het proef** en klik **Opstelling**.
1. In het drop-down menu, kies **Toegelaten slechts voor interactieve proeven die van een URL** worden gecreeerd. Interactieve proefdrukken die zijn gemaakt op basis van een ZIP-bestand, worden nu automatisch geopend in Adobe Workfront Review Tool, een webbrowser. Interactieve proefdrukken die met een URL zijn gemaakt, worden nog steeds geopend in de Desktop Proofing Viewer.
1. Klik **sparen**.

>[!NOTE]
>
>Deze wijziging geldt voor alle ZIP-proefdrukken in je Workfront-exemplaar. We raden u aan de nieuwe ervaring in uw voorvertoningsomgeving te testen voordat u deze inschakelt in Productie. U kunt gemakkelijk terug naar de Kijker van de Desktop schakelen door de **Desktop Proofing Kijker voor Interactieve het proef** rekening te veranderen die terug aan **wordt toegelaten voor alle interactieve proeven**.

