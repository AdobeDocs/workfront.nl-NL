---
product-area: projects
navigation-topic: manage-tasks
title: Taken verplaatsen
description: U kunt taken naar verschillende projecten of naar verschillende bovenliggende taken in Adobe Workfront verplaatsen.
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: 23a08c929b0a227c7a555af70ff731ef2df7a179
workflow-type: tm+mt
source-wordcount: '1360'
ht-degree: 0%

---

# Taken verplaatsen

U kunt taken in Adobe Workfront verplaatsen tussen de volgende objecten:

* Een ad-hoctaak voor een project.
* Een taak van een project aan een ander project.
* Een taak van een project onder een verschillende ouder in een ander project.
* Een taak binnen het zelfde project onder een verschillende ouder.

U kunt een taak op taakniveau verplaatsen of u kunt een taak uit een lijst met taken verplaatsen.

## Toegangsvereisten

U moet de volgende toegang hebben om de handelingen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenties*</td> 
   <td> <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot taken en projecten bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor de taken beheren</p> <p>Draag of hoger toestemmingen aan het project met capaciteit bij om Taken toe te voegen</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Een taak in een lijst verplaatsen

Een taak verplaatsen die in een takenlijst wordt weergegeven:

1. Ga naar het project dat de taak of de taken bevat die u wilt bewegen.
1. Klikken **Taken** in het linkerdeelvenster om de takenlijst weer te geven.
1. Zorg ervoor dat de **Automatisch opslaan** schakelt u in en selecteert u vervolgens de taak of taken die u wilt verplaatsen.

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >U kunt taken niet verplaatsen als de **Automatisch opslaan** schakeloptie is uitgeschakeld.

1. (Optioneel en voorwaardelijk) Als u de geselecteerde taken binnen hetzelfde project wilt verplaatsen, klikt u op de geselecteerde taken, sleept u ze naar de gewenste locatie voor het project.

   Nadat u de taken op de juiste plaats op het project hebt neergezet, worden de wijzigingen die u in de taakhiërarchie hebt aangebracht, direct opgeslagen. Alle informatie verbonden aan elke taak wordt bewogen met de taken.

1. (Voorwaardelijk) Selecteer de taak of de taken die u wilt verplaatsen en voer een van de volgende handelingen uit:

   * Klik op de knop **Meer** menu ![](assets/qs-more-menu.png) boven aan de takenlijst klikt u op **Verplaatsen naar**.
   * Klik met de rechtermuisknop op de geselecteerde taken en klik vervolgens op **Verplaatsen naar**.
   * Als u één taak selecteert, klikt u op de knop **Meer** menu ![](assets/more-icon-task-list.png) naast de taaknaam in de lijst klikt u op **Verplaatsen naar**.

   ![](assets/move-task-in-list-nwe-350x119.png)

   Het vak Taak verplaatsen wordt weergegeven

1. Ga door met het verplaatsen van de taak, zoals beschreven in de sectie [Een taak op taakniveau verplaatsen](#move-a-task-at-the-task-level) in dit artikel, te beginnen met Stap 4.

   <!--
   is this still accurate?!
   -->

## Een taak op taakniveau verplaatsen {#move-a-task-at-the-task-level}

Naast het verplaatsen van taken uit een lijst met taken kunt u een taak ook op taakniveau verplaatsen nadat u deze hebt geopend. 

1. Zoek naar een taak in je Workfront-systeem.
1. Klik op de naam van de taak om deze te openen.
1. Klik op de knop **Meer** vervolgkeuzemenu ![](assets/qs-more-menu.png) naast de naam van de taak klikt u op **Verplaatsen naar**. Het vak Taak verplaatsen wordt weergegeven.

   ![](assets/move-task-at-task-level-nwe-350x222.png)

1. (Optioneel) Werk de **Taaknaam**. De taak wordt met de nieuwe naam verplaatst op de nieuwe locatie. Workfront registreert de oorspronkelijke naam van de taak niet.

   >[!TIP]
   >
   >Dit veld is grijs en kan niet worden bewerkt als u meerdere taken in een lijst wilt verplaatsen. U kunt de muisaanwijzer boven het veld Taaknaam en een lijst met alle geselecteerde taken weergeven.
   >
   >
   >![](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. Typ de naam van de **Doelproject** waar u de taak in wilt bewegen **Doelproject selecteren** veld.

   Als u de taak binnen het zelfde project wilt bewegen, typ de naam van het huidige project.

   >[!TIP]
   >
   >* De naam van het project is hoofdlettergevoelig.
   >* U kunt ook beginnen het Aantal van de Verwijzing te typen of identiteitskaart van het project in te gaan. Hierdoor kunt u projecten met identieke namen beter van elkaar onderscheiden.
   >* Er worden slechts 100 projecten weergegeven in de lijst.


1. (Voorwaardelijk) Klik **Toegang aanvragen** om toegang tot het project te verzoeken, als u geen toegang tot het geselecteerde project hebt.
1. (Voorwaardelijk) blijf de taak aan het geselecteerde bestemmingsproject verplaatsen zonder toegang te vragen als u toegang hebt om taken aan één van de taken op het bestemmingsproject toe te voegen.

   ![](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >De gelijkaardige berichten tonen als het geselecteerde project in afwachting van goedkeuring, voltooid, of dood is, wanneer de beheerder van Workfront het toevoegen van taken aan deze projecten verhindert. Zie voor meer informatie [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Optioneel) Klik op **Opties** in het linkerdeelvenster

   of

   Omlaag schuiven naar de **Opties** in het vak Taak verplaatsen en deselecteer vervolgens een van de items in de onderstaande tabel om deze van de verplaatste taken te verwijderen. Alle opties zijn standaard geselecteerd.

   >[!IMPORTANT]
   Als u de selectie van items in de lijst Opties opheft, gaan er gegevens verloren. Informatie van de bestaande taak wordt verwijderd en kan niet worden hersteld.

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

   Voor informatie over taakbeperkingen en hoe de taakbeperkingen of projectdata kunnen worden beïnvloed, zie <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Overzicht van taakbeperking</a> en zoekt naar een specifieke beperking.</p> </td>
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
      <b>OPMERKING</b>

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



1. (Optioneel) Klik op **Bovenliggend element selecteren** in het linkerdeelvenster

   of

   Naar de **Bovenliggend element selecteren** selecteert u vervolgens de taak in het doelproject die u als bovenliggende taak van de verplaatste taak wilt instellen.

   >[!TIP]
   Wanneer u selecteert om meerdere taken in een lijst te verplaatsen, worden alle geselecteerde taken de onderliggende taken van het geselecteerde bovenliggende element.

   Voer een van de volgende handelingen uit om een bovenliggend element te selecteren:

   * In de taaklijst, selecteer één van de ouders in het projectplan.
   * Klik op het zoekpictogram ![Zoekpictogram](assets/search-icon.png) en zoek op naam naar een bovenliggende taak.

   De taak moet in de lijst worden weergegeven.

   ![Bovenliggende taak selecteren bij het verplaatsen van een taak met zoekfunctionaliteit ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Selecteer het keuzerondje voor het bovenliggende element nadat u het hebt gevonden.

   Als u geen oudertaak selecteert, worden de taken verplaatst als belangrijkste taken eerder dan subtaken en zij zullen aan het eind van de taaklijst op het bestemmingsproject worden geplaatst.

1. Klikken **Taak verplaatsen**

   of

   Klikken **Taken verplaatsen** wanneer u meerdere taken in een lijst selecteert.
De verplaatste taken zijn nu op het gespecificeerde project en of subtaken aan een oudertaak, of de laatste taken op het project.
