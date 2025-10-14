---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: Verschillen in tijd en datum berekenen'
description: Leer tijd- en datumverschillen te berekenen.
author: Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 0%

---

# Weergave: tijd- en datumverschillen berekenen

<!-- Audited: 11/2024 -->

>[!IMPORTANT]
>
>U kunt het tijd- en datumverschil in Adobe Workfront niet berekenen tussen twee verschillende objecten van dezelfde soort. U kunt bijvoorbeeld het tijd- en datumverschil niet berekenen tussen twee datums voor twee verschillende projecten, taken of problemen.

U kunt het verschil tussen het volgende berekenen:

* Het tijd- en datumverschil tussen twee datumvelden op hetzelfde object
* Het tijd- en datumverschil tussen een veld op een object en een ander veld op het bovenliggende object

>[!TIP]
>
>Deze berekeningen geven het aantal dagen tussen de twee datums aan. Het resultaat wordt in dagen weergegeven. Er wordt ook rekening gehouden met de tijdstempel in het datumveld en het aantal dagen kan worden gevolgd door decimalen als de tijdstempels niet overeenkomen. Als de taak te laat is voltooid, wordt het aantal dagen weergegeven als een negatieve waarde.

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
   <td> <p>Nieuw: </p><ul><li><p>Medewerker om een weergave te wijzigen </p></li><li>
   <p>Standaard voor het wijzigen van een rapport</p></li></ul><p>of</p><p>Huidige:</p><ul><li><p>Verzoek om een weergave te wijzigen </p></li><li>
   <p>Plan om een rapport te wijzigen</p> </li><ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Het tijd- en datumverschil berekenen tussen twee datumvelden op hetzelfde object

U kunt bijvoorbeeld het verschil berekenen tussen de Geplande Voltooiingsdatum en de Werkelijke Voltooiingsdatum van een taak.

![&#x200B; de datumverschil van de Mening &#x200B;](assets/view-planned-actual-completion-dates-datediff-column-new.png)

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Mening**, klik **Nieuwe Mening**.

1. Klik **toevoegen Kolom** en beginnen &quot;Geplande Datum van de Voltooiing&quot;in **tonen in dit kolom** gebied dan selecteren het wanneer het in de lijst toont.

1. Klik **toevoegen Kolom** en beginnen &quot;Ware Datum van de Voltooiing&quot;in **tonen in dit kolom** gebied dan selecteren het wanneer het in de lijst toont.

1. Klik **toevoegen Kolom**, dan klik **Schakelaar aan de Wijze van de Tekst**.

1. Beweeg over het gebied van de tekstwijze, en klik **Klik om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:

   ```
    displayname=Planned-Actual Completion Date
    linkedname=direct
    querysort=plannedCompletionDate
    textmode=true
    valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)
    valueformat=HTML
   ```

1. Klik **sparen**, dan **sparen Mening**.

## Het tijd- en datumverschil berekenen tussen het veld op een object en een ander veld op een bovenliggend object

Voor een lijst van voorwerpen en hun ouders, zie het &quot;Begrijpen van de Interdependentie en de Hiërarchie van de sectie van Objecten&quot;in [&#x200B; voorwerpen in Adobe Workfront &#x200B;](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) begrijpen.\
Bijvoorbeeld, kunt u het verschil tussen de Geplande Datum van Voltooiing van een taak en de Geplande Datum van Voltooiing van zijn oudertaak, of van het project berekenen dat de taak is.

![&#x200B; Mening gepland verschil van de voltooiingsdatum &#x200B;](assets/view-project-planned-task-planned-completion-dates-datediff-column-new.png)

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Mening**, klik **Nieuwe Mening**.

1. Klik **toevoegen Kolom** en beginnen &quot;Project Geplande Datum van de Voltooiing&quot;of &quot;Ouder Datum van de Voltooiing&quot;in **tonen in dit kolom** gebied dan selecteren het wanneer het in de lijst toont.

1. Klik **toevoegen Kolom** en beginnen &quot;Geplande Datum van de Voltooiing&quot;in **tonen in dit kolom** gebied dan selecteren het wanneer het in de lijst toont.

1. Klik **toevoegen Kolom**, dan klik **Schakelaar aan de Wijze van de Tekst** > **geeft de Wijze van de Tekst** uit.
1. Verwijder de tekst u in **vindt geef de Wijze van de Tekst** vakje uit, en vervang het met één van de volgende codes:

   * U kunt als volgt het verschil weergeven tussen de geplande uitvoeringsdatum van het project en die van de taak:

     ```
      displayname=Project Planned Completion - Task Planned Completion (Days)
      textmode=true
      valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)
      valueformat=HTML
     ```

   * U kunt als volgt het verschil weergeven tussen de geplande voltooiingsdatum van de bovenliggende taak en die van de taak:

     ```
      valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)
      textmode=true<br>valueformat=HTML
      displayname=Parent Planned Completion - Planned Completion (Days)
     ```

1. Klik **Gedaan**, dan **sparen Mening**.
