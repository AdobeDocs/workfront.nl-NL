---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Projecten importeren naar plannen in het scenario Scenario Planner
description: U kunt bestaande projecten in een plan invoeren. De geïmporteerde projecten worden omgezet in initiatieven en u kunt ze binnen het plan beheren zoals u een nieuw initiatief zou beheren. Het oorspronkelijke project blijft gekoppeld aan het nieuwe initiatief.
author: Alina
feature: Workfront Scenario Planner
exl-id: 20429bb1-c158-433b-9790-325cd577248e
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1594'
ht-degree: 0%

---

# Projecten importeren naar plannen in de [!DNL Scenario Planner]

U kunt bestaande projecten in een plan invoeren. De geïmporteerde projecten worden omgezet in initiatieven en u kunt ze binnen het plan beheren zoals u een nieuw initiatief zou beheren. Het oorspronkelijke project blijft gekoppeld aan het nieuwe initiatief.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: add information about what happens when you import projects and where the info from projects show up;</p>
<p>- the hours/ FTE come from WorkPerDay</p>
<p>- if a task has a Duration of 0, the FTE should be 0 for that asignee but it should still come across) </p>
</div>
-->

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] package</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>OPMERKING</b></p>
<p>Neem contact op met uw Workfront-vertegenwoordiger als u een ander Workfront-pakket hebt.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licentie</p> </td> 
   <td> <p>[!UICONTROL Light] of hoger</p> 
   <p>[!UICONTROL Review] of hoger</p> </td> 
  </tr> 
    <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>[!UICONTROL Edit] toegang tot de [!DNL Scenario Planner]</p> <p>De mening of hogere toegang tot Projecten.</p></td> 
  </tr> 
  <tr> 
   <td> <p>Objectmachtigingen </p> </td> 
   <td> <p>[!UICONTROL Manage] machtigingen voor een abonnement</p> <p>Bekijk of hoger toestemmingen aan projecten.</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie over toegang tot de Planner van het Scenario, zie [&#x200B; Toegang nodig om  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md) te gebruiken.

Voor informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang tot de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> <p>View or higher access to Projects.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>View or higher permissions to projects.</p><p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements to Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Overwegingen over het invoeren van projecten in plannen als nieuwe initiatieven

* U moet projecten creëren alvorens u hen in een plan als nieuwe initiatieven kunt invoeren.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: no caveats for project statuses yet, mentioned in the import steps as a tip) </p>
  -->

* U moet minstens [!UICONTROL View] toestemmingen aan de projecten hebben om hen in een plan als nieuw initiatief te kunnen invoeren.
* U kunt het zelfde project in veelvoudige plannen invoeren.
* Voor de projecten die u wilt importeren, moeten datums zijn opgenomen in het tijdsbestek van uw abonnement. U kunt geen projecten importeren met een [!UICONTROL Planned Completion Date] eerdere datum dan het begin van het abonnement of een [!UICONTROL Planned Start Date] later dan het einde van het abonnement.
* U kunt niet meer dan 100 projecten tegelijk importeren.
* Sommige projectinformatie wordt ook ingevoerd in het plan en wordt initiatiefinformatie. Voor informatie over welke projectinformatie in het plan wordt ingevoerd en initiatiefinformatie wordt, zie de [&#x200B; informatie van het Project die in de plan &#x200B;](#project-information-imported-into-the-plan) sectie in dit artikel wordt ingevoerd.
* Wijzigingen in de gekoppelde projecten hebben geen invloed op de initiatieven in het plan.
* Wijzigingen die worden aangebracht in de initiatieven op het plan hebben niet automatisch invloed op de gekoppelde projectwijzigingen die worden aangebracht in het initiatief, maar zijn alleen van invloed op de gekoppelde projecten wanneer u het initiatief publiceert vanuit het plan. Voor informatie over hoe het publiceren van initiatieven de verbonden projecten beïnvloedt, zie [&#x200B; Update of creeer projecten door initiatieven in  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) te publiceren.
* Als u een initiatief verwijdert dat is gemaakt door een project te importeren, wordt het project niet verwijderd.
* Als u een project verwijdert dat verband houdt met een initiatief, wordt het initiatief niet verwijderd.

## In het plan geïmporteerde projectgegevens {#project-information-imported-into-the-plan}

Wanneer u een project in een plan invoert wordt sommige projectinformatie ook ingevoerd in het plan en het wordt initiatiefinformatie. De volgende lijst toont welke projectinformatie initiatiefinformatie wordt wanneer u een project in een plan invoert:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add what happens if you import a 5 year project to a 1 year plan - how does this display?) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Projectinformatie</td> 
   <td>Initiatiefinformatie </td> 
  </tr> 
  <tr> 
   <td>Projectnaam</td> 
   <td>Initiatiefnaam</td> 
  </tr> 
  <tr> 
   <td>Geplande data van project</td> 
   <td> <p>Initiatief begint en eindigt maanden.</p> <p>Als een project in het midden van een maand begint of eindigt, worden de ingevoerde data uitgebreid tot een volledige maand in het plan. Als de geplande projectdata bijvoorbeeld 20 maart - 5 mei 2020 zijn, zijn de data van het geïmporteerde initiatief maart - mei 2020.</p> <p>Indien de geplande begin- of einddatum langer is dan de looptijd van het plan, is er een visuele indicatie dat het ingevoerde initiatief begint of eindigt na het plan. </p> </td> 
  </tr> 
  <tr> 
   <td>Functie-rollen toegewezen aan taken en problemen</td> 
   <td> <p>De Rollen van de Baan van het initiatief. </p> <p>Opmerking:   <p>Als een gebruiker rollen tijdens het leven van het project verandert, hangen de rollen die van de status van de taak af wanneer u het project invoert. De volgende scenario's bestaan:</p> 
     <ul> 
      <li> <p>Als een gebruiker die aan een taak of een kwestie is toegewezen zijn rol veranderde nadat zij hun taak als [!UICONTROL Done] merkten, voert [!DNL Workfront] in het initiatief de rol in die de gebruiker vervulde alvorens zij de taak als [!UICONTROL Done] merkten.</p> </li> 
      <li> <p>Als een gebruiker die aan een taak of kwestie wordt toegewezen de rol tijdens het leven van het project veranderde maar hun taak op de taak of de kwestie niet duidelijk als [!UICONTROL Done] wanneer u het project invoert, [!DNL Workfront] voert slechts de huidige rol van de toegewezen gebruiker in. </p> </li> 
     </ul> <p>Voor informatie over het statuut van een taak, zie "Status van de Toewijzing"in <a href="../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref"> Verklarende woordenlijst van Adobe [!DNL Workfront] terminologie </a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Project [!UICONTROL Planned Hours] gekoppeld aan taakrollen die zijn toegewezen aan taken of problemen</td> 
   <td> <p><span> afhankelijk van of het plan opstelling is om FTEs of uren te gebruiken, wordt [!UICONTROL Planned Hours] van de taken op het project of </span> [!UICONTROL Required FTEs] <span> of [!UICONTROL Required hours] op het plan </span>. </p> <p>Voor informatie over vestiging een plan om FTEs of uren te gebruiken, zie <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref"> plannen in [!DNL Scenario Planner]</a> creëren en uitgeven. </p> <p>Overweeg het volgende:</p> 
    <ul> 
     <li> <p>[!DNL Workfront] gebruikt de baanrollen die aan taken en kwesties worden toegewezen of de baanrollen die de gebruikers aan taken of kwesties worden toegewezen met betrekking tot het project worden geassocieerd en hen naar het nieuwe initiatief als Vereiste Rollen van de Baan overbrengt. </p> </li> 
     <li> <p>Wanneer het plan opstelling is om FTEs te gebruiken, worden de Geplande Uren verbonden aan de baanrollen op de taken en de kwesties van het project eerst omgezet in FTE. Deze VTE wordt vervolgens toegewezen aan de functie van het initiatief. <span> Geplande Uren worden gelijkelijk verdeeld in [!DNL Workfront]. Als een taak of een kwestie veelvoudige maanden overspant, wordt het bedrag van Geplande Uren voor elke maand in de duur van het initiatief omgezet in maandelijkse VTE en overgebracht naar elke maand van het initiatief.</span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b> Voorbeeld: </b></span></span> <span> bijvoorbeeld, als een taak aan een baanrol voor 80 Geplande Uren in September wordt toegewezen, dan toont de ingevoerde baanrol 0.5 FTE voor het initiatief in September.</span> </p> </li> 
     <li> <p>[!DNL Workfront] berekent de FTE van de vereiste functies van de Taak verbonden aan het initiatief gebruikend de volgende formule:</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>Tip: de [!DNL Scenario Planner] gaat ervan uit dat er 160 werkuren per maand zijn.</p> <p>Als een project bijvoorbeeld een duur van 1200 minuten heeft en een functie voor het project is gekoppeld aan 600 minuten geplande uren, is de FTE 0,5. Bij het importeren van het project is de vereiste taakrol FTE voor het nieuwe initiatief 0,5 voor elke maand van het initiatief. </p> </li> 
     <li>Wanneer een baanrol aan een taak op het project met nul Geplande Uren wordt toegewezen, is de Vereiste VTE voor de baanrol van het initiatief door gebrek nul. <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         (NOTE: this used to be 1, not zero in Production) 
       </MadCap:conditionalText>
      --></li> 
     <li>Wanneer een baanrol aan een taak op het project met nul [!UICONTROL Duration] wordt toegewezen, Vereiste VTE <span> of uren </span> voor de baanrol van het initiatief is nul door gebrek, zelfs als de taak Uren geplant heeft. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Projecten in een plan importeren

>[!IMPORTANT]
>
>Na het invoeren van projecten in een plan, worden zij initiatieven op het plan. Hoewel de twee items aan elkaar zijn gekoppeld, bestaan ze als onafhankelijke entiteiten en hebben ze niet automatisch invloed op elkaar wanneer ze worden bijgewerkt.
>
>Het volgende gebeurt:
>
>* Wijzigingen in het project hebben nooit invloed op het initiatief nadat u het project in het plan hebt geïmporteerd. Deze wijzigingen omvatten wijzigingen in de taakrollentoewijzingen.
>* Wijzigingen in het initiatief zijn alleen van invloed op de informatie in het gebied [!DNL Scenario Planner] over het project als u het initiatief publiceert naar het bijbehorende project. Anders hebben ze geen invloed op de [!UICONTROL Planned Hours] -informatie voor de taken en problemen van het project.
>
>  Voor informatie over hoe het publiceren van initiatieven de verbonden projecten beïnvloedt, zie [&#x200B; Update of creeer projecten door initiatieven in de Planner van het Scenario te publiceren &#x200B;](../scenario-planner/publish-scenarios-update-projects.md).

{{step1-to-scenario-planner}}

1. Klik op de naam van een abonnement waarin u projecten wilt importeren.
1. Klik op **[!UICONTROL New Initiative]** en vervolgens op **[!UICONTROL Import Projects]** .

   Het vak [!UICONTROL Import Projects] wordt weergegeven. Projecten met datums die zijn opgenomen in het tijdkader van uw abonnement, worden in een lijst weergegeven.

   ![&#x200B; de projecten van de Invoer &#x200B;](assets/project-import-ui-projects-selected-350x72.png)

   >[!TIP]
   >
   >Projecten in om het even welke statusvertoning in de lijst.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the status of the projects in the import projects UI might change; right now it's ALL statuses)</p>
   -->

1. (Facultatief) klik het **[!UICONTROL Filter icon]** ![&#x200B; pictogram van de Filter &#x200B;](assets/filter-nwepng.png) en selecteer een beschikbare filter van de lijst om de hoeveelheid projecten op uw lijst te verminderen. Door gebrek, wordt de lijst van projecten gefiltreerd door de momenteel geselecteerde projectfilter van de gebruiker in een lijst van projecten.

1. (Facultatief) klik het **[!UICONTROL Search icon]** ![&#x200B; pictogram van het Onderzoek &#x200B;](assets/search-icon.png) en voeg een sleutelwoord toe dat op om het even welk gebied op het scherm wordt getoond. De items met het zoekwoord worden automatisch in de lijst weergegeven en alle items worden verborgen.

1. (Voorwaardelijk) klik **[!UICONTROL X icon]** om het onderzoek te verwijderen en alle projecten te tonen.
1. Selecteer maximaal 100 projecten en klik op **[!UICONTROL Import]** .

   De projecten worden geïmporteerd als nieuwe initiatieven.

   Let op het volgende:

   * Een pictogram van het projectpictogram ![&#x200B; van het Project &#x200B;](assets/project-icon-sp.png) toont rechts van de initiatiefnaam.
   * Als het projecttijdschema de looptijd van het plan overschrijdt, eindigt de balk van het initiatief met een puntige marge naar links (wanneer de begindatum eerder is dan de datum van het plan) of naar rechts (wanneer de einddatum later is dan de datum van het plan).

     ![&#x200B; bar van het Project vroeger dan begindatum &#x200B;](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)

   * Het aantal maanden en de functies zijn bijgewerkt en aangepast aan die van het project.

   >[!TIP]
   >
   >De kosten in verband met de functies worden op initiatiefniveau bijgewerkt en worden niet uit het project geïmporteerd.

1. Klik op de balk die het nieuwe initiatief voorstelt om het deelvenster met initiatiefdetails rechts te openen.

   ![&#x200B; Duur van het Initiatief &#x200B;](assets/initiative-duration-with-project-duration-details-panel-350x292.png)

   Controleer de volgende informatie in het gebied **[!UICONTROL Initiative Duration]** :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Duration]</td> 
      <td>Dit is de duur van het initiatief in maanden. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative]</td> 
      <td>De begin- en einddatum van het initiatief. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Project]</td> 
      <td> <p>De [!UICONTROL Planned Start] en [!UICONTROL Completion dates] van het gekoppelde project.</p> <p>Tip: als de [!UICONTROL Project] -informatie ontbreekt, is het project verwijderd.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Bewerk de naam van het initiatief. Standaard komt deze overeen met de naam van het project.
1. (Optioneel) Voer een van de volgende handelingen uit:

   * Taken bijwerken in de sectie **[!UICONTROL Required Job Roles]**
   * De **[!UICONTROL Fixed Costs]** in de **[!UICONTROL Costs]** -sectie bijwerken

   * Klik op **[!UICONTROL Update available job roles]** of **[!UICONTROL Update available budget]** om conflicten op te lossen tussen het nieuwe initiatief en andere initiatieven in het plan.

1. (Voorwaardelijk) Klik **[!UICONTROL Apply]** om de wijzigingen in uw initiatief op te slaan.
1. Klik op **[!UICONTROL Save Plan]** om de wijzigingen in uw abonnement op te slaan.
1. (Optioneel) Als u de wijzigingen die u in het initiatief aanbrengt, wilt bijwerken naar het project waaruit het is geïmporteerd, publiceert u het project uit het plan. Voor informatie over het publiceren van plannen, zie [&#x200B; Update of creeer projecten door initiatieven in  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) te publiceren.
1. (Optioneel) Klik op het projectpictogram om het gekoppelde project te openen.

   ![&#x200B; pictogram van het Project op initiatief &#x200B;](assets/project-icon-on-initiative-highlighted-350x49.png)
