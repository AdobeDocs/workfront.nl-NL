---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Veelgestelde vragen over rapporten
description: Veelgestelde vragen over rapporten
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 0%

---

# Veelgestelde vragen over rapporten

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is the ONE anchor article for all FAQs about Reporting. Add a new FAQ in the TOC at the top first, then add the answer as a section at the bottom.)</p>
-->

Hier volgen vaak gestelde vragen over rapporten.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan, werk</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Waarom toont mijn douaneberekening voor een uurverschil niet het correcte resultaat in een kolom?

Op een projectrapport heb ik een berekening die Werkelijke uren (2) van Geplande Uren (4) aftrekt. Het resultaat dat ik krijg is 120, terwijl het 2 moet zijn.\
Mijn berekening is:
<pre>valueexpression=SUB(workRequired,actualWorkRequired)</pre>

### Antwoord

Velden met uren in Workfront worden in minuten opgeslagen. Als u het veld in een berekening gebruikt, wordt het resultaat in minuten weergegeven. Als u het resultaat in uren wilt verkrijgen, moet u het resultaat van de berekening delen door 60.

De juiste berekening is:

<pre>valueexpression=SUB(workRequired,actualWorkRequired)/60</pre>

## Waarom wordt de waarde van elk van mijn diagramelementen in een rapport niet getoond op de grafiek?

### Antwoord

Als u meer dan 50 grafiekelementen in een rapportgrafiek hebt, toont de waarde van elk element niet in de grafiek.

Wanneer u minder dan 50 elementen in een grafiek hebt, de waarde van elk element toont in de grafiek. Overweeg een filter toe te voegen of de groeperingen in het rapport te wijzigen om de hoeveelheid punten te beperken u in elk element van de grafiek toont.

## Waarom retourneert mijn verslag te veel resultaten om het diagram weer te geven?

Als ik een rapport met een grafiek stel, zie ik de foutmelding &quot;Wow daar... Dit rapport retourneerde een heleboel gegevens die de grafiek onleesbaar maken. U kunt de resultaten verkleinen door een filter toe te voegen of de groepen in het diagram te wijzigen.&quot;

### Antwoord

Deze fout betekent dat uw grafiek tot 618 verschillende resultaten-voor voorbeeld, meer dan 618 bars in een staafgrafiek bevat. Als u het weergaveprobleem wilt verhelpen, moet u de resultaten verfijnen door het huidige filter en de selecties te wijzigen.

Zie de artikelen voor informatie over het wijzigen van filters en groepen [Overzicht van filters](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) en [Overzicht van groepen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Waarom zie ik mijn taken (of kwesties) wanneer ik tot het zelfde rapport (of kalender) toegang heb zoals mijn medewerker en zij hun taken in plaats daarvan zien?

### Antwoord

Het rapport of de kalender zouden een variabele van de vervangingsfilter kunnen hebben die aan de gebruiker richt die het programma wordt geopend. In dit geval, toont het rapport informatie die op de gebruiker wordt gebaseerd die het programma wordt geopend. Pas het filter aan om het jokerteken te verwijderen dat naar de aangemelde gebruiker wijst.\
![](assets/qs--user.id-filter-variable-350x79.png)

Voor een volledige lijst van op gebruiker-gebaseerde het filtervariabelen van de Zitter, zie [Overzicht van jokertekenfiltervariabelen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Waarom lijken de gegevens in mijn verslag onvolledig?

### Antwoord

Dit kan in de meeste gevallen gebeuren als u een beperkte toegang hebt waardoor u items in het systeem niet kunt zien. Bovendien worden de items die u wilt zien niet met u gedeeld.

De maker van het rapport kan het rapport uitgeven om het met de toegangsrechten van een systeembeheerder in werking te stellen, of om het even welke gebruiker van het Plan die toegang heeft om de gegevens te zien.

Zie voor meer informatie [Een rapport uitvoeren en leveren met de toegangsrechten van een andere gebruiker](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

## Hoe kan ik rapporteren over taken (of kwesties) waaraan ik ben toegewezen, of ik nu de eigenaar van ben of niet?

### Antwoord

Om alle taken of kwesties te zien die aan u worden toegewezen, of u de Eigenaar (of Primaire Ontvanger) bent of niet, gebruik het volgende filter in een taak of een uitgiftenrapport:

1. Open een taak- of uitgifterapport.
1. Op de **Filters** tabblad, klikt u op **Filterregel toevoegen**.

1. In de **Veldnaam beginnen te typen...** veld, beginnen met typen **Naam van toewijzingsgebruiker** en selecteert u deze wanneer deze in de lijst wordt weergegeven.

   >[!NOTE]
   >
   >Gebruik de **Toegewezen aan naam** , aangezien dit slechts voor de taken en kwesties filtert waarvoor u de Primaire Ontvanger, of Eigenaar bent.

1. Selecteer de **Gelijk** modifier.
1. Begin met typen *$$USER.ID* in het tekstvak en selecteer dit in de vervolgkeuzelijst die wordt weergegeven.\
   Dit zorgt ervoor dat u alle taken en kwesties ziet die aan de het programma geopende gebruiker worden toegewezen. U kunt het jokerteken vervangen door een specifieke gebruikersnaam.\
   ![](assets/qs-tasks-assigned-to-me-assignment-users-name-filter-350x63.png)

1. Klikken **Opslaan + Sluiten**.

## Waarom worden de Add Kwesties/voegt de verbindingen van Taken niet getoond bij de bodem van mijn Kwesties en lijsten van Taken op een project?

### Antwoord

Eerst, zorg ervoor dat u de correcte toegang en de toestemmingen hebt om kwesties en taken aan een project toe te voegen. In dit geval dient u de **Problemen toevoegen** en **Taken toevoegen** koppelingen onder aan **Problemen** en **Taken** lijsten.

Er zijn echter een paar dingen die voorkomen dat deze koppelingen worden weergegeven:

* Als u het snelle filter hebt toegepast op deze lijsten, worden de koppelingen niet weergegeven. Verwijder het snelle filter en de verbindingen zouden moeten tonen zodat kunt u kwesties en taken aan uw projecten toevoegen.\
  Zie voor informatie over het snelle filter [Aan de slag met lijsten in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* Als u een **Groepering** worden toegepast op deze lijsten, worden de koppelingen niet weergegeven. Verwijder de **Groepering** en de koppelingen moeten worden weergegeven, zodat u problemen en taken aan uw projecten kunt toevoegen.\
  Voor informatie over het creëren van Groepen, zie [Overzicht van groepen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

* Als u een **Weergave** De koppelingen worden niet weergegeven op deze lijsten waarop een andere valuta dan de standaardvaluta voor het project is geselecteerd. Wijzig de **Weergave** tot **Oorspronkelijke valuta van het project** en de koppelingen moeten worden weergegeven, zodat u problemen en taken aan uw projecten kunt toevoegen.\
  Voor meer informatie over het wijzigen van de valuta in je weergave raadpleegt u [Rapporten met financiële gegevens maken met unieke wisselkoersen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

![](assets/nwe-project-original-currency-350x229.png)

## Vernieuwt de informatie in mijn rapport of dashboard automatisch?

### Antwoord

De informatie in rapporten of dashboards verfrist zich niet automatisch.

De informatie kan manueel in een caching rapport worden verfrist.\
Voor meer informatie over het verfrissen van een caching rapport, zie [Een rapport uitvoeren](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

De informatie kan manueel in een caching dashboard worden verfrist.\
Zie de sectie voor meer informatie over het vernieuwen van een dashboard in de cache. [dashboards weergeven](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md#running-dashboards) in het artikel [Aan de slag met dashboards](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Kan ik de eigenaar van een rapport wijzigen?

### Antwoord

U kunt de eigenaar van een rapport niet wijzigen. Nochtans, kan de gebruiker die het rapport creeerde andere gebruikers toestaan om het rapport uit te geven. De manier u gebruikers kunt toestaan om een rapport uit te geven hangt van het type van gebruiker af u bent.

* De beheerders van het systeem kunnen gebruikers met een vergunning van het Plan toestaan om rapporten uit te geven door de Edit optie in de rij van Rapporten te vormen om de toegang te omvatten tot Create een rapport.\
  Zie voor meer informatie [Toegang verlenen tot rapporten, dashboards en kalenders](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Eindgebruikers die toegang hebben tot het maken en delen van rapporten, kunnen afzonderlijke rapporten bewerken door deze te delen en andere gebruikers de machtiging Beheren te geven.\
  Zie voor meer informatie [Een rapport delen in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

Als u toestemmingen hebt om een rapport te bekijken of te beheren, kunt u een exemplaar van het rapport ook maken, dat u dan de eigenaar van door gebrek zult zijn. Ga voor meer informatie over het kopiëren van een rapport naar [Een kopie van een rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Waarom heb ik geen toegang tot een rapport dat eigendom is van een gedeactiveerde gebruiker?

### Antwoord

Soms is de eigenaar van het rapport ook de gebruiker die is opgegeven in het dialoogvenster **Voer dit rapport uit met de toegangsrechten van:** in het verslag. Als de **Voer dit rapport uit met de toegangsrechten van:** de gebruiker wordt gedeactiveerd, toont het rapport niet meer voor gebruikers die het rapport hebben dat met hen wordt gedeeld. Als dit gebeurt, kunt u het rapport weer toegankelijk maken door het **Voer dit Rapport uit met de toegangsrechten van:** leeg maken of een actieve gebruiker in het veld invoeren.

Meer informatie over de **Voer dit Rapport uit met de toegangsrechten van:** veld, zie [Een rapport uitvoeren en leveren met de toegangsrechten van een andere gebruiker](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md). Voor informatie over het identificeren van alle rapporten die eigendom zijn van gedeactiveerde gebruikers, raadpleegt u [Een rapport opstellen over rapportageactiviteiten](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

## Hoe heb ik toegang tot een dashboard dat een rapport bevat dat door een geschrapte gebruiker wordt bezeten?

### Antwoord

Wanneer u een gebruiker schrapt, kunt u tot om het even welke rapporten nog toegang hebben die zij, nochtans, om het even welke dashboards creeerden die het rapport omvatten ook worden geschrapt. Dit betekent dat u niet meer tot het volgende kunt toegang hebben:

* Een dashboard dat het rapport bevat
* Een aangepaste sectie die een dashboard van het rapport bevat

Ga voor meer informatie over de gevolgen van het verwijderen van een gebruiker naar [Gebruikers verwijderen](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

Als u de toegang van de Mening tot het rapport hebt, kunt u het volgende doen:

1. Maak een kopie van het rapport.\
   Ga voor meer informatie over het maken van een kopie van een rapport naar [Een kopie van een rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. Werk het dashboard bij om het gekopieerde rapport op te nemen.\
   Ga voor meer informatie over het bewerken van een dashboard naar [Een dashboard bewerken](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md).
