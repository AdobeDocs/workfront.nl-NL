---
product-area: reporting
navigation-topic: text-mode-reporting
title: Referentieverzamelingen in een rapport
description: Referentieverzamelingen in een rapport
author: Nolan
feature: Reports and Dashboards
exl-id: 18ba3f4b-ae03-4694-a2fe-fdbeeb576ea9
source-git-commit: 6bd9dc626befc4dfa4054760e7ec7d677f6da6e5
workflow-type: tm+mt
source-wordcount: '2615'
ht-degree: 0%

---

# Referentieverzamelingen in een rapport

<!-- Audited: 1/2025 -->

Wanneer u een rapport maakt in Adobe Workfront, kunt u een set objecten, hun respectievelijke velden of gekoppelde objecten weergeven in een lijst, raster of diagramindeling.

Voor meer informatie over de bouw van een rapport in Workfront, zie [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
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
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Machtigingen beheren voor een weergave, filter of groep </p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Verzamelingen begrijpen

Een verzameling is een lijst met objecten die zijn gekoppeld aan een ander object.

U hebt de volgende twee relaties tussen objecten in Workfront:

* **een één-aan-één verhouding**: Één voorwerp kan met slechts één ander voorwerp tegelijkertijd worden verbonden.\
  Een project kan bijvoorbeeld slechts aan één portfolio tegelijk worden gekoppeld.

* **een-aan-vele verhouding**: Één voorwerp kan met verscheidene andere voorwerpen tegelijkertijd worden verbonden.\
  Een project kan bijvoorbeeld meerdere taken hebben. In dit geval vormt de lijst met taken een verzameling voor het project.

>[!IMPORTANT]
>
>U kunt een rapport bouwen dat de één-op-één verhouding tussen voorwerpen toont door de standaard rapportbouwer te gebruiken. Nochtans, kunt u een rapport slechts bouwen dat de één-aan-vele verhouding tussen voorwerpen toont door de interface van de tekstwijze in de rapportbouwer te gebruiken.

Voor meer informatie over de bouw van een rapport in de standaardrapportbouwer, zie [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

Voor meer informatie over de bouw van een rapport gebruikend de interface van de tekstwijze, zie:

* [ Overzicht van de Wijze van de Tekst ](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [ Overzicht van gemeenschappelijk gebruik voor de Wijze van de Tekst ](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
* [Overzicht van syntaxis in tekstmodus](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)

## Verzamelingsobjecten en de bijbehorende velden zoeken in de API Explorer {#find-collection-objects-and-their-fields-in-the-api-explorer}

Niet alle verzamelingen kunnen worden gerapporteerd.

Als u wilt weten welke objecten aan een verzameling van andere objecten kunnen worden gekoppeld, moet u de API Explorer gebruiken.\
Voor meer informatie over de API Verkenner- lijst, zie de [ API Ontdekkingsreiziger ](../../../wf-api/general/api-explorer.md).

Om te weten te komen welke inzamelingen op kunnen worden gemeld:

1. Ga naar de [ API Ontdekkingsreiziger ](../../../wf-api/general/api-explorer.md).
1. Zoek het object van uw rapport.
1. Selecteer de **inzamelingen** tabel.

   >[!NOTE]
   >
   >Alleen de objecten op dit tabblad kunnen worden weergegeven als een verzameling in een rapport voor het object dat u hebt geselecteerd.

1. Vouw het object van de verzameling uit door erop te klikken.
1. Klik op de weergegeven koppeling om naar het object van de verzameling te gaan.\
   Dit opent de **gebieden** tabel voor het voorwerp van uw inzameling.

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

* [ Verwijzing een inzameling in de Mening van een rapport ](#reference-a-collection-in-the-view-of-a-report)
* [ Verwijzing een inzameling in de Filter van een rapport ](#reference-a-collection-in-the-filter-of-a-report)
* [Verwijzing een inzameling in de douaneherinnering van een rapport](#reference-a-collection-in-the-custom-prompt-of-a-report)

### Verwijzing een inzameling in de Mening van een rapport {#reference-a-collection-in-the-view-of-a-report}

U kunt naar een inzameling van voorwerpen in de mening van een rapport van verwijzingen voorzien, om attributen van voorwerpen te tonen verbonden aan het voorwerp van het rapport.

Bijvoorbeeld, kunt u taak tonen of informatie in een projectrapport uitgeven, door een inzamelingskolom voor taken of kwestie in de mening van het rapport te bouwen.

U kunt informatie over de taken of de kwesties, zoals namen, data, primaire wijzers, volledig percentage, enz. in de inzamelingsmening tonen.

De mening toont taak of geeft informatie uit in een lijstformaat, met elke lijn van de lijst die informatie over een taak of een kwestie vertegenwoordigt. De lijst met taken of problemen en de bijbehorende velden wordt weergegeven op dezelfde regel als het project waartoe de taken of problemen behoren.

![ issue_and_tasks_collections_in_reports.png ](assets/issue-and-tasks-collections-in-reports-350x171.png){width=400}

* [ voeg een inzamelingskolom in een rapportMening ](#add-a-collection-column-in-a-report-view) toe
* [ begrijp de lijnen van een inzamelingsmening op de Wijze van de Tekst ](#understand-the-lines-of-a-collection-view-in-text-mode)
* [Beperkingen van een verzamelingsweergave](#limitations-of-a-collection-view)

### Voeg een inzamelingskolom in een rapportmening toe {#add-a-collection-column-in-a-report-view}

Om een inzamelingskolom in een rapportmening toe te voegen:

1. Klik het **Belangrijkste** menu ![ Belangrijkste pictogram van het Menu ](assets/main-menu-icon.png), dan klik **Rapporten**.
1. Klik **Nieuw Rapport**.
1. Selecteer het voorwerp van uw rapport.
1. Navigeer weg van uw rapport, en gebruikend [ API Ontdekkingsreiziger ](../../../wf-api/general/api-explorer.md), bepaal welke inzamelingen voor het voorwerp beschikbaar zijn u voor uw rapport selecteerde.

   Voor meer informatie over het selecteren van het voorwerp van uw inzameling, zie de sectie [ inzamelingsvoorwerpen van de Vondst en hun gebieden in de API Ontdekkingsreiziger ](#find-collection-objects-and-their-fields-in-the-api-explorer) in dit artikel.

   Noteer de naam van het object voor de verzameling.

1. Gebruikend de [ API Ontdekkingsreiziger ](../../../wf-api/general/api-explorer.md), ga naar de lijst van gebieden voor het voorwerp u in de inzameling wilt tonen.

   Voor meer informatie over het vinden van de gebieden van het voorwerp van uw inzameling, zie de sectie [ de inzamelingsvoorwerpen van de Vondst en hun gebieden in de API Ontdekkingsreiziger ](#find-collection-objects-and-their-fields-in-the-api-explorer) in dit artikel.

   Noteer de naam van het veld dat u in de verzameling wilt weergeven.

1. Navigeer terug naar uw rapport, en in de **Kolommen (Mening)** lusje, klik **toevoegen Kolom**.
1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. Klik **uitgeven de Wijze van de Tekst**.
1. Selecteer alle tekst in de **dialoogdoos van de Wijze van de Tekst 0&rbrace; &lbrace;en verwijder het, dan kleef de volgende code als u naar een gebied van het inzamelingsvoorwerp van verwijzingen voorziet:**

   ```
   valueformat=HTML
   textmode=true
   type=iterate
   listdelimiter=<p>
   displayname=Column Name
   listmethod=nested(collection object name).lists
   valuefield=collection object field
   ```

1. Vervang **Naam van de Kolom** met de naam van uw kolom in de `displayname` lijn.
1. Vervang **naam van het 0&rbrace; inzamelingsvoorwerp &lbrace;met de naam van uw inzamelingsvoorwerp in de `listmethod` lijn, aangezien het in [ API Ontdekkingsreiziger ](../../../wf-api/general/api-explorer.md) verschijnt.**

1. Vervang **gebied van de inzamelingsobjecten** met de naam van het gebied van uw inzamelingsvoorwerp in de `valuefield` lijn, aangezien het in [ API Ontdekkingsreiziger ](../../../wf-api/general/api-explorer.md) verschijnt.

   U kunt **waardegebied** met **waardeuitdrukking** vervangen, als u een douaneuitdrukking in uw mening wilt tot stand brengen.

   Voor meer informatie over berekende douaneuitdrukkingen, zie [ Overzicht van berekende gegevensuitdrukkingen ](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Bijvoorbeeld, als u een lijst van de taken in een projectrapport wilt tonen. Deze verzameling gebruikt een `valuefield` -regel voor het verwijzen naar de namen van de taken.

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

     Bericht dat in een inzameling u **kwesties** voor de **listmethod** lijn, in plaats van **opTasks** moet gebruiken die de gegevensbestandnaam voor Kwesties is. Voor informatie over wanneer te gebruiken **kwestie** en wanneer om **opTask** te gebruiken wanneer het verwijzen naar kwesties, zie [ Gebruik &quot;opTask&quot;en &quot;kwestie&quot;wanneer het van verwijzingen voorzien van kwesties ](../../../manage-work/issues/issue-information/use-optask-instead-of-issue.md).

   * Als u een lijst van de taken in een projectrapport samen met hun primaire ontvanger wilt tonen, zou u a **waardeuitdrukking** lijn gebruiken voor het van verwijzingen voorzien van naar de namen van de taken naast de namen van hun primaire wijzers in plaats van **waardegebied**.

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

   ![ het rapport van het Project met taak en toegewezen inzameling ](assets/project-report-with-task-and-assignee-collection-view-nwe-350x222.png){width=400}

1. Klik **sparen**.
1. (Optioneel) Ga door met het bewerken van het rapport.

   of

   Klik **sparen + Sluiten** om het rapport te bewaren.

#### Begrijp de lijnen van een inzamelingsmening in de Wijze van de Tekst

De regels in een tekstmodusweergave voor een verzameling worden in de volgende tabel beschreven:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong> Lijn van de Steekproef </strong> </th> 
   <th><strong> Beschrijving </strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>valueformat=HTML</code> </td> 
   <td> <p>U kunt diverse waarden voor deze lijn gebruiken, maar wij adviseren dat <code style="font-weight: normal;">valueformat</code> voor een inzamelingslijst <strong> HTML zou moeten zijn.</strong></p>
   </td> 
  </tr> 
  <tr> 
   <td><code>textmode=true</code> </td> 
   <td> <p>Deze lijn wijst erop dat de kolom gebruikend tekstwijze is gevormd. Als u deze regel verwijdert, voegt Workfront deze standaard weer toe.</p> </td> 
  </tr> 
  <tr> 
   <td><code>type=iterate</code> </td> 
   <td> <p>De <code>type</code> van een lijst is altijd <code>iterate</code> wanneer u een weergave maakt.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listdelimiter=&lt;p&gt;</code> </td> 
   <td> <p>Dit is het scheidingsteken waarmee de waarden in uw lijst van elkaar worden gescheiden.<br> wij adviseren om <code>&lt;p&gt;</code> te gebruiken die een lijnonderbreking tussen de waarden toevoegt.</p> <p>U kunt ook het volgende gebruiken:</p> <p><code>&zwj;</code> (joiner met breedte nul). De waarden van de verzameling zijn niet van elkaar gescheiden.<br><strong> ,</strong> =kommascheidingsteken. De waarden van de verzameling worden gescheiden door een komma, gevolgd door geen spatie.<br><strong>/</strong> = slash separator. De waarden van de verzameling worden gescheiden door een schuine streep.<br><strong> -</strong> = streepje scheidingsteken. De waarden van de verzameling worden gescheiden door een streepje.<br> het verlaten van deze lijn leeg voegt een komma die door een ruimte tussen de waarden van de inzameling, door gebrek wordt gevolgd.</p> </td> 
  </tr> 
  <tr> 
   <td><code>displayname=</code><em> de Naam van de Kolom </em> </td> 
   <td> <p>Vervang <strong> Naam van de Kolom </strong> met de daadwerkelijke naam van uw nieuwe kolom.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listmethod=nested(collection object name).list</code> </td> 
   <td> <p> Deze lijn bepaalt de inzameling u van verwijzingen voorziet.</p> <p>Vervang <strong> naam van het inzamelingsvoorwerp </strong> met de naam van het voorwerp u in uw inzameling van verwijzingen voorziet, aangezien het in <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref"> API Ontdekkingsreiziger </a> verschijnt. Deze waarde is doorgaans de meervoudige vorm van de naam van het verzamelingsobject.</p> </td> 
  </tr> 
  <tr> 
   <td><code>valuefield=collection object field</code> </td> 
   <td> <p>Deze regel definieert naar welk veld u verwijst vanuit het verzamelingsobject.</p> <p>Vervang <strong> gebied van de inzamelingsobjecten </strong> met de naam van het gebied van het voorwerp u in uw inzameling van verwijzingen voorziet, aangezien het in <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref"> API Ontdekkingsreiziger </a> verschijnt.</p> <p>U kunt deze regel vervangen door:</p> <p><strong> waardeexpression </strong>=calculate gebied/gebieden van de inzamelingsobjecten</p> <p>Gebruikend <strong> waardeuitdrukking </strong>, kunt u  een berekende aangepaste expressie in de kolom weergeven.</p> <p>Voor meer informatie over hoe te om <strong> waardeuitdrukking </strong> lijnen te formatteren, zie <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref"> overzicht van de de wijzesyntaxis van de Tekst </a>.</p> </td> 
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

>[!NOTE]
>
>Wanneer toegepast op gebieden die veelvoudige waarden (zoals een inzameling van nota&#39;s binnen een project) bevatten, bepaalt de filter opneming als volgt:
>
>* Als alle items in een verzameling de opgegeven waarde bevatten, wordt de volledige record niet opgenomen in de resultaten.
>* Als ten minste één item in de verzameling de opgegeven waarde niet bevat, blijft de record in de resultaten.



Een verwijzing naar een inzameling in een rapportfilter toevoegen:

1. Klik het **Belangrijkste** menu ![ Belangrijkste pictogram van het Menu ](assets/main-menu-icon.png), dan klik **Rapporten**.
1. Klik **Nieuw Rapport**.
1. Selecteer het voorwerp van uw rapport.
1. Navigeer weg van uw rapport, en gebruikend [ API Ontdekkingsreiziger ](../../../wf-api/general/api-explorer.md), bepaal welke inzamelingen voor het voorwerp beschikbaar zijn u voor uw rapport selecteerde.

   Voor meer informatie over het selecteren van het voorwerp van uw inzameling, zie de sectie [ inzamelingsvoorwerpen van de Vondst en hun gebieden in de API Ontdekkingsreiziger ](#find-collection-objects-and-their-fields-in-the-api-explorer) in dit artikel.

   Noteer de naam van het object voor de verzameling.

1. Gebruikend de [ API Ontdekkingsreiziger ](../../../wf-api/general/api-explorer.md), ga naar de lijst van gebieden voor het voorwerp u in de inzameling wilt tonen.

   Voor meer informatie over het vinden van de gebieden van het voorwerp van uw inzameling, zie de sectie [ de inzamelingsvoorwerpen van de Vondst en hun gebieden in de API Ontdekkingsreiziger ](#find-collection-objects-and-their-fields-in-the-api-explorer) in dit artikel.

   Noteer het veld dat u in de verzameling wilt weergeven.

1. Navigeer terug naar uw rapport, en op het **lusje van Filters**, klik **Schakelaar aan de Wijze van de Tekst** toen **de Wijze van de Tekst** uitgeven.

1. In het **plaats de Regels van de Filter voor uw gebied van het Rapport**, kleef de volgende code:

   ```
   collection object name:collection object field=collection object value
   collection object name:collection object field_Mod=value of the modifier
   ```

1. Vervang **naam van het inzamelingsvoorwerp** met de naam van uw inzamelingsvoorwerp aangezien het in [ API Ontdekkingsreiziger ](../../../wf-api/general/api-explorer.md) verschijnt. Deze waarde is doorgaans de meervoudige vorm van de naam van het verzamelingsobject.

1. Vervang **gebied van de inzamelingsobjecten** met de naam van het gebied van uw inzamelingsvoorwerp binnen, aangezien het in [ API Ontdekkingsreiziger ](../../../wf-api/general/api-explorer.md) verschijnt.

1. Vervang **waarde van het inzamelingsvoorwerp** met de waarde van het inzamelingsvoorwerp aangezien het in Workfront verschijnt.
1. Vervang **waarde van de bepaling** met een geldige bepaling.

   Voor een lijst van bepalingen, zie [ Filter en voorwaardenbepalingen ](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).\
   Bijvoorbeeld, om een projectrapport te bouwen dat slechts projecten met taken toont die &quot;Marketing&quot;in hun naam hebben, gebruik de volgende code:

   ```
   tasks:name=Marketing
   tasks:name_Mod=cicontains
   ```

   In dit rapport worden alleen projecten weergegeven met ten minste één taak waarvoor het woord &quot;marketing&quot; in de naam voorkomt.

   ![ Marketing slechts taken in project ](assets/marketing-only-tasks-in-project-report-nwe-350x309.png){width=400}

1. Gebruik de volgende code om te filteren op de naam van een uitgave:

   ```
   issues:name=Marketing
   issues:name_Mod=cicontains
   ```

   >[!TIP]
   >
   >U moet `issues` gebruiken voor de naam van het verzamelingsobject in plaats van `optask` , waarin problemen worden weergegeven in de API Explorer.

1. Klik **Gedaan**.
1. (Optioneel) Ga door met het bewerken van het rapport.

   of

   Klik **sparen + Sluiten** om het rapport te bewaren.

### Verwijzing een inzameling in de douaneherinnering van een rapport {#reference-a-collection-in-the-custom-prompt-of-a-report}

U kunt een inzameling van voorwerpen in de douaneherinnering van een rapport van verwijzingen voorzien, om de resultaten van het rapport voor de attributen van voorwerpen te filtreren verbonden aan het voorwerp van het rapport.

Bijvoorbeeld, kunt u voor taakinformatie in een projectrapport ertoe aanzetten door een verwijzing naar de attributen van taken op het project in de douaneherinnering van het rapport te gebruiken.

>[!NOTE]
>
>U kunt geen inzamelingen in een standaardherinnering van verwijzingen voorzien.

Een aangepaste prompt is een aangepast filter waarin de instructies worden gekoppeld door en-tekens. Wij adviseren dat u uw verklaring in een filter bouwt, eerst, dan verbind de lijnen van de verklaringen met ampersands.

Voor meer informatie over de bouw van een filterverklaring met een inzamelingsverwijzing, zie de sectie [ Verwijzing een inzameling in de Filter van een rapport ](#reference-a-collection-in-the-filter-of-a-report) in dit artikel.

Om een verwijzing naar een inzameling in de douaneherinnering van een rapport toe te voegen:

1. Klik het **Belangrijkste** menu ![ Belangrijkste pictogram van het Menu ](assets/main-menu-icon.png), dan klik **Rapporten**.
1. Klik **Nieuw Rapport**.
1. Selecteer het voorwerp van uw rapport.
1. Bouw een filter met een inzamelingsverwijzing zoals die in de sectie [ Verwijzing een inzameling in de Filter van een rapport ](#reference-a-collection-in-the-filter-of-a-report) in dit artikel wordt beschreven.
1. Klik **Montages van het Rapport**.
1. Klik **Herinneringen van het Rapport**.
1. Klik **toevoegen Vragen**.
1. Klik **de Herinnering van de Douane**.
1. Specificeer de naam van de herinnering op het **Gebied**&#x200B;**naam** gebied.

1. Specificeer het Etiket van het Punt van de a **Vervolgkeuzelijst**.
1. Specificeer het volgende op het **gebied van de Voorwaarde**:

   ```
   collection object name:collection object field_Mod=value of the modifier
   ```

1. (Optioneel) Geef op of deze optie standaard wordt weergegeven in de vraag.
1. Vervang **naam van het inzamelingsvoorwerp** met de naam van uw inzamelingsvoorwerp aangezien het in [ API Ontdekkingsreiziger ](../../../wf-api/general/api-explorer.md) verschijnt. Deze waarde is doorgaans de meervoudige vorm van de naam van het verzamelingsobject.
1. Vervang **gebied van de inzamelingsobjecten** met de naam van het gebied van uw inzamelingsvoorwerp, aangezien het in de [ API Ontdekkingsreiziger ](../../../wf-api/general/api-explorer.md) verschijnt.
1. Vervang **waarde van het inzamelingsvoorwerp** met de waarde van het inzamelingsvoorwerp aangezien het in Workfront verschijnt.

   Bijvoorbeeld, als u voor projecten filtreert waarin de naam van de taak &quot;Op de markt brengen&quot;bevat, vervang **de waarde van het inzamelingsvoorwerp** met **marketing**.

1. Vervang **waarde van de bepaling** met een geldige bepaling.

   Voor een lijst van bepalingen, zie [ Filter en voorwaardenbepalingen ](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   **Voorbeeld:** Bijvoorbeeld, om een projectrapport met een douaneherinnering te bouwen waar u slechts projecten wilt tonen die minstens één taak hebben die aan een specifieke gebruiker wordt toegewezen, gebruik hieronder de code:

   ```
   tasks:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&tasks:assignedToID_Mod=in
   ```

   Dit produceert een rapport waar alle vermelde projecten minstens één taak hebben die aan de gebruiker wordt toegewezen de waarvan GUID 57cf1b7a00077c9f02f66cb09c8f86c is.

   >[!NOTE]
   >
   >U kunt niet de naam van primaire toegewezen (&quot;Toegewezen aan&quot;gebied) van een taak van verwijzingen voorzien, volgens de [ API Ontdekkingsreiziger ](../../../wf-api/general/api-explorer.md). U kunt alleen verwijzen naar de id van de primaire ontvanger.

   Bijvoorbeeld, om voor om het even welke projecten te filtreren waar om het even welke projectkwesties aan een specifieke gebruiker worden toegewezen gebruik de volgende code voor uw douaneherinnering:

   ```
   issues:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&issues:assignedToID_Mod=in
   ```

   Dit produceert een rapport waar alle vermelde projecten minstens één kwestie hebben die aan de gebruiker wordt toegewezen de waarvan GUID 57cf1b7a00077c9f02f66cb09c8f86c is.

   >[!NOTE]
   >
   >Bericht dat u **kwesties** voor de naam van het inzamelingsvoorwerp moet gebruiken. De API Explorer biedt momenteel geen naam voor verzamelingsobjecten voor problemen.

1. Klik **Gedaan**.
1. (Optioneel) Ga door met het bewerken van het rapport.

   of

   Klik **sparen + Sluiten** om het rapport te bewaren.
