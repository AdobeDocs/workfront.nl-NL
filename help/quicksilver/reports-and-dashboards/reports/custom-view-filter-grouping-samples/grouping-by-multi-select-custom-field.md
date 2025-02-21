---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: Een rapport groeperen op basis van een aangepast veld met meerdere selecties
description: U kunt alleen in de tekstmodus groeperen met de waarde in een aangepast veld met meerdere selecties in een Adobe Workfront-rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: 530dff59-0d4c-490e-b464-1d3bb1d0f36f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# Een rapport groeperen op basis van een aangepast veld met meerdere selecties

<!--Audited: 10/2024-->

U kunt alleen in de tekstmodus groeperen met de waarde in een aangepast veld met meerdere selecties in een Adobe Workfront-rapport.

Voorbeelden van aangepaste velden met meerdere selecties zijn:

* Selectievakjes
* Meerdere vervolgkeuzemenu&#39;s selecteren

Voor informatie over het gebruiken van tekstwijze, zie het overzicht van de Wijze van de Tekst van artikel [ ](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Overwegingen bij groeperen op basis van een aangepast veld met meerdere selecties

* U kunt geen rapport in kaart brengen dat een tekst-wijze groepering gebruikt. U moet een extra berekend gebied tot stand brengen dat naar het multi-uitgezochte douanegebied verwijst om het rapport door de waarde van het multi-uitgezochte gebied van de douane ook in kaart te brengen.

  Voor meer informatie, zie [ Grafiek een rapport door een multi-uitgezochte douanegebied ](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/chart-report-by-multi-select-custom-field.md).
* Items waarvoor een van de gekozen opties is geselecteerd, worden slechts één keer geteld.

  Als u bijvoorbeeld een aangepast veld Selectievakje hebt met Keuze 1 en Keuze 2 als opties, en u het formulier koppelt aan taken, worden de taken waarvoor zowel Keuze 1 als Keuze 2 is geselecteerd, afzonderlijk gegroepeerd van de taken waarvoor Alleen Keuze 1 of Keuze 2 is geselecteerd.


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
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> 
    <p>Nieuw:</p>
   <ul><li><p>Medewerker om een filter te wijzigen </p></li>
   <li><p>Standaard voor het wijzigen van een rapport</p></li> </ul>

<p>Huidige:</p>
   <ul><li><p>Verzoek om een filter te wijzigen </p></li>
   <li><p>Plan om een rapport te wijzigen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een rapport groeperen op meerdere geselecteerde aangepaste velden

Als u wilt groeperen op een aangepast veld met meerdere selecties, moet u aan de volgende voorwaarden voldoen:

* Maak het aangepaste veld voor meerdere selecties in een aangepast formulier.\
  Voor informatie over de bouw van douaneformulieren en het toevoegen van douanevelden aan hen, zie het artikel [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

* Koppel het aangepaste formulier aan objecten.
* Vul het aangepaste veld voor meerdere selecties met een waarde voor elk object.

Om door een multi-select douanegebied in een rapport te groeperen:

1. Maak een rapport of bewerk een bestaand rapport waaraan u een groep voor een aangepast veld met meerdere selecties wilt toevoegen.\
   Voor informatie over het creëren van rapporten, zie het artikel [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.
1. Klik **de Acties van het Rapport**, dan **uitgeven**.
1. Selecteer de **Groepen** tabel.
1. Klik **Schakelaar aan de Wijze van de Tekst**.

1. Selecteer de tekst in de **Groep door** doos en vervang het met de volgende code:

   <pre>
   group.0.displayName=Multi-select Naam van aangepast veld
   group.0.valueexpression={DE:Multi-select Naam van aangepast veld}
   group.0.valueformat=HTML
   group.0.textmode=true
   </pre>

1. Vervang &#39;Aangepaste veldnaam voor meerdere selecties&#39; door de werkelijke naam van het aangepaste veld voor meerdere selecties, zoals deze wordt weergegeven in uw Workfront-exemplaar.
1. Klik **sparen en Sluiten**.

   De objecten in het rapport worden gegroepeerd op de waarden van het aangepaste veld voor meerdere selecties.

   ![ Groepering mijn multi-select gebied ](assets/grouping-by-multi-select-field-text-mode-ui-example.png)

   De naam van de groepen in het rapport zijn de namen van het aangepaste veld met meerdere selecties, gevolgd door de waarden die in het veld zijn geselecteerd.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Chart a report by multi-select Custom Fields</h2>
<p>(NOTE: this moved to its own article, linked in the Note above!)</p>
<p>You cannot build a chart in a report by referencing a multi-select custom field. Instead, you can create a calculated field that records the values of the multi-select custom field on a given object and group by the calculated field.&nbsp;</p>
<ul>
<li><a href="#build-a-calculated-custom-field-that-references-a-multi-select-custom-field" class="MCXref xref">Build a calculated custom field that references a multi-select custom field</a> </li>
<li><a href="#build-a-chart-that-references-a-calculated-custom-field" class="MCXref xref">Build a chart that references a calculated custom field</a> </li>
</ul>
<p><strong>Build a calculated custom field that references a multi-select custom field</strong></p>
<p>To be able to build a calculated field that references a multi-select custom field, you must have the following prerequisites:</p>
<ul>
<li>Build the multi-select custom field in a custom form.<br>.</li>
<li>Attach the custom form to objects.</li>
<li>Populate the multi-select custom field with a value on each object.</li>
</ul>
<p>To build the calculated custom field that references the multi-select custom field:</p>
<ol>
<li value="1">Create a custom form, or edit an existing one.<br>.</li>
<li value="2">Click<strong>Add a Field</strong>, then <strong>Calculated</strong> to add the multi-select custom field to the form.</li>
<li value="3">In the <strong>Label</strong> box, name the new calculated field to indicate that it references the multi-select custom field.<br>For example: "Calculated Multi-select Field."</li>
<li value="4"> <p>In the <strong>Calculation</strong> box, enter the following code:</p><pre>{DE:Multi-select Custom Field}</pre> <p> <img src="assets/calculated-multi-select-custom-field-350x201.png" style="width: 350;height: 201;"> <br> </p> </li>
<li value="5">Replace "Multi-select Custom Field" with the actual name of your multi-select custom field, as it appears in Workfront.</li>
<li value="6"> <p>(Optional) If the multi-select custom field is already on this form and if this form is already attached to objects, enable the <strong>Update previous calculations</strong>&nbsp;option.</p> <p>This ensures that the new field is automatically populated with the value from the multi-select custom field as it is added to the forms attached to the objects already.</p> </li>
<li value="7">Click <strong>Done</strong>.</li>
<li value="8">Click <strong>Save +Close</strong>.</li>
</ol>
<p><strong>Build a chart that references a calculated custom field</strong></p>
<ol>
<li value="1"> Go to the report where you want to add the chart for the calculated field that references the multi-select custom field. </li>
<li value="2"> (Optional) To ensure that all the calculated fields that you want to chart by are populated with values, select all the objects in your report, then click <strong>Edit</strong>. </li>
<li value="3"> <p> (Optional and conditional) Enable the <strong>Recalculate Custom Expressions</strong> field, then click <strong>Save Changes</strong>.</p> <p> <img src="assets/recalculate-custom-expressions-350x259.png" style="width: 350;height: 259;"> <br> </p> </li>
<li value="4"> Click <strong>Report Actions</strong>, then <strong>Edit</strong>. </li>
<li value="5">Select the <strong>Groupings</strong> tab, then click <strong>Add Grouping</strong>. </li>
<li value="6">Add the<strong>Calculated Multi-select Field</strong> you created as your grouping. </li>
<li value="7"> <p>Select the <strong>Chart</strong> tab, and add a chart to your report.</p> <p>For information about adding a chart to a report, see the section <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Add a chart to a report</a> in the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>. </p> </li>
<li value="8">Select the <strong>Calculated Multi-select Field</strong> as one of the fields to display in the chart. </li>
<li value="9"> <p>Click <strong>Save + Close</strong>.</p> <p>The report displays the results grouped by the Calculated Multi-select Field in a chart. </p> </li>
</ol>
</div>
-->
