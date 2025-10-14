---
product-area: projects
navigation-topic: create-projects
title: Een project maken
description: Een project is een grote eenheid werk in Adobe Workfront. U kunt geheel nieuwe projecten maken, een sjabloon gebruiken of uitgaven of taken omzetten in projecten.
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: a00776ecd9f8dc14b9dce14ce9463c2bb709a363
workflow-type: tm+mt
source-wordcount: '1259'
ht-degree: 0%

---

# Een project maken

<!--remove Preview and Production references-->

<!-- Audited: 12/2023 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

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
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Nieuw: Standaard</p>
        <p>of</p>
        <p>Huidig: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Wanneer u een project creeert, ontvangt u automatisch Manage toestemmingen aan het project.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Manieren om projecten te maken

U kunt een project in Workfront tot stand brengen gebruikend één van de volgende methodes:

* Een geheel nieuw project maken zonder een sjabloon te gebruiken. In dit artikel wordt beschreven hoe u een geheel nieuw project kunt maken.

* Een bestaand project kopiëren.\
  Voor meer informatie over het kopiëren van project, zie [&#x200B; een project &#x200B;](../../../manage-work/projects/manage-projects/copy-project.md) kopiëren.

* Gebruik een sjabloon.\
  Voor meer informatie over het gebruiken van een malplaatje om een nieuw project tot stand te brengen, zie [&#x200B; een project creëren gebruikend een malplaatje &#x200B;](../../../manage-work/projects/create-projects/create-project-from-template.md).

* Een project importeren uit Microsoft Project.\
  Voor meer informatie over het invoeren van een project van het Project van MS, zie [&#x200B; een project van het Project van Microsoft invoeren &#x200B;](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* Importeer een project met de functie voor het starten van een project.

  Als beheerder van Workfront, kunt u projecten invoeren gebruikend een schop-begin.

  Voor informatie over het invoeren van gegevens gebruikend schop-begin in Workfront, zie [&#x200B; Gegevens van de Invoer in Adobe Workfront gebruikend een Kick-Begin malplaatje &#x200B;](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

  Voor informatie over het invoeren van projecten die schoppen-begin gebruiken, zie [&#x200B; Kick-Begint scenario: het eenvoudige project en de voorbereiding van de taakinvoer &#x200B;](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md).

* Publiceer een initiatief van een scenario in de Planner van het Scenario van Adobe Workfront.

  Voor informatie over de Planner van het Scenario van Workfront, zie [&#x200B; het overzicht van de Planner van het Scenario &#x200B;](../../../scenario-planner/scenario-planner-overview.md).

  Voor informatie over het creëren van projecten van het publiceren initiatieven, zie [&#x200B; Update of creeer projecten door initiatieven in de Planner van het Scenario te publiceren &#x200B;](../../../scenario-planner/publish-scenarios-update-projects.md).

* Voeg projecten toe aangezien u hen van een verslagtype in de Planning van Workfront verbindt.

  Voor informatie over toegang tot de Planning van Workfront, zie [&#x200B; Overzicht van de Toegang &#x200B;](/help/quicksilver/planning/access/access-overview.md).

  Voor informatie over het creëren van projecten door hen aan verslagen toe te voegen, zie de sectie &quot;projecten creëren wanneer het verbinden van hen met verslagen van de Planning van Workfront&quot;in het artikel [&#x200B; creeer de voorwerpen van Workfront van Workfront Planning aangezien u hen met verslagen &#x200B;](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md) verbindt

## Vereisten

Voordat u begint, moet u ervoor zorgen dat:

* Uw systeem of groepsbeheerder liet &quot;toestaan gebruikers toe om projecten tot stand te brengen zonder een malplaatje&quot;voorkeur in het gebied van de Opstelling te gebruiken.

  Voor meer informatie, zie [&#x200B; systeem-brede projectvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

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
  >Voor meer informatie over vestiging de standaardstatus en andere standaardmontages voor een nieuw project, zie [&#x200B; systeem-brede projectvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen of [&#x200B; projectvoorkeur voor een groep &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) vormen.

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

>[!NOTE]
>
>Als u een project gebruikend een malplaatje creeert, adviseren wij dat u ook het artikel [&#x200B; ziet creeert een project gebruikend een malplaatje &#x200B;](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).


1. Voer een van de volgende handelingen uit:

   * Klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek. Klik **Projecten**, dan breid **Nieuw Project** uit.
   * Ga naar een portefeuille, dan breid **Nieuw Project** uit.
   * Ga naar een programma, dan breid **Nieuw Project** uit.
   * Als u een groepsbeheerder bent, kunt u een project in de sectie van Projecten van een groep ook tot stand brengen u beheert. Voor meer informatie, zie [&#x200B; tot stand brengen en wijzigen de projecten van een groep &#x200B;](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

   ![&#x200B; Nieuw menu van het Project &#x200B;](assets/new-project-dropdown-nwe-350x358.png)

1. Klik **Nieuw Project** in het menu om een project van kras tot stand te brengen.
1. Typ een naam voor het project. Druk op Enter om de naam op te slaan.

   ![&#x200B; ga een naam voor het project &#x200B;](assets/rename-untitled-project.png) in

   De kopbal van de projectpagina toont een snel overzicht van de huidige gezondheid en de vooruitgang van een project. De informatie in de projectkopbal verandert aangezien de projectinformatie wordt bijgewerkt.

1. Klik **Begin Toevoegend Taken**.

   of

   Klik **Nieuwe Taak** om taken aan het project toe te voegen en middelen aan hen toe te wijzen.

   Voor meer informatie over het toevoegen van taken aan een project, zie [&#x200B; tot taken in een project &#x200B;](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) leiden.

1. Bewerk de projectdetails door het **Meer** menu te klikken en dan **geef** ![&#x200B; uit pictogram &#x200B;](assets/qs-edit-icon.png) naast de naam van het project uitgeeft.

   Het **geeft de dialoogvakje van het Project** uit opent.

   Voor meer informatie over het uitgeven van een project, zie [&#x200B; projecten &#x200B;](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

1. (Facultatief) na het vormen van de projectmontages en het toevoegen van de taken, kunt u het statuut van het project in **Huidige** veranderen.

   Dit wijst erop dat het project nu klaar is te beginnen en de gebruikers die aan de taken worden toegewezen kunnen nu beginnen aan het werken aan hen.

   Voor meer informatie over projectstatussen, zie [&#x200B; Toegang tot de lijst van de statussen van het systeemproject &#x200B;](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
