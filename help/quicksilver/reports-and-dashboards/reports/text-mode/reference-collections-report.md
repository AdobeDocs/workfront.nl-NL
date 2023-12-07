---
product-area: reporting
navigation-topic: text-mode-reporting
title: Referentieverzamelingen in een rapport
description: Referentieverzamelingen in een rapport
author: Nolan
feature: Reports and Dashboards
exl-id: 18ba3f4b-ae03-4694-a2fe-fdbeeb576ea9
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '2587'
ht-degree: 0%

---

# Referentieverzamelingen in een rapport

Wanneer u een rapport maakt in Adobe Workfront, kunt u een set objecten, hun respectievelijke velden of gekoppelde objecten weergeven in een lijst, raster of diagramindeling.

Ga voor meer informatie over het samenstellen van een rapport in Workfront naar [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Machtigingen beheren voor een weergave, filter of groep </p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Verzamelingen begrijpen

Een verzameling is een lijst met objecten die zijn gekoppeld aan een ander object.

U hebt de volgende twee relaties tussen objecten in Workfront:

* **Een één-op-één relatie**: Eén object kan tegelijkertijd aan slechts één ander object worden gekoppeld.\
  Een project kan bijvoorbeeld slechts aan één portfolio tegelijk worden gekoppeld.

* **Een een-op-een-relatie**: Eén object kan tegelijkertijd aan meerdere andere objecten worden gekoppeld.\
  Een project kan bijvoorbeeld meerdere taken hebben. In dit geval vormt de lijst met taken een verzameling voor het project.

>[!IMPORTANT]
>
>U kunt een rapport bouwen dat de één-op-één verhouding tussen voorwerpen toont door de standaard rapportbouwer te gebruiken. Nochtans, kunt u een rapport slechts bouwen dat de één-aan-vele verhouding tussen voorwerpen toont door de interface van de tekstwijze in de rapportbouwer te gebruiken.

Voor meer informatie over het bouwen van een rapport in de standaard rapportbouwer, zie [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Voor meer informatie over de bouw van een rapport gebruikend de interface van de tekstwijze, zie:

* [Overzicht van de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Overzicht van veelvoorkomende toepassingen voor de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
* [Overzicht van syntaxis in tekstmodus](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)

## Verzamelingsobjecten en de bijbehorende velden zoeken in de API Explorer {#find-collection-objects-and-their-fields-in-the-api-explorer}

Niet alle verzamelingen kunnen worden gerapporteerd.

Als u wilt weten welke objecten aan een verzameling van andere objecten kunnen worden gekoppeld, moet u de API Explorer gebruiken.\
Voor meer informatie over de API Verkenner- lijst, zie [API Explorer](../../../wf-api/general/api-explorer.md).

Om te weten te komen welke inzamelingen op kunnen worden gemeld:

1. Ga naar de [API Explorer](../../../wf-api/general/api-explorer.md).
1. Zoek het object van uw rapport.
1. Selecteer de **verzamelingen** tab.

   >[!NOTE]
   >
   >Alleen de objecten op dit tabblad kunnen worden weergegeven als een verzameling in een rapport voor het object dat u hebt geselecteerd.

1. Vouw het object van de verzameling uit door erop te klikken.
1. Klik op de weergegeven koppeling om naar het object van de verzameling te gaan.\
   Hierdoor wordt het **velden** voor het object van de verzameling.

   >[!NOTE]
   >
   >Alleen de velden op dit tabblad kunnen worden vermeld in het verzamelrapport of in de velden die zijn gekoppeld aan objecten die op dit tabblad worden vermeld.

## Referentieverzamelingen in rapporten

U kunt in de volgende rapporteringselementen verwijzen naar objecten uit een verzameling:

* Weergaven
* Filters
* Vragen

U kunt in de volgende rapportelementen niet verwijzen naar objecten uit een verzameling:

* Groepen
* Diagram

Bijvoorbeeld, kon u de taak van verwijzingen voorzien of inzamelingen van een projectrapport uitgeven, om taak te tonen of informatie op het projectniveau uit te geven.

* [Verwijzing een inzameling in de Mening van een rapport](#reference-a-collection-in-the-view-of-a-report)
* [Verwijzing een inzameling in de Filter van een rapport](#reference-a-collection-in-the-filter-of-a-report)
* [Verwijzing een inzameling in de douaneherinnering van een rapport](#reference-a-collection-in-the-custom-prompt-of-a-report)

### Verwijzing een inzameling in de Mening van een rapport {#reference-a-collection-in-the-view-of-a-report}

U kunt naar een inzameling van voorwerpen in de mening van een rapport van verwijzingen voorzien, om attributen van voorwerpen te tonen verbonden aan het voorwerp van het rapport.

Bijvoorbeeld, kunt u taak tonen of informatie in een projectrapport uitgeven, door een inzamelingskolom voor taken of kwestie in de mening van het rapport te bouwen.

U kunt informatie over de taken of de kwesties, zoals namen, data, primaire wijzers, volledig percentage, enz. in de inzamelingsmening tonen.

De mening toont taak of geeft informatie uit in een lijstformaat, met elke lijn van de lijst die informatie over een taak of een kwestie vertegenwoordigt. De lijst met taken of problemen en de bijbehorende velden wordt weergegeven op dezelfde regel als het project waartoe de taken of problemen behoren.\
![issue_and_tasks_collections_in_reports.png](assets/issue-and-tasks-collections-in-reports-350x171.png)

* [Voeg een inzamelingskolom in een rapportmening toe](#add-a-collection-column-in-a-report-view)
* [Begrijp de lijnen van een inzamelingsmening in de Wijze van de Tekst](#understand-the-lines-of-a-collection-view-in-text-mode)
* [Beperkingen van een verzamelingsweergave](#limitations-of-a-collection-view)

### Voeg een inzamelingskolom in een rapportmening toe {#add-a-collection-column-in-a-report-view}

Om een inzamelingskolom in een rapportmening toe te voegen:

1. Klik op de knop **Hoofd** menu ![](assets/main-menu-icon.png)en klik vervolgens op **Rapporten**.
1. Klikken **Nieuw rapport**.
1. Selecteer het voorwerp van uw rapport.
1. Navigeer weg van uw rapport, en gebruikend [API Explorer](../../../wf-api/general/api-explorer.md)bepaalt u welke verzamelingen beschikbaar zijn voor het object dat u voor het rapport hebt geselecteerd.

   Zie de sectie voor meer informatie over het selecteren van het object van de verzameling [Verzamelingsobjecten en de bijbehorende velden zoeken in de API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in dit artikel.\
   Noteer de naam van het object voor de verzameling.

1. Met de [API Explorer](../../../wf-api/general/api-explorer.md), gaat u naar de lijst met velden voor het object dat u in de verzameling wilt weergeven.

   Zie de sectie voor meer informatie over het zoeken naar de velden van het object in de verzameling [Verzamelingsobjecten en de bijbehorende velden zoeken in de API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in dit artikel.

   Noteer de naam van het veld dat u in de verzameling wilt weergeven.

1. Ga terug naar uw rapport, en in **Kolommen (weergave)** tabblad, klikt u op **Kolom toevoegen**.
1. Klikken **Overschakelen naar tekstmodus**.
1. Plaats de muis boven het dialoogvenster en klik op **Klik om tekst te bewerken**.
1. Selecteer alle tekst in het dialoogvenster **Tekstmodus** en verwijder het, dan kleef de volgende code als u naar een gebied van het inzamelingsvoorwerp van verwijzingen voorziet:

   ```
   valueformat=HTML
   textmode=true
   type=iterate
   listdelimiter=<p>
   displayname=Column Name
   listmethod=nested(collection object name).lists
   valuefield=collection object field
   ```

1. Vervangen **Kolomnaam** met de naam van de kolom in het dialoogvenster `displayname` lijn.
1. Vervangen **objectnaam verzameling** met de naam van het verzamelingsobject in het dialoogvenster `listmethod` lijn, zoals deze wordt weergegeven in de [API Explorer](../../../wf-api/general/api-explorer.md).

1. Vervangen **verzamelobject, veld** met de naam van het veld van het verzamelingsobject in het dialoogvenster `valuefield` lijn, zoals deze wordt weergegeven in de [API Explorer](../../../wf-api/general/api-explorer.md).

   U kunt **taxiveld** with **valueexpression** Als u een aangepaste expressie wilt maken in de weergave.

   Zie voor meer informatie over berekende aangepaste expressies [Overzicht van berekende gegevensexpressies](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Bijvoorbeeld, als u een lijst van de taken in een projectrapport wilt tonen. Deze verzameling gebruikt een `valuefield` lijn voor het van verwijzingen voorzien van de namen van de taken.

   Voer een van de volgende handelingen uit:

   * Gebruik de volgende code om uw kolom te bouwen:

     ```
     valueformat=HTML
     textmode=true
     type=iterate
     listdelimiter=<p>
     displayname=Project Tasks Names
     listmethod=nested(tasks).lists
     valuefield=name
     ```

   * Gebruik de volgende code om een lijst van kwesties in het rapport te tonen:

     ```
     displayname=Project Issues Names
     listdelimiter=<p>
     listmethod=nested(issues).lists
     textmode=true
     type=iterate
     valuefield=name
     valueformat=HTML
     ```

     U moet in een verzameling **kwesties** voor de **listmethod** lijn, in plaats van **opTasks** Dit is de databasenaam voor Issues. Voor informatie over wanneer gebruiken **kwestie** en wanneer **opTask** wanneer wordt verwezen naar kwesties , zie [Gebruik &quot;opTask&quot; en &quot;issue&quot; bij het verwijzen naar problemen](../../../manage-work/issues/issue-information/use-optask-instead-of-issue.md).

   * Als u een lijst van de taken in een projectrapport samen met hun primaire toegewezen wilt tonen, zou u een **valueexpression** regel voor het verwijzen naar de namen van de taken naast de namen van hun primaire toewijzingen in plaats van naar **taxiveld**.

     Gebruik de volgende code om uw kolom te bouwen:

     ```
     valueformat=HTML
     textmode=true
     type=iterate
     listdelimiter=<p>
     displayname=Tasks Names - Primary Assignee
     listmethod=nested(tasks).lists
     valueexpression=CONCAT({name},' - ',{assignedTo}.{name})
     ```

1. De volgende kolomvertoningen in het projectrapport, die van alle taken in elk project naast hun primaire wijzers een lijst maken:

   ![](assets/project-report-with-task-and-assignee-collection-view-nwe-350x222.png)

1. Klikken **Opslaan**.
1. (Optioneel) Ga door met het bewerken van het rapport.

   of

   Klikken **Opslaan + Sluiten** om het rapport op te slaan.

#### Begrijp de lijnen van een inzamelingsmening in de Wijze van de Tekst

De regels in een tekstmodusweergave voor een verzameling worden in de volgende tabel beschreven:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Voorbeeldregel</strong> </th> 
   <th><strong>Beschrijving</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>valueformat=HTML</code> </td> 
   <td> <p>U kunt verschillende waarden gebruiken voor deze regel, maar we raden u aan <code style="font-weight: normal;">valueformat</code> voor een verzamelingslijst <strong>HTML.</strong></p>
   </td> 
  </tr> 
  <tr> 
   <td><code>textmode=true</code> </td> 
   <td> <p>Deze lijn wijst erop dat de kolom gebruikend tekstwijze is gevormd. Als u deze regel verwijdert, voegt Workfront deze standaard weer toe.</p> </td> 
  </tr> 
  <tr> 
   <td><code>type=iterate</code> </td> 
   <td> <p>De <code>type</code> van een lijst altijd <code>iterate</code>, wanneer u een weergave maakt.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listdelimiter=&lt;p&gt;</code> </td> 
   <td> <p>Dit is het scheidingsteken waarmee de waarden in uw lijst van elkaar worden gescheiden.<br>We raden u aan <code>&lt;p&gt;</code> Hiermee wordt een regeleinde toegevoegd tussen de waarden.</p> <p>U kunt ook het volgende gebruiken:</p> <p><code>&amp;zwj;</code> (joiner met breedte nul). De waarden van de verzameling zijn niet van elkaar gescheiden.<br><strong>,</strong> =kommascheidingsteken. De waarden van de verzameling worden gescheiden door een komma, gevolgd door geen spatie.<br><strong>/</strong> = schuine streep. De waarden van de verzameling worden gescheiden door een schuine streep.<br><strong>-</strong> = streepjesscheidingsteken. De waarden van de verzameling worden gescheiden door een streepje.<br>Als u deze regel leeg laat, wordt een komma toegevoegd, gevolgd door standaard een spatie tussen de waarden van de verzameling.</p> </td> 
  </tr> 
  <tr> 
   <td><code>displayname=</code><em>Kolomnaam</em> </td> 
   <td> <p>Vervangen <strong>Kolomnaam</strong> met de werkelijke naam van de nieuwe kolom.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listmethod=nested(collection object name).list</code> </td> 
   <td> <p> Deze lijn bepaalt de inzameling u van verwijzingen voorziet.</p> <p>Vervangen <strong>objectnaam verzameling</strong> met de naam van het object waarnaar u verwijst in de verzameling, zoals deze wordt weergegeven in het dialoogvenster <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. Deze waarde is doorgaans de meervoudige vorm van de naam van het verzamelingsobject.</p> </td> 
  </tr> 
  <tr> 
   <td><code>valuefield=collection object field</code> </td> 
   <td> <p>Deze regel definieert naar welk veld u verwijst vanuit het verzamelingsobject.</p> <p>Vervangen <strong>verzamelobject, veld</strong> met de naam van het veld van het object waarnaar u verwijst in de verzameling, zoals deze wordt weergegeven in het dialoogvenster <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>U kunt deze regel vervangen door:</p> <p><strong>valueexpression</strong>=Berekend verzamelingsobjectveld/ velden</p> <p>Gebruiken <strong>valueexpression</strong>kunt u een berekende aangepaste expressie in de kolom weergeven.</p> <p>Voor meer informatie over opmaak <strong>valueexpression</strong> lijnen, zie <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Overzicht van syntaxis in tekstmodus</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Beperkingen van een verzamelingsweergave {#limitations-of-a-collection-view}

Overweeg de volgende beperkingen wanneer u een inzamelingsmening bouwt:

* U kunt niet de orde controleren waarin de inzamelingsgegevens worden getoond.
* U kunt geen voorwaardelijke opmaak toepassen op een verzamelingsweergave.
* U kunt van een object in een verzameling geen klikbare koppeling maken.
* U kunt geen verzamelingsweergave van een andere verzameling maken.\
  Bijvoorbeeld, kunt u niet alle wijzers op elke taak in een projectrapport tonen. U kunt de primaire toegewezen persoon alleen weergeven voor elke taak in een projectweergave.

### Verwijzing een inzameling in de Filter van een rapport {#reference-a-collection-in-the-filter-of-a-report}

U kunt een inzameling van voorwerpen in de filter van een rapport van verwijzingen voorzien, om voor de attributen van voorwerpen te filtreren verbonden aan het voorwerp van het rapport.

Bijvoorbeeld, kunt u voor taak filtreren of informatie in een projectrapport uitgeven door een verwijzing naar de attributen van taken of kwesties op het project in de filterverklaring te gebruiken.

Een verwijzing naar een inzameling in een rapportfilter toevoegen:

1. Klik op de knop **Hoofd** menu ![](assets/main-menu-icon.png)en klik vervolgens op **Rapporten**.
1. Klikken **Nieuw rapport**.
1. Selecteer het voorwerp van uw rapport.
1. Navigeer weg van uw rapport, en gebruikend [API Explorer](../../../wf-api/general/api-explorer.md)bepaalt u welke verzamelingen beschikbaar zijn voor het object dat u voor het rapport hebt geselecteerd.

   Zie de sectie voor meer informatie over het selecteren van het object van de verzameling [Verzamelingsobjecten en de bijbehorende velden zoeken in de API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in dit artikel.

   Noteer de naam van het object voor de verzameling.

1. Met de [API Explorer](../../../wf-api/general/api-explorer.md), gaat u naar de lijst met velden voor het object dat u in de verzameling wilt weergeven.

   Zie de sectie voor meer informatie over het zoeken naar de velden van het object in de verzameling [Verzamelingsobjecten en de bijbehorende velden zoeken in de API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in dit artikel.

   Noteer het veld dat u in de verzameling wilt weergeven.

1. Ga terug naar uw rapport, en in **Filters** tabblad, klikt u op **Overschakelen naar tekstmodus**.

1. In de **Filterregels instellen voor uw rapport** plakken, plakt u de volgende code:

   ```
   collection object name:collection object field=collection object value
   collection object name:collection object field_Mod=value of the modifier
   ```

1. Vervangen **objectnaam verzameling** met de naam van het verzamelingsobject zoals deze wordt weergegeven in het dialoogvenster [API Explorer](../../../wf-api/general/api-explorer.md). Deze waarde is doorgaans de meervoudige vorm van de naam van het verzamelingsobject.

1. Vervangen **verzamelobject, veld** met de naam van het veld van het verzamelingsobject in, zoals dit wordt weergegeven in het dialoogvenster [API Explorer](../../../wf-api/general/api-explorer.md).

1. Vervangen **objectwaarde van collectie** met de waarde van het verzamelingsobject zoals deze wordt weergegeven in Workfront.
1. Vervangen **waarde van de modifier** met een geldige optie.

   Zie voor een lijst met wijzigingstoetsen [Filter- en voorwaardenmodificatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).\
   Bijvoorbeeld, om een projectrapport te bouwen dat slechts projecten met taken toont die &quot;Marketing&quot;in hun naam hebben, gebruik de volgende code:

   ```
   tasks:name=Marketing
   tasks:name_Mod=cicontains
   ```

   In dit rapport worden alleen projecten weergegeven met ten minste één taak waarvoor het woord &quot;marketing&quot; in de naam voorkomt.

   ![](assets/marketing-only-tasks-in-project-report-nwe-350x309.png)

1. Gebruik de volgende code om te filteren op de naam van een uitgave:

   ```
   issues:name=Marketing
   issues:name_Mod=cicontains
   ```

   >[!TIP]
   >
   >Let op: gebruik `issues` voor de naam van het verzamelingsobject, in plaats van `optask` Dit is hoe problemen worden weergegeven in de API Explorer.

1. Klikken **Gereed**.
1. (Optioneel) Ga door met het bewerken van het rapport.

   of

   Klikken **Opslaan + Sluiten** om het rapport op te slaan.

### Verwijzing een inzameling in de douaneherinnering van een rapport {#reference-a-collection-in-the-custom-prompt-of-a-report}

U kunt een inzameling van voorwerpen in de douaneherinnering van een rapport van verwijzingen voorzien, om de resultaten van het rapport voor de attributen van voorwerpen te filtreren verbonden aan het voorwerp van het rapport.

Bijvoorbeeld, kunt u voor taakinformatie in een projectrapport ertoe aanzetten door een verwijzing naar de attributen van taken op het project in de douaneherinnering van het rapport te gebruiken.

>[!NOTE]
>
>U kunt geen inzamelingen in een standaardherinnering van verwijzingen voorzien.

Een aangepaste prompt is een aangepast filter waarin de instructies worden gekoppeld door en-tekens. Wij adviseren dat u uw verklaring in een filter bouwt, eerst, dan verbind de lijnen van de verklaringen met ampersands.

Zie de sectie voor meer informatie over het bouwen van een filterinstructie met een verzamelingsverwijzing [Verwijzing een inzameling in de Filter van een rapport](#reference-a-collection-in-the-filter-of-a-report) in dit artikel.

Om een verwijzing naar een inzameling in de douaneherinnering van een rapport toe te voegen:

1. Klik op de knop **Hoofd** menu ![](assets/main-menu-icon.png)en klik vervolgens op **Rapporten**.
1. Klikken **Nieuw rapport**.
1. Selecteer het voorwerp van uw rapport.
1. Een filter maken met een verzamelingsverwijzing zoals wordt beschreven in de sectie [Verwijzing een inzameling in de Filter van een rapport](#reference-a-collection-in-the-filter-of-a-report) in dit artikel.
1. Klikken **Rapportinstellingen**.
1. Klikken **Prompts rapporteren**.
1. Klikken **Vragen toevoegen**.
1. Klikken **Aangepaste prompt**.
1. Geef de naam van de vraag op in het dialoogvenster **Veld****naam** veld.

1. Geef een **Itemlabel vervolgkeuzelijst**.
1. Geef het volgende op in het dialoogvenster **Voorwaarde** veld:

   ```
   collection object name:collection object field_Mod=value of the modifier
   ```

1. (Optioneel) Geef op of deze optie standaard wordt weergegeven in de vraag.
1. Vervangen **objectnaam verzameling** met de naam van het verzamelingsobject zoals deze wordt weergegeven in het dialoogvenster [API Explorer](../../../wf-api/general/api-explorer.md). Deze waarde is doorgaans de meervoudige vorm van de naam van het verzamelingsobject.
1. Vervangen **verzamelobject, veld** met de naam van het veld van het verzamelingsobject, zoals dit wordt weergegeven in het dialoogvenster [API Explorer](../../../wf-api/general/api-explorer.md).
1. Vervangen **objectwaarde van collectie** met de waarde van het verzamelingsobject zoals deze wordt weergegeven in Workfront.

   Bijvoorbeeld, als u voor projecten filtreert waarin de naam van de taak &quot;Marketing&quot;bevat, vervang **objectwaarde van collectie** with **marketing**.

1. Vervangen **waarde van de modifier** met een geldige optie.

   Zie voor een lijst met wijzigingstoetsen  [Filter- en voorwaardenmodificatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   **Voorbeeld:** Bijvoorbeeld, om een projectrapport met een douaneherinnering te bouwen waar u slechts projecten wilt tonen die minstens één taak hebben die aan een specifieke gebruiker wordt toegewezen, gebruik hieronder de code:

   ```
   tasks:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&tasks:assignedToID_Mod=in
   ```

   Dit produceert een rapport waar alle vermelde projecten minstens één taak hebben die aan de gebruiker wordt toegewezen de waarvan GUID 57cf1b7a00077c9f02f66cb09c8f86c is.

   >[!NOTE]
   >
   >U kunt niet naar de naam van de primaire toegewezen persoon (veld Toegewezen aan) van een taak verwijzen, afhankelijk van het [API Explorer](../../../wf-api/general/api-explorer.md). U kunt alleen verwijzen naar de id van de primaire ontvanger.

   Bijvoorbeeld, om voor om het even welke projecten te filtreren waar om het even welke projectkwesties aan een specifieke gebruiker worden toegewezen gebruik de volgende code voor uw douaneherinnering:

   ```
   issues:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&issues:assignedToID_Mod=in
   ```

   Dit produceert een rapport waar alle vermelde projecten minstens één kwestie hebben die aan de gebruiker wordt toegewezen de waarvan GUID 57cf1b7a00077c9f02f66cb09c8f86c is.

   >[!NOTE]
   >
   Let op: gebruik **kwesties** for the collection object name. De API Explorer biedt momenteel geen naam voor verzamelingsobjecten voor problemen.

1. Klikken **Gereed**.
1. (Optioneel) Ga door met het bewerken van het rapport.

   of

   Klikken **Opslaan + Sluiten** om het rapport op te slaan.
