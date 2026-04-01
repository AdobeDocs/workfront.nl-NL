---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---
# Pull-aanvragen (PR&#39;s)

Wanneer u een trekverzoektitel of een beschrijving (bijvoorbeeld in GitHub/GitLab of wanneer gevraagd in het praatje van de Agent) ontwerpt of herziet, deze overeenkomsten volgen.

## Voortgekomen uit de Jira-kwestie

- **Source van waarheid:** leidt identiteitskaart van de Uitgave Jira van de **huidige de taknaam van het Git** (bijvoorbeeld een segment die uw project zeer belangrijk patroon aanpassen, zoals `FFENT-8796`).
- **als de taknaam een identiteitskaart van Jira omvat:** gebruik die identiteitskaart in de PR titel (zie hieronder) en verbind het in `# Context` → `## Jira`.
- **als de taknaam geen identiteitskaart van Jira omvat:** Behandel PR als niet verbonden aan een kaartje. **weglaat** de sleutel van Jira van de PR titel (uitgevonden geen kaartje). Neem nog steeds `# Context` → `## Jira` op, met de inhoud exact: `No ticket` (geen koppeling).

## PR-titel

**wanneer de taknaam een identiteitskaart van de Jira- kwestie** omvat, omvat **allebei**:

1. De **identiteitskaart van de Uitgave Jira** (b.v. `FFENT-8001`).
2. **begaat type** (zie lijst hieronder), gebruikend dit patroon:

`{type}/{JIRA-ID}- {short task description}`

Voorbeeld:

`feat/FFENT-8001- Add validation for numVariations in OCAPI request`

Gebruik een beknopte beschrijving in de stijl van het imperatief na identiteitskaart Overeenkomst met het weergegeven spatiëringspatroon: type, schuine streep, Jira-toets met afbreekstreepje, spatie en daarna de beschrijving.

**wanneer de taknaam geen identiteitskaart van de Kwestie Jira** omvat, weglaat het kaartje van de titel en het gebruik:

`{type}- {short task description}`

Voorbeeld:

`docs- Refresh Object Composite API changelog`

### Acceptabele typen toewijzen (gebruik exact deze labels vóór `/`)

- **eigenschap** — voegt een nieuwe eigenschap toe. Wanneer een nieuw inhoudsopgave-item wordt toegevoegd of de JIRA wordt verbonden met een andere `feat` -gelabelde Jira.
- **moeilijke situatie** — moeilijke situatie
- **refactor** — herschrijft/herstructureert code zonder gedrag te veranderen
- **perf** — verbetert prestaties (speciale refactor)
- **stijl** — het formatteren/whitespace slechts; geen betekenisverandering. Alleen bewerkingen
- **test** — voegt of verbetert tests toe
- **documenten** — Nieuwe toegevoegde inhoud. alleen documentatie
- **bouwt** — bouwt hulpmiddelen, CI, gebiedsdelen, projectversie, enz.
- **ops** — infrastructuur, plaatsing, steun, terugwinning, enz.
- **kor** — overige (b.v. `.gitignore`)

## PR-carrosserie — vereiste secties

Gebruik **precies deze top-level secties** (de rubrieken van de Prijsverhoging):

### 1. `# Summary`

Kort overzicht van **wat** veranderde en **waarom** (bedrijfs of technische intent).

### 2. `# Changes`

Organiseren door **dossier**. Voor elk aangeraakt bestand gebruikt u een kop van niveau 2 met het pad in achtertikken en vervolgens opsommingstekens die bewerkingen beschrijven.

Indeling:

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.

## `another/file.ts`
* Another bullet for that file.
```

### 3. `# Context`

Omvat altijd a **Jira** onderafdeling onder `# Context`.

**wanneer de taknaam een identiteitskaart van Jira omvat:** Gebruik een klikbare verbinding aan de kwestie (leidt de sleutel uit de taknaam af).

Indeling:

```markdown
# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

Vervang de sleutel en URL met het daadwerkelijke kaartje. Als meerdere tickets van toepassing zijn, moet u elk afzonderlijk vermelden in dezelfde subsectie.

**wanneer de taknaam geen identiteitskaart van Jira omvat:** houd `## Jira` en gebruik precies:

```markdown
# Context

## Jira
No ticket
```

## Voorbeeld (volledige PR-beschrijving)

```markdown
# Summary
Adds minimum and maximum constraints for numVariations in the Object Composite API v4 OpenAPI spec.

# Changes

## `static/object-composite-v4.json`
* numVariations in OCAPIRequest now includes minimum: 1 and maximum: 3 to align with the allowed range (number of variations to generate).

# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

## Voorbeeld (volledige PR-beschrijving, vertakking zonder Jira-id)

**Titel:** `docs- Refresh Object Composite API changelog`

```markdown
# Summary
Refreshes the changelog for the Object Composite API.

# Changes

## `CHANGELOG.md`
* Documents the latest OCAPI v4 constraint updates.

# Context

## Jira
No ticket
```
