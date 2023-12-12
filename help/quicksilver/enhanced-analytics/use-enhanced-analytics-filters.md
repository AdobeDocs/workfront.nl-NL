---
title: Filters toepassen in uitgebreide analyse
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Met de filters in het gedeelte Enhanced analytics van Adobe Workfront kunt u zich richten op specifieke projecten of specifieke typen gegevens.
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: 6d2494f1ccb2f9b222a953ed8bae922bd0f26389
workflow-type: tm+mt
source-wordcount: '1504'
ht-degree: 0%

---

# Filters toepassen in uitgebreide analyse

Met de filters in het gedeelte Enhanced analytics van Adobe Workfront kunt u zich richten op specifieke projecten of specifieke typen gegevens. De typen filters die u gebruikt, kunnen u inzicht geven in:

* Projecten die u bezit
* Specifieke portfolio- of programmaweergaven
* Belangrijkste prestatie - indicatoren voor een specifiek tijdsbestek (week, kwartaal, boekjaar)

Desgewenst kunt u filters toevoegen en verwijderen en behoudt Workfront de filters die u toepast, ook als u zich afmeldt.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td>
      <p>Nieuw: alle</p>
      <p>of</p>
      <p>Huidig: Zakelijk of hoger</p></td> 
  </tr>
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td>
      <p>Nieuw: Licht of hoger</p>
      <p>of</p>
      <p>Huidig: Controleren of hoger</p>
   </td> 
  </tr>
  <tr> 
   <td>Toegangsniveau* </td> 
   <td> <p>Toegang tot projecten weergeven</p> <p>U moet de toegang van de Mening tot Taken, Portfolio's, en Gebruikers ook hebben om specifieke de filteropties van het projectgebied te zien.</p> <p>Opmerking: als er beperkingen zijn geselecteerd in de sectie Aanvullende beperkingen instellen van het dialoogvenster Toegangsniveau bewerken, ziet u mogelijk niet alle informatie in de filters of op de pagina Uitgebreide analyse nadat het filter is toegepast. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objectmachtigingen </p> </td> 
   <td> <p>Weergave</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

Voor eerste vereisten voor het gebruik van Enhanced Analytics raadpleegt u [Vereisten](../enhanced-analytics/enhanced-analytics-overview.md#prerequisites) in [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

## Het filter voor het datumbereik wijzigen {#change-the-date-range-filter}

Standaard worden in de visualisaties in het gedeelte Enhanced Analytics gegevens weergegeven voor de laatste 60 dagen en de volgende 15 dagen. U kunt een nieuw datumbereik selecteren en dit toepassen op alle visualisaties in het gedeelte Uitgebreide analyse. Als u bij de pagina vandaan navigeert, wordt het standaarddatumbereik toegepast de volgende keer dat u terugnavigeert.

>[!TIP]
>
>U kunt ook met de toetsen op het toetsenbord naar een datumbereik in de kalenderwidget navigeren, deze openen en selecteren.\
>Zie de klasse [Sneltoetsen](../enhanced-analytics/enhanced-analytics-overview.md#keyboard-shortcuts) in het artikel [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

Een nieuw datumbereik selecteren:

{{step1-to-analytics}}

1. Klik in de rechterbovenhoek op het datumbereikveld om de kalenderweergave te openen.
1. Gebruik de pijlen boven de kalender om van de maand van uw begindatum de plaats te bepalen, dan selecteer de begindatum.

   ![Datumbereik selecteren](assets/filters-select-date-range-350x344.png)

1. Gebruik de pijlen boven de kalender om van de maand van uw einddatum de plaats te bepalen, dan selecteer de einddatum.
1. (Optioneel) Als u wilt inzoomen op een kleiner datumbereik, sleept u de muis van een bepaalde datum naar een andere datum op een van de visualisaties.

   Alle visualisaties op het scherm worden bijgewerkt zodat deze overeenkomen met het geselecteerde tijdframe en er wordt een tijdframfilter weergegeven naast bestaande filters. Dit filter blijft niet behouden als u zich afmeldt of wegnavigeert van het gebied Uitgebreide analyse.

   ![Tijdlijnfilter](assets/timeframe-filter-350x220.png)

## Een filter toevoegen

U kunt filters toevoegen op basis van standaardprojectvelden, aangepaste formuliervelden en thuisteams die zijn toegewezen aan projecten.

>[!TIP]
>
>U kunt ook de toetsen op het toetsenbord gebruiken om naar een nieuw filter te navigeren en dit filter toe te voegen.\
>Zie de klasse [Sneltoetsen](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) in het artikel [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

* [Een projectveldfilter toevoegen](#add-a-project-field-filter)
* [Een projectaangepast formulierfilter toevoegen](#add-a-project-custom-form-filter)
* [Een teamfilter toevoegen](#add-a-team-filter)

### Een projectveldfilter toevoegen {#add-a-project-field-filter}

Met projectveldfilters kunt u gegevens filteren voor projecten en taken op basis van de waarden die zijn ingevoerd in velden die standaard zijn opgenomen in projecten.

De volgende filtertypen voor projectvelden zijn beschikbaar:

| Veld | Gegevens weergegeven |
|---|---|
| **Project** | De gegevens van vertoningen slechts voor geselecteerde project(en) |
| **Programma** | Hiermee geeft u alleen gegevens weer voor projecten in de geselecteerde programma&#39;s |
| **Portfolio** | Gegevens worden alleen weergegeven voor projecten in de geselecteerde portfolio(s) |
| **Voorwaarde** | De gegevens van vertoningen slechts voor projecten die onlangs de geselecteerde voorwaarde(n) hadden (op doel, bij risico, of in probleem) |
| **Status** | Hiermee geeft u alleen gegevens weer voor projecten met de meest recente geselecteerde status (voltooid, huidig, in de wachtstand, geannuleerd, enzovoort) |
| **Sponsor** | Hiermee geeft u alleen gegevens weer voor projecten met de geselecteerde sponsor(en) |
| **Projecteigenaar** | De gegevens van vertoningen slechts voor projecten met de geselecteerde projecteigenaar(s) |

Aangepaste formulierfilters werken anders. Zie voor meer informatie [Een projectaangepast formulierfilter toevoegen](#add-a-project-custom-form-filter).

Een projectveldfilter toevoegen:

{{step1-to-analytics}}

1. Klik linksboven op **Filter toevoegen** Selecteer vervolgens het gewenste filtertype.

   >[!NOTE]
   >
   >Verschillende filtertypen geven verschillende gegevens weer. U kunt slechts één filtertype in een filter gebruiken. Nadat u het selecteert, is een filtertype niet beschikbaar om in een ander filter van het projectgebied te gebruiken.

1. Zoek de waarden waarvoor u gegevens wilt zien door ten minste drie tekens tekst in te voeren in het dialoogvenster **Zoeken** selecteert u vervolgens elke waarde die u in het filter wilt opnemen.

   Klik op **Alles selecteren**.

   ![Filterwaarde selecteren](assets/select-filter-value-350x251.png)

1. Klik op **Filter toepassen**.

   Het project telt op de hoogste juiste updates om op uw toegepaste filters te wijzen.

1. Herhaal deze stappen voor elk filter dat u wilt toevoegen.

   Terwijl u filters toevoegt, worden gegevens in de onderstaande visualisaties weergegeven voor maximaal 50 projecten.

   >[!TIP]
   >
   >Om gegevens voor meer dan 50 projecten te zien die door gebrek tonen, kunt u:
   >
   >   * Gebruik de pijlen op de bodem verlaten om de volgende 50 projecten in die visualisatie te tonen.\
   >     ![Pagineringspijl](assets/pagination-350x118.png)
   >   
   >   * Gebruik de **Sorteren op** vervolgkeuzelijst op een visualisatie om de projecten in een andere volgorde weer te geven.\
   >     ![Sorteren op menu](assets/sort-by-menu-350x247.png)

   Als u het datumbereik wilt aanpassen, raadpleegt u [Het filter voor het datumbereik wijzigen](#change-the-date-range-filter).

### Een projectaangepast formulierfilter toevoegen

Met het filtertype van het aangepaste formulier kunt u gegevens filteren voor projecten en taken op basis van de waarden die u hebt ingevoerd in aangepaste formuliervelden voor projecten. In tegenstelling tot andere filtertypen voor uitgebreide analyse kunt u meer dan één aangepast formulierfilter toevoegen. Elk aangepast formulierfilter bevat waarden die alleen worden ingevoerd in het geselecteerde veld op een specifiek aangepast formulier.

Een aangepast formulierfilter toevoegen:

{{step1-to-analytics}}

1. Klik in de linkerbovenhoek van het scherm op **Filter toevoegen** selecteert u vervolgens **Aangepast formulier**.

   ![Aangepast formulierfilter selecteren](assets/select-custom-form-filter-350x271.png)

1. Zoek het gewenste aangepaste formulier door ten minste drie tekens in te voeren in het tekstvak **Zoeken** en selecteert u het aangepaste formulier.
1. Selecteer het gewenste veld en voer een van de volgende handelingen uit op basis van het type veld dat u aan het filter toevoegt:

   >[!NOTE]
   >
   >Niet alle aangepaste typen krommveld kunnen aan een filter worden toegevoegd. Uitgebreide analyses ondersteunen momenteel alleen de onderstaande veldtypen.

   * **Selectievakje**, **vervolgkeuzelijst**, of **keuzerondje**: Selecteer elke waarde in het veld die u in het filter wilt opnemen of klik op de knop **Alles selecteren** selectievakje.\
     ![Waarden selectievakje](assets/custom-form-filter-checkbox-350x255.png)

   * **Datum**: Gebruik de pijlen om naar een bepaalde maand te navigeren en selecteer vervolgens de datum in het veld die u in het filter wilt opnemen.\
     ![Datumwaarde](assets/custom-form-filter-date-350x348.png)

   * **Tekst**: Voer de tekst in het veld in die u in het filter wilt opnemen.\
     ![Tekstwaarde](assets/custom-form-filter-text-350x90.png)

   * **Getal**: Voer het nummer in het veld in dat u in het filter wilt opnemen.\
     ![Nummerwaarde](assets/custom-form-filter-number-350x93.png)

1. Nadat u de waarden hebt ingevoerd of geselecteerd waarvoor u wilt filteren, klikt u op **Filter toepassen**.

   Het project telt op de hoogste juiste updates om op uw toegepaste filters te wijzen.

1. Herhaal deze stappen voor elk filter dat u wilt toevoegen.

   Terwijl u filters toevoegt, worden gegevens in de onderstaande visualisaties weergegeven voor maximaal 50 projecten.

   >[!TIP]
   >
   >Om gegevens voor meer dan 50 projecten te zien die door gebrek tonen, kunt u:
   >  
   >   * Gebruik de pijlen op de bodem verlaten om de volgende 50 projecten in die visualisatie te tonen.\
   >     ![Pagineringspijlen](assets/pagination-350x118.png)
   >   
   >   * Gebruik de **Sorteren op** vervolgkeuzelijst op een visualisatie om de projecten in een andere volgorde weer te geven.\
   >     ![Sorteren op menu](assets/sort-by-menu-350x247.png)

   Als u het datumbereik wilt aanpassen, raadpleegt u [Het filter voor het datumbereik wijzigen](#change-the-date-range-filter).

### Een teamfilter toevoegen {#add-a-team-filter}

{{step1-to-analytics}}

1. Klik in het linkerdeelvenster op **Mensen**.

   ![Personen selecteren](assets/people-area-cropped-qs-350x276.png)

1. Klik linksboven in het scherm op **Filter toevoegen** en selecteert u vervolgens de **Team** filter.
1. Zoek de teams waarvoor u gegevens wilt zien door ten minste drie tekens tekst in te voeren in het dialoogvenster **Zoeken** selecteert u vervolgens elk team dat u in het filter wilt opnemen. Om alle teams te selecteren, klik **Alles selecteren**.

   ![Teams selecteren](assets/select-team-value-350x253.png)

   >[!NOTE]
   >
   >Alle teams zijn inbegrepen als filteropties, ongeacht uw toegangsniveau.

1. Klik op **Filter toepassen**.

   Terwijl u filters toevoegt, worden de gegevens weergegeven in de onderstaande visualisaties.

   Als u het datumbereik wilt aanpassen, raadpleegt u [Het filter voor het datumbereik wijzigen](#change-the-date-range-filter).

## Een filter verwijderen

U kunt op elk gewenst moment een filter verwijderen. Als u een filter verwijdert, wordt het de volgende keer dat u het uitgebreide analysegebied bezoekt, niet weergegeven.

>[!TIP]
>
>U kunt ook toetsen op het toetsenbord gebruiken om naar een bestaand filter te navigeren en dit te verwijderen.\
>Zie de klasse [Sneltoetsen](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) in het artikel [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

Een filter verwijderen:

{{step1-to-analytics}}

1. Als u een projectveld of aangepast formulierfilter wilt verwijderen, blijft u in het dialoogvenster **Werk** gebied.

   of

   Als u een filter van het Team wilt verwijderen, selecteer **Mensen** in het linkerdeelvenster.

1. Zoek het gewenste filter en klik op de knop **X** om het te verwijderen.

   ![Verwijderen](assets/remove-filter-350x213.png)

   Het filter is niet meer actief en wordt alleen weergegeven als u het opnieuw toevoegt.
