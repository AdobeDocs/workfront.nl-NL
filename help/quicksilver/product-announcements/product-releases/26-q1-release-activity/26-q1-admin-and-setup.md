---
title: Verbeteringen beheerder eerste kwartaal 2026
description: Verbeteringen beheerder eerste kwartaal 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 5a1af10b7e3e59eb203c0507aeea15db5689e24b
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 0%

---

# Verbeteringen beheerder eerste kwartaal 2026

Op deze pagina worden de verbeteringen van de beheerder beschreven die zijn aangebracht met de release First Quarter 2026 voor de voorvertoningsomgeving. Deze verbeteringen zullen beschikbaar worden gesteld in de productieomgeving, zoals vermeld.

Voor een lijst van alle veranderingen beschikbaar op dit punt in Eerste Kwartaal 2026 versiecyclus, zie [&#x200B; Eerste Kwartaal 2026 releaseoverzicht &#x200B;](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Prioriteiten beheren in de lay-outsjabloon

>[!NOTE]
>
>Deze functie is tijdelijk niet beschikbaar in de voorvertoningsomgeving
>Voorbeeld: 2 december 2025
>Snelle productie: 14 januari 2026
>Productie voor iedereen: 15 januari 2026


U kunt Prioriteiten voor specifieke gebruikers nu in- of uitschakelen in de Indelingssjabloon. Als u voorheen Prioriteiten voor uw organisatie had uitgeschakeld, blijft deze bij deze wijziging uitgeschakeld in de lay-outsjabloon.

Prioriteiten worden automatisch opgenomen voor licentietypen die standaardtoegang tot verzoeken hebben. Bijvoorbeeld, zal een vergunning van de Medewerker Verzoeken, Borden, en Prioriteiten door gebrek in het Belangrijkste Menu zien, terwijl een Externe vergunning slechts Documenten en Borden zal zien omdat het geen toegang heeft om verzoeken te bekijken of voor te leggen.


Voor meer informatie, zie [&#x200B; het Belangrijkste Menu aanpassen gebruikend een lay-outmalplaatje &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

## Controleren op conflicten met meerdere formulieren voor berekende aangepaste velden

>[!NOTE]
>
>Voorbeeld: 18 december 2025
>Snelle productie: 14 januari 2026
>Productie voor iedereen: 15 januari 2026

Hetzelfde berekende veld kan verschillende formules hebben wanneer het is gekoppeld aan verschillende aangepaste formulieren. Als twee of meer formulieren met hetzelfde berekende veld aan een object zijn gekoppeld, moeten de formules op alle formulieren identiek zijn. Het bewerken van de formule is niet toegestaan als de wijziging een conflict kan veroorzaken.

Om de zichtbaarheid te garanderen van objecten die kunnen worden beïnvloed bij het bewerken van een expressie in aangepaste velden, hebben we een optie toegevoegd om te controleren op conflicten. In dit dialoogvenster worden alle objecten weergegeven die kunnen worden beïnvloed door het wijzigen van de formule, gegroepeerd op objecttype. U kunt naar de details van elk object navigeren en de velden bekijken om te bepalen of het veld uit een van de formulieren moet worden verwijderd of dat de expressie ongewijzigd moet blijven.

Voor meer informatie, zie [&#x200B; berekende gebieden aan een vorm &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) toevoegen.


## Invoerdatum en Ingevoerd door id die zijn opgeslagen op aangepaste objecten

>[!NOTE]
>
>Voorbeeld: 13 november 2025
>Snelle productie: 13 november 2025
>Productie voor iedereen: 13 november 2025

De ingangsdatum en de ingevoerde gegevens met de id worden nu opgeslagen op aangepaste formulieren, velden en secties. U kunt deze gegevensopties in rapporten als filters, meningen, of groeperingen gebruiken. Als u deze wilt weergeven in de lijst met aangepaste formulieren, velden of secties in Setup, voegt u Invoerdatum en Ingevoerd door: Naam als kolommen toe aan een nieuwe of bestaande weergave.

>[!NOTE]
>
>De ingangsdatum en ingegaan door identiteitskaart zijn beschikbaar slechts op douaneformulieren, gebieden, en secties die op of na 13 november 2025 worden gecreeerd.

## Updates voor knopnamen bij het bewerken van een lay-outsjabloon

>[!NOTE]
>
>Voorbeeld: 30 oktober 2025
>Snelle productie: 13 november 2025
>Productie voor iedereen: 15 januari 2026

Om meer consistentie met andere gebieden van Opstelling zoals de ontwerper van de douanevorm te verstrekken, zien de knopen u wanneer het uitgeven van een lay-outmalplaatje is veranderd **,** sparen en dicht **, en** annuleert **.** De nieuwe optie, **past** toe, staat u toe om uw veranderingen in het lay-outmalplaatje te bewaren en verder het uitgeven voort te zetten. Eerder, waren de beschikbare opties **sparen** en **annuleert**.

Voor meer informatie, zie [&#x200B; lay-outmalplaatjes &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) creëren en beheren.

## Verbeterd veldbeheer met actieve vlag op aangepaste velden

>[!NOTE]
>
>Voorbeeld: 30 oktober 2025
>Snelle productie: 13 november 2025
>Productie voor iedereen: 15 januari 2026

Als het systeem een groot aantal aangepaste velden bevat, kan het moeilijk zijn deze velden in aangepaste formulieren en rapporten te beheren. U kunt douanevelden nu inactief met de nieuwe **Actieve** vlag merken. Deze markering is beschikbaar wanneer u met een veld werkt op een aangepast formulier of wanneer u een veld uit de lijst Velden toevoegt of bewerkt.

Als u een veld inactief markeert:

* Het is uitgesloten van rapporten, filters, weergaven of andere plaatsen in Workfront waar u een aangepast veld kunt toevoegen
* Het is niet beschikbaar in de veldbibliotheek om aan andere aangepaste formulieren toe te voegen

>[!NOTE]
>
>De uitsluiting van rapporten, filters, weergaven en groepen vindt plaats nadat het veld inactief is geworden. Bestaande rapportelementen die het veld gebruiken, worden niet gewijzigd of verwijderd wanneer het veld inactief wordt gemarkeerd.

Voor meer informatie, zie [&#x200B; een douaneformulier &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.




