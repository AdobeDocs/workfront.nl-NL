---
product-area: reporting
navigation-topic: text-mode-reporting
title: Een filter bewerken in de tekstmodus
description: U kunt een filter in een lijst of rapport uitgeven gebruikend tekstwijze om tot gebieden toegang te hebben die niet beschikbaar in de standaardinterface zijn en complexere filters creëren.
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 0%

---

# Een filter bewerken in de tekstmodus

<!-- Audited: 01/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Also, draft this area in the Text Mode overview article)</p>
-->

U kunt een filter in een lijst of rapport uitgeven gebruikend tekstwijze om tot gebieden toegang te hebben die niet beschikbaar in de standaardinterface zijn en complexere filters creëren.

Zie ook de sectie voor meer voorbeelden in de tekstmodus bij het maken van een filter [Voorbeelden van aangepaste filters](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md#samples-of-custom-filters) in het artikel [Voorbeelden van aangepaste weergaven, filters en groepen: artikelindex](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

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
   <td><p>Nieuw: Standaard</p>
    <p>of</p>
    <p>Huidig: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot filters, weergaven en groepen bewerken</p> <p>Toegang tot rapporten, dashboards en kalenders bewerken om rapportelementen in een rapport te bewerken</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten beheren voor een rapport om filters in een rapport te bewerken</p> <p>Machtigingen voor een filter beheren om het te bewerken</p> </td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Voordat u de tekstmodus in een rapport of lijst gaat gebruiken, moet u altijd op de hoogte zijn van de syntaxis van de Workfront-tekstmodus.

Zie voor meer informatie:

* [Overzicht van de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Overzicht van syntaxis in tekstmodus](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Voorbeelden van aangepaste weergaven, filters en groepen: artikelindex](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Tekstmodus in een filter bewerken

Het bewerken van een filter in de tekstmodus is identiek voor rapporten en lijsten. De toegang tot van de filter van een rapport of van een lijst verschilt.

>[!TIP]
>
>We raden u aan om zoveel mogelijk van het filter te maken in de standaardmodus en het filter vervolgens om te zetten in de tekstmodus om het te bewerken.

Voor meer informatie over het bouwen van filters, zie [Overzicht van filters](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Voor informatie over het creëren van een rapport, zie [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Voer een van de volgende handelingen uit:

   1. Ga naar het rapport en klik op **Handelingen rapporteren** > **Bewerken** > **Filters** tab.
   1. Ga vanuit de lijst naar de **Filter** , plaatst u de aanwijzer boven het filter dat u wilt wijzigen en klikt u op de knop **Bewerken** pictogram ![](assets/edit-icon.png).

      De filterbuilder wordt geopend.

1. Klikken **Filterregel toevoegen** om de voorwaarden van het filter toe te voegen, klikt u op **Tekstmodus** of **Overschakelen naar tekstmodus** aan de rechterkant van de bouwer.
1. Voeg filterinstructies toe in de tekstmodus. Elke filterinstructie kan de volgende regels en aanvullende informatie bevatten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td><b>Filterlijn/informatie</b></td> 
      <td><b>Voorbeeld</b></td> 
     </tr> 
     <tr> 
      <td> <p>De veldnaam en de waarde die ermee overeenkomen zoals deze worden weergegeven in de Workfront-database.</p> <p>Deze regel is verplicht.</p> <p> Voor meer informatie over hoe objecten en velden in de database worden weergegeven, raadpleegt u <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>Gebruik de volgende regel om te filteren op taken in de status In uitvoering:</p> <p><code>status=INP</code> </p> <p><b>TIP</b>

   Wanneer het filtreren voor statussen, moet u de drie-lettercode van de status en niet de naam gebruiken.</p> </td>
   </tr> 
     <tr> 
      <td> <p>De bepaling van de gebiedsnaam en wat de bepaling evenaart. Dit geeft aan op welke voorwaarden het veld waarop u filtert, moet voldoen.</p> <p>Deze regel is verplicht.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>Als u wilt aangeven dat de status van de taken waarvoor u filtert, gelijk moet zijn aan In uitvoering, gebruikt u de volgende regel naast de bovenstaande regel:</p> <p><code>status_Mod=in</code> </p> <p>Als de bepaling een waaier is, zijn er twee lijnen om op de bepaling te wijzen.</p> 
       <div> <span class="autonumber"><span><b>VOORBEELD </b></span></span> 
        <p>Dit is een filter van de tekstwijze die taken zoekt die lopend zijn, die een Geplande Datum van de Voltooiing binnen de huidige maand hebben, en aan een gebruiker met een specifieke GUID toegewezen zijn:</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>Zie het artikel voor een volledige lijst met filtermodifiers in de tekstmodus <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter- en voorwaardenmodificatoren</a>.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Instructieoperator. Elke filterinstructie wordt standaard verbonden door de operator AND. Dit wordt niet weergegeven in de interface van de tekstmodus. U kunt ook een operator "OR" tussen twee instructies toevoegen om aan te geven dat u wilt filteren voor objecten die aan een van beide voorwaarden kunnen voldoen.</p> <p>Filteroperatoren zijn alleen vereist voor filters met meer dan één instructie.</p> <p>Tip:   
        <ul> 
         <li> <p>"OR" is hoofdlettergevoelig en moet altijd met hoofdletters worden geschreven.</p> </li> 
         <li> <p>Wanneer u de operator wijzigt van AND in OR, kan het aantal lijstitems toenemen.</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div> <span class="autonumber"><span><b>VOORBEELD </b></span></span> 
        <p>Als u wilt filteren op taken in de status In uitvoering of met de geplande Voltooiingsdatum van Vandaag, gebruikt u het volgende: </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Een vervanging, die u toestaat om de informatie in een filter te generaliseren en de huidige tijd of de gebruiker van verwijzingen te voorzien die het programma wordt geopend.</p> <p>Jokertekens zijn optioneel.</p> <p>Tip:   <p>We raden u aan jokertekens zoveel mogelijk te gebruiken om uw filters dynamischer te maken en niet dezelfde filters voor elke gebruiker of vergelijkbare tijdframes te dupliceren.</p> <p>Zie voor informatie over filterjokertekens <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Overzicht van jokertekenfiltervariabelen</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>VOORBEELD</b></span></span> 
        <p>Om voor taken te filtreren die aan de gebruiker worden toegewezen die momenteel het programma wordt geopend, gebruik het volgende:</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Ga als volgt te werk om een filterinstructie toe te voegen die is verbonden door de operator &quot;OR&quot;:

   1. Een nieuwe coderegel toevoegen en OF typen:1: gevolgd door het object of het kenmerk waarop u wilt filteren en de waarde waarmee u het wilt vergelijken. Gebruik de volgende regel om te verwijzen naar taken in een status behalve Nieuw:

      `OR:1:status=NEW`

   1. Een tweede regel toevoegen en tekst OR:1: gevolgd door het object, de modifier en de modifier-code. Als u de modifier wilt definiëren voor de coderegel die verwijst naar alle taakstatussen behalve Nieuw, gebruikt u de volgende wijzigingregel:

      `OR:1:status_Mod=notin`

      Elke regel van de nieuwe instructie moet worden voorafgegaan door &quot;OR:`<number>`:&quot;.

      Zie voor informatie over het maken van &quot;OR&quot;-instructies in een filter [Instructies OR maken in tekstmodusfilters](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

      >[!NOTE]
      >
      >U kunt meerdere &quot;OR&quot;-instructies in hetzelfde filter hebben. Telkens wanneer u een nieuwe &quot;OF&quot;verklaring hebt, stijgt het aantal na &quot;OF:&quot;.
      >
      >Om voor taken te filtreren die in een status van Bezig zijn of aan de het programma geopende gebruiker toegewezen zijn of zij hebben de Geplande Datum van Voltooiing vandaag, gebruik het volgende:
      >
      >`status=INP`
      >`status_Mod=in`
      >`OR:1:assignedToID=$$USER.ID`
      >`OR:1:assignedToID_Mod=in`
      >`OR:2:plannedCompletionDate=$$TODAY`
      >`OR:2:plannedCompletionDate_Mod=eq`

1. Klikken **Tekstmodus afsluiten** of **Gereed** om de wijzigingen in de tekstmodus op te slaan en het rapport of het filter te blijven bewerken.
1. Klikken **Opslaan + Sluiten** om uw rapport op te slaan of **Filter opslaan** om het filter in de lijst op te slaan.


