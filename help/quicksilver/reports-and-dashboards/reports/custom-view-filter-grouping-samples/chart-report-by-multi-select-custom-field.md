---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: Een rapport in kaart brengen op basis van een aangepast veld met meerdere selecties
description: U kunt een rapport alleen in een diagram weergeven op basis van een aangepast veld met meerdere selecties nadat u een extra berekend veld hebt gemaakt waarin de geselecteerde keuzen in het aangepaste veld met meerdere selecties worden vastgelegd.
author: Jenny
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: 4897f165a7316a52b968601b45f95f7045f63840
workflow-type: tm+mt
source-wordcount: '1005'
ht-degree: 0%

---

# Een rapport in een diagram weergeven op basis van een aangepast veld met meerdere selecties

<!--Audited: 11/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

In plaats van een diagram te maken met een aangepast veld met meerdere selecties, raden we u aan aparte velden te maken voor elke optie van een aangepast veld met meerdere selecties.

Voorbeelden van aangepaste velden met meerdere selecties zijn:

* Selectievakjes
* Meerdere vervolgkeuzemenu&#39;s selecteren

Voor informatie over het gebruiken van tekstwijze, zie het overzicht van de Wijze van de Tekst van artikel [&#x200B; &#x200B;](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Als het echter niet mogelijk is afzonderlijke velden te hebben voor elke optie van een veld met meerdere selecties, kunt u een rapport aan de hand van een aangepast veld met meerdere selecties weergeven door berekende aangepaste velden te gebruiken om de keuzen van het veld met meerdere selecties eerst te groeperen. Daarna, kunt u het rapport door de berekende gebieden in kaart brengen.

>[!NOTE]
>
>Items waarvoor een van de gekozen opties is geselecteerd, worden slechts één keer geteld.
>
>Als u bijvoorbeeld een aangepast veld Selectievakje hebt met Keuze 1 en Keuze 2 als opties, en u het formulier koppelt aan taken, worden de taken die zowel Keuze 1 als Keuze 2 hebben, weergegeven in een afzonderlijk diagramelement dan de taken waarvoor Alleen Keuze 1 of Keuze 2 is geselecteerd.
>
>De taken die Keuze 1 hebben geselecteerd tonen niet in het zelfde grafiekelement zoals de taken die Keuze 1 en Keuze 2 hebben geselecteerd.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Medewerker of verzoek om een filter te wijzigen </p>
   <p>Standaard of Plan om een rapport te wijzigen</p>
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

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Voordat u begint, moet u een berekend aangepast veld maken waarin de waarden worden weergegeven die in het aangepaste veld voor meerdere selecties zijn geselecteerd. Voor informatie, zie [&#x200B; een berekend douanegebied bouwen dat verwijzingen een multi-uitgezochte sectie van het douanegebied &#x200B;](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) in dit artikel.

## Een rapport weergeven op basis van meerdere geselecteerde aangepaste velden

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

U kunt geen grafiek in een rapport bouwen door naar een multi-select douanegebied van verwijzingen te verwijzen. In plaats daarvan kunt u een berekend veld maken waarmee de waarden van het aangepaste veld voor meerdere selecties voor een bepaald object en een bepaalde groep worden vastgelegd in het berekende veld. 

* [&#x200B; bouwt een berekend douanegebied dat verwijzingen een multi-uitgezochte douanegebied &#x200B;](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [Bouw een grafiek die verwijzingen een berekend douanegebied](#build-a-chart-that-references-a-calculated-custom-field)

### Een berekend aangepast veld maken dat verwijst naar een aangepast veld met meerdere selecties {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

Als u een berekend veld wilt maken dat verwijst naar een aangepast veld met meerdere selecties, moet u aan de volgende voorwaarden voldoen:

* Een aangepast veld met meerdere selecties in een aangepast formulier.\
  Voor informatie over de bouw van douaneformulieren en het toevoegen van douanevelden aan hen, zie het artikel [&#x200B; een douaneformulier &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

* Een aangepast formulier waaraan het aangepaste veld voor meerdere selecties is gekoppeld.
* Waarden voor het aangepaste veld met meerdere selecties voor elk object.

U kunt als volgt het berekende aangepaste veld bouwen dat verwijst naar het aangepaste veld voor meerdere selecties:

1. Een aangepast formulier maken of een bestaand formulier bewerken.

   Voor informatie over het creëren van douaneformulieren, zie [&#x200B; een douaneformulier &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

1. Selecteer het object of de objecten die u wilt gebruiken voor het aangepaste formulier.
1. Klik **toevoegen een Gebied**, dan **Berekend** om het multi-uitgezochte douanegebied aan de vorm toe te voegen.

1. In het **vakje van het Etiket**, noem het nieuwe berekende gebied om erop te wijzen dat het multi-select douanegebied van verwijzingen voorziet.

   Bijvoorbeeld: &quot;Berekend multiselect veld&quot;.

1. In het **vakje van de Berekening**, ga de volgende code in:

   `{DE:Multi-select Custom Field}`

   Hiermee voegt u de geselecteerde keuzen in het aangepaste veld voor meerdere selecties toe aan het berekende aangepaste veld. Als het formulier bijvoorbeeld is gekoppeld aan taken en Keuze 1 is geselecteerd in het aangepaste veld voor meerdere selecties, wordt in het berekende aangepaste veld de waarde Keuze 1 weergegeven. Als Keus 1 en Keuze 2 voor een verschillende taak worden geselecteerd, toont het berekende douanegebied de waarde &quot;Keus 1, Keuze 2&quot;.

1. Vervang &quot;Aangepast veld met meerdere selecties&quot; door de werkelijke naam van het aangepaste veld met meerdere selecties, zoals dit wordt weergegeven in Workfront.

   ![&#x200B; Berekende multi-uitgezochte gebied van de douane &#x200B;](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. (Facultatief) als multi-uitgezochte douanegebied reeds op deze vorm is en als deze vorm reeds in bijlage aan voorwerpen is, laat **toe van toepassing zijn op bestaande berekeningen** optie.

   Dit zorgt ervoor dat het nieuwe berekende veld automatisch wordt gevuld met de waarde uit het aangepaste veld voor meerdere selecties, aangezien dit veld wordt toegevoegd aan de formulieren die al aan de objecten zijn gekoppeld.

1. Klik **toepassen**.
1. Klik **sparen en Sluiten**.

   Het berekende aangepaste veld wordt toegevoegd aan het aangepaste formulier en als het formulier momenteel aan objecten is gekoppeld, wordt in het veld informatie uit het aangepaste veld met meerdere selecties ingevuld.

### Bouw een grafiek die verwijzingen een berekend douanegebied {#build-a-chart-that-references-a-calculated-custom-field}

1. (Facultatief) om ervoor te zorgen dat alle berekende gebieden die u door wilt in kaart brengen met waarden bevolkt zijn, van het lusje van Details van het rapport selecteert alle voorwerpen die de douanevorm met zowel het multi-uitgezochte douanegebied als het berekende douanegebied bevatten, dan klik **geeft** uit.
1. (Facultatief en voorwaardelijk) selecteer **opnieuw berekend het gebied van de Uitdrukkingen van de Douane**, dan klik **sparen Veranderingen**.\
   ![&#x200B; herberekenen douaneuitdrukkingen &#x200B;](assets/recalculate-custom-expressions-350x259.png)

   >[!NOTE]
   >
   >Deze optie is verwijderd uit het bulksgewijs bewerken van projecten.  U kunt uitdrukkingen voor projecten in massa nog opnieuw berekenen door **Meer** pictogram ![&#x200B; &#x200B;](assets/more-icon-45x33.png) bij de bovenkant van een projectlijst te klikken, toen **Uitdrukkingen** opnieuw berekenen.

1. Ga naar het rapport waar u de grafiek voor het berekende gebied wilt toevoegen dat multi-select douaneveld van verwijzingen voorziet.
1. Klik **de Acties van het Rapport**, dan **uitgeven**.

1. Selecteer het <strong> lusje van Groepen </strong>, dan klik <strong> groepering </strong> toevoegen.
1. Voeg het <strong> Berekende Multi uitgezochte Gebied </strong> toe u als uw groepering creeerde.
1. Selecteer het <strong> lusje van de Grafiek </strong>, en voeg een grafiek aan uw rapport toe.

   Bijvoorbeeld, kies a **Kolom** grafiek.
   <br> voor informatie over het toevoegen van een grafiek aan een rapport, zie de sectie <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref"> een grafiek aan een rapport </a> in het artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref"> een douanerapport </a> creëren.
1. Op het **Onderste (X) gebied van de As**, selecteer het <strong> Berekende Multi uitgezochte Gebied </strong> om in de grafiek te tonen.
1. Klik <strong> sparen + Sluiten </strong>.

   Het rapport toont de resultaten die door het Berekende Multi uitgezochte Gebied in een grafiek worden gegroepeerd.

   ![&#x200B; Multi uitgezochte gebied in grafiek &#x200B;](assets/chart-multi-select-field-column-chart-example.png)
