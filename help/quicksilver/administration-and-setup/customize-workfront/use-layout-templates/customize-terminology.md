---
title: De gebruikersinterfaceterminologie aanpassen met behulp van een lay-outsjabloon
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Adobe Workfront-beheerder kunt u een lay-outsjabloon gebruiken om de labels van bepaalde objecten die in Workfront worden weergegeven, aan te passen aan de termen die in uw organisatie worden gebruikt.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# De terminologie van de gebruikersinterface aanpassen met behulp van een lay-outsjabloon

Als Adobe Workfront-beheerder kunt u een lay-outsjabloon gebruiken om de labels van bepaalde objecten die in Workfront worden weergegeven, aan te passen aan de termen die in uw organisatie worden gebruikt.

Nadat u een lay-outsjabloon hebt opgeslagen waarin u de terminologie hebt gewijzigd, meldt u zich af van Workfront en weer aan, waarna de gewijzigde labels worden weergegeven op de plaatsen waar de standaardlabels in de meeste gebieden in Workfront worden weergegeven:

* Hoofdmenu
* Alle gebieden die via het hoofdmenu worden geopend
* Alle tabbladen
* Alle menu&#39;s
* Report Builder- en rapportageelementen (weergaven, filters en groepen)
* Knoppen opslaan
* Geëxporteerde bestanden
* E-mails
* Mobiele apps

>[!NOTE]
>
>* In het gebied Outlook Add-in worden de aangepaste labels niet weergegeven.
>* Er kunnen grammatica en andere problemen optreden wanneer u labels aanpast. Als u bijvoorbeeld &quot;Issue&quot; wijzigt in &quot;Request&quot;, kunnen er plaatsen in de gebruikersinterface zijn waar de uitdrukking &quot;An request&quot; wordt weergegeven. Voor meer informatie, zie [ Implicaties van het aanpassen van objecten namen ](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) in het artikel [ voorwerpen in Adobe Workfront ](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) begrijpen
>

Voor meer informatie over lay-outmalplaatjes, zie [ lay-outmalplaatjes ](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) creëren en beheren.

Voor informatie over lay-outmalplaatjes voor groepen, zie [ tot stand brengen en wijzigen de lay-outmalplaatjes van een groep ](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nadat u een lay-outmalplaatje hebt gevormd, moet u het aan gebruikers voor veranderingen toewijzen u aanbracht om aan anderen zichtbaar te zijn. Voor informatie over het toewijzen van een lay-outmalplaatje aan gebruikers, zie [ gebruikers aan een lay-outmalplaatje ](../use-layout-templates/assign-users-to-layout-template.md) toewijzen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td><p>Nieuw: Standaard</p>
  <p> Huidig: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Om deze stappen op systeemniveau uit te voeren, hebt u het toegangsniveau van de Beheerder van het Systeem nodig.
Om hen voor een groep uit te voeren, moet u een manager van die groep zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## De terminologie van de gebruikersinterface aanpassen

1. Begin werkend aan een lay-outmalplaatje, zoals die in [ wordt beschreven creeer en beheer lay-outmalplaatjes ](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klik **Vastgestelde Terminologie** dichtbij de hoger-juiste hoek van de pagina.
1. Voer een van de volgende handelingen uit:

   * Als u een andere term wilt gebruiken die door Workfront wordt geboden, klikt u op de pijl-omlaag ![](assets/dropdown-arrow.png) naast het label en klikt u vervolgens op het alternatieve label dat u in de vervolgkeuzelijst wilt gebruiken.

     >[!NOTE]
     >
     >Alternatieve labels in de vervolgkeuzelijsten worden ondersteund in versies van Workfront die zijn gelokaliseerd voor niet-Engelse talen.

   * Om uw eigen douanealternatief voor het etiket te verstrekken dat voor een voorwerp wordt getoond, klik **Vastgestelde douanenaam** rechts van het etiket, dan typ de **Enkelvoudige** en **Plurale** vormen van de douaneterm. U kunt **Terugstellen** klikken als u uw mening verandert.

     U kunt de volgende objectnamen aanpassen:

     <table style="table-layout:auto">
      <col>
      <col>
      <col>
      <tbody>
       <tr>
        <td role="rowheader"><p>Workfront-objecten</p></td>
        <td>
          <p>Portfolio</p>
          <p>Programma</p>
          <p>Project</p>
          <p>Taak</p>
          <p>Probleem</p>
          <p>Goal</p>
          <p>Resultaat</p>
          <p>Activiteit</p>
         </ul></td>
        <td><p>Voor meer informatie over deze voorwerpen, zie <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref"> voorwerpen in Adobe Workfront </a> begrijpen.</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Objecten Workfront Goals</p></td>
        <td>
         <ul>
          <p>Goal</p>
          <p>Resultaat</p>
          <p>Activiteit</p>
         </ul></td>
        <td><p>Voor deze objecten is een extra licentie vereist. Voor meer informatie, zie <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref"> overzicht van de Doelen van Adobe Workfront </a>.</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Workfront Scenario Planner-objecten</p></td>
        <td>
         <ul>
          <p>Initiatief</p>
          <p>Scenario</p>
          <p>Plan </p>
         </ul></td>
        <td><p>Voor deze objecten is een extra licentie vereist. Voor informatie, zie <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref"> begonnen worden met de Planner van het Scenario </a>.</p></td>
       </tr>
      </tbody>
     </table>

1. Wanneer u wordt gebeëindigd, klik **Gedaan**.

   >[!TIP]
   >
   >Nadat u op Gereed hebt geklikt (en zelfs nadat u de lay-outsjabloon hebt opgeslagen), kunt u altijd terugkeren naar de instelling Terminologie instellen en op Herstellen klikken naast aangepaste termen om deze weer in de standaardtoestand te brengen.

1. Blijf het lay-outmalplaatje aanpassen.

   of

   Als u wordt gebeëindigd aanpassend, klik **sparen**.

1. Om uw terminologiewijzigingen te zien:

   1. Meld u af en weer aan bij Workfront.
   1. Sluit alle geopende browsertabbladen voor uw Workfront-omgeving.

   >[!IMPORTANT]
   >
   >Dit is ook vereist voor iedereen die de lay-outsjabloon heeft gebruikt voordat u de terminologiewijzigingen aanbrengt.

Voor meer informatie over lay-outmalplaatjes, zie [ lay-outmalplaatjes ](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) creëren en beheren.
