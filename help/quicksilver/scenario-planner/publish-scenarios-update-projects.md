---
product-area: enterprise-scenario-planner-product-area
keywords: publiceren,plannen,projecten,scenario,scenario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Werk of creeer projecten door initiatieven in de Planner van het Scenario bij te publiceren
description: U kunt projecten van bestaande initiatieven tot stand brengen evenals projecten bijwerken eerder verbonden aan initiatieven door scenario's in de Planner van het Scenario van Adobe Workfront te publiceren.
author: Alina
feature: Workfront Scenario Planner
exl-id: 46d3666a-4454-4a84-8c02-a79f3947a18f
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '1550'
ht-degree: 0%

---

# Werk projecten bij of maak projecten door initiatieven te publiceren in de [!DNL Scenario Planner]

Wanneer u een scenario publiceert vanuit de [!DNL Adobe Workfront Scenario Planner] , gebeurt het volgende:

* Creeert projecten van de initiatieven op het scenario en verbindt hen samen.
* Werkt projecten bij die al gekoppeld zijn aan initiatieven over het scenario met informatie uit het gekoppelde initiatief. Projecten kunnen ook aan initiatieven worden gekoppeld wanneer u ze in een plan importeert. Voor informatie, zie [ de projecten van de Invoer in plannen in  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <p>Huidig: [!UICONTROL Business] of hoger</p>
   <p>Nieuw: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licentie*</p> </td> 
   <td> <p>Nieuw: Licht of hoger</p> 
   <p>Huidig: [!UICONTROL Review] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> 
   <p>Voor de huidige plannen van Workfront: </p>
   <p>U moet een extra licentie voor de [!DNL Adobe Workfront Scenario Planner] aanschaffen om toegang te krijgen tot de functionaliteit die in dit artikel wordt beschreven.</p> <p>Voor informatie over toegang en toestemmingen voor [!DNL Workfront Scenario Planner], zie <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref"> Toegang nodig om [!DNL Scenario Planner]</a> te gebruiken. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Toegangsniveau </td> 
   <td> <p>[!UICONTROL Edit] toegang voor de [!DNL Scenario Planner] en [!UICONTROL Projects]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objectmachtigingen </p> </td> 
   <td> <ul> 
     <li>[!UICONTROL Manage] machtigingen voor het abonnement </li> 
     <li>[!UICONTROL Manage] machtigingen voor gepubliceerde projecten</li> 
    </ul> <p>Voor informatie bij het vragen van om extra toegang tot een plan, zie <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref"> de toegang van het Verzoek tot een plan in [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang tot de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Voordat u begint:

* U moet een abonnement maken en opslaan voordat u er initiatieven van kunt publiceren.
* Toestaan de gebruikers om projecten tot stand te brengen zonder een malplaatje te gebruiken dat moet worden toegelaten in uw gebied van de Voorkeur van het Project van de Opstelling. Voor informatie, zie [ systeem-brede projectvoorkeur ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

## Overwegingen bij het publiceren van initiatieven voor projecten

* U kunt slechts één scenario van een plan publiceren.
* Eén initiatief kan slechts aan één project worden gekoppeld.
* Eén project kan aan meerdere initiatieven worden gekoppeld wanneer de initiatieven tot verschillende plannen behoren.

  >[!TIP]
  >
  >Wanneer een project op veelvoudige plannen bestaat en u informatie aan het project van alle plannen publiceert, publiceert recentste publiceert het bestaande [!DNL Scenario Planner] informatie over het project.

* Als er initiatieven in het kader van het plan worden genomen door projecten in het plan te importeren, worden de gekoppelde projecten door de publicatie van het initiatief ook bijgewerkt met informatie over initiatieven.

  >[!TIP]
  >
  >U kunt het zelfde project in veelvoudige plannen invoeren. Publiceren kan de initiatiefinformatie over een project overschrijven die aan meerdere initiatieven is gekoppeld.

  Voor informatie over het creëren van initiatieven door projecten in te voeren, zie [ projecten van de Invoer in plannen in  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Wijzigingen die in het project worden aangebracht, worden niet doorgevoerd in het gekoppelde initiatief.



## Publish-initiatieven

>[!IMPORTANT]
>
>Als u wijzigingen aanbrengt aan initiatieven in het plan, inclusief het oplossen van conflicten, moet u het initiatief opnieuw publiceren om de nieuwe informatie over het project zichtbaar te maken. Deze informatie geeft alleen weer over de projecten in verband met initiatieven wanneer u het desbetreffende initiatief publiceert. Voor informatie over het oplossen van conflicten tussen initiatieven, zie [ initiatiefconflicten oplossen in  [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)

{{step1-to-scenario-planner}}

1. (Optioneel en voorwaardelijk) Als u vanuit een bestaand abonnement wilt publiceren, klikt u op het pictogram **[!UICONTROL Filter]** ![](assets/filter-nwepng.png) rechtsboven in het abonnement en selecteert u een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>Toont alle plannen die u bezit of met u wordt gedeeld. Dit is de standaardinstelling. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL My plans]</td> 
      <td>Geeft de plannen weer die u hebt gemaakt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Shared with me]</td> 
      <td> <p>Hier worden de plannen weergegeven die u niet hebt gemaakt, maar met u hebt gedeeld.</p> <p>Belangrijk: u moet [!UICONTROL Manage] machtigingen hebben voor plannen die met u worden gedeeld om deze te kunnen publiceren. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Optioneel) Klik op het pictogram **[!UICONTROL Search]** ![](assets/search-icon.png) en typ de naam van een abonnement om het snel in de lijst te vinden.
1. (Voorwaardelijk) om van een nieuw plan te publiceren, creeer een plan.

   Voor informatie over het creëren van plannen, zie [ plannen in  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) creëren en uitgeven.

1. (Optioneel) Klik op de naam van een bestaand plan en maak nieuwe scenario&#39;s voor het plan.

   Voor informatie over het creëren van scenario&#39;s voor een plan, zie [ planscenario&#39;s in  [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md) creëren en vergelijken.

1. (Optioneel) Werk de initiatieven van een bestaand of een nieuw plan bij of maak nieuwe.

   Voor informatie over het creëren van initiatieven, zie [ initiatieven in  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md) creëren en uitgeven.

1. Klik op **[!UICONTROL Save plan]**.
1. Selecteer in het keuzemenu **[!UICONTROL Initial scenario]** het scenario dat u wilt publiceren en klik vervolgens op **[!UICONTROL Go to Publish]** rechtsboven in het scherm. ![](assets/go-to-publish-button-icon.png)

   of

   Klik op **[!UICONTROL Compare scenarios]**, houd de muisaanwijzer boven de scenario-kaart waarvan u de gegevens wilt publiceren en klik vervolgens op **[!UICONTROL Go to Publish]** ![](assets/go-to-publish-button-icon.png) .

   De pagina [!UICONTROL Publish initiatives] wordt weergegeven met een lijst met alle initiatieven in het scenario. Als een van de initiatieven eerder is gepubliceerd, wordt het projectpictogram ![](assets/project-icon-sp.png) weergegeven na de naam en wordt de datum **[!UICONTROL Last published]** in de lijst geplaatst.

   >[!TIP]
   >
   >Initiatieven die zijn gemaakt door projecten te importeren, geven rechts van hun naam ook het projectpictogram ![](assets/project-icon-sp.png) weer

   ![](assets/project-icons-and-last-published-date-in-publish-initiative-page-350x63.png)

1. (Optioneel en voorwaardelijk) Als u vanuit een bestaand abonnement wilt publiceren, klikt u op het pictogram **[!UICONTROL Filter]** ![](assets/filter-nwepng.png) rechtsboven in het abonnement en selecteert u een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>Toont alle initiatieven van het geselecteerde scenario. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Published]</td> 
      <td>Geeft initiatieven weer die u of een andere gebruiker eerder heeft gepubliceerd. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Unpublished]</td> 
      <td> <p>Geeft ongepubliceerde initiatieven weer. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/initiatives-fitler-in-publishing-screen-scenario-planner.png)

1. (Optioneel) Klik op het pictogram **[!UICONTROL Search]** ![](assets/search-icon.png) en typ de naam van een initiatief om dit snel in de lijst te vinden.
1. Selecteer een of meerdere initiatieven om er projecten van te publiceren en te maken of bij te werken, en klik vervolgens op **[!UICONTROL Publish initiatives]** .

   Dit leidt tot een nieuw project van elke geselecteerde initiatieven of werkt de bestaande verwante projecten bij, als de gepubliceerde initiatieven reeds met een project verbonden waren.

   >[!TIP]
   >
   >Nieuwe projecten hebben dezelfde naam als de gepubliceerde initiatieven.

1. (Voorwaardelijk) Voer een van de volgende handelingen uit:

   * Als u één initiatief hebt gepubliceerd, klikt u op **[!UICONTROL See associated project]** om het project te openen dat is gemaakt of bijgewerkt op basis van het initiatief.
   * Als u meerdere initiatieven hebt gepubliceerd, klikt u op **[!UICONTROL See associated projects]** om een lijst met projecten te openen die zijn gepubliceerd op basis van initiatieven. [!DNL Workfront] past standaard het filter [!DNL Scenario Planner] Projecten toe op de lijst met projecten. De projecten die het laatst zijn gepubliceerd, worden boven aan de lijst weergegeven.

     ![](assets/scenario-planner-filter-after-publishing-initiatives-350x81.png)

1. Ga naar de volgende gebieden om initiatiefinformatie over het project te bekijken:

   * **de [!UICONTROL Updates] sectie**: Een update publiceert om erop te wijzen dat het project van het initiatief werd gecreeerd of werd bijgewerkt. De update bevat de naam van het initiatief dat het project heeft gemaakt of bijgewerkt en de gekoppelde naam van het plan dat het initiatief bevat. U kunt op de naam van het abonnement in de update klikken om het abonnement te openen in de [!DNL Scenario Planner] .

     ![](assets/update-stream-confirmation-of-publish-on-project-350x65.png)

   * **het [!UICONTROL Overview] gebied van de [!UICONTROL Project Details] sectie**: Een nieuwe [!DNL Scenario Planner] sectie wordt gecreeerd op dit gebied dat informatie van het verbonden initiatief bevat.

     ![](assets/scenario-planner-on-project-details-350x135.png)

     De volgende informatie over initiatieven wordt gepubliceerd in het gedeelte [!DNL Scenario Planner] van de sectie [!UICONTROL Project Details] :

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Duration]</span> </td> 
        <td><span> de duur van het overeenkomstige initiatief wanneer het project met een initiatief verbonden is. Dit veld kan niet worden bewerkt.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Last Published Date]</span> </td> 
        <td><span> de datum toen het project het laatst van een overeenkomstig initiatief werd gepubliceerd.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Start Date]</span> </td> 
        <td><span> de eerste dag van de beginmaand van het initiatief, wanneer het project met een initiatief wordt verbonden.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative End Date]</span> </td> 
        <td><span> de laatste dag van de eindmaand van het initiatief, wanneer het project met een initiatief verbonden is. </span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Job Roles in FTEs and Hours]</span> </td> 
        <td> <p>Informatie over de bijbehorende functies en de tijdstoewijzingen voor het initiatief. Dit omvat:</p> 
         <ul> 
          <li>Functienaam</li> 
          <li>Aantal FTE's</li> 
          <li> <p>Aantal uren voor alle VTE's</p> <p>U kunt de hoeveelheid baanrollen schatten nodig voor uw plan of initiatief gebruikend uren of FTEs.</p> <p>Voor meer informatie, zie <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref"> plannen in de Planner van het Scenario creëren en uitgeven </a>. </p> </li> 
         </ul> 
      <p><b>TIP</b>

     Als het aantal functies per maand in het initiatief verschilt, wordt in dit veld het maximale aantal rollen weergegeven dat nodig is voor het initiatief. Bijvoorbeeld, als u 1 Consultant voor Januari en 2 voor Februari nodig hebt, toont de kolom 2FTE en de overeenkomstige hoeveelheid uren voor 2 FTEs voor alle maanden.</p> </td>
     </tr> 
      </tbody> 
     </table>

     >[!NOTE]
     >
     >Alle gebruikers met [!UICONTROL View] toegang tot het project kunnen de [!DNL Scenario Planner] sectie in het [!UICONTROL Overview] gebied zien. U kunt bepalen of dit gebied wordt weergegeven in de [!UICONTROL Details] -sectie met behulp van een lay-outsjabloon. Als gebruikers geen lay-outmalplaatje hebben verbonden aan hen, toont dit gebied door gebrek.
     >
     >   
     >   
     >   * Voor informatie over het toevoegen van of het verwijderen van gebieden in de [!UICONTROL Details] sectie die een lay-outmalplaatje gebruiken, zie [ de [!UICONTROL Details] mening aanpassen gebruikend een lay-outmalplaatje ](../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
     >   * Voor meer informatie over het bekijken van informatie in het [!UICONTROL Overview] gebied van [!UICONTROL Project Details], zie [[!UICONTROL Manage] informatie in het [!UICONTROL Overview] gebied van het project ](../manage-work/projects/manage-projects/understand-project-overview-area.md).
     >   
     >

   * **het [!UICONTROL Role Allocation] paneel in [!UICONTROL Workload Balancer] of de taaklijst van het project**: De informatie over roltoewijzing over het initiatief bevolkt op dit gebied, naast roltoewijzingen over het project.

     Voor meer informatie, zie [ Overzicht van het verzoenen van middeltoewijzingen tussen projecten en initiatieven ](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

     ![](assets/role-allocation-panel-350x174.png)

     Wijzigingen in de data of middelen van het project hebben geen invloed op het desbetreffende initiatief of op de gebieden van het project die initiatiefinformatie bevatten.

   * **het [!UICONTROL Resource Budgeting] gebied van [!UICONTROL Business Case] van het project**: Een nieuwe optie voor het beheren van projectmiddelen die [!DNL Scenario Planner] informatie gebruiken wordt toegevoegd in het [!UICONTROL Resource Budgeting] gebied van [!UICONTROL Business Case] van het project.

     Voor meer informatie, zie [ middelen van de Begroting in [!UICONTROL Business Case] gebruikend  [!DNL Scenario Planner]](../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

     ![](assets/sp-in-business-case-selected-350x110.png)

1. (Optioneel) Controleer de volgende informatie in de [!DNL Scenario Planner] nadat u een scenario hebt gepubliceerd:

   * Het gepubliceerde scenario wordt het eerste scenario nadat u initiatieven van het publiceert.
   * U kunt niet van een ander scenario publiceren nadat u een scenario minstens eens hebt gepubliceerd.
   * De optie [!UICONTROL Go to Publish] wordt uit alle andere scenario&#39;s verwijderd nadat ten minste één initiatief van een scenario is gepubliceerd.
   * Naast de projectpictogrammen van de gepubliceerde initiatieven in het plan wordt een groene indicator weergegeven.

     ![](assets/indicator-for-published-initiative-icon-350x119.png)

   * Een groene &quot;Gepubliceerde&quot;indicatorvertoningen bij de bovenkant van het scenario en op de scenario kaart en het Gepubliceerde gebied wordt bevolkt op de scenario kaart die op het aantal initiatieven in het scenario wijst die zijn gepubliceerd.

     ![](assets/published-scenario-highlighted-350x632.png)

     >[!TIP]
     >
     >Als alle projecten die uit de initiatieven van het scenario worden gepubliceerd, worden geschrapt, wordt de aanwijzing dat het scenario is gepubliceerd geschrapt. Voor informatie, zie [ projecten van de Schrapping ](../manage-work/projects/manage-projects/delete-projects.md).

1. (Optioneel) Werk de informatie over het initiatief bij en herhaal het hierboven beschreven proces om het initiatief opnieuw te publiceren en actualiseer de initiatiefinformatie over het gekoppelde project.

   Voor informatie over het uitgeven van initiatieven, zie [ initiatieven in  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md) creëren en uitgeven.


