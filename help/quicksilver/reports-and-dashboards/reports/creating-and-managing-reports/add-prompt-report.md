---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Een vraag toevoegen aan een rapport
description: Filters en herinneringen zijn gelijkaardig in die zin dat zij allebei de hoeveelheid informatie beperken die u in een rapport toont.
author: Nolan
feature: Reports and Dashboards
exl-id: b4058fb3-7360-474f-8be1-1c6b584749b0
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1369'
ht-degree: 0%

---

# Een vraag toevoegen aan een rapport

<!-- Audited: 11/2024 -->

## Het verschil tussen aanwijzingen en filters

Filters en herinneringen zijn gelijkaardig in die zin dat zij allebei de hoeveelheid informatie beperken die u in een rapport toont.

U bouwt een filter wanneer u de informatie die in het rapport wordt getoond door de zelfde criteria wilt worden gefiltreerd telkens als u het rapport in werking stelt. Filters worden één keer gemaakt en zijn hard gecodeerd in het rapport. Voor meer informatie over de bouw van filters, zie het overzicht van artikel [ Filters ](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

De herinnering is open filters die kunnen worden aangepast en verschillend worden toegepast telkens als u een rapport in werking stelt.

Wanneer u herinneringen aan uw rapport toevoegt, kunt u de het filtreren informatie aanpassen door de snelle criteria uit te geven telkens als u het rapport in werking stelt. Het rapport loopt met een verschillende filter telkens, afhankelijk van welke bepalingen u kiest, in plaats van hard coderen de bepalingen eens in de filter van het rapport.

De herinneringen fungeren als een aanpasbaar filter op rapporten die vlak kunnen worden bijgewerkt alvorens u het rapport in werking stelt. U kunt generieke rapporten creëren en dan de resultaten beperken die op informatie worden gebaseerd u voor die dag of op de informatie wilt zien die voor een reeks criteria individueel aan u relevant is. Als u bijvoorbeeld een Uren-rapport hebt en u de gegevens van het rapport wilt wijzigen op basis van de volgende criteria:

* De datums waarop de uren zijn vastgelegd
* De gebruikers die de uren hebben ingevoerd
* Het aantal ingevoerde uren

U zou drie herinneringen bouwen waar de voorwaarden de vereiste criteria zijn en het rapport zou verschillend kijken telkens als u het in werking stelt, volgens welke informatie u voor uw herinneringen kiest.

Met een filter kan Adobe Workfront alleen de uren laten zien die tussen juni en augustus van dit jaar zijn ingevoerd. Nochtans, met een herinnering, kunt u een verschillend tijdkader gebruiken telkens als u het rapport in werking stelt (bijvoorbeeld, tussen Januari en Februari of Oktober en December).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
    <td> 
      <p>Nieuw:</p>
         <ul>
         <li><p>Standaard</p></li>
         </ul>
      <p>Huidige:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen*</td> 
   <td> <p>Machtigingen beheren voor een rapport</p></td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

U moet een rapport creëren alvorens u een herinnering aan het kunt toevoegen.

Voor instructies bij het creëren van een rapport, zie [ een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md) creëren

## Een prompt maken

1. Ga naar het rapport waar u een herinnering wilt toevoegen.
1. Breid {de Acties van het 0} Rapport **uit, en klik dan** uitgeven **.**

1. Klik de **knoop van de Montages van het Rapport**.
1. Klik het **Prompts van het Rapport** lusje, dan klik **toevoegen een Herinnering**.\
   ![ de herinneringen van het Rapport tabel ](assets/create-report-prompt-tab.png)

1. (Voorwaardelijk) Selecteer het gebied dat u de herinnering wilt worden gebaseerd op. Typ de naam van het veld en klik om het te selecteren wanneer het veld in de lijst wordt weergegeven.\
   Welke opties beschikbaar zijn voor gebruikers die het rapport uitvoeren, is afhankelijk van het veld dat u selecteert.\
   Als u bijvoorbeeld een datumveld selecteert, zoals Datum van feitelijke voltooiing in een taakrapport, is &quot;Datum van werkelijke voltooiing&quot; de naam van de vraag. Wanneer het uitgeven van deze herinnering aangezien u dit rapport in werking stelt, kunt u van een reeks bepalingen kiezen om uw het filtreren verklaring te bouwen. Dit proces is identiek aan het bouwen van een filter. Voor meer informatie over bepalingen, zie [ Filter en voorwaardenbepalingen ](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Voorwaardelijk) klik **Herinnering van de Douane** om een douaneherinnering tot stand te brengen.

   Een douaneherinnering is een vooraf bepaalde herinnering waar u de het filtreren criteria hard codeert alvorens u het rapport in werking stelt. In dit opzicht is een aangepaste prompt dichter bij een filter dan bij een vraag.

   Nochtans, blijft de herinnering zo flexibel zoals een regelmatige herinnering omdat u van verscheidene vooraf bepaalde verklaringen kunt kiezen, in tegenstelling tot het hebben van enkel één hard - gecodeerde filter in het rapport.

   Geef de volgende informatie op voor de aangepaste prompt: de voorwaarde van een aangepaste prompt kan alleen worden bewerkt in de tekstmodus. Hierdoor kunnen meerdere voorwaarden op één veld worden toegepast.

   * **Naam van het Gebied:** dit is de naam van de herinnering, aangezien u het ziet alvorens u het rapport in werking stelt.
   * **het Etiket van het Punt van de Dropdown:** dit is de naam van één van de opties binnen de herinnering aangezien u het ziet alvorens u het rapport in werking stelt.
   * **Voorwaarde:** ga een voorwaarde in die de herinnering bepaalt.
   * **Gebrek:** u kunt één punt selecteren om de standaardoptie voor deze herinnering te zijn.

   Gebruik dezelfde syntaxis als u zou gebruiken bij het invoeren van een tekstmodusfilter en sluit u uw instructies aan op &quot;&amp;&quot;. Voor meer informatie over het uitgeven van een filter op tekstwijze, zie [ een filter uitgeven gebruikend tekstwijze ](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

   Bijvoorbeeld, kon het **gebied van de Voorwaarde** van de douaneherinnering voor de volgende scenario&#39;s als dit kijken:

   * alle taken met betrekking tot toekomstige projecten waarbij de projectstatus Idea, Requested, Planed en Current is:

     ```
     project:plannedStartDate=$$TODAY&project:plannedStartDate_Mod=gte&project:status=IDA,REQ,PLN,CUR&project:status_Mod=in
     ```

   * alle taken in voltooide (vroegere) projecten waar de projectstatus wordt voltooid of Dead:

     ```
     project:actualCompletionDate=$$TODAY&project:actualCompletionDate_Mod=lte&project:status=CPL,DED&project:status_Mod=in
     ```

   Voor meer informatie over de bepalingen van de tekstwijze, zie [ Filter en voorwaardenbepalingen ](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >U kunt niet de voorwaarden van een douaneherinnering veranderen wanneer u het rapport in werking stelt, zoals u een standaardherinnering zou. U kunt zo vele vooraf bepaalde voorwaarden voor een douaneherinnering hebben aangezien u nodig hebt.

1. (Optioneel) Herhaal stap 4 of 5 om zoveel aanwijzingen als nodig te maken.
1. Klik **Gedaan**, dan klik **sparen+Sluiten** om het rapport te bewaren.

## Een vraag toepassen op een rapport

Wanneer u een herinnering hebt aan een rapport wordt toegevoegd, is het standaardlusje van het rapport altijd de Herinneringen tabel die.

Om een rapport met een herinnering in werking te stellen:

1. Ga naar het rapport met de prompt.

   ![ het rapportherinneringen van de Looppas ](assets/run-report-prompts.png)

1. Kies een voorwaarde voor één of alle herinneringen die op **worden getoond Vragen** tabel.\
   (Optioneel) U kunt de vragen leeg laten en het rapport niet filteren op basis van de voorwaarden voor de vraag.

1. Klik **Rapport van de Looppas**.\
   (Voorwaardelijk) als u de herinneringen bevolkte, wordt het rapport gefiltreerd door de voorwaarden u voor uw herinneringen hebt gekozen.\
   (Voorwaardelijk) als u de herinneringen leeg verliet, wordt het rapport niet gefiltreerd door de snelle voorwaarden. Het rapport wordt weergegeven alsof het niet is gefilterd.

   >[!NOTE]
   >
   >Een rapport dat een filter naast een herinnering bevat filtert de resultaten volgens zowel de criteria die in de filter en de herinnering gecombineerd worden bepaald.

## Beperkingen voor het delen van rapporten die worden gevraagd om rapporten

>[!CAUTION]
>
>Wanneer u een veroorzaakt rapport deelt, zowel het programma geopende als niet het programma geopende gebruikers die het rapport bekijken gebruikend de openbare aandeelverbinding kan niet het rapport in werking stellen gebruikend zijn herinneringen. In dit geval, zullen de resultaten van de rapportvertoning zonder enige herinneringen toe te passen, en de getoonde informatie in plaats daarvan op het toegangsniveau en de toestemmingen van de gebruiker of de Looppas van het rapport als het toegangsniveau van de Gebruiker en toestemmingen, als wordt geplaatst.

Hieronder volgt een beperking voor het delen van rapporten die worden gevraagd door Workfront:

* Wanneer u een rapport openbaar deelt, kunnen de gebruikers niet het rapport met toegepaste herinneringen in werking stellen, tenzij zij: hebben de geloofsbrieven van Workfront, login eerst, en navigeren aan het rapport direct in Workfront (niet door de openbare aandeelverbinding).

  Voor meer informatie over het delen van rapporten, zie het artikel [ een rapport in Adobe Workfront ](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md) delen.

* Wanneer u een veroorzaakt rapport voor levering plant omvat het rapport in de e-mailgehechtheid ongevraagd de gegevens van het rapport. Wanneer de gebruiker de verbinding in e-mail klikt om tot het rapport toegang te hebben, moeten zij login eerst om het rapport te bekijken en de herinnering zelf in werking te stellen.

  Voor informatie over het plannen van een geleverd rapport, zie [ Plan een automatische rapportlevering ](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

* Wanneer het runnen van een rapport met een op datum-gebaseerde herinnering, zullen de rapportresultaten worden gefiltreerd gebaseerd op de montages van de de tijdzone van uw browser. Dit kan lichte verschillen in de datumwaaiers veroorzaken die in een veroorzaakt rapport voor data worden getoond die aan het begin of eind van een maand zijn. Als de de tijdzonemontages van uw browser aan een specifieke plaats gebonden zijn, zullen de variaties in de lokale tijd van die plaats (zoals gehechtheid aan zomertijd) ook in de data worden verwerkt die voor een veroorzaakt rapport worden getoond. Dit kan leiden tot kleine verschillen in datumbereik tussen gebruikers in dezelfde tijdzone, maar met verschillende locatie-instellingen.
