---
title: De terminologie van de gebruikersinterface aanpassen met behulp van een lay-outsjabloon
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Adobe Workfront-beheerder kunt u een lay-outsjabloon gebruiken om de labels van bepaalde objecten die in Workfront worden weergegeven, aan te passen aan de termen die in uw organisatie worden gebruikt.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '607'
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
>* Er kunnen grammatica en andere problemen optreden wanneer u labels aanpast. Als u bijvoorbeeld &quot;Issue&quot; wijzigt in &quot;Request&quot;, kunnen er plaatsen in de gebruikersinterface zijn waar de uitdrukking &quot;An request&quot; wordt weergegeven. Zie voor meer informatie [Implicaties van het aanpassen van objectnamen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) in het artikel [Objecten in Adobe Workfront begrijpen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
>


Voor informatie over lay-outsjablonen voor groepen raadpleegt u [De lay-outsjablonen van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Toegangsvereisten

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
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Om deze stappen op systeemniveau uit te voeren, hebt u het toegangsniveau van de Beheerder van het Systeem nodig.
Om hen voor een groep uit te voeren, moet u een manager van die groep zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## De terminologie van de gebruikersinterface aanpassen

1. Beginnen met het werken aan een lay-outsjabloon, zoals beschreven in [Lay-outsjablonen maken en beheren](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klikken **Terminologie instellen** in de rechterbovenhoek van de pagina.
1. Voer een van de volgende handelingen uit:

   * Klik op de pijl-omlaag als u een andere term van Workfront wilt gebruiken  ![](assets/dropdown-arrow.png) naast het label klikt u op het gewenste alternatieve label in de vervolgkeuzelijst.

      >[!NOTE]
      >
      >Alternatieve labels in de vervolgkeuzelijsten worden ondersteund in versies van Workfront die zijn gelokaliseerd voor niet-Engelse talen.

   * Als u uw eigen aangepaste alternatief wilt opgeven voor het label dat voor een object wordt weergegeven, klikt u op **Aangepaste naam instellen** rechts van het label typt u vervolgens het **Enkelvoudig** en **meervoudig** vormen van de aangepaste term. U kunt op **Herstellen** als je van gedachten verandert.

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
        <td><p>Zie voor meer informatie over deze objecten <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Objecten in Adobe Workfront begrijpen</a>.</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Objecten Workfront Goals</p></td>
        <td>
         <ul>
          <p>Goal</p>
          <p>Resultaat</p>
          <p>Activiteit</p>
         </ul></td>
        <td><p>Voor deze objecten is een extra licentie vereist. Zie voor meer informatie <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Overzicht van Adobe Workfront-doelen</a>.</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Workfront Scenario Planner-objecten</p></td>
        <td>
         <ul>
          <p>Initiatief</p>
          <p>Scenario</p>
          <p>Plan </p>
         </ul></td>
        <td><p>Voor deze objecten is een extra licentie vereist. Zie voor meer informatie <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">Aan de slag met de functie Scenario Planner</a>.</p></td>
       </tr>
      </tbody>
     </table>

1. Als u klaar bent, klikt u op **Gereed**.

   >[!TIP]
   >
   >Nadat u op Gereed hebt geklikt (en zelfs nadat u de lay-outsjabloon hebt opgeslagen), kunt u altijd terugkeren naar de instelling Terminologie instellen en op Herstellen klikken naast aangepaste termen om deze weer in de standaardtoestand te brengen.

1. Blijf het lay-outmalplaatje aanpassen.

   of

   Als u klaar bent met het aanpassen, klikt u op **Opslaan**.

1. Om uw terminologiewijzigingen te zien:

   1. Meld u af en weer aan bij Workfront.
   1. Sluit alle geopende browsertabbladen voor uw Workfront-omgeving.

   >[!IMPORTANT]
   >
   >Dit is ook vereist voor iedereen die de lay-outsjabloon heeft gebruikt voordat u de terminologiewijzigingen aanbrengt.

Voor meer informatie over lay-outsjablonen raadpleegt u [Lay-outsjablonen maken en beheren](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
