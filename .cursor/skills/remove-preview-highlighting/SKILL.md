---
name: remove-preview-highlighting
description: ""
source-git-commit: 3e76f4a798a55a674a5ada2661c4b6bbb55195f2
workflow-type: tm+mt
source-wordcount: '891'
ht-degree: 0%

---


# Markering voor voorvertoningen verwijderen (Workfront)

## Bereik

Pas slechts toe wanneer **allen** waar zijn:

1. De gebruiker verzocht dit werkschema (b.v. zegt **&quot;voorproefbenadrukking verwijderen&quot;** of duidelijk de zelfde intent).
2. Het weg van het dossier van de Prijsverhoging **bevat** niet **`product-announcements`** (sluit de volledige omslagboom, b.v. versienota&#39;s, bèta&#39;s, aankondigingen onder `help/quicksilver/product-announcements/` uit).
3. Het dossier van de Prijsverhoging is **niet** vermeld onder **[Uitgesloten wegen](#excluded-paths)** hieronder.
4. De voorgrond van het Markeringen-bestand bevat **`Courtney`** op de `author:` -regel (enige auteur of coauteur).
5. Het artikel heeft **minstens één** van:
   - De voorproef-milieu **taal in lichaamseigen of echte fragmentparagrafen** (typische patronen: &quot;benadrukte informatie,&quot;het milieu van de Voorproef,&quot;nog niet over het algemeen beschikbaar,&quot;snel-versie nota&#39;s)— **niet** een gelijke van **verbindingstekst alleen** op een TOC/indexpagina (zie hieronder); of
   - elk HTML-element met **`class="preview"`** (bijvoorbeeld `<span class="preview">` , `<div class="preview">` ); of
   - Een voorproeffragment **variabele** zoals **`{{highlighted-preview}}`** of **`{{highlighted-preview-article-level}}`**.

Als het bereik onduidelijk is, bevestigt u dit voordat u gaat bewerken.

**TOC/indexpagina&#39;s - overslaat altijd dit geval:** **** zet nooit een dossier op de inventaris wanneer **slechts** voorproef-gerelateerde formulering **binnen** de vertoningstekst van een prijsdaling van de verbinding die bij **een ander** artikel richt (b.v. *verzend een rapport in het milieu van de zandbak van de Voorproef )*) **en** het dossier heeft **geen** `class="preview"`, **geen** fragmentvariabelen, en **geen** voorproefboilerplate in **prose buiten verbindingen**. Dit is geen voorproefmarkering op die pagina-het is slechts een verwijzing van TOC. Is op om het even welke index/TOC, niet slechts één dossier van toepassing.

### Uitgesloten paden

Voeg deze elementen nooit toe aan de inventaris of bewerk ze in deze workflow, tenzij de gebruiker deze expliciet overschrijft:

- `help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/send-to-aem.md` — parallelle voorvertoning versus productielimieten vereisen een doelbewuste redactionele beslissing buiten de automatisering.
- `help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-manage-reports.md` — rapporteert inhoudsopgave. Het enige &#39;voorvertoningssignaal&#39; is de koppeling naar het artikel met de levering van de voorvertoning van de sandbox.

## Vereiste workflow (mens in de lus)

Bewerk de repo zonder goedkeuring niet **in grote hoeveelheden.**

1. **Overzicht**\
   Maak een gesorteerde lijst met paden die voldoen aan de bovenstaande bereikregels (zoek in de repo naar de voorkeur voor `help/` bomen). **weglaat** om het even welke weg onder **`product-announcements`**, om het even welke weg onder **[Uitgesloten wegen](#excluded-paths)**, en om het even welke **TOC/index** pagina die **TOC/indexpagina&#39;s** aanpassen onder Toepassingsgebied. Als de gebruiker zegt dat een weergegeven bestand geen voorvertoningsmarkering heeft, verwijdert u het uit de uitvoering en maakt u de criteria strenger in plaats van bewerkingen te forceren.

2. **Begin**\
   Vraag of om met het **eerste** artikel in de lijst (of een weg te beginnen de gebruikersnamen).

3. **per artikel — toon eerst, geef na O.K. uit**
   - Lees het bestand.
   - Voorstel geeft duidelijk uit: **vóór/na uittreksels** of een geconcentreerde diff-stijl beschrijving van wat zal veranderen.
   - **wacht** op expliciete goedkeuring (b.v. &quot;oke,&quot;van toepassing,&quot;ja&quot;zijn alvorens het dossier te schrijven.

4. **Na elk dossier**\
   Vraag of om naar het **volgende** artikel (of eind te bewegen/overslaan).

## Inhoudsregels (GA: voorvertoningsinhoud wordt het document)

Wanneer het verwijderen van voorproef die voor **algemene beschikbaarheid** benadrukt, is het doel: **houd het gedrag dat voor Voorproef** werd gedocumenteerd, verouderd **&quot;in productie&quot;/ vertakkingen van het oud-proces**, dan **verwijdert voorproef-slechts etiketten en omslagen** zodat leest het onderwerp als huidig voor alle klanten.

### Parallelle stappen

- Als het artikel een stap (of genummerd punt) **geframed als &quot;in productie&quot;** (of gelijkwaardig: huidige productie/bestaand productiegedrag) **heeft en** a **parallel** stap geframed als **&quot;in voorproef&quot;** (of het milieu van de Voorproef):
   - **verwijder** de in-productie stap (de oude weg).
   - **houd** de **stof van de voorproefstap**, maar **verwoord** zodat is het **niet** Voorproef-specifiek (verwijder &quot;in voorproef,&quot;het milieu van de Voorproef,&quot;enz.). De nummering aanpassen zodat de lijst consistent blijft.

Als de structuur dubbelzinnig (geen duidelijke parallel) is, **einde** en toon beide kandidaten; vraag de gebruiker die om blokkeert te houden.

### Parallelle secties

- Als a **sectie** (rubriek + lichaam) **over &quot;in het productiemilieu&quot;** is en er is a **parallelle sectie** **over &quot;in het voorproefmilieu&quot;**:
   - **verwijder** de productie-milieu sectie (de vervangen inhoud).
   - **vervangt** met de inhoud van de voorproefsectie, dan **verwijdert** voorproef-milieu formulering en om het even welke **`class="preview"`** omslagen zodat is de sectie neutraal (GA-klaar).

### Fragmenten en kennisgevingen aan het begin van artikelen

- Verwijder **voorproef-slechts bouwsteen** blokken (overspannen/div of paragrafen die slechts verklaren dat de benadrukte inhoud slechts Voorproef-slechts, snelle versie, zandbak, enz. is) zodra de eigenschap GA is.
- Verwijder verbindingen of zinnen het waarvan **slechts** doel voorproefbeschikbaarheid is, tenzij de gebruiker zegt om een verschillende bericht te houden.

### HTML `class="preview"`

- Verwijder **het openen en het sluiten markeringen** voor elementen die **`class="preview"`** gebruiken, **het houden van binneninhoud** (prijsdown/HTML binnen de markering).
- Verwerk zowel **`<span class="preview">`** als **`<div class="preview">`**, en het zelfde patroon op andere markeringen (b.v. **`<p class="preview">`**, **`<li class="preview">`**) wanneer zij in **zichtbare** (niet-gecommenteerde) lichaamsinhoud verschijnen.
- Lijst-/tabelstructuur behouden; verbroken lijsten of spaties verwijderen na loskoppelen.

### Secties met opmerkingen (HTML-opmerkingen)

- **** schrapt, unwrap niet, of anders **wijzigt** om het even welke inhoud binnen **`<!-- … -->`** HTML commentaren **tenzij de gebruiker uitdrukkelijk zegt** wat te doen (b.v. schrapt de volledige commentaar, de klassen van de prijsvoorproef binnen de commentaar slechts, uncomment voor GA).
- Als voorproef-verwante inhoud of **`class="preview"`** **slechts** binnen commentaren verschijnt, **vraag die uit** wanneer het herzien van het artikel: zeg wat in de commentaar is en **vraag** wat te doen. **Gebrek: laat gecommenteerde secties ongewijzigd.**

### Wat moet u doen?

- Voer deze workflow niet uit op paden onder **`product-announcements`** (opmerkingen bij de release en verwante); de voorraad moet deze uitsluiten.
- Maak geen inventaris of geef wegen uit die onder **[Uitgesloten wegen](#excluded-paths)** worden vermeld tenzij de gebruiker uitdrukkelijk vraagt om te omvatten.
- **verwijdert of uitgeeft** niet **(**) blokken automatisch `<!-- … -->` {uit; volg **Commented-out secties** hierboven.
- Verwijder &quot;Voorproef&quot;niet wanneer het **niet** over dit eigenschap-beschikbaarheidspatroon (b.v. [ het milieu van Sandbox van de Voorproef ](·) als a **productnaam** in Verwante context)-gebruiksoordeel is en vraagt als onzeker.
- Wijzig `author:` of de niet-verwante voorgrond alleen als de gebruiker hierom vraagt.
- Ga niet **over tonen → keur** stap goed.

## Kwaliteitscontroles voordat bewerkingen worden gepresenteerd

- Geen resterende **`class="preview"`** over het overeengekomen wijzigingsbereik.
- Geen zwevende dubbele koppen of nummers van gebroken stappen.
- De inleiding leest correct **zonder** tegenstrijdig GA (niet &quot;slechts in Voorproef&quot;voor verscheepte eigenschappen).

## Verwijzingen

- Pas **[de documentatiestijl van Workfront ](https://experienceleague.adobe.com/)** en repo overeenkomsten (begaat/PR regels als de gebruiker begaat) aan.
