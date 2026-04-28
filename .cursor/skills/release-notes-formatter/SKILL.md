---
name: release-notes-formatter
description: Maak en valideer de opmerkingen bij de Workfront-release voor consistentie, correcte structuur en juiste koppelingen. Alleen gebruiken voor releaseopmerkingenbestanden in directory's met productreleases of wanneer de gebruiker opmerkingen bij de release, productreleases of driemaandelijkse releases vermeldt. Niet toepassen op artikelen of algemene documentatie.
source-git-commit: ec081e557ec48adcfcb3833bf11dcee91312ef4e
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---


# Opmaak opmerkingen bij release

Maakt en valideert Adobe Workfront-releaseopmerkingen in de map `help/quicksilver/product-announcements/product-releases/` .

## Paginatypen

Identificeer het paginatype van dossierweg en inhoud:

| Paginatype | Bestandspatroon | Sjabloon |
|-----------|-------------|----------|
| **Overzicht** | `{YY}-q{N}-release-overview.md` | [ reference.md#overview ](reference.md#overview-page-template) |
| **Gebied van het Product** | `{YY}-q{N}-{area}.md` | [ reference.md#product-area ](reference.md#product-area-page-template) |
| **Planning** | `planning-release-activity-{YY}-q{N}.md` | Vergelijkbaar met productgebied |
| **kijken en voelen** | `look-and-feel-updates-{YY}-q{N}.md` | [ reference.md#look-and-feel ](reference.md#look-and-feel-page-template) |

## Opmaakworkflow

### Stap 1: Achtergrond valideren

Vereiste velden voor alle pagina&#39;s met opmerkingen bij de release:

```yaml
---
title: <descriptive title>
description: <matches or summarizes the title>
author: <author name>
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: <existing UUID — never generate or change>
---
```

Regels:
- `feature` moet exact `Product Announcements` zijn
- `recommendations` moet exact `noDisplay, noCatalog` zijn
- Nooit een `exl-id` uitvinden — alleen opnemen als er al een bestaat
- Voeg `draft: Probably` niet toe aan echte pagina&#39;s (alleen sjablonen)

### Stap 2: Structuur op paginatype valideren

#### Productgebiedpagina&#39;s

1. **H1**: `{Written Quarter} {Area} enhancements`
   - Voorbeeld: `# Second Quarter 2026 Administrator enhancements`
   - Het kwartaal moet worden opgeschreven: &quot;First Quarter&quot;, &quot;Second Quarter&quot;, &quot;Third Quarter&quot;, &quot;Fourth Quarter&quot;

2. **Intro paragraaf**: Beschrijft het gebied en de verbindingen aan het overzicht
   - Moet met het **overzichtsdossier 1 van het correcte kwart** verbinden
   - Veelvoorkomende fout: koppelen naar vorig kwartaal (bijvoorbeeld `26-q1` in plaats van `26-q2` )

3. **H2 per eigenschap**: Functietitel als kop
   - **Nieuwste eigenschappen eerst** — de meest recente versienota moet als eerste H2 na de intro paragraaf verschijnen
   - Oudere functies volgen in omgekeerde chronologische volgorde

4. **callout blok van de Datum** na elke H2:

```markdown
>[!NOTE]
>
>Preview: {Month Day, Year}
>Production fast release: {Month Day, Year}
>Production for everyone: {Month Day, Year}
```

5. **Lichaam**: Functiebeschrijving en koppeling naar Help-documentatie

#### Overzichtspagina&#39;s

1. **H1**: `{Written Quarter} release overview`

2. **Intro paragraaf** met geplande versiemaand

3. **`>[!IMPORTANT]`blok** met de lijst van het versieschema

4. **H2`Adobe Workfront enhancements`** met lijst met ankerkoppelingen:

```markdown
* [Administrator enhancements](#administrator-enhancements)
* [Document enhancements](#document-enhancements)
```

5. **H3 per productgebied** met de eigenschaplijst van HTML (zie [ reference.md ](reference.md#overview-feature-table))
   - Binnen elke lijst, **nieuwste eigenschappen eerst** - de meest recente rij verschijnt bij de bovenkant van de lijst (na de kopbalrij)

6. **het slepen secties** (H2): Opmerkingen bij de release voor andere gebieden, updates van viewer voor desktopproefdrukken, aankondigingen, API-versie, onderhoudsupdates, trainingsupdates

### Stap 3: Koppelingen valideren

- **verbinding van het Overzicht in de pagina&#39;s van het productgebied**: Moet naar hetzelfde kwartaal verwijzen
   - Juist: `26-q2-release-activity/26-q2-release-overview.md`
   - Onjuist: `26-q1-release-activity/26-q1-release-overview.md`
- **de verbindingen van het Anker in overzicht**: Moet overeenkomen met de H3-id&#39;s (kleine letters, koppeltekens)
- **de verbindingen van de Eigenschap in overzichtstabellen**: Moet gebruiken `class="MCXref xref" xrefformat="{para}"`
- **van de Hulp documentverbindingen**: Moet beginnen met `/help/quicksilver/`

### Stap 4: Datums valideren

- Indeling: `{Month} {Day}, {Year}` (bijvoorbeeld &quot;12 maart 2026&quot;)
- `TBD` gebruiken voor onbekende datums
- Datums op de pagina met productgebieden `>[!NOTE]` moeten overeenkomen met de bijbehorende tabelrij
- Voorvertoningsdatums moeten voorafgaan aan productiedata

### Stap 5: Algemene correcties

Deze correcties toepassen bij het opmaken:

| Probleem | Repareren |
|-------|-----|
| Onjuist overzicht van het kwartaal van koppelingen | Bijwerken om overeen te komen met het eigen kwartaal van het bestand |
| Ontbrekend `>[!NOTE]` datumblok | Blok toevoegen na kop van functie H2 |
| Inconsistente datumnotatie | Standaardiseren tot `Month Day, Year` |
| Ontbrekende lege regel voor `>[!NOTE]` | Lege regel toevoegen |
| Extra spaties in bijschriftlijnen | Navolgende witruimte bijsnijden |
| HTML in productgebiedpagina&#39;s | Als markering behouden (HTML is alleen voor overzichtstabellen) |
| Ontbrekend `exl-id` | Laat het weg — genereren er geen |

## Naamgevingsconventies voor bestanden

| Type | Patroon | Voorbeeld |
|------|---------|---------|
| Overzicht | `{YY}-q{N}-release-overview.md` | `26-q2-release-overview.md` |
| Productgebied | `{YY}-q{N}-{area-slug}.md` | `26-q2-admin-and-setup.md` |
| Map | `{YY}-q{N}-release-activity/` | `26-q2-release-activity/` |

Slakken in standaardgebied: `admin-and-setup`, `documents`, `projects`, `reports`, `requests`, `other`

## Kwarttoewijzing

| Kwart | Geschreven formulier | Maanden |
|---------|-------------|--------|
| V1 | Eerste kwartaal | Jan-Mar |
| V2 | Tweede kwartaal | Apr-Jun |
| V3 | Derde kwartaal | Jul-sep |
| V4 | Vierde kwartaal | okt-dec |

De driemaandelijkse productierestitutie landt doorgaans op de donderdag van de tweede volledige week van de laatste maand van het kwartaal.

## Controlelijst voor validatie

Controleer bij het bekijken van een bestand met releaseopmerkingen:

- [ ] De voorgrond heeft alle vereiste gebieden met correcte waarden
- [ ] H1 komt overeen met de indeling van het paginatype
- [ ] Koppeling in overzicht verwijst naar het juiste kwartaal
- [ ] Elke functie heeft een `>[!NOTE]` datumblok (pagina&#39;s in het productgebied)
- [ ] De datumnotatie is consistent (`Month Day, Year`)
- [ ] De tabelrijen met functies in het overzicht komen overeen met de inhoud van de productpagina
- [ ] Geen verbroken interne koppelingen
- [ ] Ankerkoppelingen in overzicht komen overeen met ID&#39;s van H3-sectie
- [ ] Functies worden als nieuwste geordend (zowel pagina&#39;s voor productgebieden als overzichtstabellen)

## Aanvullende bronnen

- Voor volledige HTML malplaatjes en voorbeelden, zie [ reference.md ](reference.md)
