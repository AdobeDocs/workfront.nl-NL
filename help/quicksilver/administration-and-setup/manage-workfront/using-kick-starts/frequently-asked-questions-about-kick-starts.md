---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart,trap-start,kickstart,trap-start
navigation-topic: use-kick-starts
title: Veelgestelde vragen over Kick-Starts
description: Zoek antwoorden op veelgestelde vragen over het importeren en exporteren van Workfront-gegevens met Kick-Starts.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 1ebdb3797e30a7e06f4dfd4a7e0e5f540351c126
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Veelgestelde vragen over Kick-Starts

De volgende vragen worden vaak gesteld over Kick-Starts:

## Waarom ontvang ik deze fout wanneer ik probeer om een Kick-Begin dossier in te voeren: &quot;Uw bestand was juist, maar er is niets geïmporteerd?&quot;

### Antwoord

Het is mogelijk dat een van de volgende drie elementen ontbreekt in het Kick-Start-bestand:

1. De **isNew** kolom moet worden ingesteld op **TRUE** voor alle items die u wilt importeren. **isNew** moet **TRUE** omdat u nieuwe gegevens alleen kunt importeren met een Kick-start. U kunt bestaande gegevens niet wijzigen via Kick-Start. U kunt andere rijen in het spreadsheet hebben met **isNew = FALSE** maar deze rijen worden niet geïmporteerd.

1. &#x200B; Het bestand moet een lege rij hebben voordat de koppen van de gegevens kunnen worden gestart.
1. &#x200B; De Excel-werkbladen hebben de juiste naam of namen nodig.

Wanneer het werken met Kick-Starts, adviseren wij eerst om het Kick-start Malplaatje te downloaden, manueel het met de correcte gegevens te bevolken en dan het terug in Adobe Workfront in te voeren.

Voor meer informatie over het correct invoeren van gegevens in Workfront die Kick-Starts gebruiken, zie [Gegevens naar Adobe Workfront importeren met een Kick-startsjabloon](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## Waarom ontvang ik deze fout bij het importeren van uren naar Workfront met behulp van een Kick-Start-bestand: &quot;Gebruiker met waarde(n) &quot;null&quot; niet gevonden?&quot;

### Antwoord

De fout verwijst naar GUID van de gebruiker die met de uren wordt geassocieerd.

Om dit aan te pakken:

1. Een lege Kick-startsjabloon exporteren voor de **Uren** alleen object.\
   Voor meer informatie over het uitvoeren van een leeg Kick-Begin Dossier, zie &quot;het Uitvoeren van het Kick-Begin Malplaatje&quot;in  [Gegevens naar Adobe Workfront importeren met een Kick-startsjabloon](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. Kopieer de gegevens handmatig van het originele Kick-Start en plak deze in het lege bestand.\
   Doe dit voor elke kolom.
1. Importeer het nieuwe bestand opnieuw.\
   De Kick-Start kan beter worden geïmporteerd.

## Waarom wordt het landveld niet ingevuld in het gebruikersprofiel bij het importeren Kick-Start?

### Probleem

Bij het importeren van een Kick-start gebruiker met het veld **setCountry**, die gegevens komen niet naar het land op het gebruikersprofiel.

### Antwoord

Als de gebruiker voor Verenigd Gebruikersbeheer (UUM) of het Systeem van Adobe Identity Management (IMS) wordt toegelaten, **Land** -veld accepteert alleen landcodewaarden (bijvoorbeeld VS, GB, IN). Controleer of de **setCountry** in de Kick-Start-sjabloon worden de waarden van de landcode gebruikt voordat u de sjabloon importeert.

Voor meer informatie over het correct invoeren van gegevens in Workfront die Kick-Starts gebruiken, zie [Gegevens naar Adobe Workfront importeren met een Kick-startsjabloon](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
