---
product-area: requests
navigation-topic: create-requests
title: Verzonden verzoeken zoeken
description: Leer over de gebieden van Adobe Workfront waar u van verzoeken kunt de plaats bepalen die u of iemand anders indiende of verzoeken die u nooit hebt voorgelegd en als ontwerpen bewaard.
author: Alina
feature: Requests
topic: Collaboration
role: User
exl-id: cfa2383a-9594-4867-9b48-11b8ea281486
source-git-commit: 78b4724ca8d5df15ed76e9e882179e3cb127282c
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 0%

---

# Verzonden aanvragen zoeken

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

U kunt de volgende typen verzoeken zoeken die u of iemand anders heeft verzonden, of aanvragen die u hebt gestart maar die u nooit hebt verzonden. U kunt deze aanvragen vinden in de volgende gebieden van Adobe Workfront:

* Het **Workfront** lusje van het gebied van Verzoeken in Workfront: Zoek verzoeken die aan de verzoekrijen van Workfront in de volgende secties worden voorgelegd:
   * **voorgelegde sectie**: Alle verzoeken die u of iemand anders voorlegde en u toegang tot minstens Mening hebt.
   * **sectie van het Ontwerp**: Alle verzoeken die u begon maar u nooit beëindigde en u voorlegde nooit. Voor meer informatie over ontwerp verzoeken, zie [ Adobe Workfront verzoeken ](../../../manage-work/requests/create-requests/create-submit-requests.md) creëren en voorleggen.

  >[!TIP]
  >
  >U kunt alleen uw eigen conceptaanvragen bekijken.

* Het **Planning** lusje van het gebied van Verzoeken in Workfront: plaats verzoeken die aan de aanvraagformulieren van de Planning van Workfront worden voorgelegd. Uw organisatie moet een pakket voor Workfront-planning aanschaffen. Raadpleeg de volgende artikelen voor meer informatie:

   * [Een aanvraagformulier maken en beheren in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
   * [Adobe Workfront-planningsverzoeken verzenden om records te maken](/help/quicksilver/planning/requests/submit-requests.md)


## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Nieuw: Medewerker of hoger</p>
   of
   <p>Huidig: Verzoek of hoger</p>
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
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Verzonden aanvragen zoeken

Om van verzoeken de plaats te bepalen die u of andere gebruikers hebben voorgelegd:

{{step1-to-requests}}

1. (Voorwaardelijk) als uw organisatie een pakket van de Planning van Workfront kocht, klik het **Workfront** lusje om de verzoeken van Workfront te bekijken.
1. Klik **Voorgelegd** in het linkerpaneel om alle voorgelegde verzoeken te bekijken.

   U kunt maximaal 2000 verzoeken weergeven en deze kunnen op meerdere pagina&#39;s worden weergegeven.

   >[!TIP]
   >
   >U kunt de kolommen in de lijst Verzendverzoeken niet aanpassen.

   ![](assets/nwe-submitted-requests-new-list-350x57.png)


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

1. (Facultatief) selecteer een verzoek in de lijst, dan klik het **Open Samenvatting** pictogram ![](assets/open-summary-with-text-nwe.png) om het Summiere paneel te openen en extra informatie over het verzoek te tonen, commentaren, documenten toe te voegen, of het toe te wijzen. Voor informatie over het Summiere paneel, zie [ Overzicht ](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

   >[!TIP]
   >
   >Als het deelvenster Samenvatting al is geopend, verandert het pictogram Samenvatting openen in Samenvatting sluiten.

1. (Facultatief en voorwaardelijk) klik het **X** pictogram in de hoger-juiste hoek of het **Dichte Samenvatting** pictogram ![](assets/close-summary-with-text-nwe.png) om het Summiere Comité te sluiten.

   Als een kwestie in een taak of een project werd omgezet en de kwestie in het omzettingsproces werd geschrapt, is het Summiere paneel leeg. Voor informatie over het omzetten van kwesties, zie [ Overzicht van het omzetten van kwesties in Adobe Workfront ](../../../manage-work/issues/convert-issues/convert-issues.md).

1. Van het **pictogram van de Filter** ![](assets/filter-nwepng.png) in het hoogste recht van de lijst, selecteer om het even welke filters die in de hieronder lijst worden vermeld.

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

1. (Optioneel) Klik op het **pictogram ![](assets/search-icon.png) van de pagina met filters** boven aan de lijst om naar een verzoek op naam te zoeken. De lijst wordt bijgewerkt met resultaten die overeenkomen met uw zoekcriteria.

   <!--
   <li value="9" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Click the <strong>Complete</strong> subtab to view requests that have been completed.</p> <p>(NOTE: this step will stay drafted even after release. We can't see Completed at this time!) <br>Requests with an Actual Completion Date or whose resolving object has an Actual Completion Date are listed in the Complete subtab.<br>Once a request receives an Actual Completion Date, it stays in the Recently Completed area for 10 business days. After that, it is moved to the Completed area. <br>For information about resolving and resolvable objects, see the article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </li>
   -->

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Optional) Select an option from the <strong>Sort by</strong> drop-down menu to sort the requests by the following criteria:   (NOTE: this step will stay drafted even after release. We can't see Completed at this time!)  
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

1. (Facultatief en voorwaardelijk) als uw organisatie een pakket van de Planning van Workfront kocht, klik het **Planning** lusje, dan klik **voorgelegde** in het linkerpaneel om de verzoeken van de Planning van Workfront te bekijken.

   **Filters van het Gebruik** en **Kolommen** om de informatie in de lijst van het Verzoek van de Planning bij te werken. </span><span class="preview">

   <span class="preview">![](assets/workfront-planning-tab-submitted-section-in-requests-area.png)</span>

   Voor informatie, zie [ de Verzoeken van de Planning van Adobe Workfront voorleggen om verslagen ](/help/quicksilver/planning/requests/submit-requests.md) tot stand te brengen.


