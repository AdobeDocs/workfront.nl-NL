---
title: Verbeteringen voor aangepaste formulieren
description: De volgende belangrijke verbeteringen zijn aangebracht voor het beheer van aangepaste formulieren in de release 22.2.
author: Luke
exl-id: 81568eab-8a65-4767-b8ab-fb9353a90bb6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# Verbeteringen voor aangepaste formulieren

De volgende belangrijke verbeteringen zijn aangebracht voor het beheer van aangepaste formulieren in de release 22.2.

## Elementwidgets toevoegen

U kunt afbeelding insluiten in uw aangepaste formulieren. Op deze manier kunt u interactiever en visueel communiceren met aangepaste formuliergebruikers. Binnenkort zijn er nog meer widgettypen beschikbaar.

![](assets/image-in-custom-form.png)

Wanneer een aangepast formulier met een widget aan een object is gekoppeld, kunnen gebruikers die met het object werken dit in de volgende gebieden zien:

* Het gebied van Details van het voorwerp (bijvoorbeeld voor een project, het gebied van Details van het Project) &#x200B;

   ![](assets/see-image-details-page.png)

* Het vak Bewerken voor het object als dit de nieuwe Adobe Workfront-ervaring bevat (bijvoorbeeld de vakken Project bewerken en Taak bewerken) &#x200B;

   ![](assets/image-see-in-edit.png)

Gebruikers kunnen de widget momenteel niet zien in de volgende gebieden: &#x200B;

* Lijsten en rapporten
* Home en overzicht
* Het vak Bewerken voor het object, als dit object er anders uitziet dan de nieuwe Adobe Workfront-ervaring (bijvoorbeeld het vak Kosten bewerken)
* De Workfront Mobile-app &#x200B;

Zie voor meer informatie over het toevoegen van widgets aan aangepaste formulieren [Een afbeelding of andere middelenwidget toevoegen of bewerken in een aangepast formulier](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Een aangepast formulier koppelen aan meerdere objecttypen

U kunt meerdere objecttypen koppelen aan elk nieuw aangepast formulier:

![](assets/new-custom-form-object-types.png)

Of een bestaand aangepast formulier:

![](assets/add-object-type-existing-form.png)

Op deze manier kunt u één aangepast formulier maken dat u kunt gebruiken voor projecten, taken, uitgaven en andere typen objecten die worden ondersteund voor aangepaste formulieren.

Dit is vooral handig wanneer u een uitgave of taak converteert, omdat u een aangepast formulier en de bijbehorende gegevens kunt overdragen naar het geconverteerde object. U hoeft niet langer exacte kopieën van hetzelfde aangepaste formulier voor verschillende objecttypen te maken en te onderhouden, het aangepaste formulier handmatig aan het project toe te voegen.

>[!INFO]
>
>**Voorbeeld:**
>
>Iemand verzendt een interne IT-aanvraag (uitgave) en geeft informatie over wat nodig is in een bijgevoegd aangepast formulier.
>
>U zet de uitgave om in een project voor de gebruikers die aan het zullen werken.
>
>Omdat het aangepaste formulier met de details van de verzender is gekoppeld aan zowel het type Issue als het type Project, worden het aangepaste formulier en al deze details tijdens de conversie overgedragen naar het project.

>[!NOTE]
>
>Wanneer de conversie plaatsvindt, moet het aangepaste formulier al zijn gekoppeld aan het objecttype waarnaar u converteert.

Voor instructies over het toevoegen van een middelenwidget aan een aangepast formulier, raadpleegt u [Een afbeelding of andere middelenwidget toevoegen of bewerken in een aangepast formulier](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

Houd rekening met het volgende wanneer u een aangepast formulier met meerdere objecten maakt of bewerkt:

* [Machtigingsopties voor sectie-einden](#permission-options-for-section-breaks)
* [Compatibiliteit met aangepaste velden berekenen](#calculated-custom-field-compatibility)
* [Let op het verwijderen van een objecttype uit een aangepast formulier](#caution-about-deleting-an-object-type-from-a-custom-form)

### Machtigingsopties voor sectie-einden

De set opties voor machtigingen voor sectie-einden die beschikbaar zijn voor de typen Uitgave-, Taak-, Project- en Gebruikersobjecten heeft één andere machtigingsoptie dan de set machtigingsopties voor alle andere objecttypen: Beperkte bewerking.

![](assets/section-break-permissions-limited-edit.png)

De reeks toestemmingen van de sectieonderbreking beschikbaar voor alle andere objecten types (Portfolio, Document, Programma, Uitgaven, Bedrijf, Herhaling, het Verslag van de Facturering, en Groep) omvat geen Beperkte Edit:

![](assets/section-break-permissions-no-limited-edit.png)

In een aangepast formulier dat is gekoppeld aan objecttypen uit beide groepen, gebruikt het systeem een algemene set machtigingen voor secties-einden die werken voor alle objecttypen. Met name in plaats van de optie Beperkte bewerkingsmachtigingen te gebruiken, vervangt deze algemene set de optie Bewerken met machtiging door de optie Beperkte bewerkingsmachtigingen. De optie Bewerken is compatibel met alle objecttypen.

Wanneer u een objecttype koppelt dat andere machtigingsopties gebruikt dan de andere objecttypen die al op een aangepast formulier voorkomen, wordt een bericht weergegeven waarin u kunt overschakelen naar de algemene set machtigingsopties voor het formulier. Deze wijziging is van toepassing op alle velden, zelfs als deze niet onder een sectie-einde vallen.

Zie voor meer informatie [Een sectie-einde toevoegen aan een aangepast formulier](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).

### Compatibiliteit met aangepaste velden berekenen

Als in een aangepast formulier met meerdere objecten een berekend veld verwijst naar velden die beschikbaar zijn voor gebruik met alle gekoppelde objecttypen van het formulier (zoals {name}, {description} en {entryDate} die beschikbaar zijn voor meerdere objecttypen), worden de gegevens correct berekend, ongeacht het object waaraan u het toevoegt.

Als u bijvoorbeeld een formulier met meerdere objecten hebt voor projecten en uitgaven en u een berekend veld toevoegt dat de expressie {name} bevat, wordt in het veld de projectnaam weergegeven wanneer u het formulier aan een project toevoegt en voegt u de taaknaam het formulier aan een taak toe.

Als een berekend veld in het formulier echter verwijst naar een veld dat niet compatibel is met alle objecttypen van het formulier, wordt u in een bericht gewaarschuwd dat u wijzigingen wilt aanbrengen.

>[!INFO]
>
>**Voorbeeld:** In een aangepast formulier dat is gekoppeld aan het taakobjecttype, maakt u een berekend aangepast veld dat verwijst naar het ingebouwde veld Toegewezen aan: Naam, zodat de naam van de primaire ontvanger kan worden weergegeven wanneer het formulier aan een taak is gekoppeld:
>
>
```
>Assigned To: Name{assignedTo}.{name}
>```
>
>Later voegt u het objecttype Project toe aan het aangepaste formulier. Een waarschuwingsbericht geeft aan dat het objecttype Project niet compatibel is met het berekende aangepaste veld. Dit komt doordat het veld Toegewezen aan niet beschikbaar is voor projecten.

Wanneer dit voorkomt, kunt u één van het volgende doen:

* Verwijder een van de twee incompatibele items uit het aangepaste formulier. Dit is het objecttype of het veld waarnaar wordt verwezen.
* Beide items behouden en de filtervariabele voor jokertekens gebruiken `$$OBJCODE` als een voorwaarde in een IF-expressie om twee verschillende versies van het veld In laden te maken. Hierdoor werkt het veld goed, ongeacht het type object waaraan het formulier is gekoppeld.

   Gebruikend het bovenstaande voorbeeld, hoewel er geen ingebouwde Toegewezen aan is: Het gebied van de naam voor projecten, is er een ingebouwd gebied van de Eigenaar (dat automatisch met de naam van de persoon invult die het project creeerde, tenzij iemand manueel dit verandert). In het veld Aangepast in lading kunt u dus `$$OBJCODE` zoals hieronder getoond om het gebied van de Eigenaar van verwijzingen te voorzien wanneer het douaneformulier aan een project in bijlage is, en toegewezen aan: Veld benoemen wanneer het formulier aan een taak is gekoppeld:

   ```
   IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})
   ```

>[!NOTE]
>
>  Als u een objecttype toevoegt vóór een veldnaam, verwijst dit naar het bovenliggende object van het object, zodat u het niet kunt gebruiken `{project}.{name}` met een project, maar u kunt het met een taak gebruiken.

Zie voor instructies over het toevoegen van een berekend aangepast veld aan een aangepast formulier [Berekende gegevens toevoegen aan een aangepast formulier](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Voor meer informatie over variabelen zoals `$$OBJCODE`, zie [Variabelen van jokerfilter](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

### Let op het verwijderen van een objecttype uit een aangepast formulier

U kunt op elk gewenst moment een objecttype op een aangepast formulier verwijderen, maar dit moet met de nodige voorzichtigheid gebeuren. Als gebruikers het aangepaste formulier al hebben gekoppeld aan objecten van het type dat u wilt verwijderen, en er gegevens aan hebben toegevoegd, worden die gegevens permanent verwijderd wanneer u dat objecttype op het formulier verwijdert.

Er is ook geen meldingssysteem om mensen die het aangepaste formulier gebruiken te waarschuwen dat het is verwijderd.

Zie voor meer informatie [Een aangepast veld of aangepaste widget uit het systeem verwijderen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
