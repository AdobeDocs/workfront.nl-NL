---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: Een rapport in een diagram weergeven op basis van een aangepast veld met meerdere selecties
description: U kunt geen rapport door een multi-select douanegebied in kaart brengen. U moet een extra berekend gebied tot stand brengen dat naar het multi-uitgezochte douanegebied verwijst om het rapport door de waarde van het multi-uitgezochte gebied van de douane ook in kaart te brengen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# Een rapport in een diagram weergeven op basis van een aangepast veld met meerdere selecties

U kunt geen rapport door een multi-select douanegebied in kaart brengen. U moet een extra berekend gebied tot stand brengen dat naar het multi-uitgezochte douanegebied verwijst om het rapport door de waarde van het multi-uitgezochte gebied van de douane ook in kaart te brengen.

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
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

Voordat u begint, moet u een berekend aangepast veld maken waarin de waarden worden weergegeven die in het aangepaste veld voor meerdere selecties zijn geselecteerd. Zie voor meer informatie de [Een berekend aangepast veld maken dat verwijst naar een aangepast veld met meerdere selecties](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) in dit artikel.

## Een rapport weergeven op basis van meerdere geselecteerde aangepaste velden

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

U kunt geen grafiek in een rapport bouwen door naar een multi-select douanegebied van verwijzingen te verwijzen. In plaats daarvan kunt u een berekend veld maken waarmee de waarden van het aangepaste veld voor meerdere selecties voor een bepaald object en een bepaalde groep worden vastgelegd in het berekende veld. 

* [Een berekend aangepast veld maken dat verwijst naar een aangepast veld met meerdere selecties](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [Bouw een grafiek die verwijzingen een berekend douanegebied](#build-a-chart-that-references-a-calculated-custom-field)

### Een berekend aangepast veld maken dat verwijst naar een aangepast veld met meerdere selecties {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

U moet aan de volgende voorwaarden voldoen om een berekend veld te kunnen maken dat verwijst naar een aangepast veld met meerdere selecties:

* Maak het aangepaste veld voor meerdere selecties in een aangepast formulier.\
   Zie het artikel voor informatie over het maken van aangepaste formulieren en het toevoegen van aangepaste velden aan deze formulieren [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* Koppel het aangepaste formulier aan objecten.
* Vul het aangepaste veld voor meerdere selecties met een waarde voor elk object.

U kunt als volgt het berekende aangepaste veld bouwen dat verwijst naar het aangepaste veld voor meerdere selecties:

1. Een aangepast formulier maken of een bestaand formulier bewerken.\
   Zie het artikel voor informatie over het maken van aangepaste formulieren [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Selecteer het object of de objecten die u wilt gebruiken voor het aangepaste formulier.
1. Klikken **Veld toevoegen** vervolgens **Berekend** om het aangepaste veld voor meerdere selecties toe te voegen aan het formulier.

1. In de **Label** geeft u het nieuwe berekende veld een naam om aan te geven dat het naar het aangepaste veld voor meerdere selecties verwijst.\
   Bijvoorbeeld: &quot;Berekend multiselect veld.&quot;

1. In de **Berekening** voert u de volgende code in:

   ```
   {DE:Multi-select Custom Field}
   ```

1. Vervang &quot;Aangepast veld met meerdere selecties&quot; door de werkelijke naam van het aangepaste veld met meerdere selecties, zoals dit wordt weergegeven in Workfront.

   ![](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. (Optioneel) Als het aangepaste veld voor meerdere selecties al op dit formulier staat en als dit formulier al aan objecten is gekoppeld, schakelt u het selectievakje **Vorige berekeningen bijwerken** optie.\
   Zo wordt het nieuwe veld automatisch gevuld met de waarde van het aangepaste veld voor meerdere selecties, wanneer dit wordt toegevoegd aan de formulieren die al aan de objecten zijn gekoppeld.

1. Klikken **Gereed**.
1. Klikken **Opslaan +Sluiten**.

### Bouw een grafiek die verwijzingen een berekend douanegebied {#build-a-chart-that-references-a-calculated-custom-field}

1. (Optioneel) Als u wilt dat alle berekende velden waarop u een diagram wilt maken, gevuld zijn met waarden, selecteert u alle objecten in uw rapport die het aangepaste formulier bevatten met zowel het aangepaste veld voor meerdere selecties als het berekende aangepaste veld en klikt u vervolgens op **Bewerken**.
1. (Optioneel en voorwaardelijk) Schakel de optie **Aangepaste expressies opnieuw berekenen** veld, klik vervolgens op **Wijzigingen opslaan**.\
   ![](assets/recalculate-custom-expressions-350x259.png)

1. Ga naar het rapport waar u de grafiek voor het berekende gebied wilt toevoegen dat multi-select douaneveld van verwijzingen voorziet.
1. Klikken **Handelingen rapporteren** vervolgens **Bewerken**.

1. Selecteer <strong>Groepen</strong> tab, en klik vervolgens op <strong>Groepering toevoegen</strong>.
1. Voeg de<strong>Berekend veld voor meerdere selecties</strong> hebt u als groep gemaakt.
1. Selecteer <strong>Diagram</strong> en voeg een grafiek aan uw rapport toe.<br>Voor informatie over het toevoegen van een grafiek aan een rapport, zie de sectie <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Een diagram toevoegen aan een rapport</a> in het artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Een aangepast rapport maken</a>.
1. Selecteer <strong>Berekend veld voor meerdere selecties</strong> als een van de velden die in het diagram moeten worden weergegeven.
1. Klikken <strong>Opslaan + Sluiten</strong>.<br>Het rapport toont de resultaten die door het Berekende Multi-uitgezochte Gebied in een grafiek worden gegroepeerd.
