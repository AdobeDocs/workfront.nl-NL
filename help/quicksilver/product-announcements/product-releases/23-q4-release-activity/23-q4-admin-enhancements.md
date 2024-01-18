---
title: Verbeteringen beheerder vierde kwartaal 2023
description: Verbeteringen beheerder vierde kwartaal 2023
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7ed37978-b821-488e-9ca1-b81825255be3
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Verbeteringen beheerder vierde kwartaal 2023

Op deze pagina worden alle beheerderverbeteringen beschreven die zijn aangebracht met de release van het vierde kwartaal van 2023 voor de voorvertoningsomgeving. Deze verbeteringen zijn beschikbaar gesteld in de productieomgeving met de release van 23.10.

Voor een lijst van alle veranderingen beschikbaar op dit punt in het Vierde Kwart de versiecyclus van 2023, zie [Overzicht release 4de kwartaal 2023](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## Beslissingen over proefdrukken en documenten beschikbaar voor klanten van het oudere licentiemodel

Oudere klanten die nog niet zijn overgestapt op het nieuwe Adobe Workfront-licentiemodel, kunnen nu in één rapport gegevens zien met het aantal bewijsmiddelen/documentbeslissingen per gebruiker per maand. Deze gegevens zijn beschikbaar wanneer u een rapport Gebruikersbesluiten uitvoert.

Zie voor meer informatie [Objecten in Adobe Workfront begrijpen](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) en [Het aantal proef- en documentbeslissingen voor alle gebruikers weergeven](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/view-number-of-decisions-for-users.md).

## Berekende velden op aangepaste formulieren kunnen nu de joker $$USER gebruiken

De `$$USER` jokerteken is nu beschikbaar in berekende aangepaste velden en externe opzoekvelden op de nieuwe formulierontwerper. Verwijzen `$$USER` in een berekening wordt de huidige gebruikersnaam toegevoegd. U kunt het jokerteken ook gebruiken met een ander veld. Bijvoorbeeld: `$$USER.{name}` voegt de naam van de huidige gebruiker toe.

Zie voor meer informatie over berekende velden [Berekende velden toevoegen met de formulierontwerper](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Waardeopties van een externe API toevoegen aan een aangepast formulier

een nieuw veldtype, **Externe zoekopdracht**, is nu beschikbaar op de aangepaste formulierontwerper. Wanneer u gegevens op een extern systeem hebt opgeslagen, kunt u met dit veldtype opties laden vanuit een externe API en filteren op basis van andere veldwaarden in het aangepaste formulier.

Wanneer het formulier aan een object wordt toegevoegd, worden de waarden die door de API worden geretourneerd, weergegeven in een vervolgkeuzelijst en kan de gebruiker er een selecteren.

>[!NOTE]
>
>De nieuwe **Externe zoekopdracht** veldtype is niet beschikbaar in de verouderde formulierbuilder.

Zie voor meer informatie [Een formulier ontwerpen met de formulierontwerper](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
