---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Een aangepast rapport maken
description: Als u begrijpt hoe rapporten moeten worden gemaakt, kunt u toegang bieden tot de informatie die uw organisatie nodig heeft in Adobe Workfront. U kunt elk van de ingebouwde rapporten gebruiken die beschikbaar zijn in Workfront, of u kunt uw eigen rapporten helemaal zelf samenstellen.
author: Nolan
feature: Reports and Dashboards
exl-id: 10c4df37-f09f-4b91-9cfd-3d0c3835bc7b
source-git-commit: b774a74863bb35e3477a69ff11189c40a6d66437
workflow-type: tm+mt
source-wordcount: '1809'
ht-degree: 0%

---


# Een aangepast rapport maken

Als u begrijpt hoe rapporten moeten worden gemaakt, kunt u toegang bieden tot de informatie die uw organisatie nodig heeft in Adobe Workfront. U kunt elk van de ingebouwde rapporten gebruiken die beschikbaar zijn in Workfront, of u kunt uw eigen rapporten helemaal zelf samenstellen.

Voor meer informatie over ingebouwde rapporten, zie [Ingebouwde Adobe Workfront-rapporten gebruiken](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

Voor informatie over het creëren van een rapport door het te kopiëren, zie [Een kopie van een rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Zie de sectie Leren op de Adobe Experience League-site voor meer informatie over het maken en beheren van rapporten, waaronder klassen, video&#39;s en zelfstudies.

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
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>U zult beheertoestemmingen aan het rapport verkrijgen u creeert</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Een rapport maken {#create-a-report}

Om op een video van te letten hoe te om een rapport tot stand te brengen, zie dit [Een aangepast rapport maken](#Walk-thr) hieronder.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek klikt u op **Rapporten**.
1. Klikken **Nieuw rapport** Selecteer vervolgens het objecttype dat u voor het rapport wilt gebruiken.

   De rapportbuilder laadt.

   Zie de sectie voor specifieke informatie over beschikbare objectrapporten [Objecten rapporteren](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) in het artikel [Objecten in Adobe Workfront begrijpen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   ![](assets/nwe-select-new-report-350x666.png)

   >[!TIP]
   >
   >U kunt ook een rapport maken door een kopie van een bestaand rapport te maken. Zie voor meer informatie [Een kopie van een rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. In de rapportaannemer, voeg het volgende aan uw rapport toe:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Functie</th> 
      <th>Beschrijving</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Kolommen (weergave)</td> 
      <td> <p>Het toevoegen van kolommen aan uw rapport bepaalt welke informatie uw rapport bevat.</p> <p>Zie voor meer informatie over het toevoegen van een kolom <a href="#add-columns-view-to-a-report" class="MCXref xref">Kolommen (weergave) toevoegen aan een rapport</a>.<br></p> </td> 
     </tr> 
     <tr> 
      <td>Groepen</td> 
      <td> <p>Het toevoegen van groeperingen aan uw rapport bepaalt hoe uw rapport wordt georganiseerd.</p> <p>Ga voor meer informatie over het toevoegen van een groep naar <a href="#add-groupings-to-a-report" class="MCXref xref">Groepen toevoegen aan een rapport</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Filters</td> 
      <td> <p>Het toevoegen van filterregels aan uw rapport bepaalt informatie u in uw rapport ziet.</p> <p>Ga voor meer informatie over het toevoegen van een filter naar <a href="#add-filters-to-a-report" class="MCXref xref">Filters toevoegen aan een rapport</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Diagram</td> 
      <td> <p>Het toevoegen van een grafiek aan uw rapport bepaalt hoe de informatie in uw rapport visueel wordt voorgesteld.</p> <p>Zie voor meer informatie over het toevoegen van een diagram <a href="#add-a-chart-to-a-report" class="MCXref xref">Een diagram toevoegen aan een rapport</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Op om het even welk punt tijdens het proces van de rapportverwezenlijking, klik **Toepassen** om uw wijzigingen op te slaan.
1. Klik op **Opslaan + Sluiten**.

### Kolommen (weergave) toevoegen aan een rapport {#add-columns-view-to-a-report}

1. Een rapport maken zoals wordt beschreven in het dialoogvenster [Een rapport maken](#create-a-report) in dit artikel.
1. Selecteer in de rapportbuilder de optie **Kolommen (weergave)** om de kolommen te identificeren die in het rapport moeten verschijnen.
1. (Optioneel) Klik op **Een bestaande weergave toepassen** om een bestaande weergave te gebruiken.

   Ga voor meer informatie over het maken van een nieuwe weergave naar [Overzicht van weergaven in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Als u een nieuwe kolom wilt toevoegen, klikt u **Kolom toevoegen**.

   of

   Als u een bestaande kolom wilt wijzigen, selecteert u de kolom die u wilt wijzigen en klikt u op de (x) naast de huidige naam.

1. Typ het veld dat u wilt toevoegen. Als het veld beschikbaar is, wordt het gevuld voor elk object waaraan het kan worden gekoppeld. Klik op de naam van het veld om het aan de kolom toe te voegen.

   Voor meer informatie over de gebieden u in de kolommen ziet, zie [Woordenlijst met Adobe Workfront-terminologie](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

   ![](assets/nwe-add-column-typeahead-350x459.png)

1. (Optioneel) In het dialoogvenster **Kolominstellingen** gebied, selecteren **Sorteren op deze kolom** Als u de waarden in de kolom in oplopende alfabetische volgorde wilt sorteren, geeft u aan of de lijst deze kolom als eerste sortering moet gebruiken.

   U kunt veelvoudige niveaus van soorten in een rapportmening hebben als u door de waarde in één kolom eerst wilt sorteren, de waarde in een tweede kolom tweede, etc.

   Als meerdere resultaten identiek zijn volgens de eerste sorteercriteria, worden ze gesorteerd in de volgorde van de tweede sorteercriteria. Als meerdere resultaten identiek zijn volgens de eerste en tweede sorteercriteria, worden ze gesorteerd op basis van de derde sortering, enz.

   >[!NOTE]
   >
   >Als u een veld toevoegt dat verwijst naar een object dat te ver verwijderd is van het object waarop u rapporteert, kunt u mogelijk niet sorteren op dit veld.\
   >Een uitgiftenrapport kan bijvoorbeeld niet worden gesorteerd op het veld Projecteigenaar omdat het verwijst naar 3 extra objecten: Project, Eigenaar en Naam. Nochtans, kunt u dit gebied aan een probleemrapport nog toevoegen en de informatie voor het zien.

   <!--outdated: To learn more about cross-object references in reports, see the section "Advanced Reporting Part 1 of 3" in the [Reports and Dashboards Learning Path](https://one.workfront.com/s/learningpath2/workfront-reporting-MC7MZT2BOL2ZC2LMJ4MA3EMHOCNY?tabset-dc70e=2).-->

1. (Optioneel) Als u groepen gebruikt en u de gegevens in een kolom wilt samenvatten (samenvoegen), klikt u op de knop **Deze kolom samenvatten met** vervolgkeuzelijst in de **Kolominstellingen** selecteert u vervolgens de optie die u wilt gebruiken om de gegevens in de kolom samen te voegen.

   De samengevoegde informatie wordt weergegeven in de kolom in de rijen voor cijfergroepering.

   ![Samengevoegde samenvatting over groepen](assets/aggregate-summary-displays-on-groupings-2022-350x195.png)

   Voor meer informatie over het samenvatten van gegevens in een kolom, zie [Overzicht van weergaven in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

   >[!NOTE]
   >
   >De volgende uitzonderingen zijn van toepassing op bovenliggende objecten (bijvoorbeeld bovenliggende taken) wanneer u waarden samenvoegt voor de volgende velden in groepen:
   >
   >* Alle getallen en valutavelden behalve Werkelijke uren (bijvoorbeeld Geplande/Werkelijke loonkosten, Geplande/Werkelijke kosten, Geplande/Werkelijke kosten, Geplande/Geplande uren) tellen alleen de waarden voor de kindertaken en standalone taken samen. De waarden voor de bovenliggende taken of ouders van ouders worden niet samengevoegd.
   >* Werkelijke uren tellen de waarden voor de hoofdbovenliggende en zelfstandige taken samen; ze tellen de getallen voor de bovenliggende taken of de onderliggende taken niet samen.
   >* Aangepaste gegevensvelden voor getal- en valutawaarden bevatten alle taken: ouders, kinderen, ouders van ouders en zelfstandige taken.

   Voor meer informatie over het gebruiken van groeperingen in een rapport, zie [Overzicht van groepen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. (Optioneel) Klik op **Geavanceerde opties** om de volgende informatie voor de kolom te specificeren:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aangepast kolomlabel</td> 
      <td> <p>Geef een aangepast label voor de kolom op. Dit label vervangt het standaardlabel.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Veldindeling</td> 
      <td> <p>Selecteer de indeling waarin u de waarden voor de velden in de kolom wilt weergeven.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Deze kolom tonen wanneer deze zich op een dashboard bevindt</td> 
      <td> <p>Selecteer deze optie om deze kolom op een dashboard te tonen, wanneer het rapport naast elkaar met een ander rapport wordt getoond. Als deze optie is uitgeschakeld, wordt deze kolom niet weergegeven wanneer u het rapport weergeeft op een dashboard waar rapporten naast elkaar worden weergegeven.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kolomregels</td> 
      <td> <p>Klikken <strong>Een regel toevoegen voor deze kolom</strong> om voorwaardelijke opmaak toe te voegen aan de kolom. Nadat u een regel hebt toegevoegd, kunt u veld- en tekststijlen definiëren voor de weergave van velden die overeenkomen met die regel. Klikken <strong>Regel toevoegen</strong> nadat u klaar bent met het definiëren van de regel. Zie voor meer informatie over voorwaardelijke opmaak in een weergave <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md" class="MCXref xref">Voorwaardelijke opmaak gebruiken in weergaven</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Toepassen** om uw wijzigingen tot nu toe toe toe toe te passen en het rapport verder te bewerken met de volgende opties.

   Klikken **Opslaan + Sluiten** als u klaar bent met het bewerken van de kolommen in het rapport en u het rapport wilt opslaan.

### Groepen toevoegen aan een rapport {#add-groupings-to-a-report}

1. Een rapport maken zoals wordt beschreven in het dialoogvenster [Een rapport maken](#create-a-report) in dit artikel.
1. Selecteer in de rapportbuilder de optie **Groepen** om te identificeren hoe u punten in het rapport wilt groeperen.
1. Klikken **Groepering toevoegen** om een nieuwe groep toe te voegen.

   of

   Kies **Een bestaande groepering toepassen** om een bestaande groep te selecteren
   ![](assets/nwe-add-grouping-350x230.png)

1. Typ het veld dat u als groep wilt toevoegen. Als het veld beschikbaar is, wordt het gevuld voor elk object waaraan het kan worden gekoppeld. Klik op de naam van het veld om het aan die groep toe te voegen.
1. (Optioneel) U kunt een groep maken in de tekstmodus door te klikken op **Overschakelen naar tekstmodus**. Zie voor meer informatie over het gebruik van de tekstmodus [Overzicht van de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

   Zie voor meer informatie over het maken van nieuwe groepen [Overzicht van groepen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. (Optioneel) Selecteer **Deze groep standaard samenvouwen** als u wilt dat de resultaten in deze groep worden samengevouwen in plaats van uitgevouwen.

   Deze instelling is standaard uitgeschakeld en de resultaten van de groepering worden altijd weergegeven in een uitgevouwen lijst.

   >[!TIP]
   >
   >* Wanneer u groepen handmatig aanpast wanneer u een lijst weergeeft, onthoudt Workfront uw handmatige voorkeur totdat u zich afmeldt. Wanneer u zich weer aanmeldt, wordt de lijst weergegeven volgens deze instelling.
   >* De resultaten van een groepering tonen altijd uitgevouwen na de toegang tot hen van een grafiekelement.

1. (Optioneel) U kunt een matrixgroepering maken om de resultaten in een rasterindeling weer te geven.

   Voor meer informatie over het bouwen van een matrixrapport, zie [Een matrixrapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Klikken **Toepassen** om uw wijzigingen tot nu toe toe toe toe te passen en het rapport verder te bewerken met de volgende opties.

   Klikken **Opslaan + Sluiten** als u klaar bent met het bewerken van de groepen in het rapport en u het rapport wilt opslaan.

### Filters toevoegen aan een rapport {#add-filters-to-a-report}

1. Een rapport maken zoals wordt beschreven in het dialoogvenster [Een rapport maken](#create-a-report) in dit artikel.
1. Selecteer in de rapportbuilder de optie **Filters** om de hoeveelheid informatie te identificeren die u het rapport wilt omvatten.
1. Klikken **Filterregel toevoegen** een aangepast filter toevoegen.\
   of\
   Kies **Een bestaand filter toepassen** een bestaand filter gebruiken.

   ![](assets/nwe-add-a-filter-350x93.png)

1. Als u klikt **Filterregel toevoegen** typt u het veld dat u als filter wilt toevoegen. Als het veld beschikbaar is, wordt het gevuld voor elk object waaraan het kan worden gekoppeld. Klik op de naam van het veld om het aan dat filter toe te voegen.\
   Gebruik filtermodifiers om het filter te maken. Zie voor meer informatie over filtermodifiers [Filter- en voorwaardenmodificatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   Zie voor meer informatie over het maken van nieuwe filters [Overzicht van filters in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Optioneel) U kunt desgewenst een filter maken in de tekstmodus door op **Overschakelen naar tekstmodus**.

   Zie voor meer informatie over het gebruik van de tekstmodus [Overzicht van de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

1. Klikken **Toepassen** als u klaar bent met het bewerken van de filters in het rapport om uw wijzigingen tot nu toe toe toe te passen en het rapport verder te bewerken met de volgende opties.

   Klikken **Opslaan + Sluiten** als het rapport en u het rapport wilt bewaren.

### Een diagram toevoegen aan een rapport {#add-a-chart-to-a-report}

1. Een rapport maken zoals wordt beschreven in het dialoogvenster [Een rapport maken](#create-a-report) in dit artikel.
1. Selecteer in de rapportbuilder de optie **Diagram** selecteert u vervolgens het type diagram dat u wilt toevoegen.

   ![](assets/nwe-add-a-chart-350x247.png)

   Voor meer informatie over het bouwen van een grafiek in een rapport, zie [Een diagram toevoegen aan een rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. Klikken **Toepassen** om uw wijzigingen tot nu toe toe toe toe te passen en het rapport verder te bewerken met de volgende opties.

   Klikken **Opslaan + Sluiten** als u klaar bent met het bewerken van het rapport en u het rapport wilt opslaan.
