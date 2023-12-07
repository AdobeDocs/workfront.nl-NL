---
product-area: projects
navigation-topic: create-projects
title: Een project maken
description: Een project is een grote eenheid werk in Adobe Workfront. U kunt geheel nieuwe projecten maken, een sjabloon gebruiken of uitgaven of taken omzetten in projecten.
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: 45c82f659d02dca69d2a2c390b084330773d4252
workflow-type: tm+mt
source-wordcount: '1243'
ht-degree: 0%

---

# Een project maken

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is linked from the UI from the Projects global nav section in classic. Do not change/ remove)</p>
-->

Projecten vormen een groot deel van het werk dat in Adobe Workfront moet worden verricht.

## Toegangsvereisten

<!--drafted for P&P - replace table below with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Nieuw abonnement: standaard</p>
        <p>of</p>
        <p>Huidig plan: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau*</td> 
   <td> <p>Toegang tot projecten bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over toegang tot projecten, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Toegang verlenen tot projecten</a>. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Wanneer u een project creeert, ontvangt u automatisch Manage toestemmingen aan het project.</p> <p> Zie voor informatie over projectmachtigingen <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Een project delen in Adobe Workfront</a>.</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Manieren om projecten te maken

U kunt een project in Workfront tot stand brengen gebruikend één van de volgende methodes:

* Een geheel nieuw project maken zonder een sjabloon te gebruiken. In dit artikel wordt beschreven hoe u een geheel nieuw project kunt maken.

* Een bestaand project kopiëren.\
  Voor meer informatie over het kopiëren van project, zie [Een project kopiëren](../../../manage-work/projects/manage-projects/copy-project.md).

* Gebruik een sjabloon.\
  Voor meer informatie over het gebruiken van een malplaatje om een nieuw project tot stand te brengen, zie [Een project maken met een sjabloon](../../../manage-work/projects/create-projects/create-project-from-template.md).

* Een project importeren uit Microsoft Project.\
  Voor meer informatie over het invoeren van een project van het Project van MS, zie [Een project importeren uit Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* Importeer een project met de functie voor het starten van een project.

  Als beheerder van Workfront, kunt u projecten invoeren gebruikend een schop-begin.

  Voor informatie over het importeren van gegevens met gebruik van de functie voor het starten in Workfront raadpleegt u [Gegevens naar Adobe Workfront importeren met een Kick-startsjabloon](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

  Voor informatie over het invoeren van projecten gebruikend schoppen, zie [Kick-Starts-scenario: eenvoudig project en taak de invoervoorbereiding](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md).

* Publiceer een initiatief van een scenario in de Planner van het Scenario van Adobe Workfront. Voor de Scenario Planner is een aanvullende licentie vereist. Voor informatie over de Workfront Scenario Planner raadpleegt u [Overzicht van de functie Scenario Planner](../../../scenario-planner/scenario-planner-overview.md). Voor informatie over het creëren van projecten van het publiceren initiatieven, zie  [Werk of creeer projecten door initiatieven in de Planner van het Scenario bij te publiceren](../../../scenario-planner/publish-scenarios-update-projects.md).

## Vereisten

Voordat u begint, moet u ervoor zorgen dat:

* Uw systeem of groepsbeheerder liet &quot;toestaan gebruikers toe om projecten tot stand te brengen zonder een malplaatje&quot;voorkeur in het gebied van de Opstelling te gebruiken.

  Zie voor meer informatie [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Nieuwe standaardinstellingen voor project

Wanneer u een project maakt, past Workfront er een set standaardinstellingen op toe. De modi Status, Groep en Planning zijn bijvoorbeeld vooraf ingesteld wanneer u een project maakt.

Overweeg het volgende:

* Als beheerder van Workfront of een groepsbeheerder, kunt u de standaardmontages voor een nieuw project vormen wanneer het vormen van de Voorkeur van het Project voor uw volledige instantie van Workfront of voor een groep.
* Workfront past de instellingen van de groep toe, indien aanwezig, voordat deze de instellingen toepast die door de Workfront-beheerder zijn ingesteld.
* De standaardstatus van een nieuw project komt overeen met de status die is gedefinieerd door uw Workfront-beheerder in het gebied met projectvoorkeuren of door een groepsbeheerder (of Workfront-beheerder) in het gebied met projectvoorkeuren voor een groep.

  >[!NOTE]
  >
  >Wij adviseren dat de standaardstatus voor een nieuw project Planning is. Aangezien u veranderingen in het nieuwe project aanbrengt, zorgt dit ervoor dat de berichten niet worden verzonden naar de gebruikers die aan het project worden toegewezen.
  >
  >Voor meer informatie over vestiging de standaardstatus en andere standaardmontages voor een nieuw project, zie [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) of [Projectvoorkeuren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

* De volgende scenario&#39;s bestaan voor hoe Workfront de Groep en Status van een nieuw project bepaalt:

   * Als u een project van kras creeert, is de Groep van het project uw Groep van het Huis.

     De status van het project is de standaardstatus in de projectvoorkeuren van uw thuisgroep, indien aanwezig, of van uw Workfront-instantie. U kunt de standaardstatus veranderen wanneer het creëren van het project in om het even welke status beschikbaar voor de Groep van het project.

   * Als u een project gebruikend een malplaatje creeert, nemen de montages van het malplaatje belangrijkheid over de montages die door de Workfront of de groepsbeheerder worden gevestigd.

     De Groep van het nieuwe project is de Groep van het malplaatje. Als het malplaatje niet met een Groep wordt geassocieerd, dan is de Groep van het project de Groep van het Huis van de gebruiker die tot het project leidt.

     De standaardstatus van een nieuw project dat van een malplaatje wordt gecreeerd beantwoordt aan de status door uw beheerder van Workfront in het belangrijkste gebied van de Voorkeur van het Project of door een groepsbeheerder (of beheerder van Workfront) in het gebied van de Voorkeur van het Project voor de groep wordt bepaald. U kunt de standaardstatus veranderen wanneer het creëren van een project van een malplaatje, in om het even welke status van de Groep van het project dat of de Groep van het malplaatje, of de Groep van het Huis van de gebruiker is die tot het project leidt.

   * Als u een project creeert door een kwestie om te zetten, is de groep van een nieuw project de Groep van het bestaande project van de kwestie. Als de gebruiker die de kwestie omzet geen toegang tot het project van de kwestie heeft of als het project van de kwestie geen Groep heeft, is de Groep van het nieuwe project de Groep van het Huis van de gebruiker die de kwestie omzet.

     De statussen van het nieuwe project passen de groepsstatus van de groep aan het project aan, dat of de Groep van het oorspronkelijke project of de Groep van het Huis van de gebruiker is die de kwestie omzet.

     Als u een malplaatje gebruikt wanneer u het project door de kwestie creeert om te zetten, verwijs naar het tweede scenario hierboven om te begrijpen welke Groep en welke Status Workfront op het nieuwe project van toepassing is.

## Een geheel nieuw project maken

1. Voer een van de volgende handelingen uit:

   * Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon-left-nav.png) in de linkerbovenhoek Klikken **Projecten** vervolgens uitvouwen **Nieuw project**.
   * Naar een portfolio gaan en vervolgens uitvouwen **Nieuw project**.
   * Naar een programma gaan en vervolgens uitvouwen **Nieuw project**.
   * Als u een groepsbeheerder bent, kunt u een project in de sectie van Projecten van een groep ook tot stand brengen u beheert. Zie voor meer informatie [Projecten van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

   ![Menu Nieuw project](assets/new-project-dropdown-nwe-350x358.png)

1. Klikken **Nieuw project** in het menu om een geheel nieuw project te maken.
1. Typ een naam voor het project. Druk op Enter om de naam op te slaan.

   ![Geef een naam op voor het project](assets/rename-untitled-project.png)

   De kopbal van de projectpagina toont een snel overzicht van de huidige gezondheid en de vooruitgang van een project. De informatie in de projectkopbal verandert aangezien de projectinformatie wordt bijgewerkt.

1. Klikken **Taken toevoegen starten**.

   of

   Klikken **Nieuwe taak** om taken aan het project toe te voegen en middelen aan hen toe te wijzen.

   Voor meer informatie over het toevoegen van taken aan een project, zie [Taken maken in een project](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Bewerk de projectdetails door op de knop **Meer** en vervolgens **Bewerken** ![](assets/qs-edit-icon.png) naast de naam van het project.

   De **Project bewerken** wordt geopend.

   Zie voor meer informatie over het bewerken van een project [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).

1. (Optioneel) Nadat u de projectinstellingen hebt geconfigureerd en de taken hebt toegevoegd, kunt u de status van het project wijzigen in **Huidig**.

   Dit wijst erop dat het project nu klaar is te beginnen en de gebruikers die aan de taken worden toegewezen kunnen nu beginnen aan het werken aan hen.

   Voor meer informatie over projectstatussen, zie [Heb toegang tot de lijst van de statussen van het systeemproject](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
