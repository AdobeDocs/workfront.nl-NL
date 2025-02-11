---
product-area: agile-and-teams
navigation-topic: iterations
title: Een herhaling maken
description: Herhalingen vormen een sleutelcomponent voor de ploegen van de Trommel in het plannen van het werkcapaciteit. [!DNL Adobe Workfront]  staat de rumoer teams toe om hun werk te beheren door veelvoudige herhalingen te creëren om teambehoeften aan te passen.
author: Lisa
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: 6ae8e48361114e897d0be83ae81f8344074a5ec2
workflow-type: tm+mt
source-wordcount: '992'
ht-degree: 0%

---

# Een herhaling maken

Herhalingen vormen een sleutelcomponent voor de ploegen van de Trommel in het plannen van het werkcapaciteit. Met [!DNL Adobe Workfront] kunnen teams van het type Scrum agile hun werk beheren door meerdere versies te maken die voldoen aan de teambehoeften.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> <p>Nieuw: [!UICONTROL Light] of hoger</p> 
   of
   <p>Huidig: [!UICONTROL Review] of hoger</p> </td> 
  </tr>
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een herhaling toevoegen

U kunt een herhaling in de lijst toevoegen om snel een herhaling te maken en er later taken en problemen aan toe te voegen.

{{step1-to-team}}

1. (Facultatief) klik het **[!UICONTROL Switch team]** pictogram van de pictogram ![ Schakelaar teampictogram ](assets/switch-team-icon.png), dan of selecteer een nieuw team van het Trommel van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

1. Klik op het tabblad **[!UICONTROL Iterations]** op **[!UICONTROL Add iteration]** .

   ![ klik toevoegen herhaling ](assets/click-add-iteration.png)

1. Geef het volgende op:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Iteration Name]</strong></td> 
      <td>Voer de naam van de herhaling in.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Goal]</strong></td> 
      <td>Voeg om het even welke doelstellingen toe u voor de herhaling hebt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Start Date]</strong></td> 
      <td>Voer de datum in waarop de herhaling moet worden gestart.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL End Date]</strong></td> 
      <td><p>Voer de datum in waarop de herhaling moet worden beëindigd. [!DNL Workfront] raadt u aan een einddatum in te stellen die niet langer mag zijn dan 4 weken na de begindatum.</p><p>Tip: kies een werkdag als einddatum. In de uitbouwgrafiek worden slechts werkdagen gebruikt voor de berekeningen.<br> door gebrek, gebruikt het burndown diagram het standaardprogramma om werkdagen (zoals die in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref"> worden beschreven leidt tot een programma </a>) te bepalen. Of, om team-specifieke niet-werkdagen op te nemen, kunnen de mobiele teams verkiezen om een afwisselend programma (zoals die in "het Bepalen van een Afwisselend Programma van het Team voor Grafieken"in <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref"> wordt beschreven creëren een flexibel team </a>) te gebruiken.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Geef de capaciteit voor de herhaling op. Dit is het aantal punten of uren uw team in de herhaling kan verwezenlijken. Het getal dat u invoert, moet gelijk zijn aan of groter zijn dan het aantal punten of uren vanaf de som van alle artikelen in de herhaling.<br>[!DNL Workfront] vult dit veld standaard vooraf met 50 capaciteit. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Geef het focuspercentage van het team op. Als alle leden van het team zich volledig op deze herhaling zullen richten, zou de nadruk 100% zijn.<br>[!DNL Workfront] vult dit veld standaard voor 100% in. </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik op **[!UICONTROL Add iteration]**. Nu je een herhaling hebt gemaakt, moet je verhalen toevoegen. Voor meer informatie, zie [ verhalen aan een bestaande herhaling ](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) toevoegen.

## Een herhaling plannen op het tabblad [!UICONTROL Backlog]

Gebruik de functie [!UICONTROL Plan Iteration] om een herhaling te maken met behulp van taken op uw achterstand.

{{step1-to-team}}

1. (Facultatief) klik het **[!UICONTROL Switch team]** pictogram van de pictogram ![ Schakelaar teampictogram ](assets/switch-team-icon.png), dan of selecteer een nieuw team van het Trommel van het drop-down menu of onderzoek naar een team in de onderzoeksbar.

1. Selecteer **[!UICONTROL Backlog]** in het linkerdeelvenster. Klik vervolgens op **[!UICONTROL Plan Iteration]** .

1. Geef de volgende informatie op:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Iteration Name]</strong></td> 
      <td>Geef een naam voor de herhaling op.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Start Date]</strong></td> 
      <td> Geef de datum op waarop de herhaling moet worden gestart.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL End Date]</strong> </td> 
      <td><p>Geef de datum op waarop de herhaling moet worden beëindigd. [!DNL Workfront] raadt u aan een einddatum in te stellen die niet langer mag zijn dan 4 weken na de begindatum.</p><p>Tip: kies een werkdag als einddatum. In de uitbouwgrafiek worden slechts werkdagen gebruikt voor de berekeningen.<br> door gebrek, gebruikt het burndown diagram het standaardprogramma om werkdagen (zoals die in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref"> worden beschreven leidt tot een programma </a>) te bepalen. Of, om team-specifieke niet-werkdagen op te nemen, kunnen de mobiele teams verkiezen om een afwisselend programma (zoals die in <a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md" class="MCXref xref"> wordt beschreven Gebruik een afwisselend teamprogramma voor burndown grafieken </a>) te gebruiken.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Geef het focuspercentage van het team op. Als alle leden van het team zich volledig op deze herhaling zullen richten, zou de nadruk 100% zijn.<br>[!DNL Workfront] vult dit veld vooraf in met de gemiddelde waarde van eerdere herhalingen van uw team. Als dit de eerste herhaling van uw team is, is deze veldwaarde standaard 0.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Geef de capaciteit voor de herhaling op. Dit is het aantal punten of uren uw team in de herhaling kan verwezenlijken. Het getal dat u invoert, moet gelijk zijn aan of groter zijn dan het aantal punten of uren vanaf de som van alle artikelen in de herhaling.<br>[!DNL Workfront] vult dit veld vooraf in met de gemiddelde waarde van eerdere herhalingen van uw team. Als dit de eerste herhaling van uw team is, is deze veldwaarde standaard 0.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Goal]</strong></td> 
      <td> Geef een doel voor de herhaling op. Dit veld is niet verplicht.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Selecteer artikelen om deze nu aan de herhaling toe te voegen. U kunt deze stap ook overslaan en op een later tijdstip artikelen aan een herhaling toevoegen. De verhalen boven aan de achterstand hebben een hogere prioriteit. Artikelen worden groen gemarkeerd als ze in de capaciteit passen; ze worden rood gemarkeerd als ze dat niet doen.
U kunt zowel taken als uitgaven toevoegen aan één herhaling:

   * **om taken aan de herhaling toe te voegen:** op het **[!UICONTROL Backlog]** lusje, zorg ervoor dat het **[!UICONTROL Stories]** lusje wordt geselecteerd (dit lusje wordt geselecteerd door gebrek wanneer het bekijken van de achterstand). Selecteer de artikelen die u aan de herhaling wilt toevoegen.

     Wanneer u taken aan een herhaling toevoegt, wordt de begindatum van de taak berekend zoals die in [[!UICONTROL Understand] wordt beschreven hoe de datums van de taakbegin wanneer toegevoegd aan een herhaling ](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration) worden berekend.

   * **om kwesties aan de herhaling toe te voegen:** op het **[!UICONTROL Backlog]** lusje, klik **[!UICONTROL Issues]** tabel. Selecteer de kwesties u aan de herhaling wilt toevoegen.

1. Klik op **[!UICONTROL Save].**
De herhaling wordt gemaakt.

1. (Facultatief) om verhalen aan een bestaande herhaling toe te voegen, zie [ verhalen aan een bestaande herhaling ](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) toevoegen.

## Begrijp hoe de datums van de taakbegin wanneer toegevoegd aan een herhaling worden berekend {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

Wanneer u een taak als een artikel toevoegt aan een herhaling, wordt de beperking [!UICONTROL Must Finish On task] gebruikt voor elk artikel. In de meeste gevallen wordt de geplande begindatum van de taak berekend op basis van de volgende formule:

[!UICONTROL Iteration End Date] minus (-) [!UICONTROL Task Duration] is gelijk aan (=) [!UICONTROL Task Planned Start Date]

[!UICONTROL Project End Date] wordt gebruikt in plaats van de Einddatum van de Interferatie als de begindatum van het project na de begindatum van de iteratie is, en de einddatum van het project is na de einddatum van de herhaling.

U kunt de individuele teams van het Trommel vormen om de projectdata door gebrek, eerder dan de herhalingsdata te gebruiken. Voor informatie, zie de sectie [ vormen hoe de data worden toegepast wanneer het toevoegen van het werkpunten aan een herhaling ](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) in artikel [ Scrum ](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md) vormt.
