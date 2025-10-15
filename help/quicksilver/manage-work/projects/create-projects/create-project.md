---
product-area: projects
navigation-topic: create-projects
title: Een project maken
description: Een project is een grote eenheid werk in Adobe Workfront. U kunt geheel nieuwe projecten maken, een sjabloon gebruiken of uitgaven of taken omzetten in projecten.
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 0%

---

# Een project maken

<!--remove Preview and Production references-->

<!-- Audited: 12/2023 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Projecten vormen een groot deel van het werk dat in Adobe Workfront moet worden verricht.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p>
        <p>Plan</p> </td> 
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

Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p>
        <p>or</p>
        <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project, you automatically receive Manage permissions to the project.</p> </td> 
  </tr> 
 </tbody> 
</table>-->


## Manieren om projecten te maken

U kunt een project in Workfront tot stand brengen gebruikend één van de volgende methodes:

* Een geheel nieuw project maken zonder een sjabloon te gebruiken. In dit artikel wordt beschreven hoe u een geheel nieuw project kunt maken.

* Een bestaand project kopiëren.\
  Voor meer informatie over het kopiëren van project, zie [ een project ](../../../manage-work/projects/manage-projects/copy-project.md) kopiëren.

* Gebruik een sjabloon.\
  Voor meer informatie over het gebruiken van een malplaatje om een nieuw project tot stand te brengen, zie [ een project creëren gebruikend een malplaatje ](../../../manage-work/projects/create-projects/create-project-from-template.md).

* Een project importeren uit Microsoft Project.\
  Voor meer informatie over het invoeren van een project van het Project van MS, zie [ een project van het Project van Microsoft invoeren ](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* Importeer een project met de functie voor het starten van een project.

  Als beheerder van Workfront, kunt u projecten invoeren gebruikend een schop-begin.

  Voor informatie over het invoeren van gegevens gebruikend schop-begin in Workfront, zie [ Gegevens van de Invoer in Adobe Workfront gebruikend een Kick-Begin malplaatje ](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

  Voor informatie over het invoeren van projecten die schoppen-begin gebruiken, zie [ Kick-Begint scenario: het eenvoudige project en de voorbereiding van de taakinvoer ](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md).

* Publiceer een initiatief van een scenario in de Planner van het Scenario van Adobe Workfront.

  Voor informatie over de Planner van het Scenario van Workfront, zie [ het overzicht van de Planner van het Scenario ](../../../scenario-planner/scenario-planner-overview.md).

  Voor informatie over het creëren van projecten van het publiceren initiatieven, zie [ Update of creeer projecten door initiatieven in de Planner van het Scenario te publiceren ](../../../scenario-planner/publish-scenarios-update-projects.md).

* Voeg projecten toe aangezien u hen van een verslagtype in de Planning van Workfront verbindt.

  Voor informatie over toegang tot de Planning van Workfront, zie [ Overzicht van de Toegang ](/help/quicksilver/planning/access/access-overview.md).

  Voor informatie over het creëren van projecten door hen aan verslagen toe te voegen, zie de sectie &quot;projecten creëren wanneer het verbinden van hen met verslagen van de Planning van Workfront&quot;in het artikel [ creeer de voorwerpen van Workfront van Workfront Planning aangezien u hen met verslagen ](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md) verbindt

## Vereisten

Voordat u begint, moet u ervoor zorgen dat:

* Uw systeem of groepsbeheerder liet &quot;toestaan gebruikers toe om projecten tot stand te brengen zonder een malplaatje&quot;voorkeur in het gebied van de Opstelling te gebruiken.

  Voor meer informatie, zie [ systeem-brede projectvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

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
  >Voor meer informatie over vestiging de standaardstatus en andere standaardmontages voor een nieuw project, zie [ systeem-brede projectvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen of [ projectvoorkeur voor een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) vormen.

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
>Als u een project gebruikend een malplaatje creeert, adviseren wij dat u ook het artikel [ ziet creeert een project gebruikend een malplaatje ](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Voer een van de volgende handelingen uit:

   * Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek. Klik **Projecten**, dan breid **Nieuw Project** uit.
   * Ga naar een portefeuille, dan breid **Nieuw Project** uit.
   * Ga naar een programma, dan breid **Nieuw Project** uit.
   * Als u een groepsbeheerder bent, kunt u een project in de sectie van Projecten van een groep ook tot stand brengen u beheert. Voor meer informatie, zie [ tot stand brengen en wijzigen de projecten van een groep ](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

   ![ Nieuw menu van het Project ](assets/new-project-dropdown-nwe-350x358.png)

1. Klik **Nieuw Project** in het menu om een project van kras tot stand te brengen.
1. Typ een naam voor het project. Druk op Enter om de naam op te slaan.

   ![ ga een naam voor het project ](assets/rename-untitled-project.png) in

   De kopbal van de projectpagina toont een snel overzicht van de huidige gezondheid en de vooruitgang van een project. De informatie in de projectkopbal verandert aangezien de projectinformatie wordt bijgewerkt.

1. Klik **Begin Toevoegend Taken**.

   of

   Klik **Nieuwe Taak** om taken aan het project toe te voegen en middelen aan hen toe te wijzen.

   Voor meer informatie over het toevoegen van taken aan een project, zie [ tot taken in een project ](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) leiden.

1. Bewerk de projectdetails door het **Meer** menu te klikken en dan **geef** ![ uit pictogram ](assets/qs-edit-icon.png) naast de naam van het project uitgeeft.

   Het **geeft de dialoogvakje van het Project** uit opent.

   Voor meer informatie over het uitgeven van een project, zie [ projecten ](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

1. (Facultatief) na het vormen van de projectmontages en het toevoegen van de taken, kunt u het statuut van het project in **Huidige** veranderen.

   Dit wijst erop dat het project nu klaar is te beginnen en de gebruikers die aan de taken worden toegewezen kunnen nu beginnen aan het werken aan hen.

   Voor meer informatie over projectstatussen, zie [ Toegang tot de lijst van de statussen van het systeemproject ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
