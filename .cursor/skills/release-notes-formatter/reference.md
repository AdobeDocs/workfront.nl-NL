---
source-git-commit: ec081e557ec48adcfcb3833bf11dcee91312ef4e
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---
# Referentiesjablonen voor opmerkingen bij de release

Gedetailleerde sjablonen voor elk type releasenotitiepagina. Deze zijn gebaseerd op de sjablonen in
`help/quicksilver/product-announcements/product-releases/release-note-templates/` en
de feitelijke opmaak die in recente kwartaalversies is gebruikt.

&#x200B;---

## Paginasjabloon productgebied

```markdown
---
title: {Written Quarter} {Year} {Area} enhancements
description: {Written Quarter} {Year} {Area} enhancements
author: {Author}
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: {existing UUID}
---
# {Written Quarter} {Year} {Area} enhancements

This page describes {Area} enhancements made with the {Written Quarter} {Year} release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the {Written Quarter} {Year} release cycle, see [{Written Quarter} {Year} release overview](/help/quicksilver/product-announcements/product-releases/{YY}-q{N}-release-activity/{YY}-q{N}-release-overview.md).

## Feature Title Here

>[!NOTE]
>
>Preview: {Month Day, Year}
>Production fast release: {Month Day, Year}
>Production for everyone: {Month Day, Year}

Feature description paragraph.

For more information, see [Help article title](/help/quicksilver/path/to/article.md).
```

### Regels voor productgebiedpagina&#39;s

- Markeringen (niet HTML) gebruiken voor inhoud van het lichaam
- Elke functie krijgt een H2-kop
- De `>[!NOTE]` -callout moet een lege regel hebben voordat deze wordt uitgevoerd
- De `>[!NOTE]` -indeling is exact:

  ```
  >[!NOTE]
  >
  >Preview: {date}
  >Production fast release: {date}
  >Production for everyone: {date}
  ```

- Als een functie tijdelijk is verwijderd, voegt u na de datum een regel toe:

  ```
  >
  >This feature has been temporarily removed from the Production environment on {date}.
  ```

- Help-koppelingen gebruiken absolute paden die beginnen met `/help/quicksilver/`

&#x200B;---

## Overzicht van paginasjabloon

```markdown
---
title: {Written Quarter} {Year} release overview
description: This page provides information about functionality that is included in the {Written Quarter} {Year} release. These enhancements are planned to become available in the Production environment throughout the quarter.
author: {Author}
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: {existing UUID}
---
# {Written Quarter} {Year} release overview

This page provides information about functionality that is included in the {Written Quarter} {Year} release scheduled for {Release Month} {Year}.

The enhancements on this page are available in the Preview environment. This page will be updated with additional enhancements as the {Written Quarter} {Year} release nears its planned Production release.

>[!IMPORTANT]
>
>
>Monthly and quarterly releases are planned to be available on the Thursday of the second full week of the month, unless otherwise specified.
>
>|Monthly release|Quarterly release|
>|----|----|
>|<ul><li>{VV}.{M} ({Month Day, Year})</li><li>{VV}.{M} ({Month Day, Year})</li><li>{VV}.{M} ({Month Day, Year})</li></ul>|<ul><li>{VV}.{M} ({Month Day, Year})</li></ul>|
>
>Note that for the final release of each quarter ({VV}.{M} this quarter), users on the fast release schedule will receive the release one day early ({Month Day, Year}).
>
>For more information on the fast release process, see [Enable or disable the fast release process](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront enhancements

* [Administrator enhancements](#administrator-enhancements)
* [Document enhancements](#document-enhancements)
* [Project enhancements](#project-enhancements)
* [Reporting enhancements](#reporting-enhancements)
* [Requesting enhancements](#requesting-enhancements)
* [Other enhancements](#other-enhancements)
```

### Tabel met overzichtsfuncties

Elke H3-productsectie bevat een HTML-tabel. Deze exacte structuur gebruiken:

```html
### {Area} enhancements

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
              <tr>
        <td><strong>Feature</strong>
        </td>
        <td><strong>Preview</strong></td>
        <td><strong>Fast release</strong></td>
        <td><strong>Quarterly</strong></td>
        </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/{YY}-q{N}-release-activity/{YY}-q{N}-{area}.md" class="MCXref xref" xrefformat="{para}">Feature Title</a><p>Short description of the feature.</p>
        </td>
        <td><p>{Month Day, Year}</p></td>
        <td><p>{Month Day, Year}</p></td>
        <td><p>{Month Day, Year}</p></td>
    </tr>
            </tbody>
        </table>
```

#### Tabelregels

- Functiecel: `<a>` -tag met `class="MCXref xref" xrefformat="{para}"` gevolgd door `<p>` -beschrijving
- De `href` -koppeling verwijst naar de pagina met het productgebied (geen specifiek anker)
- Datumcellen: verpakt in `<p>` -tags
- Voeg `<p>[!BADGE Off schedule]{type=Neutral}</p>` toe na de koppeling voor items die niet volgens schema zijn
- Leeg `<p></p>` nadat de koppeling is geaccepteerd als er geen badge nodig is
- HTML-inspringing consistent houden met bestaande bestanden

### Secties voor navolgende overzichten

Na alle tabellen voor productgebieden:

```markdown
## Release notes for other areas

### Workfront Fusion enhancements

New features in Workfront Fusion are available in Production at a cadence outside of the standard release schedule. For more information about the latest features, see [Adobe Workfront Fusion release activity](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Workfront Planning enhancements

New features in Workfront Planning are available in Production. For more information about the latest features, see [{Written Quarter} {Year} release activity for Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-{YY}-q{N}.md).

There are no updates for the following at this point in the release:

* Scenario Planner
* Proof
* Goals

## Desktop proofing viewer updates

{Version info if available, otherwise omit section}

## Announcements

{Announcement content}

### API version {NN}

{API version info}

### Workfront Maintenance Updates

For information about the maintenance updates made during the {Written Quarter} {Year} release, see [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Training updates

Explore the latest updates made to learning programs, learning paths, videos, and guides for each Adobe Workfront product release. For more information, see the "What's New" section of the [Workfront Tutorials page](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html).
```

&#x200B;---

## Paginasjabloon weergeven en weergeven

```markdown
---
title: Look-and-feel updates during the {Written Quarter} {Year} release time frame
description: Look-and-feel updates during the {Written Quarter} {Year} release time frame
author: {Author}
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: {existing UUID}
---

# Look-and-feel updates during the {Written Quarter} {Year} release time frame

This page describes minor updates to the look and feel of various areas of the Adobe Workfront application that were made within the {Written Quarter} {Year} release timeframe. These enhancements will be made available in the Production environment a minimum of 2 weeks after releasing to Preview.

For a list of all changes available with the {Written Quarter} {Year} release, see [{Written Quarter} {Year} Release overview](/help/quicksilver/product-announcements/product-releases/{YY}-q{N}-release-activity/{YY}-q{N}-release-overview.md).

## Feature Title

>[!NOTE]
>
>Preview release: {Month Day, Year}; Planned Production release: {Month Day, Year}

Description of the look-and-feel change.
```

&#x200B;---

## Opmaak datumbijschrift

### Productgebiedpagina&#39;s (meerdere regels)

```markdown
>[!NOTE]
>
>Preview: March 5, 2026
>Production fast release: April 15, 2026
>Production for everyone: April 16, 2026
```

### Pagina&#39;s met uiterlijk (één regel)

```markdown
>[!NOTE]
>
>Preview release: March 5, 2026; Planned Production release: March 19, 2026
```

### Wekelijkse pagina&#39;s (één regel)

```markdown
>[!NOTE]
>
>Preview release: February 9, 2023; Planned Production release: February 23, 2023
```

&#x200B;---

## Bekende inconsistenties om te controleren op

1. **Verkeerde overzichtskwartaal** — De pagina&#39;s van het productgebied verbinden soms met het overzicht van het vorige kwart (b.v., `26-q1` in plaats van `26-q2`)
2. **de data van de voorproef die verkeerd jaar** tonen - de lijsten van het Overzicht tonen soms vorig jaar in de kolom van de Voorproef (b.v., &quot;2025&quot;in plaats van &quot;2026&quot;)
3. **Ontbrekende het sluiten `</tr>` markeringen** - sommige de lijstrijen van HTML ontbreken juiste sluitende markeringen
4. **`content-type: release-notes`** — Aanwezigheid in oudere bestanden, weggelaten op nieuwere pagina&#39;s van het 26-q2-productgebied. Volg het patroon van het huidige kwartaal.
5. **Typo in malplaatje** - het blik-en-voelt malplaatje heeft `relesae` in plaats van `release`; altijd de juiste spelling gebruiken
6. **Ontbrekende `<p></p>` na eigenschapverbinding** - sommige overzichtslijstrijen laten de lege `<p>` markering na de `<a>` markering weg
