---
title: Filters toepassen in uitgebreide analyse
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Met de filters in het gedeelte Enhanced analytics van Adobe Workfront kunt u zich richten op specifieke projecten of specifieke typen gegevens.
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: 59e021aa3ae66e4fc8d9ce9eb57616f948e6cd90
workflow-type: tm+mt
source-wordcount: '1528'
ht-degree: 0%

---

# Filters toepassen in uitgebreide analyse

>[!IMPORTANT]
>
>Enhanced Analytics wordt de week van 26 mei uit Workfront verwijderd. Workfront Data Connect is een nieuwe, alternatieve oplossing die kan worden gebruikt om alle Enhanced Analytics-visualisaties die u momenteel gebruikt, te repliceren. <br> zie de [ Verbeterde 2&rbrace; gids van de Afleiding van Analytics &lbrace;voor meer informatie.](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)


<!-- Audited: 12/2023 -->

Met de filters in het gedeelte Enhanced analytics van Adobe Workfront kunt u zich richten op specifieke projecten of specifieke typen gegevens. De typen filters die u gebruikt, kunnen u inzicht geven in:

* Projecten die u bezit
* Specifieke portfolio- of programmaweergaven
* Belangrijkste prestatie - indicatoren voor een specifiek tijdsbestek (week, kwartaal, boekjaar)

Desgewenst kunt u filters toevoegen en verwijderen en behoudt Workfront de filters die u toepast, ook als u zich afmeldt.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>
      <p>Nieuw: alle</p>
      <p>of</p>
      <p>Huidig: Zakelijk of hoger</p></td> 
  </tr>
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
      <p>Nieuw: Licht of hoger</p>
      <p>of</p>
      <p>Huidig: Controleren of hoger</p>
   </td> 
  </tr>
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten weergeven</p> <p>U moet ook toegang tot taken, portfolio's en gebruikers weergeven om specifieke filteropties voor projectvelden te kunnen zien.</p> <p>Nota: Als de beperkingen in de <strong> Vastgestelde extra beperkingen </strong> sectie van de Edit dialoog van het Niveau van de Toegang worden geselecteerd, kunt u niet alle informatie in de filters of op de Verbeterde analytische pagina zien nadat de filter wordt toegepast.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objectmachtigingen </p> </td> 
   <td> <p>Weergave</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Voor eerste vereisten aan het gebruiken van Verbeterde Analytics, zie [&#128279;](../enhanced-analytics/enhanced-analytics-overview.md#prerequisites) Vereisten  in [ Verbeterd analyseoverzicht ](../enhanced-analytics/enhanced-analytics-overview.md).

## Het filter voor het datumbereik wijzigen {#change-the-date-range-filter}

Standaard worden in de visualisaties in het gedeelte Enhanced Analytics gegevens weergegeven voor de laatste 60 dagen en de volgende 15 dagen. U kunt een nieuw datumbereik selecteren en dit toepassen op alle visualisaties in het gedeelte Uitgebreide analyse. Als u bij de pagina vandaan navigeert, wordt het standaarddatumbereik toegepast de volgende keer dat u terugnavigeert.

>[!TIP]
>
>U kunt ook met de toetsen op het toetsenbord naar een datumbereik in de kalenderwidget navigeren, deze openen en selecteren.\
>Voor meer informatie, zie de [ kortere weg van het Toetsenbord ](../enhanced-analytics/enhanced-analytics-overview.md#keyboard-shortcuts) sectie in het artikel [ Verbeterde analyseoverzicht ](../enhanced-analytics/enhanced-analytics-overview.md).

Een nieuw datumbereik selecteren:

{{step1-to-analytics}}

1. Klik in de rechterbovenhoek op het datumbereikveld om de kalenderweergave te openen.
1. Gebruik de pijlen boven de kalender om van de maand van uw begindatum de plaats te bepalen, dan selecteer de begindatum.

   ![ Uitgezochte datumwaaier ](assets/filters-select-date-range-350x344.png)

1. Gebruik de pijlen boven de kalender om van de maand van uw einddatum de plaats te bepalen, dan selecteer de einddatum.
1. (Optioneel) Als u wilt inzoomen op een kleiner datumbereik, sleept u de muis van een bepaalde datum naar een andere datum op een van de visualisaties.

   Alle visualisaties op het scherm worden bijgewerkt zodat deze overeenkomen met het geselecteerde tijdframe en er wordt een tijdframfilter weergegeven naast bestaande filters. Dit filter blijft niet behouden als u zich afmeldt of wegnavigeert van het gebied Uitgebreide analyse.

   ![ filter Tijdframe ](assets/timeframe-filter-350x220.png)

## Een filter toevoegen

U kunt filters toevoegen op basis van standaardprojectvelden, aangepaste formuliervelden en thuisteams die zijn toegewezen aan projecten.

>[!TIP]
>
>U kunt ook de toetsen op het toetsenbord gebruiken om naar een nieuw filter te navigeren en dit filter toe te voegen.\
>Voor meer informatie, zie de [ kortere weg van het Toetsenbord ](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) sectie in het artikel [ Verbeterde analyseoverzicht ](../enhanced-analytics/enhanced-analytics-overview.md).

* [ voeg een filter van het projectgebied ](#add-a-project-field-filter) toe
* [ voeg een filter van de projectdouanevorm toe ](#add-a-project-custom-form-filter)
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
| **Eigenaar van het Project** | De gegevens van vertoningen slechts voor projecten met de geselecteerde projecteigenaar(s) |

Aangepaste formulierfilters werken anders. Voor meer informatie, zie [ een de vormfilter van de projectdouane ](#add-a-project-custom-form-filter) toevoegen.

Een projectveldfilter toevoegen:

{{step1-to-analytics}}

1. Op de bovenkant links, klik **filter** toevoegen, dan selecteren het gewenste filtertype.

   >[!NOTE]
   >
   >Verschillende filtertypen geven verschillende gegevens weer. U kunt slechts één filtertype in een filter gebruiken. Nadat u het selecteert, is een filtertype niet beschikbaar om in een ander filter van het projectgebied te gebruiken.

1. Bepaal de plaats van de waarden u gegevens voor wilt zien door minstens drie karakters van tekst op het **1&rbrace; gebied van het Onderzoek in te gaan &lbrace;, dan elke waarde te selecteren u in de filter wilt omvatten.**

   Om alle huidige waarden te selecteren, klik **Uitgezocht allen**.

   ![ Uitgezochte filterwaarde ](assets/select-filter-value-350x251.png)

1. Nadat u alle gewenste waarden selecteert, klik **filter** toepassen.

   Het project telt op de hoogste juiste updates om op uw toegepaste filters te wijzen.

1. Herhaal deze stappen voor elk filter dat u wilt toevoegen.

   Terwijl u filters toevoegt, worden gegevens in de onderstaande visualisaties weergegeven voor maximaal 50 projecten.

   >[!TIP]
   >
   >Om gegevens voor meer dan 50 projecten te zien die door gebrek tonen, kunt u:
   >
   >   * Gebruik de pijlen op de bodem verlaten om de volgende 50 projecten in die visualisatie te tonen.\
   >     ![ de pijl van de Paginering ](assets/pagination-350x118.png)
   >   
   >   * Gebruik de **Soort door** drop-down menu op een visualisatie om de projecten in een verschillende orde te bekijken.\
   >     ![ Soort door menu ](assets/sort-by-menu-350x247.png)

   Om de datumwaaier aan te passen, zie [ de filter van de datumwaaier veranderen ](#change-the-date-range-filter).

### Een projectaangepast formulierfilter toevoegen

Met het filtertype van het aangepaste formulier kunt u gegevens filteren voor projecten en taken op basis van de waarden die u hebt ingevoerd in aangepaste formuliervelden voor projecten. In tegenstelling tot andere filtertypen voor uitgebreide analyse kunt u meer dan één aangepast formulierfilter toevoegen. Elk aangepast formulierfilter bevat waarden die alleen worden ingevoerd in het geselecteerde veld op een specifiek aangepast formulier.

Een aangepast formulierfilter toevoegen:

{{step1-to-analytics}}

1. In de upper-left hoek van het scherm, klik **toevoegen Filter**, dan selecteren **de vorm van de Douane**.

   ![ Uitgezochte de filter van de douanevorm ](assets/select-custom-form-filter-350x271.png)

1. Bepaal de plaats van de douanevorm u door minstens drie karakters van tekst op het **gebied van het Onderzoek** in te gaan wilt, dan de douanevorm selecteren.
1. Selecteer het gewenste veld en voer een van de volgende handelingen uit op basis van het type veld dat u aan het filter toevoegt:

   >[!NOTE]
   >
   >Niet alle aangepaste typen krommveld kunnen aan een filter worden toegevoegd. Uitgebreide analyses ondersteunen momenteel alleen de onderstaande veldtypen.

   * **doos van de Controle**, **drop-down**, of **radioknoop**: Selecteer elke waarde op het gebied dat u in uw filter wilt omvatten, of klik **Uitgezocht Al** controledoos.\
     ![ de dooswaarden van de Controle ](assets/custom-form-filter-checkbox-350x255.png)

   * **Datum**: Gebruik de pijlen om aan een specifieke maand te navigeren, dan selecteer de datum op het gebied dat u in uw filter wilt omvatten.\
     ![ waarde van de Datum ](assets/custom-form-filter-date-350x348.png)

   * **Tekst**: Ga de tekst binnen het gebied in dat u in uw filter wilt omvatten.\
     ![ waarde van de Tekst ](assets/custom-form-filter-text-350x90.png)

   * **Aantal**: Ga het aantal binnen het gebied in dat u in uw filter wilt omvatten.\
     ![ waarde van het Aantal ](assets/custom-form-filter-number-350x93.png)

1. Nadat u ingaat of de waarden selecteert u wilt filtreren voor, **toepassen Filter**.

   Het project telt op de hoogste juiste updates om op uw toegepaste filters te wijzen.

1. Herhaal deze stappen voor elk filter dat u wilt toevoegen.

   Terwijl u filters toevoegt, worden gegevens in de onderstaande visualisaties weergegeven voor maximaal 50 projecten.

   >[!TIP]
   >
   >Om gegevens voor meer dan 50 projecten te zien die door gebrek tonen, kunt u:
   >  
   >   * Gebruik de pijlen op de bodem verlaten om de volgende 50 projecten in die visualisatie te tonen.\
   >     ![ de pijlen van de Paginering ](assets/pagination-350x118.png)
   >   
   >   * Gebruik de **Soort door** drop-down menu op een visualisatie om de projecten in een verschillende orde te bekijken.\
   >     ![ Soort door menu ](assets/sort-by-menu-350x247.png)

   Om de datumwaaier aan te passen, zie [ de filter van de datumwaaier veranderen ](#change-the-date-range-filter).

### Een teamfilter toevoegen {#add-a-team-filter}

{{step1-to-analytics}}

1. In het linkerpaneel, klik **Mensen**.

   ![ Uitgezochte Mensen ](assets/people-area-cropped-qs-350x276.png)

1. Op de bovenkant verlaten van het scherm, klik **filter** toevoegen, dan selecteren de **3&rbrace; filter van het Team &lbrace;.**
1. Bepaal de plaats van de teams u gegevens voor wilt zien door minstens drie karakters van tekst in het **gebied van het Onderzoek** in te gaan, dan elk team selecteren u in de filter wilt omvatten. Om alle teams te selecteren, klik **Uitgezocht allen**.

   ![ Uitgezochte teams ](assets/select-team-value-350x253.png)

   >[!NOTE]
   >
   >Alle teams zijn inbegrepen als filteropties, ongeacht uw toegangsniveau.

1. Nadat u alle gewenste teams selecteert, klik **filter** toepassen.

   Terwijl u filters toevoegt, worden de gegevens weergegeven in de onderstaande visualisaties.

   Om de datumwaaier aan te passen, zie [ de filter van de datumwaaier veranderen ](#change-the-date-range-filter).

## Een filter verwijderen

U kunt op elk gewenst moment een filter verwijderen. Als u een filter verwijdert, wordt het de volgende keer dat u het uitgebreide analysegebied bezoekt, niet weergegeven.

>[!TIP]
>
>U kunt ook toetsen op het toetsenbord gebruiken om naar een bestaand filter te navigeren en dit te verwijderen.\
>Voor meer informatie, zie de [ kortere weg van het Toetsenbord ](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) sectie in het artikel [ Verbeterde analyseoverzicht ](../enhanced-analytics/enhanced-analytics-overview.md).

Een filter verwijderen:

{{step1-to-analytics}}

1. Als u een projectgebied of een filter van de douanevorm wilt verwijderen, op het **1&rbrace; gebied van het Werk &lbrace;blijven.**

   of

   Als u een filter van het Team wilt verwijderen, uitgezochte **Mensen** in het linkerpaneel.

1. Bepaal de plaats van de gewenste filter en klik **X** om het te verwijderen.

   ![ verwijder ](assets/remove-filter-350x213.png)

   Het filter is niet meer actief en wordt alleen weergegeven als u het opnieuw toevoegt.
