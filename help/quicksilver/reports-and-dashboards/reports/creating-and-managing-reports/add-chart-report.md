---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Een diagram toevoegen aan een rapport
description: U kunt uw rapporten verbeteren door een grafiek toe te voegen. U kunt grafieken toevoegen aan bestaande rapporten of aan rapporten die u creeert.
author: Nolan
feature: Reports and Dashboards
exl-id: 9b58d68c-4b7b-4344-bde3-7c65e2e1aac8
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '2739'
ht-degree: 0%

---

# Een diagram toevoegen aan een rapport

<!--Audited: 11/2024-->

U kunt uw rapporten verbeteren door een grafiek toe te voegen. U kunt grafieken toevoegen aan bestaande rapporten of aan rapporten die u creeert.

Alvorens u een grafiek aan een rapport toevoegt, zou u een Mening en een Groepering voor het rapport moeten tot stand brengen.

U kunt geen grafieken aan de meeste rapporten toevoegen tenzij u eerst de informatie in het rapport groepeert. Het enige diagram dat zonder groepering kan worden toegevoegd, is een diagramdiagram.

Voor informatie over meningen, zie [&#x200B; Overzicht van Meningen in Adobe Workfront &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Voor meer informatie over groeperingen, zie [&#x200B; Overzicht van Groepen in Adobe Workfront &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

Als uw rapport teveel punten toont, wordt een grafiek niet gecreeerd. In dit geval, moet u ook een Filter aan het rapport toevoegen om het aantal resultaten in uw rapport te verminderen.

Voor meer informatie over filters, zie [&#x200B; Overzicht van Filters &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
      <p>Standard</p>
      <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuratie op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een diagram toevoegen aan een rapport

1. Ga naar een bestaand rapport of maak een nieuw rapport. Voor meer informatie over het creëren van een nieuw rapport, zie [&#x200B; een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

1. (Voorwaardelijk) als u naar een bestaand rapport ging, klik {de Acties van het 0} Rapport **>** uitgeven **.**

1. Zorg ervoor dat het **lusje van Kolommen (Mening)** is bijgewerkt om de informatie te tonen u in het rapport van een grafiek wilt voorzien.

   Voor informatie over om tot de Mening voor het rapport te leiden of te wijzigen, zie [&#x200B; tot meningen in Adobe Workfront &#x200B;](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) leiden of uitgeven.

1. Klik het **lusje van Groepen** en voeg een groepering toe.

   >[!TIP]
   >
   >* U kunt een grafiek aan een rapport slechts toevoegen wanneer de rapportresultaten worden gegroepeerd.
   >* Groepen in tekstmodus worden niet ondersteund in grafieken. Voor meer informatie over tekst-wijze groeperingen, zie [&#x200B; een groepering uitgeven gebruikend tekstwijze &#x200B;](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md).
   >* Als u één groepering toevoegt die één metrisch vertegenwoordigt, tonen alle grafieken behalve een cirkeldiagram elk resultaat in de groepering als de zelfde kleur.

   Voor meer informatie over het creëren van groeperingen, zie [&#x200B; groepen in Adobe Workfront &#x200B;](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-groupings.md) creëren.

1. Selecteer de **Grafiek** tabel.

1. Klik op een diagramtype om dit te selecteren.\
   ![&#x200B; het type van Grafiek selectie &#x200B;](assets/unshimmed-report-builder-chart.png)

1. Selecteer een van de volgende typen grafieken:

   * [&#x200B; grafiek van de Kolom &#x200B;](#column-chart)
   * [&#x200B; Grafiek van de Bar &#x200B;](#bar-chart)
   * [&#x200B; Schijfgrafiek &#x200B;](#pie-chart)
   * [&#x200B; grafiek van de Lijn &#x200B;](#line-chart)
   * [&#x200B; Grafiek van de Tanden &#x200B;](#gauge-chart)
   * [Bubble-grafiek](#bubble-chart)

1. Klik **sparen + Sluiten** om de grafiek en het rapport te bewaren.

### Kolomdiagram {#column-chart}

Om a **grafiek van de Kolom** aan uw rapport toe te voegen:

1. Begin toevoegend een grafiek aan uw rapport, zoals die in [&#x200B; wordt beschreven voeg een grafiek aan een rapport &#x200B;](#add-a-chart-to-a-report) toe.

1. Op het **Linker (Y) gebied van de As**, selecteer de waarden die u op de Y as van de grafiek wilt omvatten, dan selecteren hoe u de informatie wilt worden samengevat in **die door** gebied wordt samengevat.

1. (Facultatief) klik **de Kleuren van de Douane** om aangewezen kleuren aan elk van de kolommen toe te wijzen.\
   Voor meer informatie over het aanpassen van grafiekkleuren, zie [&#x200B; kaartkleuren &#x200B;](#customize-chart-colors) aanpassen.

1. Op het **Onderste (X) gebied van de As**, selecteer de Groepering die u in de grafiek wilt omvatten.

1. (Facultatief) klik **Tonen in 3D** om de grafiek in een driedimensionale mening te tonen.

1. (Facultatief) **Kolommen van de Groep**: Selecteer deze optie om te bepalen hoe u de kolommen wilt worden gegroepeerd.\
   Selecteer een van de volgende opties:

   * Klik op een van de volgende opties om te selecteren hoe de gegroepeerde kolommen worden weergegeven:

      * **zij aan zij**
      * **Gestapeld**
      * **Gestapeld aan 100%**

   * Selecteer de Groepering die u in de grafiek van de **Gegevens van de Groep door** drop-down menu wilt omvatten.
   * (Facultatief) klik **de Kleuren van de Douane** om de kleuren van de kolommen aan te passen.\
     Voor meer informatie over het aanpassen van grafiekkleuren, zie [&#x200B; kaartkleuren &#x200B;](#customize-chart-colors) aanpassen.

1. (Facultatief) klik **Grafiek van de Combinatie** om een extra waarde in de grafiek te omvatten, evenals hoe u de informatie wilt worden samengevat.\
   Overweeg de volgende opties:

   * **Plot op Secundaire As**: Selecteer deze optie om de gegevens op de rechterkant van de grafiek te plotten.
   * **Type van Grafiek**: Selecteer of u deze extra waarde als lijn of derde kolom wilt worden getoond.

1. Klik **sparen + Sluiten** om de grafiek en het rapport te bewaren.

### Staafdiagram {#bar-chart}

Om a **grafiek van de Bar** aan uw rapport toe te voegen:

1. Begin toevoegend een grafiek aan uw rapport, zoals die in [&#x200B; wordt beschreven voeg een grafiek aan een rapport &#x200B;](#add-a-chart-to-a-report) toe.

1. Op het **gebied van de As van 0&rbrace; Onder (X), selecteer de waarden die u op de X as van de grafiek wilt omvatten, dan selecteren hoe u de informatie wilt worden samengevat in** die door **gebied wordt samengevat.**

1. (Facultatief) klik **de Kleuren van de Douane** om de kleuren van de bars aan te passen.\
   Voor meer informatie over het aanpassen van grafiekkleuren, zie [&#x200B; kaartkleuren &#x200B;](#customize-chart-colors) aanpassen.

1. In het **Linkergebied (Y) van de As**, selecteer de Groepering die u in de grafiek wilt omvatten.

1. (Facultatief) klik **Tonen in 3D** om de grafiek in een driedimensionale mening te tonen.

1. (Facultatief) klik **Bars van de Groep** om te bepalen hoe u de bars wilt worden gegroepeerd.\
   Selecteer een van de volgende opties:

   * Klik op een van de volgende opties om te selecteren hoe de gegroepeerde balken worden weergegeven:

      * **zij aan zij**
      * **Gestapeld**
      * **Gestapeld aan 100%**

   * Selecteer hoe u de informatie in de grafiek van de **Gegevens van de Groep door** drop-down menu wilt groeperen.
   * (Facultatief) klik **de Kleuren van de Douane** om de kleuren van uw kolommen aan te passen.\
     Voor meer informatie over het aanpassen van grafiekkleuren, zie [&#x200B; kaartkleuren &#x200B;](#customize-chart-colors) aanpassen.

1. (Facultatief) klik **Grafiek van de Combinatie** om een extra waarde in de grafiek te omvatten, evenals hoe u de informatie wilt worden samengevat.

1. Klik **sparen + Sluiten** om de grafiek en het rapport te bewaren.

>[!IMPORTANT]
>
>Met staafdiagrammen beperken tot 23 of minder balken, omdat staafdiagrammen met meer dan 23 balken niet alle staaflabels correct weergeven.

### Cirkeldiagram {#pie-chart}

Om a **Schijf** grafiek aan uw rapport toe te voegen:

1. Begin toevoegend een grafiek aan uw rapport, zoals die in [&#x200B; wordt beschreven voeg een grafiek aan een rapport &#x200B;](#add-a-chart-to-a-report) toe.

1. Op het **gebied van Waarden**, selecteer de waarden die u op het rapport wilt worden getoond, dan selecteren hoe u de informatie wilt worden samengevat in **samengevat door** gebied.\
   Op het **gebied van Bruiloeken**, selecteer de Groepering die u in de grafiek wilt omvatten. De Groepering wordt vertegenwoordigd door de segmenten van de grafiek.

1. (Facultatief) klik **de Kleuren van de Douane** om de kleuren van de wiggen op de grafiek aan te passen.\
   Voor meer informatie over het aanpassen van grafiekkleuren, zie [&#x200B; kaartkleuren &#x200B;](#customize-chart-colors) aanpassen.

1. (Facultatief) klik **Tonen in 3D** om de grafiek in een driedimensionale mening te tonen.

1. Op **toon Resultaten als** gebied, selecteer hoe u de resultaten in de grafiek wilt tonen. Overweeg de volgende opties:

   * **Percentage**: De grafiekresultaten tonen als percentage.
   * **Aantallen**: De grafiekresultaten tonen als aantal.

1. Klik **sparen + Sluiten** om de grafiek en het rapport te bewaren.

### Lijndiagram {#line-chart}

Om a **grafiek van de Lijn** aan uw rapport toe te voegen:

1. Begin toevoegend een grafiek aan uw rapport, zoals die in [&#x200B; wordt beschreven voeg een grafiek aan een rapport &#x200B;](#add-a-chart-to-a-report) toe.

1. Op het **Linker (Y) gebied van de As**, selecteer de waarden die u op de Y as van de grafiek wilt omvatten, dan selecteren hoe u de informatie wilt worden samengevat in **die door** gebied wordt samengevat.

1. Op het **Onderste (X) gebied van de As**, selecteer de Groepering die u in de grafiek wilt omvatten.

1. (Facultatief) klik **Lijnen van de Groep**, om een extra groepering voor de grafiek te selecteren.\
   (Facultatief) klik **de Kleuren van de Douane** om de kleuren voor uw nieuwe groepering aan te passen.\
   Voor meer informatie over het aanpassen van grafiekkleuren, zie [&#x200B; kaartkleuren &#x200B;](#customize-chart-colors) aanpassen.

1. (Facultatief) klik **Grafiek van de Combinatie** om uw lijnen door een extra waarde te combineren.\
   Houd rekening met de volgende opties:

   * Selecteer de waarde die u in het diagram wilt opnemen en hoe u de informatie wilt samenvatten.
   * Klik het **Plot op Secundaire het gebied van de As** om de gegevens op de rechterkant van de grafiek te plotten.

1. Klik **sparen + Sluiten** om de grafiek en het rapport te bewaren.

### Grijsgrafiek {#gauge-chart}

A **grafiek van de Gage** toont het aantal verslagen die aan een bepaalde criteria in een grafiekformaat voldoen. De indicator van de maat wijst op het aantal verslagen die aan de criteria voldoen die in de mening en groepering van het rapport worden geselecteerd. Een rapportgroepering wordt niet vereist om een grafiekgrafiek te vormen.

Om a **grafiek van het 1&rbrace; Grijs &lbrace;aan uw rapport toe te voegen:**

1. Begin toevoegend een grafiek aan uw rapport, zoals die in [&#x200B; wordt beschreven voeg een grafiek aan een rapport &#x200B;](#add-a-chart-to-a-report) toe.

1. Op het **gebied van Waarden**, selecteer de waarden die u op het rapport wilt worden getoond, dan selecteren hoe u de informatie wilt worden samengevat in **samengevat door** gebied. Als u **Telling van het Verslag** selecteert, zijn de getoonde waarden het voorwerp van het rapport.

1. Op het **gebied van Indicatoren**, selecteer de Groepering die u in de grafiek wilt omvatten. De groepering wordt vertegenwoordigd door de indicatorlijn op de grafiek.\
   Als u een Groepering hebt die twee punten bevat, worden twee indicatoren getoond op de grafiek.\
   Bijvoorbeeld, als u een Groepering van de Status van het Project hebt, en er twee projectstatussen (Huidige en Op Greep) zijn, bevat uw Grafiek twee meters. Zij zullen wijzen op het aantal projecten dat in die status verkeert.\
   (Optioneel) Selecteer **Totaal** op het **3&rbrace; gebied van Indicatoren &lbrace;om het totaal van de voorwerpen te tonen die op het** worden geselecteerd Waarden **gebied.**

1. (Facultatief) klik **Voeg een andere Waaier van de Waarde** toe om een waardewaaier aan de grafiek toe te voegen.

1. (Facultatief) op het **gebied van de Waaier van de Waarde 0&rbrace; &lbrace;, specificeer de waaier van waarden en de kleur om die waarden te vertegenwoordigen om op de grafiek van het Grijs te tonen.**

1. Klik **sparen + Sluiten** om de grafiek en het rapport te bewaren.

### Bubble-grafiek {#bubble-chart}

U kunt tot drie gebieden van één voorwerp in a **Bubble** grafiek tonen. Dit betekent u tot vier gegevenspunten in een borstelgrafiek kunt tonen. Elke entiteit met drie bijbehorende velden wordt weergegeven als een cirkel die twee van de velden binnen haar locatie binnen de X- en Y-as uitdrukt. Het derde veld wordt weergegeven door de grootte van de cirkel.

Om a **Bubble** grafiek aan uw rapport toe te voegen:

1. Begin toevoegend een grafiek aan uw rapport, zoals die in [&#x200B; wordt beschreven voeg een grafiek aan een rapport &#x200B;](#add-a-chart-to-a-report) toe.

1. In het **Linkergebied (Y) van de As**, selecteer de waarden die u op de as van Y van de grafiek wilt omvatten. De waarden komen uit het standpunt van het verslag. Specificeer hoe u de informatie wilt worden samengevat in **samengevat door** gebied.

1. Op het **gebied van de As van de Onderkant (X)**, selecteer de waarden die u op de as van X van de grafiek wilt omvatten. De waarden komen uit het standpunt van het verslag. Geef op hoe de gegevens moeten worden samengevat.

   >[!NOTE]
   >
   >Zorg ervoor dat u ten minste één kolom hebt die is samengevat om dit veld actief te maken.\
   >Voor meer informatie over het samenvatten van de informatie in een rapportkolom, zie [&#x200B; een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

1. Op het **gebied van de Grootte van de Bubbel**, selecteer de waarden die u door de grootte van de bellen in de grafiek wilt vertegenwoordigen. De waarden komen uit het standpunt van het verslag. Geef op hoe de gegevens moeten worden samengevat.

   >[!NOTE]
   >
   >Zorg ervoor dat u ten minste één kolom hebt die is samengevat om dit veld actief te maken.\
   >Voor meer informatie over het samenvatten van de informatie in een rapportkolom, zie [&#x200B; een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

1. Op het **gebied van Bubbles**, selecteer de Groepering die u in de grafiek wilt omvatten. De groepering wordt vertegenwoordigd door de plaatsing van de bellen op de grafiek.

1. Op het **gebied van de Kleur van de Bubbel**, selecteer het gebied dat u door de kleuren van de bellen wilt worden vertegenwoordigd.

   De **Bubble Kleur** kan een Groepering zijn u in het rapport bepaalt, maar de optie is slechts beschikbaar als u een Groepering op het **Bubbles** gebied kiest dat de **Naam** van een oudervoorwerp met betrekking tot het voorwerp van het rapport, zoals **Naam van het Project** voor een taakrapport of **Naam van het Programma** voor een projectrapport bevat.

   Bijvoorbeeld, als u **Naam van het Project** in een taakrapport selecteerde, kunt u **Status van de Taak** als **Bubble van de Kleur** gebied toevoegen.

   ![&#x200B; status van de Taak als bel kleur &#x200B;](assets/bubbles-field-correct-can-select-bubbles-color-example.png)

   Nochtans, als u **Status van de Taak** voor het **Bubbles** gebied selecteerde, kunt u niet het gebied van de Kleur van de Bubbel van de a **&#x200B;**&#x200B;selecteren. Ook, kunt u niet **Naam van het Project** voor het **Bubble gebied van de Kleur** selecteren, zelfs wanneer u **Naam van het Project** voor het **Bubbles** gebied selecteert.

   ![&#x200B; kan bellen kleur &#x200B;](assets/bubbles-field-wrong-cannot-select-bubbles-color-example.png) niet selecteren

1. Klik **sparen + Sluiten** om de veranderingen in de interfacebouwer te bewaren.

## Grafiekkleuren aanpassen {#customize-chart-colors}

U kunt Workfront de kleuren laten selecteren van de elementen in het diagram of u kunt deze aanpassen terwijl u een diagram toevoegt aan uw rapporten. Als uw grafiek één enkele Groepering bevat die metrisch-zulke zoals een taakrapport vertegenwoordigt dat het aantal taken toont die door Ware VoltooiingsDatum-elk resultaat in de Groepering wordt gegroepeerd in de zelfde kleur wordt getoond.

U kunt slechts één kleur kiezen voor velden die worden weergegeven in de weergave van het rapport. U kunt verscheidene kleuren-voor elke optie-voor gebieden kiezen die in de Groepering van het rapport worden getoond.

>[!IMPORTANT]
>
>Voor datumvelden kunt u slechts één kleur selecteren voor diagramelementen.

Grafiekkleuren aanpassen:

1. Terwijl het bouwen van een rapport, ga naar het **lusje van de Grafiek** in de rapportbouwer.

1. Selecteer een grafiektype om aan uw rapport toe te voegen.\
   Voor meer informatie over het toevoegen van een grafiek aan uw rapport, zie [&#x200B; een grafiek aan een rapport &#x200B;](#add-a-chart-to-a-report) toevoegen.

1. Klik **de Kleuren van de Douane** wanneer dit gebied beschikbaar is.\
   Het dialoogvenster Aangepaste kleuren wordt weergegeven.\
   ![&#x200B; de kleuren van de Douane in grafieken &#x200B;](assets/unshimmed-custom-colors-in-charts.png)

   >[!NOTE]
   >
   >U kunt aangepaste kleuren koppelen aan elk veld dat u kunt groeperen en aan bepaalde velden die in een weergave kunnen worden weergegeven, inclusief aangepaste velden. De aangepaste velden of aangepaste opties voor de velden die u kiest in het dialoogvenster Aangepaste kleur, zijn hoofdlettergevoelig.

1. U kunt een van de volgende opties selecteren:

   * **Gebruik één kleur**: Alle elementen van de grafiek zullen in de geselecteerde kleur tonen.
   * **voegt Kleur** toe: voeg een douanekleur voor een mogelijke waarde van het geselecteerde gebied toe.
   * **verwijder allen**: Selecteer deze optie om alle hierboven gespecificeerde gebiedswaarden en kleuren te verwijderen.
   * **Geen Waarde**: Selecteer dit gebied en een douanekleur om de grafiekkolom te tonen die &quot;geen waarde&quot;punten groepeert. Dit zijn items die niet kunnen worden gegroepeerd met een van de opties van het veld dat in de groep is geselecteerd.
   * **Alle Andere Waarden**: Selecteer dit gebied en een douanekleur om alle andere grafiekelementen te tonen de waarvan opties hierboven niet worden bepaald.

     >[!NOTE]
     >
     >De kleuren u onlangs hebt uitgegeven tonen rechts van de **knoop van de Kleuren van de Douane**. Wanneer u met de muis over een kleur beweegt, wordt de naam van het bijbehorende veld weergegeven. U kunt een kleur ook klikken om het uit te geven zonder **de Kleuren van de Douane** opnieuw te openen.

1. Een kleur kiezen:
Klik in de kleurkiezer om een kleur te selecteren.
OF
Geef een hexadecimale kleurwaarde voor de kleur op.

1. Klik ergens buiten het dialoogvenster Aangepaste kleuren om het te sluiten. De kleuren die u hebt geselecteerd, worden automatisch opgeslagen.

1. Klik **sparen + Sluiten** om de grafiek te bewaren en het rapport in werking te stellen.

## Een diagram exporteren

U kunt een grafiek naar een .pdf- dossier uitvoeren.

Een diagram exporteren:

1. Op het grafieklusje van een rapport, klik **Uitvoer** om de grafiek naar .pdf uit te voeren.\
   Er wordt een .pdf-bestand naar uw computer gedownload.

1. Open het .pdf-bestand.\
   Het geëxporteerde bestand bevat de volgende gegevens:

   * Een afbeelding van het diagram.
   * Een titel die de naam van het rapport is.
   * Een unieke bestandsnaam die is gebaseerd op de naam van het rapport.
   * Een voettekst met de datum en tijd waarop het rapport is geëxporteerd en het paginanummer.

## Een diagram verwijderen uit een rapport

Om een grafiek uit een rapport te verwijderen:

1. Open het **lusje van de Grafiek** van de rapportbouwer.

1. Klik op de knop &quot;x&quot; rechts van de diagramtypen om het diagram te verwijderen.

1. Klik **sparen + Sluiten**.

## Beperkingen tijdens werken met grafieken

Houd rekening met de volgende beperkingen wanneer u werkt met diagrammen:

* De **sectie van de Voorproef van de Grafiek** aan het recht van de rapportbouwer bevat geen daadwerkelijke gegevens van uw rapport. U moet de grafiek bewaren en het van het **Diagram** lusje bekijken om de grafiek met uw gegevens te zien.

* Sommige diagramelementen kunnen niet worden bewerkt:

   * U kunt het lettertype en de tekengrootte niet wijzigen op de waarden van elk element.
   * U kunt de namen van de assen in het diagram niet wijzigen.

* U kunt de legenda van het diagram niet bewerken.
* Wanneer u berekende velden gebruikt voor uw groepen, kunt u niet op de diagramelementen klikken.
* Het meest aantal gegevenspunten u in een grafiek kunt tonen is vier, in een borstelgrafiek. Alle andere grafiektypes tonen twee of een maximum van drie gegevenspunten.
