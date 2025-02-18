---
title: Verbeteringen beheerder vierde kwartaal 2023
description: Verbeteringen beheerder vierde kwartaal 2023
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7ed37978-b821-488e-9ca1-b81825255be3
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# Verbeteringen beheerder vierde kwartaal 2023

Op deze pagina worden alle beheerderverbeteringen beschreven die zijn aangebracht met de release van het vierde kwartaal van 2023 voor de voorvertoningsomgeving. Deze verbeteringen zijn beschikbaar gesteld in de productieomgeving met de release van 23.10.

Voor een lijst van alle veranderingen beschikbaar op dit punt in het Vierde Kwartaal 2023 versiecyclus, zie [ Vierde Kwartaal 2023 releaseoverzicht ](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## Beslissingen over proefdrukken en documenten beschikbaar voor klanten van het oudere licentiemodel

Oudere klanten die nog niet zijn overgestapt op het nieuwe Adobe Workfront-licentiemodel, kunnen nu in één rapport gegevens zien met het aantal bewijsmiddelen/documentbeslissingen per gebruiker per maand. Deze gegevens zijn beschikbaar wanneer u een rapport Gebruikersbesluiten uitvoert.

Voor meer informatie, zie [ voorwerpen in Adobe Workfront ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) begrijpen en [ bekijk het aantal proef en documentbesluiten voor alle gebruikers ](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/view-number-of-decisions-for-users.md).

## Berekende velden op aangepaste formulieren kunnen nu de joker $$USER gebruiken

Het jokerteken `$$USER` is nu beschikbaar in berekende aangepaste velden en externe opzoekvelden op de nieuwe formulierontwerper. Door naar `$$USER` te verwijzen in een berekening, wordt de id van de huidige gebruiker toegevoegd. U kunt het jokerteken ook gebruiken met een ander veld. `$$USER.{name}` voegt bijvoorbeeld de naam van de huidige gebruiker toe.

Voor meer informatie over berekende gebieden, zie [ berekende gebieden met de vormontwerper ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) toevoegen.

## Waardeopties van een externe API toevoegen aan een aangepast formulier

Een nieuw gebiedstype, **Externe raadpleging**, is nu beschikbaar op de ontwerper van de douanevorm. Wanneer u gegevens op een extern systeem hebt opgeslagen, kunt u met dit veldtype opties laden vanuit een externe API en filteren op basis van andere veldwaarden in het aangepaste formulier.

Wanneer het formulier aan een object wordt toegevoegd, worden de waarden die door de API worden geretourneerd, weergegeven in een vervolgkeuzelijst en kan de gebruiker er een selecteren.

>[!NOTE]
>
>Het nieuwe **Externe raadpleging** gebiedstype is niet beschikbaar op de bouwer van de erfenisvorm.

Voor meer informatie, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.
