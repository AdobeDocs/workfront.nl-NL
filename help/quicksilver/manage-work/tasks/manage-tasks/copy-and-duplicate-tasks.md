---
product-area: projects
navigation-topic: manage-tasks
title: Taken kopiëren en dupliceren
description: U kunt een taak van een project aan een ander project kopiëren, of u kunt een taak binnen het zelfde project dupliceren.
author: Alina
feature: Work Management
exl-id: daf89062-cf58-4c39-83ff-727d969a9630
source-git-commit: 1f749ba9a54ce75a917e4b1e95713ac7abeaa66b
workflow-type: tm+mt
source-wordcount: '1705'
ht-degree: 0%

---

# Taken kopiëren en dupliceren

U kunt een taak van een project aan een ander project kopiëren, of u kunt een taak binnen het zelfde project dupliceren.

U kunt een of meer taken of bovenliggende taken tegelijk kopiëren of dupliceren.

## Toegangsvereisten

<!-- drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a task</p> <p>Contribute or higher permissions to the project</p> 
   <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Werk of hoger </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot taken en projecten bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een taak beheren </p> <p>Contribute of hoger machtigingen voor het project</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Overwegingen bij het kopiëren van taken

Houd rekening met het volgende wanneer u een taak kopieert:

* Problemen worden niet met de taak gekopieerd.
* De mijlpalen worden overgebracht naar de gekopieerde taak en uit de originele taak verwijderd.
* Wanneer u een taak van één project aan een ander kopieert, zouden de taakdata kunnen worden herberekend. Bij de herberekening wordt rekening gehouden met het tijdschema dat voor het nieuwe project wordt gebruikt en met het tijdschema voor het project op basis van informatie.

U kunt een taak kopiëren in de volgende gebieden van de Adobe Workfront-webtoepassing:

* Op het taakniveau, vanaf **Meer pictogram** ![](assets/qs-more-menu-19x7.png) rechts van de taaknaam.

  Zie voor meer informatie de [Een taak kopiëren op taakniveau](#copy-a-task-at-the-task-level) in dit artikel.

* Voer een van de volgende handelingen uit in een takenlijst:

   * Klik met de rechtermuisknop op de naam van een taak.
   * Selecteer de taak (of taken) en vouw de **Meer** pictogram ![](assets/more-icon-task-list.png) boven aan de takenlijst.
   * Selecteer een taak en breid de **Meer** pictogram ![](assets/more-icon-task-list.png) naast de taaknaam.

     Deze optie is niet beschikbaar als u meerdere taken selecteert.

  Zie voor meer informatie de [Taken in een lijst kopiëren](#copy-tasks-in-a-list) in dit artikel.

## Taken in een lijst kopiëren {#copy-tasks-in-a-list}

1. Ga naar het project dat de taak of de taken bevat die u wilt kopiëren.

   of

   Ga naar een taakrapport.

1. Klikken **Taken** in het linkerdeelvenster.
1. Klik op de knop **Menu van de overzichtsmodus** ![](assets/qs-list-mode-or-save-mode-icon-small.png) vervolgens **Automatisch opslaan**.

   >[!IMPORTANT]
   >
   >U kunt taken alleen in een lijst kopiëren wanneer u uw wijzigingen automatisch opslaat. Voor informatie over het opslaan van opties tijdens het bewerken van taken raadpleegt u [Taken in een lijst bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Selecteer de taak of taken die u wilt kopiëren en voer een van de volgende handelingen uit:

   * Klik op de knop **Het menu Meer** boven aan de takenlijst klikt u op **Kopiëren naar**.
   * Klik met de rechtermuisknop op de geselecteerde taken en klik vervolgens op **Kopiëren naar**.
   * Als u één taak selecteert, klikt u op de knop **Meer** menu ![](assets/more-icon-task-list.png) naast de taaknaam in de lijst klikt u op **Kopiëren naar**.

   ![](assets/copy-task-in-list-nwe-350x131.png)

1. Doorgaan met het kopiëren van de taak, zoals beschreven in de sectie [Een taak kopiëren op taakniveau](#copy-a-task-at-the-task-level) te beginnen met Stap 4.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this still accurate?!)
   </MadCap:conditionalText>
   -->

## Een taak kopiëren op taakniveau {#copy-a-task-at-the-task-level}

Naast het kopiëren van taken in een lijst met taken kunt u ook een taak kopiëren nadat u deze hebt geopend. 

1. Zoek naar een taak in je Workfront-systeem.
1. Klik op de naam van de taak om deze te openen. 
1. Klik op de knop **Meer** vervolgkeuzemenu ![](assets/qs-more-menu.png) naast de naam van de taak klikt u op **Kopiëren** **tot**.

   ![](assets/taskcopy-to-at-the-task-level-nwe-350x200.png)

   Het vak Taak kopiëren wordt weergegeven.

1. (Optioneel) Werk de **Taaknaam**.

   >[!TIP]
   >
   >Dit veld is grijs en kan niet worden bewerkt als u ervoor kiest meerdere taken in een lijst te kopiëren. U kunt de muisaanwijzer boven het veld Taaknaam en een lijst met alle geselecteerde taken weergeven.
   >
   >![](assets/copy-task-multiple-tasks-box-with-list-of-task-names-nwe-350x130.png)

1. Typ de naam van de **Doelproject** waar u de taak in wilt kopiëren **Doelproject selecteren** veld. 

   >[!TIP]
   >
   >* De naam van het project is hoofdlettergevoelig.
   >* U kunt ook beginnen het Aantal van de Verwijzing te typen of identiteitskaart van het project in te gaan. Hierdoor kunt u projecten met identieke namen beter van elkaar onderscheiden.
   >* Er worden slechts 100 projecten weergegeven in de lijst.

   De huidige projectnaam wordt standaard weergegeven. Als u de taak binnen het zelfde project wilt kopiëren, verlaat dit gebied onveranderd.

1. (Voorwaardelijk) Klik **aanvraagtoegang** om toegang tot het project te verzoeken, als u geen toegang tot het geselecteerde project hebt.
1. (Voorwaardelijk) blijf de taak aan het geselecteerde bestemmingsproject kopiëren zonder toegang te vragen als u toegang hebt om taken aan één van de taken op het bestemmingsproject toe te voegen.

   ![](assets/copy-task-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >De gelijkaardige berichten tonen als het geselecteerde project in afwachting van goedkeuring, voltooid, of dood is, wanneer de beheerder van Workfront het toevoegen van taken aan deze projecten verhindert. Zie voor meer informatie [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. Klikken **Opties** in het linkerpaneel, dan schrap de taakattributen die u niet met de taak wilt kopiëren. Alle opties zijn standaard geselecteerd.

   >[!TIP]
   >
   Selecteren en vervolgens selectie opheffen **Alles selecteren** deselecteert alle opties.

   Schakel een van de volgende opties uit als u deze niet wilt overbrengen naar de gekopieerde taak. In de volgende tabel wordt beschreven wat er gebeurt wanneer de opties zijn uitgeschakeld:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Restrictie</td> 
      <td> <p>De taakbeperking wordt geplaatst aan zo spoedig mogelijk of zo laat mogelijk gebaseerd op het plaatsen van de Wijze van het projectprogramma.</p> <p> Als deze optie is geselecteerd, wordt de huidige beperking van de taak overgedragen naar de gekopieerde taak. </p> <p>Opmerking: Wanneer het bewegen of het kopiëren van een taak met datum-specifieke beperkingen aan een ander project en de beperkingsdata van de taak zijn buiten de data van het nieuwe project, of verandert de Beperking van de Taak in zo spoedig mogelijk of zo laat mogelijk of de Geplande Begin of Geplande Voltooiingsdata van de projecten worden aangepast. Sommige voorbeelden van datum-specifieke beperkingen zijn moet beginnen, moet beëindigen, begin niet vroeger dan, begin niet later dan, enz. Voor informatie over taakbeperkingen en hoe de taakbeperkingen of projectdata kunnen worden beïnvloed, zie <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Overzicht van taakbeperking</a> en zoekt naar een specifieke beperking.</p> </td> 
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
      <td>De taakstatus is Nieuw. Anders behoudt de gekopieerde taak de status van de bestaande taak.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Financiële informatie</td> 
      <td>De financiële informatie van de taak wordt verwijderd.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alle voorgangers</td> 
      <td> <p>Dit betekent dat de afhankelijkheden niet worden overgedragen naar de gekopieerde taken. </p> <p>Als deze optie is geselecteerd, blijven de voorgangers in de groep gekopieerde taken behouden en worden de andere taken verwijderd.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenten</td> 
      <td> <p>De aan de taak gekoppelde documenten worden niet naar de gekopieerde taak overgebracht. Dit zijn versies, proefdrukken en gekoppelde documenten.</p> <p>Dit omvat geen documentgoedkeuringen. Documentgoedkeuringen kunnen nooit worden gekopieerd wanneer een taak wordt gekopieerd.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Herinneringsmeldingen</td> 
      <td>De taakherinneringen worden niet overgedragen naar de gekopieerde taak. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uitgaven</td> 
      <td>De uitgaven die op de taak worden geregistreerd brengen niet naar de gekopieerde taak over. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Machtigingen</td> 
      <td>Workfront verwijdert de namen van alle entiteiten die worden weergegeven in de lijst voor delen van de taak. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aangepaste gegevens</td> 
      <td> <p>De waarden voor de aangepaste velden worden gewist en de aangepaste formulieren worden overgebracht naar de gekopieerde taak. </p> <p>Als deze optie is geselecteerd, worden zowel de formulieren als de waarden voor de aangepaste velden overgebracht naar de gekopieerde taak. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1.  (Optioneel) Klik op **Bovenliggend element selecteren** in het linkerpaneel, dan selecteer de taak in het bestemmingsproject die u de ouder van de gekopieerde taak wilt worden.

   >[!TIP]
   >
   Wanneer u selecteert om meerdere taken in een lijst te kopiëren, worden alle geselecteerde taken de onderliggende taken van het geselecteerde bovenliggende element.

   Voer een van de volgende handelingen uit om een bovenliggend element te selecteren:

   * In de taaklijst, selecteer één van de ouders in het projectplan.
   * Klik op het zoekpictogram ![Zoekpictogram](assets/search-icon.png) en zoek op naam naar een bovenliggende taak.

   De taak moet in de lijst worden weergegeven.

   ![Bovenliggende taak selecteren bij het verplaatsen van een taak met zoekfunctionaliteit ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Selecteer het keuzerondje voor het bovenliggende element nadat u het hebt gevonden. 

   Als u geen oudertaak selecteert, worden de taken gekopieerd als belangrijkste taken eerder dan subtaken en zij zullen aan het eind van de taaklijst op het bestemmingsproject worden geplaatst. 

1. Klikken **Taak kopiëren**

   of

   Klikken **Taken kopiëren** wanneer u meerdere taken in een lijst selecteert.
De gekopieerde taken zijn nu op het gespecificeerde project en of subtaken aan de geselecteerde oudertaak, of de laatste taken op het project.

## Taken dupliceren

U kunt een taak snel dupliceren in een takenlijst als u een identieke taak nodig hebt voor hetzelfde project.

* [Overwegingen bij het dupliceren van taken](#considerations-for-duplicating-tasks)
* [Taken dupliceren](#duplicate-tasks)

### Overwegingen bij het dupliceren van taken {#considerations-for-duplicating-tasks}

* U kunt een taak alleen in een takenlijst dupliceren wanneer de lijst op taaknummer wordt gesorteerd.

* De nieuwe taak krijgt dezelfde naam als de oorspronkelijke taak.
* U kunt niet selecteren welke informatie aan de nieuwe taak wordt gedupliceerd. Bijna alle informatie van de originele taak zal naar de gedupliceerde taak, met inbegrip van ouderverhouding, door gebrek worden overgebracht.
* De volgende punten worden niet overgebracht naar de nieuwe taak:

   * Aangemeld aantal uren
   * Notities
   * Problemen
   * Alleen de voorgangers die zich in dezelfde groep gekopieerde taken bevinden, worden ook gekopieerd met hun opvolgertaken.

     **Voorbeeld:** Bijvoorbeeld, als u Taak 2 en zijn voorganger, Taak 1, tezelfdertijd kopieert, dan hebt u een exemplaar van Taak 2 en een exemplaar van Taak 1. Het exemplaar van Taak 1 zal voorganger van het exemplaar van Taak 2 zijn. Maar als u enkel Taak 2 kopieert zonder zijn voorganger te kopiëren, dan zal zijn exemplaar geen voorganger hebben.

* Wanneer u een bovenliggende taak dupliceert, worden alle onderliggende taken ook gedupliceerd, zelfs wanneer de onderliggende taken niet zijn geselecteerd.
* U kunt meerdere taken tegelijk dupliceren.

  U kunt echter niet meerdere taken tegelijk dupliceren die niet opeenvolgend zijn.

* Mijlpalen worden verplaatst naar de nieuwe taak en uit de oorspronkelijke taak verwijderd.

### Taken dupliceren

1. Ga naar het project dat de taak of de taken bevat die u wilt dupliceren.
1. Klikken **Taken** in het linkerdeelvenster.
1. Voer een van de volgende handelingen uit:

   * (Voorwaardelijk) Klik op de knop **Menu van de overzichtsmodus** ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **Automatisch opslaan**, selecteert u de taken die u wilt dupliceren en klikt u op de knop **Het menu Meer** ![](assets/qs-more-menu-29x11.png) > **Dupliceren**.

     ![](assets/duplicate-tasks-in-list-nwe-350x196.png)

   * (Voorwaardelijk) Klik op de knop **Menu van de overzichtsmodus** ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **Handmatig opslaan** > **Standaard** of **Tijdlijnplanning** Voer vervolgens de volgende handelingen uit:

      1. Selecteer de taak of taken die u wilt dupliceren en klik op **Dupliceren**.
      1. (Optioneel) Klik op **Ongedaan maken** om uw wijzigingen om te keren en de taken niet te dupliceren.
      1. (Optioneel en voorwaardelijk) Klik op **Opnieuw** als u eerder had geklikt **Ongedaan maken** om de wijzigingen te behouden en de taken te dupliceren.

      1. Klikken **Opslaan** om uw wijzigingen op te slaan.

   1. Taken in een lijst bewerken
