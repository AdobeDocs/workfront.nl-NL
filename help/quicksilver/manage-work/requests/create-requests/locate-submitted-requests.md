---
product-area: requests
navigation-topic: create-requests
title: Verzonden verzoeken weergeven
description: Leer over de gebieden van Adobe Workfront waar u verzoeken kunt bekijken die u of iemand anders heeft ingediend of verzoeken die u nooit hebt verzonden en als concepten bent opgeslagen.
author: Alina
feature: Requests
topic: Collaboration
role: User
exl-id: cfa2383a-9594-4867-9b48-11b8ea281486
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: ca8f1375d641531eaf11e3889ccb67a6fbe1788f
workflow-type: tm+mt
source-wordcount: '1441'
ht-degree: 0%

---

# Verzonden verzoeken weergeven

<!--
Remove production and preview references at release
-->

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

U kunt de aanvragen bekijken die u of iemand anders heeft verzonden, of u kunt verzoeken die u bent begonnen maar u hebt het verzenden nooit voltooid. De onvoltooide verzoeken worden opgeslagen als concepten.

U kunt ingediende aanvragen vinden in de volgende gebieden van Adobe Workfront:

* Het gebied Verzoeken van Workfront
* De widget Mijn verzoeken thuis

In het gebied Verzoeken worden de volgende verzoeken weergegeven, afhankelijk van de manier waarop u dit wilt weergeven:

* Workfront vraagt om een oudere ervaring
* Workfront en planningsaanvragen wanneer u de nieuwe ervaring gebruikt.

  >[!NOTE]
  >
  >* U kunt alleen uw eigen conceptaanvragen bekijken.
  >* In de nieuwe ervaring met aanvragen staan de ingediende verzoeken en concepten in dezelfde lijst.
  >* Concepten die zijn gemaakt in de oudere ervaring, worden niet weergegeven in de nieuwe verzoekervaring.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Willekeurig Adobe Workront- of Adobe Workflow-pakket</p> 
   <p>Willekeurig Adobe Workfront-planningspakket</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Medewerker of hoger</p>
   <p>Aanvraag of hoger</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td><p>Toegang tot problemen bewerken</p></td> 
  </tr>
  <tr>
   <td role="rowheader">Objectmachtigingen</td> 
   <td><p>Machtigingen of hoger weergeven voor de aanvragen</p></td> 
  </tr> 
  <!--
  tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
  </tr> 
  -->
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Verzonden verzoeken weergeven op het gebied Verzoeken

U kunt ingediende verzoeken bekijken in het gebied van Verzoeken of in Mijn Verzoeken widget in Huis.

Voor informatie over Mijn Verzoeken, zie [ Gebruik de Mijn widget van Verzoeken ](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

Het bekijken van voorgelegde verzoeken is afhankelijk van de vraag of u de nieuwe of oudere ervaring gebruikt.

* [Verzonden aanvragen weergeven in de nieuwe ervaring die u opvraagt](#view-submitted-requests-in-the-new-requesting-experience)
* [Verzonden aanvragen in de oudere versie weergeven en ervaringen aanvragen](#view-submitted-requests-in-the-legacy-requesting-experience)

### Verzonden aanvragen weergeven in de nieuwe ervaring die u opvraagt

>[!NOTE]
>
>* Als u de Planning van Workfront hebt, verschijnen uw verzoeken van Workfront en van de Planning in de zelfde lijst. De verzoeken van Workfront tonen de waarde `Issue` in de **het type van Objecten** kolom.
>* Er worden standaard maximaal 50 verzoeken weergegeven in de lijst in het gebied Verzoeken. Schuif naar de onderkant van de lijst om meer verzoeken weer te geven.

U kunt ingediende verzoeken bekijken in het gebied van Verzoeken en in Mijn Verzoeken widget in Huis.

>[!NOTE]
>
>De volgende objecten hebben koppelingen van de lijst met aanvragen in het gebied Verzoeken en in de widget Mijn verzoeken, wanneer u de nieuwe ervaring voor aanvragen inschakelt:
>
>* De plannen en Workfront verzoeken op het gebied van Onderwerp.
>* Planningsrecords die zijn gemaakt op basis van planningsverzoeken in het veld Object dat is gemaakt.
>* <span class="preview"> de taken en de kwesties van Workfront die van de verzoeken van Workfront op het gecreeerde Voorwerp gebied, in het milieu van de Voorproef worden omgezet. </span>

Om verzoeken te bekijken die u of andere gebruikers in de nieuwe het vragen ervaring hebben voorgelegd:

{{step1-to-requests}}

1. Zorg ervoor dat het **gebruik nieuwe ervaring** plaatsen in de hoger-juiste hoek van het scherm wordt aangezet.

   De lijst met aanvragen wordt weergegeven.

1. (Optioneel) Als u naar een aanvraag wilt zoeken, typt u in de zoekbalk rechtsboven in de lijst. Zoekresultaten worden weergegeven terwijl u typt.
1. (Optioneel) Als u de manier wilt beheren waarop de informatie in de lijst met aanvragen wordt weergegeven, werkt u de volgende weergaveelementen voor de lijst bij:

   * Weergave
   * Filter
   * Kolommen

   <div class="preview">

   * **Groepering**
   * Cellen opmaken
   * Rijhoogte

   </div>

   Voor meer informatie bij het beheren van informatie in de verzoekenlijst, zie [ Uitgebreide lijsten van het Gebruik ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

1. (Facultatief) controleer het statuut van een verzoek door de **kolom van de Status** te controleren. De volgende statussen zijn beschikbaar in de nieuwe ervaring die u opvraagt:

   * **Ontwerp**: Dit verzoek is nog niet voorgelegd.
   * **In afwachting van Overzicht**: (De Planning slechts) Dit verzoek heeft fiatteurs, en geen van de fiatteurs hebben het verzoek geopend.
   * **In Overzicht**: (Planning slechts) Dit verzoek heeft fiatteurs en minstens één fiatteur heeft het verzoek geopend, maar geen besluit is genomen.
   * **Verworpen**: (Planning slechts) Dit verzoek heeft fiatteurs en is verworpen. Met dit verzoek wordt geen record gemaakt.
   * **Bezig**:
      * Workfront-verzoeken: het verzoek is omgezet en het werk is aan de gang.
      * Aanvragen voor Workfront-planning: De voltooiing van de aanvraag wordt toegewezen aan een specifiek planningsveld en de veldwaarde komt nog niet overeen met de voltooiingswaarde.

        Voor meer informatie, zie [ de details van de Configuratie van de Opstelling ](/help/quicksilver/planning/requests/create-request-form.md#set-up-configuration-details) in artikel creëren en beheren een verzoekvorm in de Planning van Adobe Workfront.
   * **Volledig**: Het verzoek wordt voltooid.

### Verzonden aanvragen in de oudere versie weergeven en ervaringen aanvragen

Om verzoeken te bekijken die u of andere gebruikers in de erfenis hebben voorgelegd die ervaring opvraagt:

{{step1-to-requests}}

1. (Voorwaardelijk) als uw organisatie een pakket van de Planning van Workfront kocht, klik het **Workfront** lusje om de verzoeken van Workfront te bekijken.
1. Klik **Voorgelegd** in het linkerpaneel om alle voorgelegde verzoeken te bekijken.

   U kunt maximaal 2000 verzoeken weergeven en deze kunnen op meerdere pagina&#39;s worden weergegeven.

   >[!TIP]
   >
   >U kunt de kolommen in de lijst Verzendverzoeken niet aanpassen.

   ![ voorgelegde verzoeken nieuwe lijst ](assets/nwe-submitted-requests-new-list-350x57.png)


1. De volgende kolommen worden standaard weergegeven:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">Naam</td> 
         <td> <p>De naam van de aanvraag.</p> <p>Klik op de naam van een aanvraag om deze te openen. </p> <p><b>TIP</b>

   Als de kwestie niet werd bewaard toen het in een taak of een project werd omgezet, wordt de naam van de kwestie verduisterd en kan niet meer worden geklikt. Voor informatie over het omzetten van kwesties, zie <a href="../../../manage-work/issues/convert-issues/convert-issues.md" class="MCXref xref"> Overzicht van het omzetten van kwesties in Adobe Workfront </a>. </p> </td>
   </tr> 
      <tr> 
         <td role="rowheader">Omgezet in</td> 
         <td> <p>De naam van het oplossende voorwerp dat een taak of een project kan zijn dat het verzoek werd omgezet in. </p> <p>Klik op de naam van de taak of het project om deze te openen. </p> <p>Als de aanvraag niet is geconverteerd, is dit veld leeg. </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Pad</td> 
         <td>De naam van de verzoekrij, onderwerpgroepen, en rijonderwerpen waar het verzoek oorspronkelijk werd voorgelegd. </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Status</td> 
         <td>De huidige status van het verzoek of van het oplossende voorwerp (taak of project)</td> 
      </tr> 
      <tr> 
         <td role="rowheader">Invoerdatum</td> 
         <td>De datum waarop het verzoek werd ingediend of de datum waarop het oplossende voorwerp werd gecreeerd als het verzoek werd geschrapt toen het werd omgezet. </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Datum laatste update</td> 
         <td> <p>De datum waarop het verzoek voor het laatst is bijgewerkt.</p> <p>De lijst Verzendverzoeken wordt standaard gesorteerd op dit veld. </p> </td> 
      </tr> 
      </tbody> 
      </table>

1. (Optioneel) Klik op de kop van een kolom om deze te sorteren.

   >[!TIP]
   >
   >Wanneer u bij de lijst Verzendverzoeken vandaan navigeert, blijft de geselecteerde sorteeroptie behouden.

1. (Facultatief) selecteer een verzoek in de lijst, dan klik de **Open Samenvatting** pictogram ![ Open samenvatting met tekst ](assets/open-summary-with-text-nwe.png) om het Samenvattingspaneel te openen en extra informatie over het verzoek te tonen, commentaren, documenten toe te voegen, of het toe te wijzen. Voor informatie over het Summiere paneel, zie [ Overzicht ](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

   >[!TIP]
   >
   >Als het deelvenster Samenvatting al is geopend, verandert het pictogram Samenvatting openen in Samenvatting sluiten.

1. (Facultatief en voorwaardelijk) klik het **X** pictogram in de hoger-juiste hoek of het **Dichte Samenvatting** pictogram ![ dicht overzicht met tekst ](assets/close-summary-with-text-nwe.png) om het Summiere Comité te sluiten.

   Als een kwestie in een taak of een project werd omgezet en de kwestie in het omzettingsproces werd geschrapt, is het Summiere paneel leeg. Voor informatie over het omzetten van kwesties, zie [ Overzicht van het omzetten van kwesties in Adobe Workfront ](../../../manage-work/issues/convert-issues/convert-issues.md).

1. Van het **pictogram van de Filter** ![ pictogram van de Filter ](assets/filter-nwepng.png) in het hoogste recht van de lijst, selecteer om het even welke filters die in de hieronder lijst worden vermeld.

   >[!TIP]
   >
   >U kunt filters in de Ingediende sectie van het gebied van Verzoeken niet wijzigen.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alles</td> 
      <td>Alle ingediende verzoeken, ongeacht hun status of wie ze heeft ingediend.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Openen</td> 
      <td> <p>Alle ingediende verzoeken die momenteel open zijn, ongeacht wie ze heeft ingediend. U kunt alleen een aanvraag indienen waarvoor u ten minste machtigingen hebt om de weergave hier weer te geven als u deze niet zelf hebt verzonden. </p> <p>Aanvragen zonder de datum van feitelijke voltooiing of waarvan het oplossende object geen werkelijke datum van voltooiing heeft, worden vermeld op het subtabblad Openen.</p> <p><b>TIP</b>

   Verzoeken die zich in een status bevinden die niet gelijk is aan Gesloten, worden als open beschouwd.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Mijn verzoeken</td> 
      <td>Verzoeken die u hebt verzonden, ongeacht hun status. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mijn open verzoeken</td> 
      <td> <p>Verzoeken die u hebt verzonden en die nog open zijn. </p> <p>Aanvragen zonder de datum van feitelijke voltooiing of waarvan het oplossende object geen werkelijke afsluitdatum heeft, worden weergegeven op het subtabblad Mijn geopende verzoeken. </p> <p><b>TIP</b>

   Verzoeken die zich niet in een status bevinden die gelijk is aan Gesloten, worden als open beschouwd.</p> </td>
   </tr> 
    </tbody> 
   </table>

1. (Facultatief) klik het **pictogram** pictogram van het Onderzoek ![ bij de bovenkant van de lijst om naar een verzoek door naam te zoeken. ](assets/search-icon.png) De lijst wordt bijgewerkt met resultaten die overeenkomen met uw zoekcriteria.

   <!--

   1. (Conditional) To display only Workfront Request queues, search or filter for `Issue` object types.</span>
   -->

   <!--
   <li> <p>Click the <strong>Complete</strong> subtab to view requests that have been completed.</p> <p>(NOTE: this step will stay drafted even after release. We can't see Completed at this time!) <br>Requests with an Actual Completion Date or whose resolving object has an Actual Completion Date are listed in the Complete subtab.<br>Once a request receives an Actual Completion Date, it stays in the Recently Completed area for 10 business days. After that, it is moved to the Completed area. <br>For information about resolving and resolvable objects, see the article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </li>
   -->

   <!--
   <li>(Optional) Select an option from the <strong>Sort by</strong> drop-down menu to sort the requests by the following criteria:   (NOTE: this step will stay drafted even after release. We can't see Completed at this time!)  
   <ul>
   <li><strong>Assigned To</strong>: Requests are sorted alphabetically by the name of the assignee using the following criteria: 
   <ul>
   <li>All requests assigned to users are sorted first, in the order of the users' names.</li>
   <li>Requests assigned to job roles are sorted secondly, in the order of the job roles' names and are listed after all the requests assigned to users.</li>
   <li>Requests that are assigned to teams are sorted last, in the order of the teams' names and are listed after all the requests assigned to users and those assigned to job roles.</li>
   <li>All unassigned requests are listed last, in the order of their Entry Date. </li>
   </ul></li>
   <li><strong>Submitted On</strong>: Requests are sorted chronologically by the date when they were submitted.</li>
   <li><strong>Recently Updated</strong> (this is the default): Requests are sorted chronologically by the date of their last update.</li>
   <li><strong>Name</strong>: Requests are sorted alphabetically by name. </li>
   <li><strong>Priority</strong>: Requests are sorted in the order of their priority.</li>
   <li><strong>Queue</strong>: Requests are sorted alphabetically by the name of the requests queue where they were submitted. </li>
   <li><strong>Status</strong>: Requests are sorted alphabetically by their status. </li>
   </ul></li>
   -->

1. Klik **Concepten** om alle opgestelde verzoeken te bekijken. Workfront slaat een onbeperkt aantal concepten op voor elke aanvraagwachtrij in deze map. Wanneer u een nieuw verzoek voor een rijonderwerp ingaat dat reeds een ontwerp heeft, zult u worden ertoe aangezet om een bestaand ontwerp te gebruiken. Voor meer informatie, zie [ verzoeken van concepten ](../../../manage-work/requests/create-requests/create-requests-from-drafts.md) creëren.

   <!--
   Planning tab has been removed and no longer visible in legacy Requests area: 
   (Optional and conditional) If your organization purchased a Workfront Planning package, click the **Planning** tab, then click **Submitted** in the left panel to view Workfront Planning requests. 
      Use **Filters** and **Columns** to update the information in the Planning request list. 
      ![Planning tab submitted section in Requests area](assets/workfront-planning-tab-submitted-section-in-requests-area.png)
      For information, see [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md).
   -->


1. (Facultatief) controleer het statuut van een verzoek door de **kolom van de Status** te controleren. De volgende statussen zijn beschikbaar in de nieuwe ervaring die u opvraagt:

   * **Ontwerp**. Dit verzoek is nog niet ingediend.
   * **Bezig**
   * **Volledig**


