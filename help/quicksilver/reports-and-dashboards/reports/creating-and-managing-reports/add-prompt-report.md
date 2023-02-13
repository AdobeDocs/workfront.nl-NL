---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Een vraag toevoegen aan een rapport
description: Filters en herinneringen zijn gelijkaardig in die zin dat zij allebei de hoeveelheid informatie beperken die u in een rapport toont.
author: Nolan
feature: Reports and Dashboards
exl-id: b4058fb3-7360-474f-8be1-1c6b584749b0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 0%

---

# Een vraag toevoegen aan een rapport

## Het verschil tussen aanwijzingen en filters

Filters en herinneringen zijn gelijkaardig in die zin dat zij allebei de hoeveelheid informatie beperken die u in een rapport toont.

U bouwt een filter wanneer u de informatie die in het rapport wordt getoond door de zelfde criteria wilt worden gefiltreerd telkens als u het rapport in werking stelt. Filters worden één keer gemaakt en zijn hard gecodeerd in het rapport. Raadpleeg het artikel voor meer informatie over het maken van filters. [Overzicht van filters in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

De herinnering is open filters die kunnen worden aangepast en verschillend worden toegepast telkens als u een rapport in werking stelt.

Wanneer u herinneringen aan uw rapport toevoegt, kunt u de het filtreren informatie aanpassen door de snelle criteria uit te geven telkens als u het rapport in werking stelt. Het rapport loopt met een verschillende filter telkens, afhankelijk van welke bepalingen u kiest, in plaats van hard coderen de bepalingen eens in de filter van het rapport.

De herinneringen fungeren als een aanpasbaar filter op rapporten die vlak kunnen worden bijgewerkt alvorens u het rapport in werking stelt. U kunt generieke rapporten creëren en dan de resultaten beperken die op informatie worden gebaseerd u voor die dag of op de informatie wilt zien die voor een reeks criteria individueel aan u relevant is. Als u bijvoorbeeld een Uren-rapport hebt en u de gegevens van het rapport wilt wijzigen op basis van de volgende criteria:

* De datums waarop de uren zijn vastgelegd
* De gebruikers die de uren hebben ingevoerd
* Het aantal ingevoerde uren

U zou drie herinneringen bouwen waar de voorwaarden de vereiste criteria zijn en het rapport zou verschillend kijken telkens als u het in werking stelt, volgens welke informatie u voor uw herinneringen kiest.

Met een filter kan Adobe Workfront alleen de uren laten zien die tussen juni en augustus van dit jaar zijn ingevoerd. Nochtans, met een herinnering, kunt u een verschillend tijdkader gebruiken telkens als u het rapport in werking stelt (bijvoorbeeld, tussen Januari en Februari of Oktober en December).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

U moet een rapport creëren alvorens u een herinnering aan het kunt toevoegen.

Voor instructies over het maken van een rapport raadpleegt u [Een rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)

## Een prompt maken

1. Ga naar het rapport waar u een herinnering wilt toevoegen.
1. Uitbreiden **Handelingen rapporteren** en klik vervolgens op **Bewerken**.

1. Klikken **Rapportinstellingen**.
1. In de **Prompts rapporteren** gebied, klikken **Vragen toevoegen**.\
   ![](assets/qs-add-a-prompt-350x216.png)

1. (Voorwaardelijk) Selecteer het gebied dat u de herinnering wilt worden gebaseerd op. Typ de naam van het veld en klik om het te selecteren wanneer het veld in de lijst wordt weergegeven.\
   Welke opties beschikbaar zijn voor gebruikers die het rapport uitvoeren, is afhankelijk van het veld dat u selecteert.\
   Als u bijvoorbeeld een datumveld selecteert, zoals Datum van feitelijke voltooiing in een taakrapport, is &quot;Datum van werkelijke voltooiing&quot; de naam van de vraag. Wanneer het uitgeven van deze herinnering aangezien u dit rapport in werking stelt, kunt u van een reeks bepalingen kiezen om uw het filtreren verklaring te bouwen. Dit proces is identiek aan het bouwen van een filter. Zie voor meer informatie over wijzigingstoetsen [Filter- en voorwaardenmodificatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Voorwaardelijk) Klik **Aangepaste prompt** om een aangepaste prompt te maken.

   Een douaneherinnering is een vooraf bepaalde herinnering waar u de het filtreren criteria hard codeert alvorens u het rapport in werking stelt. In dit opzicht is een aangepaste prompt dichter bij een filter dan bij een vraag.

   Nochtans, blijft de herinnering zo flexibel zoals een regelmatige herinnering omdat u van verscheidene vooraf bepaalde verklaringen kunt kiezen, in tegenstelling tot het hebben van enkel één hard - gecodeerde filter in het rapport.

   Geef de volgende informatie op voor de aangepaste prompt: De voorwaarde van een aangepaste prompt kan alleen worden bewerkt in de tekstmodus. Hierdoor kunnen meerdere voorwaarden op één veld worden toegepast.

   * **Veldnaam:** Dit is de naam van de herinnering, aangezien u het ziet alvorens u het rapport in werking stelt.
   * **Label:** Dit is de naam van één van de opties binnen de herinnering aangezien u het ziet alvorens u het rapport in werking stelt.
   * **Voorwaarde:** Voer een voorwaarde in die de vraag definieert.

   Gebruik dezelfde syntaxis als u zou gebruiken bij het invoeren van een tekstmodusfilter en sluit u uw instructies aan op &quot;&amp;&quot;. Voor meer informatie over het bewerken van een filter in de tekstmodus raadpleegt u [Een filter bewerken in de tekstmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

   De **Voorwaarde** het gebied van de douaneherinnering voor de volgende scenario&#39;s zou als dit kunnen kijken:

   * alle taken voor toekomstige projecten waarbij de projectstatus Idea, Requested, Planed en Current is:

      ```
      project:plannedStartDate=$$TODAY&project:plannedStartDate_Mod=gte&project:status=IDA,REQ,PLN,CUR&project:status_Mod=in
      ```

   * alle taken in voltooide (vroegere) projecten waar de projectstatus wordt voltooid of Dead:

      ```
      project:actualCompletionDate=$$TODAY&project:actualCompletionDate_Mod=lte&project:status=CPL,DED&project:status_Mod=in
      ```
   Voor meer informatie over de bepalingen van de tekstwijze, zie [Filter- en voorwaardenmodificatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >U kunt niet de voorwaarden van een douaneherinnering veranderen wanneer u het rapport in werking stelt, zoals u een standaardherinnering zou. U kunt zo vele vooraf bepaalde voorwaarden voor een douaneherinnering hebben aangezien u nodig hebt.

1. (Optioneel) Herhaal stap 4 of 5 om zoveel aanwijzingen als nodig te maken.
1. Klikken **Gereed** en klik vervolgens op **Opslaan en sluiten** om het rapport op te slaan.

## Een vraag toepassen op een rapport

Wanneer u een herinnering hebt aan een rapport wordt toegevoegd, is het standaardlusje van het rapport altijd de Herinneringen tabel die.

Om een rapport met een herinnering in werking te stellen:

1. Ga naar het rapport met de prompt.

   ![](assets/qs-prompt-drop-downs-350x229.png)

1. Kies een voorwaarde voor één of alle herinneringen die op worden getoond **Vragen** tab.\
   (Optioneel) U kunt de vragen leeg laten en het rapport niet filteren op basis van de voorwaarden voor de vraag.

1. Klikken **Rapport uitvoeren**.\
   (Voorwaardelijk) als u de herinneringen bevolkte, wordt het rapport gefiltreerd door de voorwaarden u voor uw herinneringen hebt gekozen.\
   (Voorwaardelijk) als u de herinneringen leeg verliet, wordt het rapport niet gefiltreerd door de snelle voorwaarden. Het rapport wordt weergegeven alsof het niet is gefilterd.

   >[!NOTE]
   >
   >Een rapport dat een filter naast een herinnering bevat filtert de resultaten volgens zowel de criteria die in de filter en de herinnering gecombineerd worden bepaald.

## Beperkingen voor het delen van rapporten die worden gevraagd om rapporten

>[!CAUTION]
>
>Wanneer u een veroorzaakt rapport buiten Workfront deelt, moet de gebruiker die het rapport bekijkt aan Workfront worden het programma geopend om het rapport in werking te stellen gebruikend de herinnering. Als de gebruiker die het rapport bekijkt niet het programma wordt geopend, alle resultaten van de rapportvertoning zonder de herinnering toe te passen.

Hieronder volgt een beperking voor het delen van rapporten die worden gevraagd door Workfront:

* Wanneer u een rapport openbaar deelt kunnen de gebruikers niet het rapport in werking stellen door de herinnering toe te passen, tenzij zij de geloofsbrieven van Workfront en login eerst hebben om het rapport in Workfront te bekijken.

   Zie het artikel voor meer informatie over het delen van rapporten [Een rapport delen in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
* Wanneer u een veroorzaakt rapport voor levering plant, omvat het rapport in de e-mailgehechtheid de gegevens van het rapport genummerd. Wanneer de gebruiker de verbinding in e-mail klikt om tot het rapport toegang te hebben, moeten zij login eerst om het rapport te bekijken en de herinnering zelf in werking te stellen.

   Voor informatie over het plannen van een geleverd rapport, zie [Plan een automatische levering van rapporten](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).
