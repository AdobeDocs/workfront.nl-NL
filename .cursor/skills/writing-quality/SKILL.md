---
name: writing-quality
description: De kwaliteit van technisch schrijven voor Workfront-artikelen en algemene documentatie beoordelen en verbeteren. Hiermee past u de Workfront Documentation Style Guide en de beginselen van de Developing Quality Technical Information toe. Gebruiken bij het bewerken, reviseren of schrijven van artikelen, overzichtsartikelen, verwijzingsartikelen of algemene documentatie. Niet gebruiken voor releaseopmerkingen — gebruik in plaats daarvan de release-notes-formatter-vaardigheden.
source-git-commit: ec081e557ec48adcfcb3833bf11dcee91312ef4e
workflow-type: tm+mt
source-wordcount: '1120'
ht-degree: 0%

---


# Schrijfkwaliteit

Revisies en verbetert Workfront-documentatie met behulp van de Workfront Documentation Style Guide en DQTI-principes.

## Workflow

Bij het reviseren of bewerken van inhoud:

1. Het doelbestand lezen
2. Pas de onderstaande regels toe — los problemen rechtstreeks op of markeer ze
3. De intentie en technische nauwkeurigheid van de auteur behouden
4. Voor gedetailleerde terminologie, leestekens, en procedureregels, zie [&#x200B; reference.md &#x200B;](reference.md)

## Stem en standpunt

- Het gebruik **tweede persoon** (&quot;u kan...&quot;) wanneer het richten van de lezer
- Gebruik contracties voor een conversatie-toon (niet, dat kan niet, dat is het, dat zijn ze)
- Gebruik &quot;We adviseren&quot; voor beste praktijken — niet &quot;Dit wordt aanbevolen&quot; of &quot;U moet het doen&quot;
- Wanneer het schrijven voor één gebruikersgroep, verwijzing andere rollen in derde persoon (&quot;u kunt bekijken... De Workfront-beheerder kan echter beperkingen instellen...&quot;)
- Gebruik nooit gendered pronounings — herstructureer de zin of gebruik &quot;zij&quot;
- Geen schuine streep voor keuzes — gebruik &quot;of&quot; (&quot;hij of zij&quot; niet &quot;hij/zij&quot;)

## Helderheid (DQTI)

- Eén idee per zin
- Zin onder ~25 woorden houden waar mogelijk
- Lood met de actie of het resultaat, niet achtergrondcontext
- Gebruik het eenvoudigste woord dat de betekenis overbrengt (&quot;use&quot; niet &quot;use&quot;, &quot;start&quot; niet &quot;initiëren&quot;, &quot;about&quot; niet &quot;regarding&quot;)
- Voorkom nominalisaties (&quot;creeer&quot; niet &quot;de verwezenlijking van&quot;, &quot;vorm&quot;niet &quot;de configuratie van&quot;)
- Gebruik specifieke, betonnen taal — vermijd vage termen (&quot;verscheidene&quot;, &quot;diverse&quot;, &quot;sommige&quot;)
- Vermijd dubbele negatieven
- Gebruik optionele uitspraak (&quot;wie&quot;, &quot;wie&quot;) om de structuur van de zin helderder te maken

## Betaaldheid (DQTI)

- Gebruik specifieke voorbeelden in plaats van abstracte beschrijvingen
- realistische waarden opnemen in voorbeelden
- Geef de exacte UI-elementen, -velden en -gebieden een naam.

## Taakoriëntatie (DQTI)

- Focus op wat de gebruiker ** kan doen, niet wat het systeem *is*
- De procedures van het leiden met dwingende werkwoorden (&quot;creeer een taak&quot;, &quot;vorm berichten&quot;)
- Zorg ervoor dat de gebruiker voldoende context heeft om te handelen, maar niet meer
- Omvat een verbinding aan gedetailleerde hulp (&quot;voor meer informatie, zie [ artikel ].&quot;)

## Kapitalisatie

- **Koppen**: Het geval van de zin altijd (&quot;creeer een taak&quot;niet &quot;creeer een Taak&quot;)
- **de termijnen van Workfront**: Capitalize slechts wanneer het van verwijzingen voorzien van een element UI direct
   - Rechtstreekse verwijzing: &quot;Vul het veld Geplande aanmaakdatum in.&quot;
   - Indirecte verwijzing: &quot;Elke taak moet een geplande einddatum hebben.&quot;
   - Tip: als u &quot;de&quot; of &quot;a&quot; vóór de term kunt plaatsen, moet deze meestal in kleine letters worden weergegeven
- **Knopen**: Volg het hoofdlettergebruik van de gebruikersinterface, behalve knoppen met hoofdletters → hoofdlettergebruik
- **Rollen**: &quot;Systeembeheerder&quot; voor de rol in de gebruikersinterface; &quot;Workfront-beheerder&quot; voor de persoon

## Koppen

- Gebruik dwingende opdracht in het geval van een zin (&quot;Maak een taak&quot;, &quot;vorm toegangsniveaus&quot;)
- De rubrieken zouden op taak-gebaseerd moeten zijn — beschrijf wat de gebruiker zal verwezenlijken
- Overzicht van artikelen eindigt met &quot;overzicht&quot; (&quot;Overzicht van projecten&quot;)
- Lange secties opsplitsen in meerdere koppen met duidelijke subdoelen

## Kruisverwijzingen en koppelingen

Gebruik deze exacte patronen:

| Situatie | Indeling |
|-----------|--------|
| Koppeling na het geven van informatie | &quot;Voor meer informatie, zie [ de naam van het Artikel ].&quot; |
| Koppeling zonder voorafgaande informatie | &quot;Voor informatie, zie [ de naam van het Artikel ].&quot; |
| Koppeling maken naar een sectie in een ander artikel | &quot;Voor meer informatie, zie &rbrack; de naam van de Sectie 0&rbrace; &lbrace;in [ naam van het Artikel ].&quot;&lbrack; |
| Koppeling maken naar een sectie in hetzelfde artikel | &quot;Voor meer informatie, zie {de naam van de Sectie 0} &rbrack; in dit artikel.&quot;&lbrack; |

- In een alinea: inline met de tekst
- In een procedurestap: op een nieuwe regel na de stap
- Meerdere koppelingen: een lijst met opsommingstekens gebruiken
- Gebruik &quot;rechterbovenhoek&quot; / &quot;linkerbovenhoek&quot; voor schermposities

## Vet en cursief

- **Vette** klikbare acties en UI elementen binnen slechts procedurestappen
- Niet vette UI-elementen buiten procedurestappen
- Namen van dialoogvensters, paginanamen, pictogramnamen of menunamen buiten stappen niet vet maken
- Het gebruik *cursief* voor tekst de gebruiker zou moeten typen (&quot;Type *my.workfront.com* in het vakje URL&quot;)
- Nooit cursief maken voor accenten — de zin herstructureren

## Notities, Tips en Waarschuwingen

Maak spaarzaam gebruik — overmatig gebruik maakt ze onzichtbaar voor lezers.

- Maximaal één opmerking/tip/waarschuwing per sectie
- Meerdere notities nooit stapelen
- Verwante notities combineren tot één notitie met een lijst met opsommingstekens
- Gebruik geen notities om nieuwe functionaliteit aan te kondigen — wijzig in plaats daarvan de artikeltekst

| Type | Doel |
|------|---------|
| `>[!NOTE]` | Info die niet in de alinea past; frustratie vermijden; versioning/compatibiliteit |
| `>[!TIP]` | Aangenaam om suggesties te hebben die het leven van de gebruiker gemakkelijker maken |
| `>[!IMPORTANT]` | Belangrijke informatie over de stap of procedure |
| `>[!WARNING]` | De gebruiker informeren over mogelijk gegevensverlies |

## Procedures

- Gebruik dwingende opdrachtkoppen (&quot;Een taak maken&quot;)
- Inleiding alleen indien nodig — de titel dient te volstaan
- Voorkeursindeling voor intro: oneindige zin + dubbele punt (&quot;Een tijdelijk wachtwoord maken:&quot;)
- Procedures die uit één stap bestaan, gebruiken nog steeds een genummerde lijst
- Gebruik &quot;type&quot; of &quot;select&quot; — vermijd vage woorden zoals &quot;set&quot; of &quot;specify&quot;
- Voorwaardelijke stappen: &quot;(Voorwaardelijk) Als u lid bent van meerdere teams, selecteert u...&quot;
- Optionele stappen: &quot;(Optioneel) Als u een emoji wilt toevoegen, klikt u..&quot;
- Beschrijf de systeemreactie voordat deze plaatsvindt of onmiddellijk daarna
- Meerdere methoden: document eerst de meest eenvoudige manier, en gebruik vervolgens &quot;Of&quot;

### Rechterhoeksegmenten in procedures

- Gebruik `>` om menu-/tabnavigatie weer te geven: &quot;Klik **E-mail** > **Meldingen**&quot;
- Vet de knopnamen, niet de haakjes
- Spaties rond haakjes opnemen
- Gebruik geen haakjes voor navigatie in het hoofdmenu — gebruik het fragment in het hoofdmenu

## Referentie leestekens

| Regel | Voorbeeld |
|------|---------|
| Oxford comma altijd | &quot;Motief, middel en kans&quot; |
| Komma vóór &quot;dan&quot; in procedures | &quot;Klik Opstelling, dan klik Interface.&quot; |
| Komma na jaar op datum midden | &quot;2 januari 2016, uitgave van...&quot; |
| Geen komma met alleen maand en jaar | &quot;Januari 2016&quot; |
| Dubbele punt voor lijst, kleine letter na | &quot;Selecteer een van de volgende opties: optie A&quot; |
| Geen dubbele punt na procedurekoppen | &quot;Een taak maken&quot; (niet &quot;Een taak maken:&quot;) |
| Em-streepjes met mate | De zin indien mogelijk herstructureren |
| Perioden in bestandsextensies | &quot;Een PDF-bestand uploaden&quot; |

Voor volledige leestekens en terminologieregels, zie [&#x200B; reference.md &#x200B;](reference.md).

## Volledigheid (DQTI)

- Alle informatie opnemen die de gebruiker moet begrijpen en gebruiken
- Geen informatie opnemen die de gebruiker niet nodig heeft
- Altijd een koppeling naar gedetailleerde documentatie met de tekst &quot;Voor meer informatie&quot; opgeven
- Standaardwaarden documentsysteem: &quot;(Standaard)&quot; in lijsten of beschrijf in de zin

## Organisatie (DQTI)

- Logische structuur met progressieve openbaarmaking (overzicht → details → referentie)
- Nieuwste inhoud eerst voor pagina&#39;s met tijdvolgorde (bijv. releaseopmerkingen)
- Eén onderwerp per sectie
- Lijsten gebruiken voor 3+ parallelle items
- Tabellen gebruiken voor gestructureerde vergelijkingen of veldbeschrijvingen
- Vermijd wand-van-tekstparagrafen — onderbreking in verteerbare brokken

## Artikeltypen

| Type | Doel | Titel Conventie |
|------|---------|-----------------|
| Overzicht | Context, diagrammen, hoe dingen werken — geen procedures | Eindigt met &quot;overzicht&quot; |
| Hoe kan ik | Specifieke taak met duidelijke stappen | Imperatief werkwoord |
| Aan de slag | Info + koppelingen instellen voor nieuwe gebruikers | &quot;Aan de slag met...&quot; |
| Referentie | Veldbeschrijvingen in tabellen | Beschrijvende naamwoorden |

## Controlelijst voor validatie

Controleer na het bewerken:

- [ ] Tweede persoon gedurende de gehele periode (&quot;u&quot;), gebruikte contracties
- [ ] Als in een zin op alle koppen
- [ ] Workfront-termen worden correct gekapitaliseerd (direct versus indirect referentie)
- [ ] Alleen vet maken op acties waarop kan worden geklikt in stappen van de procedure
- [ ] Kruisverwijzingen gebruiken de standaardindeling (&quot;Zie voor meer informatie...&quot;)
- [ ] Opmerkingen/tips/waarschuwingen niet gestapeld, max. één per sectie
- [ ] Oxford komma wordt consistent gebruikt
- [ ] Processtappen gebruiken specifieke werkwoorden (type, selecteer, klik — niet &quot;set&quot; of &quot;specify&quot;)
- [ ] Voorwaardelijke/optionele stappen die correct zijn gelabeld
- [ ] Geen gendered pronouns
- [ ] Zinnen zijn duidelijk, concreet en taakgericht
