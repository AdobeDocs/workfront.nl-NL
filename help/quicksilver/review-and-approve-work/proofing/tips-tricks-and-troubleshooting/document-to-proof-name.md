---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Documentnaam gewijzigd na uploaden en bevat een ongeldig teken
description: Bepaalde documenten kunnen niet worden geconverteerd naar proefdrukken.
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# Documentnaam gewijzigd na uploaden en bevat een ongeldig teken

## Probleem

Bepaalde documenten kunnen niet worden geconverteerd naar proefdrukken.

## Oorzaak

Bestanden die naar Workfront zijn geüpload, kunnen bepaalde tekens in bestandsnamen niet bevatten. Als een bestand een van de volgende tekens in de bestandsnaam bevat, worden de tekens uit de bestandsnaam verwijderd wanneer het bestand wordt geüpload: `! # % * \ | ' " / ? < > { } [ ]` .

Als een documentnaam wordt bijgewerkt en na de eerste upload een ongeldig teken bevat, mislukt het genereren van de proefdruk.

## Oplossing

Verwijder het ongeldige teken uit de documentnaam:

1. Selecteer het document, dan klik **Details van het Document**.
1. Klik op de documentnaam, verwijder het ongeldige karakter, en druk binnengaan.

   Ongeldige tekens: `! # % * \ | ' " / ? < > { } [ ]`

   ![&#x200B; de naam van het Document &#x200B;](assets/doc-name.png)

1. Vernieuw de pagina en genereer de proefdruk.
