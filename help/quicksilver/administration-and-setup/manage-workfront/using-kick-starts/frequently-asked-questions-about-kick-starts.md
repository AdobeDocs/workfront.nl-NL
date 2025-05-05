---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart,trap-start,kickstart,trap-start
navigation-topic: use-kick-starts
title: Veelgestelde vragen over Kick-Starts
description: Zoek antwoorden op veelgestelde vragen over het importeren en exporteren van Workfront-gegevens met Kick-Starts.
author: LIsa
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Veelgestelde vragen over Kick-Starts

De volgende vragen worden vaak gesteld over Kick-Starts:

## Waarom ontvang ik deze fout bij het importeren van een Kick-Start-bestand: &quot;Uw bestand was juist, maar er is niets geïmporteerd?&quot;

### Antwoord

Het is mogelijk dat een van de volgende drie elementen ontbreekt in het Kick-Start-bestand:

1. De **isNew** kolom moet aan **WAAR** voor alle punten worden geplaatst u wilt invoeren. **isNew** moet **WAAR** zijn omdat u nieuwe gegevens met een Kick-Begin kunt slechts invoeren. U kunt bestaande gegevens niet wijzigen via Kick-Start. U kunt andere rijen in spreadsheet met **hebben isNew = VALS** maar, zullen deze rijen niet invoeren.

1. &#x200B; Het bestand moet een lege rij hebben voordat de koppen van de gegevens kunnen worden gestart.
1. &#x200B; De Excel-werkbladen hebben de juiste naam of namen nodig.

Wanneer het werken met Kick-Starts, adviseren wij eerst om het Kick-start Malplaatje te downloaden, manueel het met de correcte gegevens te bevolken en dan het terug in Adobe Workfront in te voeren.

Voor meer informatie over het correct invoeren van gegevens in Workfront die Kick-Begint gebruiken, zie [ Gegevens van de Invoer in Adobe Workfront gebruikend een Kick-Begin malplaatje ](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## Waarom ontvang ik deze fout bij het importeren van uren naar Workfront met behulp van een Kick-Start-bestand: &quot;Gebruiker met primaire-sleutelwaarde(n) &quot;null&quot; niet gevonden?&quot;

### Antwoord

De fout verwijst naar GUID van de gebruiker die met de uren wordt geassocieerd.

Om dit aan te pakken:

1. Exporteer een leeg Kick-Begin malplaatje voor het **slechts 1&rbrace; voorwerp van Uren &lbrace;.**\
   Voor meer informatie over het uitvoeren van een leeg Kick-Begin Dossier, zie &quot;het Uitvoeren van het Sjabloon van het Kick-Begin&quot;in [ Gegevens van de Invoer in Adobe Workfront gebruikend een Kick-Begin malplaatje ](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. Kopieer de gegevens handmatig van het originele Kick-Start en plak deze in het lege bestand.\
   Doe dit voor elke kolom.
1. Importeer het nieuwe bestand opnieuw.\
   De Kick-Start kan beter worden geïmporteerd.

## Waarom wordt het landveld niet ingevuld in het gebruikersprofiel bij het importeren Kick-Start?

### Probleem

Wanneer het invoeren van een Kick-Begin van de Gebruiker met het gebied **setCountry**, komen die gegevens niet over aan het land op het gebruikersprofiel.

### Antwoord

Als de gebruiker voor het Verenigde Beheer van de Gebruiker (UUM) of Systeem van Identity Management van de Adobe (IMS) wordt toegelaten, keurt het **gebied van het Land** slechts landcodewaarden (bijvoorbeeld, V.S., GB, IN) goed. Verifieer dat het **setCountry** gebied in uw Kick-Begin malplaatje landcodewaarden alvorens u invoert gebruikt.

Voor meer informatie over het correct invoeren van gegevens in Workfront die Kick-Begint gebruiken, zie [ Gegevens van de Invoer in Adobe Workfront gebruikend een Kick-Begin malplaatje ](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
