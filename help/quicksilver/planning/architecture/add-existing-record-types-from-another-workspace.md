---
title: Bestaande recordtypen toevoegen uit een andere Workspace
description: Recordtypen zijn de objecttypen voor Adobe Workfront Planning. In de Planning van Workfront, kunt u een bestaand verslagtype toevoegen dat in een andere werkruimte wordt gecreeerd.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: bfb0fd2956ffb9384a09882864668d5dba33a53b
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Bestaande recordtypen uit een andere werkruimte toevoegen

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

Als werkruimtenmanager, kunt u een verslagtype toevoegen dat in een werkruimte aan een werkruimte bestaat die u in de Planning van Adobe Workfront beheert.

U moet een recordtype eerst als gecentraliseerd aanwijzen voordat werkruimtenmanagers het als een bestaand recordtype in andere werkruimten kunnen toevoegen.

U kunt een recordtype instellen als gecentraliseerd wanneer u het maakt of bewerkt terwijl u de instellingen voor de werkruimte van het recordtype definieert.

Voor informatie, zie [ mogelijkheden van de dwars-werkruimte voor verslagtypes ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) vormen.

Alvorens verslagen aan een werkruimte van een gecentraliseerd verslagtype toe te voegen, zie het artikel [ overzicht van de types van het interwerkruimterecord van het artikel ](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

## Toegangsvereisten

+++ Breid uit om de toegangsvereisten voor de functionaliteit in dit artikel te bekijken.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr>

</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<ul><li><p>Willekeurig Workfront-pakket</p></li>
en
<li><p>Planning Plus-pakket</p></li></ul>
<!--Or:
<ul><li><p>Any Workflow package</p> </li>
And
<li><p>Planning Prime or Ultimate package</p></li></ul>-->
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningspakket wordt opgenomen. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Rechten beheren in een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr>  
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Een recordtype maken op basis van een bestaand recordtype

1. Begin creërend een verslagtype, zoals die in het artikel [ wordt beschreven creeer verslagtypes ](/help/quicksilver/planning/architecture/create-record-types.md), dan klik **voegt bestaand** toe. <!--check this - the option might have been renamed in the UI-->

   ![ Modal om verslagtype met optie toe te voegen van een andere werkruimte ](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. Klik **verdergaan**.
1. In **kies verslagtype** doos, klik de kaart voor het verslagtype dat u van een bestaande werkruimte wilt toevoegen, dan **toevoegen** klikken.

   Het recordtype wordt toegevoegd aan de geselecteerde werkruimte.

   >[!TIP]
   >
   >Als er geen recordtypen zijn geconfigureerd om aan een andere werkruimte te worden toegevoegd, wordt de optie om deze uit een andere werkruimte toe te voegen niet weergegeven wanneer u een recordtype maakt.

   De volgende dingen doen zich voor:

   * De volgende informatie wordt ook toegevoegd van het bestaande gecentraliseerde recordtype:

      * Alle oorspronkelijke velden
      * Alle recordverbindingen
   * U kunt records weergeven die zijn toegevoegd vanuit andere werkruimten, alleen als u ten minste weergavemachtigingen hebt voor die werkruimten.
   * Het **gecentraliseerde verslagtype** pictogram ![ Gecentraliseerde verslagtype pictogram ](assets/global-icon.png) wordt toegevoegd aan de kaart van het nieuwe verslagtype.
   * Het read-only **Workspace** gebied wordt toegevoegd aan de nieuwe lijst van het verslagtype mening. In het veld wordt weergegeven in welke werkruimte elke record is gemaakt.

     >[!NOTE]
     >
     >* U kunt de weergave, geavanceerde instellingen of originele velden van het nieuwe recordtype niet bewerken. U kunt het recordtype en alle oorspronkelijke velden en instellingen alleen vanuit de oorspronkelijke werkruimte bewerken.

1. (Optioneel) Klik en sleep het nieuwe recordtype naar een willekeurige sectie in de werkruimte.

<!--This will be released later with another epic: 1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.-->

1. (Facultatief) klik op **Meer** menu ![ Meer menu ](assets/more-menu.png) in de kaart van het nieuwe verslagtype, of rechts van de naam van het verslagtype op zijn pagina, dan klik **Schrapping**.
1. (Voorwaardelijk) Type **schrapt** op het verstrekte gebied, dan klik **permanent schrapt**.

   De volgende dingen doen zich voor:

   * Het recordtype dat is gemaakt op basis van een gecentraliseerd recordtype, wordt verwijderd uit de geselecteerde werkruimte.
   * Het oorspronkelijke recordtype en de bijbehorende velden blijven in de oorspronkelijke werkruimte staan.
   * Het recordtype blijft in alle andere werkruimten waar het is toegevoegd.
   * De records die vanuit de huidige werkruimte aan het recordtype zijn toegevoegd, worden verwijderd. Alle andere records die zijn toegevoegd vanuit extra werkruimten waar het gecentraliseerde recordtype is toegevoegd, blijven behouden.





