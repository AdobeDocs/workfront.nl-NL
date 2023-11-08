---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: tijd- en datumverschillen berekenen'
description: Bouw een mening die het verschil tussen twee datumgebieden op een voorwerp of tussen een datumgebied op een voorwerp en een ander datumgebied op het oudervoorwerp toont.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
source-git-commit: 324ad45b52dafa96c2854f1fec1172b88643bdc2
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Weergave: tijd- en datumverschillen berekenen

>[!IMPORTANT]
>
>U kunt het tijd- en datumverschil in Adobe Workfront niet berekenen tussen twee verschillende objecten van dezelfde soort. U kunt bijvoorbeeld het tijd- en datumverschil niet berekenen tussen twee datums voor twee verschillende projecten, taken of problemen.

U kunt het verschil tussen het volgende berekenen:

* Het tijd- en datumverschil tussen twee datumvelden op hetzelfde object
* Het tijd- en datumverschil tussen het veld op een object en een ander veld op het bovenliggende object

>[!TIP]
>
>Deze berekeningen geven het aantal dagen tussen de twee datums aan. Het resultaat wordt in dagen weergegeven. Er wordt ook rekening gehouden met de tijdstempel in het datumveld en het aantal dagen kan worden gevolgd door decimalen als de tijdstempels niet overeenkomen. Als de taak te laat is voltooid, wordt het aantal dagen weergegeven als een negatieve waarde.

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
   <td> <p>Verzoek om een weergave te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Het tijd- en datumverschil berekenen tussen twee datumvelden op hetzelfde object

U kunt bijvoorbeeld het verschil berekenen tussen de Geplande Voltooiingsdatum en de Werkelijke Voltooiingsdatum van een taak.

![](assets/view-planned-actual-completion-dates-datediff-column-350x92.png)

1. Ga naar een takenlijst.
1. Van de **Weergave** vervolgkeuzelijst, klikt u op **Nieuwe weergave**.

1. Klikken **Kolom toevoegen** en typ &quot;Geplande afsluitdatum&quot; in het dialoogvenster **Tonen in deze kolom** selecteert u het veld wanneer het in de lijst wordt weergegeven.

1. Klikken **Kolom toevoegen** en typ &quot;Datum van daadwerkelijke voltooiing&quot; in het dialoogvenster **Tonen in deze kolom** selecteert u het veld wanneer het in de lijst wordt weergegeven.

1. Klikken **Kolom toevoegen** en klik vervolgens op **Overschakelen naar tekstmodus**.

1. Houd de cursor boven het gebied van de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:

   ```
   displayname=Planned-Actual Completion Date<br>linkedname=direct<br>querysort=plannedCompletionDate<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)<br>valueformat=HTML
   ```

1. Klikken **Opslaan** vervolgens **Weergave opslaan**.

## Het tijd- en datumverschil berekenen tussen het veld op een object en een ander veld op een bovenliggend object

Voor een lijst met objecten en hun bovenliggende elementen raadpleegt u de sectie &#39;Interdependentie en hiërarchie van objecten begrijpen&#39; in [Objecten in Adobe Workfront begrijpen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
Bijvoorbeeld, kunt u het verschil tussen de Geplande Datum van Voltooiing van een taak en de Geplande Datum van Voltooiing van zijn oudertaak, of van het project berekenen dat de taak is.

![](assets/view-project-planned-task-planned-completion-dates-datediff-column-350x184.png)

1. Ga naar een takenlijst.
1. Van de **Weergave** vervolgkeuzelijst, klikt u op **Nieuwe weergave**.

1. Klikken **Kolom toevoegen** en typ &quot;&quot;Geplande Voltooiingsdatum van project&quot; of &quot;Bovenliggende Voltooiingsdatum&quot; in het dialoogvenster **Tonen in deze kolom** selecteert u het veld wanneer het in de lijst wordt weergegeven.

1. Klikken **Kolom toevoegen** en typ &quot;Geplande afsluitdatum&quot; in het dialoogvenster **Tonen in deze kolom** selecteert u het veld wanneer het in de lijst wordt weergegeven.

1. Klikken **Kolom toevoegen** en klik vervolgens op **Overschakelen naar tekstmodus**.

1. Houd de cursor boven het gebied van de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervangt het door een van de volgende codes:

   * U kunt als volgt het verschil weergeven tussen de geplande uitvoeringsdatum van het project en die van de taak:

     ```
     displayname=Project Planned Completion - Task Planned Completion (Days)<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>valueformat=HTML
     ```

   * U kunt als volgt het verschil weergeven tussen de geplande voltooiingsdatum van de bovenliggende taak en die van de taak:

     ```
     valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>textmode=true<br>valueformat=HTML<br>displayname=Parent Planned Completion - Planned Completion (Days)
     ```

1. Klikken **Opslaan** vervolgens **Weergave opslaan**.
