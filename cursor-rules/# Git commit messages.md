---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---
# Berichten begaan door it

Deze regel altijd toepassen. Wanneer u het ontwerp of een git produceert begaan bericht (bijvoorbeeld in de Controle van Source begaan vakje of wanneer gevraagd in het praatje van de Agent), volg dit formaat.

## Onderwerpregel (alleen eerste regel)

- Ongeveer **50 karakters of minder**.
- vatten de verandering in **dwingende stemming** samen (b.v. &quot;voeg toe...&quot;, &quot;Repareren...&quot;, &quot;Refactor..&quot;).

## Lege regel

Verlaat één **lege lijn** na het onderwerp vóór het lichaam.

## Lichaam (gedetailleerde beschrijving)

- De lijnen van de terugslag bij ongeveer **72 karakters** (met inbegrip van de kogelprefix en de ruimte).
- Gebruik **kogellijnen** voor de verklaring. Elk opsommingsteken moet beginnen met precies een van de volgende:
   - **📖** — gebruik wanneer de verandering **&#x200B;**&#x200B;iets nieuw toevoegt: nieuwe dossiers, nieuwe secties, nieuwe eigenschappen, nieuwe kopballen, net-nieuwe lijnen, of andere greenfield inhoud.
   - **✏️** — gebruik wanneer de verandering **&#x200B;**&#x200B;bestaand werk wijzigt: geeft aan bestaande lijnen uit, werkt aan bestaande secties, heractoren van bestaande code, of verandert in huidige inhoud.

Pas **📖** of **✏️** toe op elk opsommingsteken, zodat duidelijk is wat er is geïntroduceerd en wat er is gewijzigd.

## Sjabloon

Vul de plaatsaanduidingen in (verlaat geen punthaken in het definitieve bericht):

```
<Summarize change(s) in around 50 characters or less>

<More detailed explanatory description of the change wrapped into about 72
characters with bullets. >
```

## Voorbeeld

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```
