---
product-area: projects
navigation-topic: manage-tasks
title: Taken verplaatsen
description: U kunt taken naar verschillende projecten of naar verschillende bovenliggende taken in Adobe Workfront verplaatsen.
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: 412645a802bdf9057bb61a5a96df257daa1c3948
workflow-type: tm+mt
source-wordcount: '1547'
ht-degree: 0%

---

# Taken verplaatsen

<!--Audited: 12/2024-->


<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>


U kunt taken in Adobe Workfront verplaatsen tussen de volgende objecten:

* Een ad-hoctaak voor een project.
* Een taak van een project aan een ander project.
* Een taak van een project onder een verschillende ouder in een ander project.
* Een taak binnen het zelfde project onder een verschillende ouder.

U kunt een taak op taakniveau verplaatsen of u kunt een taak uit een lijst met taken verplaatsen.
U kunt één taak verplaatsen of meerdere taken tegelijk uit een takenlijst verplaatsen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de handelingen in dit artikel uit te voeren:

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
   <td> <p>Nieuw abonnement: standaard </p> 
 <p>of</p>  
<p>Huidig abonnement: Werk of hoger </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot taken en projecten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor de taken beheren</p> <p>Contribute of hogere toestemmingen aan het project met capaciteit toevoegen Taken</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het verplaatsen van taken

Houd rekening met het volgende wanneer u een taak verplaatst:

* Wanneer u een taak van één project aan een ander verplaatst, zouden de taakdata kunnen worden herberekend. Bij de herberekening wordt rekening gehouden met het tijdschema dat voor het nieuwe project wordt gebruikt en met het tijdschema voor het project op basis van informatie.

* U hebt de kans om sommige punten te selecteren verbonden aan de taak naar de verplaatste taak tijdens het het bewegen proces te verplaatsen. De volgende objecten worden echter standaard overgebracht naar de verplaatste taak:

   * Problemen
   * Aangemeld aantal uren
   * Opmerkingen van gebruikers
   * Aangepaste formulieren en aangepaste veldgegevens
   * Subtaken

De volgende items worden standaard niet verplaatst met de taak:

* Mijlpalen

<div class="preview">

* Uw systeem of groepsbeheerder kan u verhinderen taken te bewegen die het programma geopende uren, afhankelijk van hoe zij vormen toestaan gebruikers om taken en kwesties met geregistreerde urenvoorkeur in het gebied van de Opstelling te bewegen. Voor informatie, zie [ de taak en de uitgevende voorkeur van het systeem brede ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) vormen.

</div>


## Taken in een lijst verplaatsen

1. Ga naar het project dat de taak of de taken bevat die u wilt bewegen.
1. Klik **Taken** in het linkerpaneel om de taaklijst te tonen.
1. Klik het **pictogram van de Wijze van het 0} Plan ![](assets/plan-mode-icon.png) en zorg ervoor dat** autosave **knevel wordt toegelaten, dan selecteer de taak of de taken die u wilt bewegen.**

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >U kunt geen taken bewegen wanneer **Autosave** knevel gehandicapt is.

1. (Optioneel en voorwaardelijk) Als u de geselecteerde taken binnen hetzelfde project wilt verplaatsen, klikt u op de geselecteerde taken, sleept u ze naar de gewenste locatie voor het project.

   Nadat u de taken op de juiste plaats op het project hebt neergezet, worden de wijzigingen die u in de taakhiërarchie hebt aangebracht, direct opgeslagen. Alle informatie verbonden aan elke taak wordt bewogen met de taken.

1. (Voorwaardelijk) Selecteer de taak of de taken die u wilt verplaatsen en voer een van de volgende handelingen uit:

   * Klik **Meer** menu ![](assets/qs-more-menu.png) bij de bovenkant van de taaklijst, dan klik **Beweging aan**.
   * Klik de geselecteerde taken met de rechtermuisknop aan, dan klik **Beweging aan**.
   * Wanneer het selecteren van één taak, klik **Meer** menu ![](assets/more-icon-task-list.png) naast de taaknaam in de lijst, dan klik **Beweging aan**.

   ![](assets/move-task-in-list-nwe-350x119.png)

   De **vakvertoningen van de Taak van de Beweging**

1. Ga met het bewegen van de taak voort, zoals die in de sectie [ wordt beschreven Beweeg een taak op het taakniveau ](#move-a-task-at-the-task-level) in dit artikel, die met Stap 4 begint.

   <!--
   is this still accurate?!
   -->

## Een taak op taakniveau verplaatsen {#move-a-task-at-the-task-level}

Naast het verplaatsen van taken uit een lijst met taken kunt u een taak ook op taakniveau verplaatsen nadat u deze hebt geopend.

1. Zoek naar een taak in je Workfront-systeem.
1. Klik op de naam van de taak om deze te openen.
1. Klik **Meer** drop-down menu ![](assets/qs-more-menu.png) naast de naam van de taak, dan klik **Beweging aan**. Het vak Taak verplaatsen wordt weergegeven.

   ![](assets/move-task-at-task-level-nwe-350x222.png)

1. (Facultatief) werk de **Naam van de Taak** bij. De taak wordt met de nieuwe naam verplaatst op de nieuwe locatie. Workfront registreert de oorspronkelijke naam van de taak niet.

   >[!TIP]
   >
   >Het veld Taaknaam wordt grijs weergegeven en kan niet worden bewerkt wanneer u ervoor kiest meerdere taken in een lijst te verplaatsen. U kunt de muisaanwijzer boven het veld Taaknaam en een lijst met alle geselecteerde taken weergeven.
   >
   >
   >![](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. Typ de naam van het **Project van de Bestemming** waar u de taak op het **Uitgezochte gebied van het Project van de Bestemming** wilt bewegen.

   Als u de taak binnen het zelfde project wilt bewegen, typ de naam van het huidige project.

   >[!TIP]
   >
   >* De naam van het project is hoofdlettergevoelig.
   >* U kunt ook het Referentienummer typen of de id van het project invoeren. Hierdoor kunt u projecten met identieke namen beter van elkaar onderscheiden.
   >* Er worden slechts 100 projecten weergegeven in de lijst.

1. (Voorwaardelijk) klik **toegang van het Verzoek** om toegang tot het project te verzoeken, als u geen toegang tot het geselecteerde project hebt.
1. (Voorwaardelijk) blijf de taak aan het geselecteerde bestemmingsproject verplaatsen zonder toegang te vragen als u toegang hebt om taken aan één van de taken op het bestemmingsproject toe te voegen.

   ![](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >De gelijkaardige berichten tonen als het geselecteerde project in afwachting van goedkeuring, voltooid, of dood is, wanneer de beheerder van Workfront het toevoegen van taken aan deze projecten verhindert. Voor meer informatie, zie [ systeem-brede projectvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

1. (Facultatief) klik **Opties** in het linkerpaneel

   of

   De rol neer aan de **sectie van Opties** in de doos van de Taak van de Beweging, dan schrapt om het even welke punten die in de lijst hieronder worden vermeld om hen uit de verplaatste taken te verwijderen. Alle opties zijn standaard geselecteerd.

   >[!IMPORTANT]
   >
   >Als u de selectie van items in de lijst Opties opheft, gaan er gegevens verloren. Informatie van de bestaande taak wordt verwijderd en kan niet worden hersteld.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alles selecteren</td> 
      <td>Schakel deze optie uit als u alle gegevens uit de taak wilt verwijderen wanneer u de taak naar de nieuwe locatie verplaatst. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Restrictie</td> 
      <td> <p>De taakbeperking wordt geplaatst aan zo spoedig mogelijk of zo laat mogelijk gebaseerd op het plaatsen van de Wijze van het projectprogramma.</p> <p> Als deze optie is geselecteerd, wordt de huidige beperking van de taak overgedragen met de taak. </p> 
      <p><b>OPMERKING</b>

   Wanneer het bewegen of het kopiëren van een taak met datum-specifieke beperkingen aan een ander project en de beperkingsdata van de taak zijn buiten de data van het nieuwe project, of verandert de Beperking van de Taak in zo spoedig mogelijk of zo laat mogelijk of de Geplande Begin of Geplande Voltooiingsdata van de projecten worden aangepast.

   Hieronder volgen voorbeelden van datumspecifieke beperkingen:
   <ul>
      <li> Starten bij</li>
      <li> Moet worden voltooid op</li>
      <li> Niet eerder starten dan</li>
      <li> Niet later starten dan</li>
      </ul>

   Voor informatie over taakbeperkingen en hoe de taakbeperkingen of projectdata kunnen worden beïnvloed, zie {het overzicht van de Beperking van de Taak 0} </a> en zoek een specifieke beperking.<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref"></p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Toewijzingen</td> 
      <td> <p>Alle toewijzingen worden uit de taak verwijderd. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Goedkeuringsproces</td> 
      <td>Alle goedkeuringsprocessen worden uit de taak verwijderd.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Voortgang</td> 
      <td>De taakstatus is Nieuw. Anders blijft de bestaande taakstatus behouden. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Financiële informatie</td> 
      <td>De financiële informatie van de taak wordt verwijderd en Workfront werkt het type van taakkosten aan Geen Kosten en het type van taakopbrengst bij niet Facultable. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alle voorgangers</td> 
      <td> <p>Wanneer geselecteerd, wordt het gebiedsdeel een dwars-projectvoorganger wanneer u de taak naar een ander project verplaatst. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenten</td> 
      <td> <p>De documenten die aan de taak zijn gekoppeld, worden niet naar de verplaatste taak overgedragen. Dit zijn versies, proefdrukken en gekoppelde documenten.</p> <p>Dit omvat geen documentgoedkeuringen. Documentgoedkeuringen kunnen nooit worden verplaatst wanneer een taak wordt verplaatst.</p> 
      <b> NOTA </b>

   Als u ervoor kiest de documenten niet met de taak te laten verplaatsen, worden de documenten verwijderd en gedurende 30 dagen in de prullenbak geplaatst. Een beheerder kan ze herstellen en ze worden hersteld op de verplaatste taak.

   Als de taak wordt geschrapt nadat het wordt bewogen, zullen de herstelde documenten in het gebied van Documenten van de gebruikerspagina van de beheerder worden geplaatst die hen herstelt.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Herinneringsmeldingen</td> 
      <td>De taakherinneringen worden niet overgedragen naar de verplaatste taak. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uitgaven</td> 
      <td>De uitgaven die op de taak worden geregistreerd brengen niet naar de verplaatste taak over. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Machtigingen</td> 
      <td> <p>Workfront verwijdert de namen van alle entiteiten die worden weergegeven in de lijst voor delen van de taak. </p> </td> 
     </tr> 
    </tbody> 
   </table>



1. (Facultatief) klik **Uitgezochte Ouder** in het linkerpaneel

   of

   De rol aan de **Uitgezochte Ouder** sectie, selecteert dan de taak in het bestemmingsproject dat u de ouder van de verplaatste taak wilt worden.

   >[!TIP]
   >
   >Wanneer u selecteert om meerdere taken in een lijst te verplaatsen, worden alle geselecteerde taken de onderliggende taken van het geselecteerde bovenliggende element.

   Voer een van de volgende handelingen uit om een bovenliggend element te selecteren:

   * In de taaklijst, selecteer één van de ouders in het projectplan.
   * Klik het pictogram van het onderzoekspictogram ![ Onderzoek ](assets/search-icon.png) en onderzoek naar een oudertaak door naam.

   De taak wordt weergegeven in de lijst.

   ![ Uitgezochte oudertaak wanneer het bewegen van een taak met onderzoeksfunctionaliteit ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Selecteer het keuzerondje voor het bovenliggende element nadat u het hebt gevonden.

   Als u geen oudertaak selecteert, worden de taken verplaatst als belangrijkste taken eerder dan subtaken en zij worden geplaatst aan het eind van de taaklijst op het bestemmingsproject.

1. Klik **de taak van de Beweging**

   of

   Klik **de taken van de Beweging** wanneer u veelvoudige taken in een lijst selecteert.

   De verplaatste taken zijn nu op het gespecificeerde project en of subtaken aan een oudertaak, of de laatste taken op het project.
