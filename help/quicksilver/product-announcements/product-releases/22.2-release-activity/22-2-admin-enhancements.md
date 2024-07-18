---
title: 22.2 Beheerdersverbeteringen
description: 22.2 Beheerdersverbeteringen
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 55fb0b85-937d-4903-8a64-6f627dd4291f
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 0%

---

# 22.2 Beheerdersverbeteringen

Op deze pagina worden alle beheerderverbeteringen beschreven die zijn aangebracht met de versie 22.2 voor de voorvertoningsomgeving. Deze verbeteringen worden beschikbaar gesteld in de productieomgeving

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

4 april 2022. Voor een lijst van alle veranderingen beschikbaar met de versie 22.2, zie [ 22.2 Overzicht van de Versie ](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Een aangepast formulier configureren om met meerdere objecttypen te werken

Nu kunt u een nieuw of bestaand aangepast formulier configureren om te werken met meerdere objecttypen, waardoor het formulier veel nuttiger wordt. Gebruikers kunnen het formulier toevoegen en invullen op alle typen objecten waarvoor u het configureert.

Eerder kon u een aangepast formulier zo configureren dat het slechts met één objecttype kon werken.

Deze functionaliteit werkt met alle aangepaste formulieren die eerder in uw Workfront-systeem zijn gemaakt. Als u bijvoorbeeld al een aangepast formulier hebt dat is gemaakt voor het taakobjecttype, kunt u het formulier nu zo configureren dat het ook werkt met andere objecttypen, zoals Project en Issue.

Voor meer informatie, zie het sectie [ Begin creërend een douaneformulier ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start) in artikel [ creeer of geef een douaneformulier ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) uit.

>[!NOTE]
>
>* Op het moment dat deze functie voor het eerst in de voorbeeldweergave werd geïntroduceerd, konden we tijdelijk geen aangepast formulier voor meerdere objecten kopiëren. Die mogelijkheid werd op 24 maart ingeschakeld. Voor informatie over het kopiëren van een douanevorm, zie [ Kopieer een douanevorm om nieuwe tot stand te brengen ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).
>* In een berekend aangepast veld zijn sommige velden waarnaar u verwijst mogelijk niet compatibel met objecttypen die zijn geconfigureerd voor het formulier. Onze oplossing is een jokerkaart waarmee de berekening verschillende waarden kan uitvoeren, afhankelijk van het object waaraan het formulier is gekoppeld. Op 24 maart hebben we de wilde kaart toegevoegd. Voor informatie over hoe te om het te gebruiken, zie de sectie [ Berekende douanegebieden in multi-objecten douaneformulieren ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat) in het artikel [ berekende gegevens aan een douaneformulier ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) toevoegen.
>* Voor sectie-einden in aangepaste formulieren hebben we een set algemene weergave- en bewerkingsmachtigingen gemaakt die werken voor alle objecttypen die u kunt configureren voor een formulier. In één scenario, ontdekten wij dat één van deze toestemmingen, Beperkte Edit, fouten op een vorm kon veroorzaken. Dit werd vastgesteld op 24 maart. Voor meer informatie over sectieonderbrekingen, zie [ een sectieonderbreking aan een douaneformulier ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md) toevoegen.
>

## De blauwdrukcatalogus is beschikbaar voor alle gebruikers en beheerders kunnen aanvragen toestaan

Alle Adobe Workfront-gebruikers kunnen nu door de catalogus met beschikbare blauwdrukken bladeren. Voor meer informatie, zie [ doorbladeren de catalogus van blauwdrukken en verzoekinstallatie van blauwdrukken ](../../../administration-and-setup/blueprints/browse-catalog.md).

Bovendien kan de systeembeheerder toegang voor gebruikers toestaan om installatie van blauwdrukken te verzoeken. Als u een aanvraagwachtrij toewijst om de aanvragen op te slaan, kunnen gebruikers aanvragen indienen in de blauwdrukcatalogus. Voor meer informatie, zie [ toegang tot blauwdrukken ](../../../administration-and-setup/blueprints/configure-access-to-blueprints.md) vormen.

## Een afbeelding toevoegen aan een aangepast formulier

In een aangepast formulier dat u maakt of bewerkt, kunt u nu een afbeelding toevoegen en informatieve of instructieve knopinfo opnemen die gebruikers kunnen lezen wanneer ze de muisaanwijzer op de afbeelding plaatsen.

Dit kan bijvoorbeeld handig zijn om branding voor een nieuw product weer te geven of om visuele informatie te geven die mensen nodig hebben wanneer ze het formulier invullen.

Eerder waren aangepaste formulieren volledig gebaseerd op tekst.

>[!NOTE]
>
>In de nieuwe Adobe Workfront zijn gebieden zichtbaar die nog niet zijn gemoderniseerd, zoals het vak dat wordt weergegeven wanneer u items in bulk bewerkt, worden aangepaste formulierafbeeldingen niet weergegeven. Ze zullen worden weergegeven wanneer we deze gebieden blijven bijwerken.

Voor meer informatie, zie [ een activa widget in een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md) toevoegen of uitgeven.

## Nieuwe standaardconfiguraties op toegangsniveau

Om beter aan de behoeften van de meeste beheerders aan te passen die nieuwe toegangsniveaus creëren, hebben wij de standaardconfiguratie voor de &quot;verfijnen uw montages&quot;hieronder vermelde opties veranderd. Deze worden weergegeven wanneer u op het tandwielpictogram ![](assets/gear-icon-in-access-levels.png) op de knop Bewerken klikt.

Met al deze wijzigingen wordt een optie uitgeschakeld die eerder standaard was ingeschakeld. Als dit niet aan de behoeften van uw organisatie past, kunt u hen toelaten wanneer u opstelling een nieuw toegangsniveau, of om het even welk tijd later.

>[!IMPORTANT]
>
>Deze standaardconfiguratieverandering beïnvloedt slechts toegangsniveaus die u van nu creeert, niet om het even welke die u eerder creeerde.

* In een nieuw toegangsniveau met een de vergunningstype van het Plan:

   * Delen op het hele systeem is nu uitgeschakeld voor projecten, taken, problemen, portfolio&#39;s, programma&#39;s, rapporten, filters, documenten en sjablonen.
   * De mening de Ingebouwde Rapporten en de Rapporten van het Aandeel Openbaar zijn ook gehandicapt voor rapporten.
   * Documenten delen is ook voor documenten uitgeschakeld.

* In een nieuw toegangsniveau met een de vergunningstype van het Werk:

   * Delen op het hele systeem is nu uitgeschakeld voor filters en documenten.
   * Documenten delen is ook voor documenten uitgeschakeld.

* In een nieuw toegangsniveau met een vergunningstype van het Verzoek of van het Overzicht:

   * Delen op het hele systeem is nu uitgeschakeld voor filters.

## Een groep deactiveren

Naarmate uw interne organisaties veranderen, moet u mogelijk stoppen met het gebruik van bepaalde groepen in Workfront en nieuwe maken. Om dit te helpen, hebben wij de capaciteit toegevoegd om een groep te deactiveren zonder zijn historische gegevens te verliezen. Voor gewone gebruikers die ze niet hoeven te zien, worden inactieve groepen gewist uit groepsday-aheadvelden.

U kunt nog steeds opties, voorkeuren en objectkoppelingen zoeken en configureren voor inactieve groepen die u beheert. Als u een groep deactiveert, verandert er niets aan de objecten waaraan de groep is gekoppeld.

Eerder was het niet mogelijk om een groep te deactiveren.

Voor meer informatie, zie [ een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md) deactiveren of reactiveren.

## Verbeteringen in de historie van de blauwdrukinstallatie

Wanneer u een blauwdruk installeert, toont een bericht nu de specifieke voorwerpen (zoals rollen, teams, of groepen) die met succes met de blauwdruk en om het even welke voorwerpen werden geïnstalleerd die om niet konden installeren. U kunt ook de lijst met geïnstalleerde objecten weergeven op de pagina Vervagingsdetails door op Details weergeven te klikken naast een specifieke installatie in de tabel met installatiegeschiedenis.

Voor meer informatie, zie [ een blauwdruk ](../../../administration-and-setup/blueprints/blueprints-install.md) installeren.

![](assets/blueprints-installation-history-350x95.png)

## Er wordt nu een waarschuwing weergegeven wanneer u een alleen voorbeeldontwerp in productie installeert

Bepaalde blauwdrukken kunnen alleen worden geïnstalleerd in de voorbeeldomgeving voor testdoeleinden.

Als u toegang hebt tot inhoud met alleen voorvertoning in uw productieomgeving, Sandbox 1 of Sandbox 2, is de installatieknop niet actief en ziet u mogelijk een waarschuwingsbericht.

Voor meer informatie, zie [ een blauwdruk ](../../../administration-and-setup/blueprints/blueprints-install.md) installeren.
