---
title: Rapport over het gebied Updates
description: Het rapport Dagboekingang bevat systeemupdates van het gebied Updates van projecten, taken, problemen en andere objecten die voorheen alleen beschikbaar waren via de Adobe Workfront API. Hoewel dit een geavanceerd rapport is dat is bedoeld voor specifieke gebruiksgevallen, maakt het verteerbaardere formaat het voor u gemakkelijker om over projectactiviteit en systeemupdates binnen Workfront te rapporteren.
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: ecf947ce-54d8-4103-8903-f455b1d86c39
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '2738'
ht-degree: 0%

---

# Rapport over het gebied Updates

Het rapport Dagboekingang bevat systeemupdates van het gebied Updates van projecten, taken, problemen en andere objecten die voorheen alleen beschikbaar waren via de Adobe Workfront API. Hoewel dit een geavanceerd rapport is dat is bedoeld voor specifieke gebruiksgevallen, maakt het verteerbaardere formaat het voor u gemakkelijker om over projectactiviteit en systeemupdates binnen Workfront te rapporteren.

>[!TIP]
>
>Het rapport van de Ingang van het Dagboek bevat slechts systeemupdates van het gebied van Updates van voorwerpen. Als u opmerkingen wilt rapporteren die nog in het gedeelte Updates staan, moet u het notitierapport gebruiken.\
>Voor meer informatie over het verslag van de Nota, zie [ Mening alle updates in een Nota- rapport ](../../../workfront-basics/updating-work-items-and-viewing-updates/view-all-updates-in-a-report.md). ‍

Het rapport van de Ingang van het Dagboek kan tonen:

* Aantal statuswijzigingen
* Wanneer een taak of kwestie werd geschrapt
* De manier waarop waarden in belangrijke aangepaste velden zijn gewijzigd tijdens de levenscyclus van een project
* Welke belangrijke data zijn veranderd tijdens de levenscyclus van een project
* Als de eigenaar van een project is gewijzigd

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
   <td> <p>Nieuw: Standaard </p><p>of </p><p>Huidig: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening aan de voorwerpen die de dagboekingangen bevatten u in het rapport toont</p> <p>Nadat u het rapport hebt gemaakt, ontvangt u beheerdersmachtigingen voor het rapport</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Voordat u de in dit artikel beschreven handelingen kunt uitvoeren, moet u het volgende controleren:

* Alle velden waarvoor je een melding wilt maken, worden bijgehouden in Workfront. U kunt alleen gegevens rapporteren in het gebied Updates dat wordt bijgehouden.

  Leren hoe te om gebieden toe te voegen die u Workfront wilt volgen, zie [ systeemupdates ](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md) vormen.

* Om het even welke douanegebieden die u wilt melden hebben de plaatsende **veranderingen van het het gebiedsgebied van de Vertoning in toegelaten updatevoer**.

## Overzicht van het Dagboekingrapport

Omdat het rapport van de Ingang van het Dagboek systeemupdates vraagt, kan het een significant aantal resultaten terugkeren. Om deze reden, adviseren wij dat u aan specifiek voorwerp-zoals projecten, programma&#39;s, portefeuilles, groepen, etc.-wanneer het creëren van het rapport filtreert.

Om meer over de verschillende objecten types in Workfront te leren, zie [ voorwerpen in Adobe Workfront ](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) begrijpen.

>[!NOTE]
>
>Omdat het rapport van de Ingang van het Dagboek zo veel gegevens terugkeert, wordt het uitvoeren en de geplande rapportlevering niet gesteund.

De standaardmening voor dit rapport bevat de volgende kolommen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Veld</th> 
   <th>Toelichting</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong> Naam van het Gebied </strong> </td> 
   <td> <p><span style="font-weight: normal;"> de naam van het beïnvloede gebied. Afhankelijk van hoe u opstelling het rapport, deze kolom Status, identiteitskaart van de Eigenaar, de Naam van de Taak, Geplande Datum van de Voltooiing, of andere gebieden kon bevatten.</span> </p> <p><span style="font-weight: normal;"> wanneer </span> <strong> DE </strong>:<span style="font-weight: normal;"> vertoningen in deze kolom, wijst het erop dat het vermelde gebied een douanegebied is.</span></p> </td> 
  </tr> 
  <tr> 
   <td><strong> Type van Verandering </strong> </td> 
   <td> <p>Het type wijziging dat in het desbetreffende veld wordt aangebracht. Afhankelijk van de filterregels die u instelt en de acties die gebruikers ondernemen, kan het volgende in dit veld worden weergegeven:</p> 
    <ul> 
     <li> <p>Toevoegen</p> </li> 
     <li> <p>Audit</p> </li> 
     <li> <p>Verwijderen</p> </li> 
     <li> <p>Samenvatting</p> </li> 
     <li> <p>Bewerken</p> </li> 
     <li> <p>Herstellen</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong> Top ObjCode </strong> </td> 
   <td> <p>Het hoogste bovenliggende object in de hiërarchie.</p> </td> 
  </tr> 
  <tr> 
   <td><strong> Reikwijdte </strong> </td> 
   <td> <p>Het type object dat is gewijzigd.</p> </td> 
  </tr> 
  <tr> 
   <td><strong> Datum van de Ingang </strong> </td> 
   <td> <p>De datum waarop het veld is gewijzigd.</p> </td> 
  </tr> 
  <tr> 
   <td><strong> die door Naam </strong> wordt uitgegeven </td> 
   <td> <p>De gebruiker die het veld heeft gewijzigd.</p> </td> 
  </tr> 
 </tbody> 
</table>

Om de informatie in dit rapport te organiseren, kunt u de ingebouwde groepering gebruiken genoemd Project. De groepering van het Project geeft u een primaire groepering van de Naam van het Project en een secundaire groepering van de Datum van de Ingang. U kunt deze bestaande groepering tijdens rapportverwezenlijking toepassen, of u kunt het toepassen wanneer het bekijken van het rapport.

Zie de desbetreffende sectie voor meer informatie over het instellen van de weergaven, filters en groepen die u voor uw rapport wilt gebruiken:

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: from&nbsp;Luke: Take this for what it's worth, but part of me wonders if all of these subsections should be separate articles.</p>
<p>The biggest reason for breaking these up would be searchability, in my mind. For example, as a user, I might want to know how to see if the owner of a project changed. If I search the help site for that, I would be a lot more likely to find a separate article called "See if the owner of a project changed" vs an article titled "Create a Journal Entry report" because "Journal Entry" might mean nothing to me.) </p>
</div>
-->

* [ zie welke statusveranderingen voorkwamen ](#see-what-status-changes-occurred)
* [ zie wanneer een taak of een kwestie werd geschrapt ](#see-when-a-task-or-issue-was-deleted)
* [ zie hoe de douanevelden tijdens de het levenscyclus van een project ](#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle) veranderden
* [ zie hoe de Geplande Datum van de Voltooiing tijdens de het levenscyclus van een project ](#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle) veranderde
* [Controleren of de eigenaar van een project is gewijzigd](#see-if-the-owner-of-a-project-changed)

## Controleren welke statuswijzigingen zijn opgetreden {#see-what-status-changes-occurred}

U kunt opstelling het rapport van de Ingang van het Dagboek om te tonen:

* Hoeveel statuswijzigingen zijn aangebracht in een project, taak of uitgave

* Wat was de vorige status vóór de wijziging
* Wie de status heeft gewijzigd
* Wanneer de status is gewijzigd

Als u de gezondheid van een project wilt zien, kon u opstelling het rapport ook om deze zelfde informatie te tonen gebruikend het 1} gebied van de Voorwaarde van het project **{.**

Deze informatie kan worden gebruikt om met controle te helpen en te illustreren hoe goed u en uw organisatie plannen.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;for tip below: When analytics adds the status option, update this note to say "these entries (status or condition changes)")</p>
-->

>[!TIP]
>
>Als u het verschil in dagen tussen voorwaardenveranderingen wilt vergelijken, kunt u Verbeterde analysemogelijkheden gebruiken.\
>Meer over Verbeterde analyses leren, zie [ Verbeterd analyseoverzicht ](../../../enhanced-analytics/enhanced-analytics-overview.md).

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Rapporten**.
1. Klik **Nieuw Rapport**, dan uitgezochte **Ingang van het Dagboek**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   De rapportbuilder laadt.

1. In de **Kolommen (Mening)** tabel, voeg de volgende kolommen toe:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Kolom</th> 
      <th>Toelichting</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Veldnaam</p> </td> 
      <td> <p>De naam van het desbetreffende veld. In dit geval, <strong> status </strong> zou in deze kolom moeten tonen.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Type wijzigen</p> </td> 
      <td> <p>Het type van verandering die aan het beïnvloede gebied wordt aangebracht, zoals <strong> voegt </strong> toe, <strong> schrapt </strong>, of <strong> geeft </strong> uit.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Bewerkt op naam</p> </td> 
      <td> <p>De naam van de gebruiker die de status heeft bijgewerkt.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Invoerdatum</p> </td> 
      <td> <p>De datum waarop de status is gewijzigd.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Oude tekstwaarde</p> </td> 
      <td> <p>De sleutel voor de vorige status. Hier volgen de statussleutels voor de standaardstatus van een project:</p> 
       <ul> 
        <li> <p> <strong> CUR </strong>: Huidige</p> </li> 
        <li> <p><strong> VERBORGEN </strong>: Dode</p> </li> 
        <li> <p><strong> ONH </strong>: Op Greep</p> </li> 
        <li> <p><strong> PLN </strong>: Planning</p> </li> 
        <li> <p><strong> CPL </strong>: Volledig</p> </li> 
        <li> <p><strong> REQ </strong>: Gevraagd</p> </li> 
        <li> <p><strong> APR </strong>: Goedgekeurd</p> </li> 
        <li> <p><strong> REJ </strong>: Geweigerd</p> </li> 
        <li> <p><strong> IDA </strong>: Idea</p> </li> 
       </ul> <p>Als uw organisatie aangepaste statussen heeft ingesteld, worden mogelijk andere statussleutels in deze kolom weergegeven. Neem contact op met uw Workfront-beheerder of groepsbeheerder voor meer informatie over de aangepaste status die gerelateerd is aan een statussleutel.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nieuwe tekstwaarde</p> </td> 
      <td> <p>De sleutel voor de bijgewerkte status.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">ObjCode boven</p> </td> 
      <td> <p>Het hoogste bovenliggende object voor het veld met de statuswijziging.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Toepassingsgebied</p> </td> 
      <td> <p>Het type object waarvoor de status is gewijzigd.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Naam van uitgave <br> (optioneel)</p> </td> 
      <td> <p>De naam van de kwestie die een statusverandering had.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Taaknaam <br> (optioneel)</p> </td> 
      <td> <p>De naam van de taak waarvoor de status is gewijzigd.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Voor meer informatie bij het toevoegen van kolommen, zie [ Overzicht van Meningen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. In het **lusje van Filters**, klik **filterregel** toevoegen, dan voeg de Naam van het filterregel **Gebied** toe > **Gelijk** > **status**.

   ![](assets/nwe-journal-entry-status-filter-rules-350x90.png)

   >[!TIP]
   >
   >Om op voorwaardenveranderingen te rapporteren, kunt u in plaats daarvan de naam van het filterregel **Gebied** toevoegen > **Gelijk** > **Voorwaarde**.

   Voor meer informatie bij het toevoegen van filters, zie [ Overzicht van Filters ](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Optioneel) Voeg een vraag toe om de focus van het rapport te beperken en de laadtijden te verkorten.

   of

   Maak aanvullende filterregels om specifieke projecten, taken of problemen op te nemen.

   >[!IMPORTANT]
   >
   >Creërend een filterregel die de bepaling **gebruikt bevat** kan ladingstijden eigenlijk verhogen. Om deze reden, adviseren wij gebruikend een verschillende bepaling zoals **Gelijk** wanneer mogelijk om voor een specifiek project of objecten identiteitskaart op hoger niveau te filtreren.

   Leren hoe te om een herinnering toe te voegen, zie [ een herinnering aan een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md) toevoegen.

1. In het **lusje van Groepen**, klik **een Bestaande Groepering** toepassen, dan selecteren **Project**.

   Voor meer informatie bij het toevoegen van groeperingen, zie [ Overzicht van Groepen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klik **sparen + Sluiten**.

   Uw nieuwe rapport wordt geladen.

## Controleren wanneer een taak of probleem is verwijderd {#see-when-a-task-or-issue-was-deleted}

U kunt opstelling het rapport van de Ingang van het Dagboek om te tonen:

* Welke taken of problemen zijn verwijderd
* Wie een taak of probleem heeft verwijderd

Zo ziet u wanneer een taak of uitgave is verwijderd:

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Rapporten**.
1. Klik **Nieuw Rapport**, dan uitgezochte **Ingang van het Dagboek**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   De rapportbuilder laadt.

1. In de **Kolommen (Mening)** tabel, voeg de volgende kolommen toe:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Kolom</th> 
      <th>Toelichting</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Toepassingsgebied</p> </td> 
      <td> <p>Het type object dat is verwijderd.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Type wijzigen</p> </td> 
      <td> <p>Het soort verandering dat is gebeurd. De <strong> schrapping </strong> veranderingsvertoningen in deze kolom.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Invoerdatum</p> </td> 
      <td> <p>De datum waarop de taak of uitgave is verwijderd.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Bewerkt op naam</p> </td> 
      <td> <p>De naam van de gebruiker die de taak of uitgave heeft verwijderd.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Projectnaam</p> </td> 
      <td> <p>De naam van het project waarvoor taken of problemen zijn verwijderd.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Voor meer informatie bij het toevoegen van kolommen, zie [ Overzicht van Meningen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. In het **lusje van Filters**, klik **toevoegen filterregel**, dan voeg de volgende filters toe:

   * **Type van Verandering** > **Gelijk** > **Schrapping**
   * **identiteitskaart van het Project** > **Gelijk** > **`<project>`**

     <!--WRITER check link; this png file has spaces
     [![](assets/classic-task-or-issue-deleted-350x90.png)](../../../Resources/Images/Reports/Creating and Managing Reports/QS_Task or issue deleted.png)-->

   Voor meer informatie bij het toevoegen van filters, zie [ Overzicht van Filters ](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Optioneel) Voeg een vraag toe om de focus van het rapport te beperken en de laadtijden te verkorten.

   of

   Maak aanvullende filterregels om specifieke projecten, taken of problemen op te nemen.

   >[!IMPORTANT]
   >
   >Creërend een filterregel die de bepaling **gebruikt bevat** kan ladingstijden eigenlijk verhogen. Om deze reden, adviseren wij gebruikend een verschillende bepaling zoals **Gelijk** wanneer mogelijk om voor een specifiek project of objecten identiteitskaart op hoger niveau te filtreren.

   Leren hoe te om een herinnering toe te voegen, zie [ een herinnering aan een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md) toevoegen.

1. (Facultatief) in het **lusje van Groepen 0}, klik** een Bestaande Groepering **toepassen, dan selecteren** Project **.**

   Voor meer informatie bij het toevoegen van groeperingen, zie [ Overzicht van Groepen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klik **sparen + Sluiten**.

   Uw nieuwe rapport wordt geladen.

## Bekijk hoe aangepaste velden zijn gewijzigd tijdens de levenscyclus van een project {#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle}

U kunt belangrijke gebiedsveranderingen tijdens de loop van het project volgen. Om dit te doen, kunt u opstelling de Ingang van het Dagboek aan spoor:

* Als bepaalde aangepaste velden zijn toegevoegd, bijgewerkt of bewerkt
* Wanneer deze wijzigingen hebben plaatsgevonden
* Wie heeft de wijzigingen aangebracht

Zo ziet u hoe aangepaste velden tijdens de levenscyclus van een project zijn gewijzigd:

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Rapporten**.
1. Klik **Nieuw Rapport**, dan uitgezochte **Ingang van het Dagboek**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   De rapportbuilder laadt.

1. In de **Kolommen (Mening)** tabel, voeg de volgende kolommen toe:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Kolom</th> 
      <th>Toelichting</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Veldnaam</p> </td> 
      <td> <p>De naam van het desbetreffende aangepaste veld.</p> <p><span style="font-weight: normal;"> wanneer </span> <strong> DE </strong>:<span style="font-weight: normal;"> vertoningen in deze kolom, wijst het erop dat het vermelde gebied een douanegebied is.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Type wijzigen</p> </td> 
      <td> <p>Het type van verandering die aan het beïnvloede gebied wordt aangebracht, zoals <strong> voegt </strong> toe, <strong> schrapt </strong>, of <strong> geeft </strong> uit.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Bewerkt op naam</p> </td> 
      <td> <p>De naam van de gebruiker die het aangepaste veld heeft bijgewerkt.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Invoerdatum</p> </td> 
      <td> <p>De datum waarop de waarde in het aangepaste veld is gewijzigd.</p> <p>U moet dit veld in aflopende volgorde sorteren.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Oude getalwaarde</p> </td> 
      <td> <p>De vorige getalwaarde in het aangepaste veld.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nieuwe getalwaarde</p> </td> 
      <td> <p>De huidige getalwaarde in het aangepaste veld.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Waarde van oude datum</p> </td> 
      <td> <p>De vorige datumwaarde in het aangepaste veld.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nieuwe datumwaarde</p> </td> 
      <td> <p>De huidige datumwaarde in het aangepaste veld.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Oude tekstwaarde</p> </td> 
      <td> <p>De vorige tekstwaarde in het aangepaste veld.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nieuwe tekstwaarde</p> </td> 
      <td> <p>De huidige tekstwaarde in het aangepaste veld.</p> <p>Als het douanegebied een typeahead gebied is, toont de <strong> Nieuwe kolom van de Waarde van de Tekst </strong> objecten identiteitskaart</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Voor meer informatie bij het toevoegen van kolommen, zie [ Overzicht van Meningen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. In het **lusje van Filters**, klik **toevoegen filterregel**, dan voeg de volgende filters toe:

   * **>** bevat de Naam van het Gebied van de Ingang van het Dagboek **>** DE ****

     >[!TIP]
     >
     >Om dit rapport tot specifieke douanegebieden te beperken, voeg de naam van het Gebied van de Ingang van het Dagboek **>** Gelijk **>**`<custom field>`**toe.**

   * **identiteitskaart van het Project** > **Gelijk** > **`<project>`**

     ![](assets/qs-custom-form-changes-filter-350x92.png)

   Voor meer informatie bij het toevoegen van filters, zie [ Overzicht van Filters ](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Optioneel) Voeg een vraag toe om de focus van het rapport te beperken en de laadtijden te verkorten.

   of

   Maak aanvullende filterregels om specifieke projecten, taken of problemen op te nemen.

   >[!IMPORTANT]
   >
   >Creërend een filterregel die de bepaling **gebruikt bevat** kan ladingstijden eigenlijk verhogen. Om deze reden, adviseren wij gebruikend een verschillende bepaling zoals **Gelijk** wanneer mogelijk om voor een specifiek project of objecten identiteitskaart op hoger niveau te filtreren.

   Leren hoe te om een herinnering toe te voegen, zie [ een herinnering aan een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md) toevoegen.

1. In het **lusje van Groepen**, klik **een Bestaande Groepering** toepassen, dan selecteren **Project**.

   Voor meer informatie bij het toevoegen van groeperingen, zie [ Overzicht van Groepen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klik **sparen + Sluiten**.

   Uw nieuwe rapport wordt geladen.

## Zie hoe de geplande afwerkingsdatum is gewijzigd tijdens de levenscyclus van een project {#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle}

U kunt opstelling het rapport van de Ingang van het Dagboek tonen hoe vaak de Geplande Datum van de Voltooiing in de loop van het leven van een project verandert.

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Rapporten**.
1. Klik **Nieuw Rapport**, dan uitgezochte **Ingang van het Dagboek**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   De rapportbuilder laadt.

1. In de **Kolommen (Mening)** tabel, voeg de volgende kolommen toe:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Kolom</th> 
      <th>Toelichting</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Veldnaam</p> </td> 
      <td> <p>De naam van het desbetreffende veld.</p> <p><span style="font-weight: normal;"> wanneer </span> <strong> DE </strong>:<span style="font-weight: normal;"> vertoningen in deze kolom, wijst het erop dat het vermelde gebied een douanegebied is.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Type wijzigen</p> </td> 
      <td>Het type van verandering dat gebeurde, zoals <strong> voegt </strong> toe, <strong> schrapt </strong>, of <strong> geeft </strong> uit.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Bewerkt op naam</p> </td> 
      <td> <p>De naam van de gebruiker die de geplande Voltooiingsdatum van het project heeft bijgewerkt.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Invoerdatum</p> </td> 
      <td> <p>De datum waarop de geplande afsluitdatum van het project is gewijzigd.</p> <p>U moet dit veld in aflopende volgorde sorteren.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">ObjCode boven</p> </td> 
      <td> <p>Het hoogste bovenliggende object voor het veld waarvoor de geplande wijziging van de voltooiingsdatum is opgetreden.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Toepassingsgebied</p> </td> 
      <td> <p>Het object waarvoor de geplande aanmaakdatum is gewijzigd.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Waarde van oude datum</p> </td> 
      <td> <p>De vorige waarde voor de Geplande Datum van Voltooiing.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nieuwe datumwaarde</p> </td> 
      <td> <p>De huidige waarde voor de Geplande Voltooiingsdatum.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Projectnaam</p> <p>(Optioneel)</p> </td> 
      <td> <p>De naam van het project waarvan de geplande aanmaakdatum is gewijzigd.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Taaknaam</p> <p>(Optioneel)</p> </td> 
      <td> <p>De naam van de taken in het project waarvoor de geplande wijziging van de Voltooiingsdatum heeft plaatsgevonden.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Naam van uitgave</p> <p>(Optioneel)</p> </td> 
      <td>De naam van de problemen in het project waarvoor de geplande wijziging van de Voltooiingsdatum geldt.</td> 
     </tr> 
    </tbody> 
   </table>

   Voor meer informatie bij het toevoegen van kolommen, zie [ Overzicht van Meningen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. In het **lusje van Filters**, klik **toevoegen filterregel**, dan voeg het volgende toe:

   * **Naam van het Gebied** > **Gelijk** > **Datum**
   * **identiteitskaart van het Project** > **Gelijk** > **`<project>`**

   ![](assets/qs-planned-completion-date-change-filter-350x91.png)

   Voor meer informatie bij het toevoegen van filters, zie [ Overzicht van Filters ](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Optioneel) Voeg een vraag toe om de focus van het rapport te beperken en de laadtijden te verkorten.

   of

   Maak aanvullende filterregels om specifieke projecten, taken of problemen op te nemen.

   >[!IMPORTANT]
   >
   >Creërend een filterregel die de bepaling **gebruikt bevat** kan ladingstijden eigenlijk verhogen. Om deze reden, adviseren wij gebruikend een verschillende bepaling zoals **Gelijk** wanneer mogelijk om voor een specifiek project of objecten identiteitskaart op hoger niveau te filtreren.

   Leren hoe te om een herinnering toe te voegen, zie [ een herinnering aan een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md) toevoegen.

1. In het **lusje van Groepen**, klik **een Bestaande Groepering** toepassen, dan selecteren **Project**.

   Voor meer informatie bij het toevoegen van groeperingen, zie [ Overzicht van Groepen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klik **sparen + Sluiten**.

   Uw nieuwe rapport wordt geladen.

## Controleren of de eigenaar van een project is gewijzigd {#see-if-the-owner-of-a-project-changed}

U kunt opstelling het rapport van de Ingang van het Dagboek om te tonen hoeveel keer het project eigenaar-of projectmanager-verandert over de cursus van het leven van een project.

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Rapporten**.
1. Klik **Nieuw Rapport**, dan uitgezochte **Ingang van het Dagboek**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   De rapportbuilder laadt.

1. In de **Kolommen (Mening)** tabel, voeg de volgende kolommen toe:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Kolom</th> 
      <th>Toelichting</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Veldnaam</p> </td> 
      <td>De naam van het desbetreffende veld. De <strong> ownerID </strong> vertoningen in deze kolom.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Type wijzigen</p> </td> 
      <td> <p>Het type van verandering dat gebeurde, zoals <strong> voegt </strong> toe, <strong> schrapt </strong>, of <strong> geeft </strong> uit.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">ObjCode boven</p> </td> 
      <td> <p>Het hoogste oudervoorwerp voor het project dat de projecteigenaar bijgewerkt had.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Invoerdatum</p> </td> 
      <td>De datum waarop de eigenaar van het project is gewijzigd.<br> u zou door dit gebied in dalende orde moeten sorteren.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Bewerkt op naam</p> </td> 
      <td> <p>De naam van de gebruiker die de eigenaar van het project heeft bijgewerkt.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Aanvullende informatie 1</p> </td> 
      <td> <p>De huidige eigenaar van het project.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Aanvullende informatie 2</p> </td> 
      <td> <p>De vorige eigenaar van het project.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Projectnaam</p> </td> 
      <td> <p>Het project waarbij het veld Projecteigenaar is bijgewerkt.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Voor meer informatie bij het toevoegen van kolommen, zie [ Overzicht van Meningen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. In het **lusje van Filters**, klik **toevoegen filterregel**, dan voeg het volgende toe:

   * **Naam van het Gebied** > **Gelijk** > **ownerID**
   * **identiteitskaart van het Project** > **Gelijk** > **`<project name>`**

     ![](assets/qs-owner-changes-filter-350x94.png)

   Voor meer informatie bij het toevoegen van filters, zie [ Overzicht van Filters ](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Optioneel) Voeg een vraag toe om de focus van het rapport te beperken en de laadtijden te verkorten.

   of

   Maak aanvullende filterregels om specifieke projecten, taken of problemen op te nemen.

   >[!IMPORTANT]
   >
   >Creërend een filterregel die de bepaling **gebruikt bevat** kan ladingstijden eigenlijk verhogen. Om deze reden, adviseren wij gebruikend een verschillende bepaling zoals **Gelijk** wanneer mogelijk om voor een specifiek project of objecten identiteitskaart op hoger niveau te filtreren.

   Leren hoe te om een herinnering toe te voegen, zie [ een herinnering aan een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md) toevoegen.

1. (Facultatief) in het **lusje van Groepen 0}, klik** een Bestaande Groepering **toepassen, dan selecteren** Project **.**

   Voor meer informatie bij het toevoegen van groeperingen, zie [ Overzicht van Groepen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klik **sparen + Sluiten**.

   Uw nieuwe rapport wordt geladen.
